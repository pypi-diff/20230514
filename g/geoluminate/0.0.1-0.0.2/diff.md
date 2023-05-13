# Comparing `tmp/geoluminate-0.0.1.tar.gz` & `tmp/geoluminate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoluminate-0.0.1.tar", max compression
+gzip compressed data, was "geoluminate-0.0.2.tar", max compression
```

## Comparing `geoluminate-0.0.1.tar` & `geoluminate-0.0.2.tar`

### file list

```diff
@@ -1,379 +1,398 @@
--rw-r--r--   0        0        0     1089 2023-05-08 12:24:18.006423 geoluminate-0.0.1/LICENSE
--rw-r--r--   0        0        0     2251 2023-05-08 12:24:18.006423 geoluminate-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/__init__.py
--rw-r--r--   0        0        0     2729 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/admin.py
--rw-r--r--   0        0        0      107 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/api.py
--rw-r--r--   0        0        0      472 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/apps.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/backends/__init__.py
--rw-r--r--   0        0        0      739 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/backends/celery.py
--rw-r--r--   0        0        0     1646 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/backends/storage.py
--rw-r--r--   0        0        0     4300 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/base.py
--rw-r--r--   0        0        0     1149 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/local_defaults.py
--rw-r--r--   0        0        0     2050 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/production_defaults.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/__init__.py
--rw-r--r--   0        0        0     9296 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/admin.py
--rw-r--r--   0        0        0     3361 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/api.py
--rw-r--r--   0        0        0     3640 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/authentication.py
--rw-r--r--   0        0        0      476 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/cache.py
--rw-r--r--   0        0        0     1801 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/celery.py
--rw-r--r--   0        0        0     1171 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/cms.py
--rw-r--r--   0        0        0      235 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/comments.py
--rw-r--r--   0        0        0      116 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/configuration.py
--rw-r--r--   0        0        0      937 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/database.py
--rw-r--r--   0        0        0      601 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/email.py
--rw-r--r--   0        0        0     7389 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/general.py
--rw-r--r--   0        0        0      317 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/invitations.py
--rw-r--r--   0        0        0      434 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/language.py
--rw-r--r--   0        0        0      298 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/lockdown.py
--rw-r--r--   0        0        0      885 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/logging.py
--rw-r--r--   0        0        0      545 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/security.py
--rw-r--r--   0        0        0      177 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/seo.py
--rw-r--r--   0        0        0     1370 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/static.py
--rw-r--r--   0        0        0      703 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/storage.py
--rw-r--r--   0        0        0      534 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/conf/settings/thumbnailer.py
--rw-r--r--   0        0        0      393 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/__init__.py
--rw-r--r--   0        0        0      184 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/__init__.py
--rw-r--r--   0        0        0      244 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/apps.py
--rw-r--r--   0        0        0     3064 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/mixins.py
--rw-r--r--   0        0        0     4579 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/monkeypatch.py
--rw-r--r--   0        0        0    21920 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/admin/base.html
--rw-r--r--   0        0        0       32 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/admin/base_site.html
--rw-r--r--   0        0        0      547 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/admin/change_list_object_tools.html
--rw-r--r--   0        0        0     1041 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/django_spaghetti/plate.html
--rw-r--r--   0        0        0    15565 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/jazzmin_translate/application.html
--rw-r--r--   0        0        0     2758 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/jazzmin_translate/base.html
--rw-r--r--   0        0        0     4519 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/jazzmin_translate/index.html
--rw-r--r--   0        0        0     3401 2023-05-08 12:24:18.010423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/jazzmin_translate/language.html
--rw-r--r--   0        0        0     4559 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/admin/templates/postgres_metrics/table.html
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/admin/tests/__init__.py
--rw-r--r--   0        0        0      910 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/admin/tests/test_urls.py
--rw-r--r--   0        0        0     1455 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/admin/urls.py
--rw-r--r--   0        0        0     5744 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/admin/views.py
--rw-r--r--   0        0        0      183 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/__init__.py
--rw-r--r--   0        0        0      476 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/access_policies.py
--rw-r--r--   0        0        0      188 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/apps.py
--rw-r--r--   0        0        0      282 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/menus.py
--rw-r--r--   0        0        0      422 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/permissions.py
--rw-r--r--   0        0        0      333 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/renderers.py
--rw-r--r--   0        0        0      443 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/throttling.py
--rw-r--r--   0        0        0      441 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/urls.py
--rw-r--r--   0        0        0      722 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/utils.py
--rw-r--r--   0        0        0       51 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/v1/__init__.py
--rw-r--r--   0        0        0      919 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/v1/serializers.py
--rw-r--r--   0        0        0      857 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/v1/urls.py
--rw-r--r--   0        0        0     2716 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/api/v1/views.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/gis/__init__.py
--rw-r--r--   0        0        0      497 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/gis/admin.py
--rw-r--r--   0        0        0      572 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/gis/db_functions.py
--rw-r--r--   0        0        0     2160 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/gis/managers.py
--rw-r--r--   0        0        0     1273 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/gis/serializers.py
--rw-r--r--   0        0        0      271 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/gis/urls.py
--rw-r--r--   0        0        0     1474 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/gis/views.py
--rw-r--r--   0        0        0      303 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/__init__.py
--rw-r--r--   0        0        0      576 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/admin.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/api/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/api/serialize.py
--rw-r--r--   0        0        0      356 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/api/urls.py
--rw-r--r--   0        0        0     2694 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/api/views.py
--rw-r--r--   0        0        0      242 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/apps.py
--rw-r--r--   0        0        0     2472 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/filters.py
--rw-r--r--   0        0        0      609 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/menus.py
--rw-r--r--   0        0        0      515 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/migrations/__init__.py
--rw-r--r--   0        0        0     1218 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/models.py
--rw-r--r--   0        0        0      477 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/urls.py
--rw-r--r--   0        0        0     2466 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/literature/views.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/__init__.py
--rw-r--r--   0        0        0      595 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/adapters.py
--rw-r--r--   0        0        0     2029 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/admin.py
--rw-r--r--   0        0        0      207 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/apps.py
--rw-r--r--   0        0        0     4618 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/forms.py
--rw-r--r--   0        0        0     1481 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/managers.py
--rw-r--r--   0        0        0     6017 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/migrations/0001_initial.py
--rw-r--r--   0        0        0      853 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/migrations/0002_auto_20230301_1346.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/migrations/__init__.py
--rw-r--r--   0        0        0     1856 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/models.py
--rw-r--r--   0        0        0      920 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/signals.py
--rw-r--r--   0        0        0      238 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/account_inactive.html
--rw-r--r--   0        0        0      192 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/activation_email.html
--rw-r--r--   0        0        0      413 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/base.html
--rw-r--r--   0        0        0      249 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email/base_message.txt
--rw-r--r--   0        0        0      484 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0        0        0       61 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email/email_confirmation_signup_message.txt
--rw-r--r--   0        0        0       61 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email/email_confirmation_signup_subject.txt
--rw-r--r--   0        0        0      127 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email/email_confirmation_subject.txt
--rw-r--r--   0        0        0      530 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email/password_reset_key_message.txt
--rw-r--r--   0        0        0      114 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email/password_reset_key_subject.txt
--rw-r--r--   0        0        0     3828 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email.html
--rw-r--r--   0        0        0      924 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email_confirm.html
--rw-r--r--   0        0        0      218 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/logged_out.html
--rw-r--r--   0        0        0      933 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/login.html
--rw-r--r--   0        0        0      514 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/logout.html
--rw-r--r--   0        0        0      110 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/cannot_delete_primary_email.txt
--rw-r--r--   0        0        0      238 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/email_confirmation_resend.txt
--rw-r--r--   0        0        0       99 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/email_confirmation_sent.txt
--rw-r--r--   0        0        0       81 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/email_confirmed.txt
--rw-r--r--   0        0        0       85 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/email_deleted.txt
--rw-r--r--   0        0        0      138 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/logged_in.txt
--rw-r--r--   0        0        0       72 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/logged_out.txt
--rw-r--r--   0        0        0       82 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/password_changed.txt
--rw-r--r--   0        0        0       78 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/password_set.txt
--rw-r--r--   0        0        0       79 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/primary_email_set.txt
--rw-r--r--   0        0        0       97 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/messages/unverified_primary_email.txt
--rw-r--r--   0        0        0      301 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/orcid/login.html
--rw-r--r--   0        0        0      521 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_change.html
--rw-r--r--   0        0        0     1022 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_reset.html
--rw-r--r--   0        0        0      471 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_reset_done.html
--rw-r--r--   0        0        0      939 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      248 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      418 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_set.html
--rw-r--r--   0        0        0     1812 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/signup.html
--rw-r--r--   0        0        0      261 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/signup_closed.html
--rw-r--r--   0        0        0      432 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/verification_sent.html
--rw-r--r--   0        0        0      794 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/account/verified_email_required.html
--rw-r--r--   0        0        0      659 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/base.html
--rw-r--r--   0        0        0      366 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/components/form_success.html
--rw-r--r--   0        0        0     1314 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/connected_accounts.html
--rw-r--r--   0        0        0     1990 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/email.html
--rw-r--r--   0        0        0      212 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/login_or_register.html
--rw-r--r--   0        0        0      166 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modal_link.html
--rw-r--r--   0        0        0     1115 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/add_email.html
--rw-r--r--   0        0        0     1139 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/change_password.html
--rw-r--r--   0        0        0     1096 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/deactivate_account.html
--rw-r--r--   0        0        0     1370 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/forgot_password.html
--rw-r--r--   0        0        0     1901 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/login.html
--rw-r--r--   0        0        0     1163 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/register.html
--rw-r--r--   0        0        0     2716 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/navbar_widget.html
--rw-r--r--   0        0        0      941 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/settings.html
--rw-r--r--   0        0        0      402 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/dashboard/panels/projects.html
--rw-r--r--   0        0        0      567 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/dashboard/panels/publications.html
--rw-r--r--   0        0        0     1072 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/dashboard/sections/orcid.html
--rw-r--r--   0        0        0      321 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0     1653 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/socialaccount/connections.html
--rw-r--r--   0        0        0      828 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/socialaccount/login.html
--rw-r--r--   0        0        0      433 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/socialaccount/login_cancelled.html
--rw-r--r--   0        0        0      831 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/socialaccount/signup.html
--rw-r--r--   0        0        0      595 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/user/account.html
--rw-r--r--   0        0        0      532 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/user/community.html
--rw-r--r--   0        0        0      433 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/user/components/account_sidebar.html
--rw-r--r--   0        0        0      503 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/user/components/add_email_modal.html
--rw-r--r--   0        0        0      578 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/user/dashboard.html
--rw-r--r--   0        0        0      505 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/user/profile.html
--rw-r--r--   0        0        0      529 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templates/user/why_orcid.html
--rw-r--r--   0        0        0     1249 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/templatetags/authentication.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/tests/__init__.py
--rw-r--r--   0        0        0      985 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/tests/factories.py
--rw-r--r--   0        0        0     1148 2023-05-08 12:24:18.014423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_admin.py
--rw-r--r--   0        0        0      683 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_drf_urls.py
--rw-r--r--   0        0        0      912 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_drf_views.py
--rw-r--r--   0        0        0     1282 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_forms.py
--rw-r--r--   0        0        0      184 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_models.py
--rw-r--r--   0        0        0      609 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_swagger.py
--rw-r--r--   0        0        0      581 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_tasks.py
--rw-r--r--   0        0        0      680 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_urls.py
--rw-r--r--   0        0        0     3661 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/tests/test_views.py
--rw-r--r--   0        0        0      378 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/urls.py
--rw-r--r--   0        0        0      402 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/utils.py
--rw-r--r--   0        0        0     2321 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/contrib/user/views.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/__init__.py
--rw-r--r--   0        0        0     1192 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/datatables/__init__.py
--rw-r--r--   0        0        0      937 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/datatables/adapters.py
--rw-r--r--   0        0        0      574 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/datatables/apps.py
--rw-r--r--   0        0        0     1213 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/datatables/metadata.py
--rw-r--r--   0        0        0     4298 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/datatables/renderers.py
--rw-r--r--   0        0        0      756 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/datatables/spectacular.py
--rw-r--r--   0        0        0      577 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/datatables/urls.py
--rw-r--r--   0        0        0     3746 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/datatables/views.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/forms/__init__.py
--rw-r--r--   0        0        0     2040 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/forms/fields.py
--rw-r--r--   0        0        0     2802 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/forms/widgets.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/management/commands/__init__.py
--rw-r--r--   0        0        0      622 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/management/commands/celery_worker.py
--rw-r--r--   0        0        0      343 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/management/commands/geoluminate.py
--rw-r--r--   0        0        0      818 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/mixins.py
--rw-r--r--   0        0        0     1299 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/core/validators.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/db/__init__.py
--rw-r--r--   0        0        0     3191 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/db/fields.py
--rw-r--r--   0        0        0     2012 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/db/models.py
--rw-r--r--   0        0        0      459 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/forms.py
--rw-r--r--   0        0        0      435 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/menus.py
--rw-r--r--   0        0        0     6841 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/middleware.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/migrations/__init__.py
--rw-r--r--   0        0        0     8415 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/models.py
--rw-r--r--   0        0        0     1102 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/static/admin/css/custom-admin.min.css
--rw-r--r--   0        0        0      482 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/static/admin/css/custom-admin.min.css.map
--rw-r--r--   0        0        0     1329 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/static/admin/css/custom-admin.scss
--rw-r--r--   0        0        0      152 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/static/admin/js/array_select2_tag.js
--rw-r--r--   0        0        0     1005 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/static/geoluminate/css/custom-admin.min.css
--rw-r--r--   0        0        0      523 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/static/geoluminate/css/custom-admin.min.css.map
--rw-r--r--   0        0        0     1548 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/static/geoluminate/css/custom-admin.scss
--rw-r--r--   0        0        0   129352 2023-05-08 12:24:18.018423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.eot
--rw-r--r--   0        0        0   689922 2023-05-08 12:24:18.022423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.svg
--rw-r--r--   0        0        0   129048 2023-05-08 12:24:18.022423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    87352 2023-05-08 12:24:18.022423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.woff
--rw-r--r--   0        0        0    74508 2023-05-08 12:24:18.026423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    34388 2023-05-08 12:24:18.026423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.eot
--rw-r--r--   0        0        0   144451 2023-05-08 12:24:18.026423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.svg
--rw-r--r--   0        0        0    34092 2023-05-08 12:24:18.026423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    16804 2023-05-08 12:24:18.026423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.woff
--rw-r--r--   0        0        0    13580 2023-05-08 12:24:18.026423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   192116 2023-05-08 12:24:18.026423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.eot
--rw-r--r--   0        0        0   839388 2023-05-08 12:24:18.030423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.svg
--rw-r--r--   0        0        0   191832 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.ttf
--rw-r--r--   0        0        0    98020 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.woff
--rw-r--r--   0        0        0    75440 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    23032 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/brand.svg
--rw-r--r--   0        0        0    22489 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/icon.svg
--rw-r--r--   0        0        0    22489 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/icon_original.svg
--rw-r--r--   0        0        0    59514 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/logo.svg
--rw-r--r--   0        0        0    45386 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/logo_test.svg
--rw-r--r--   0        0        0    36930 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/original.svg
--rw-r--r--   0        0        0     1350 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/audio.svg
--rw-r--r--   0        0        0     1929 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/ball-triangle.svg
--rw-r--r--   0        0        0     2322 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/bars.svg
--rw-r--r--   0        0        0     1926 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/circles.svg
--rw-r--r--   0        0        0     2051 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/grid.svg
--rw-r--r--   0        0        0     1360 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/hearts.svg
--rw-r--r--   0        0        0      697 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/oval.svg
--rw-r--r--   0        0        0     1463 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/puff.svg
--rw-r--r--   0        0        0     1787 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/rings.svg
--rw-r--r--   0        0        0     2809 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/spinning-circles.svg
--rw-r--r--   0        0        0     1321 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/tail-spin.svg
--rw-r--r--   0        0        0     1973 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/js/comments.js
--rw-r--r--   0        0        0     2181 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/js/custom-admin.js
--rw-r--r--   0        0        0     2554 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/js/custom.js
--rw-r--r--   0        0        0     2118 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/js/jquery.shave.min.js
--rw-r--r--   0        0        0     2134 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/js/shave.min.js
--rw-r--r--   0        0        0     6066 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/js/spin.js
--rw-r--r--   0        0        0      266 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/_variables.scss
--rw-r--r--   0        0        0       65 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_dropdown.scss
--rw-r--r--   0        0        0     1196 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_header.scss
--rw-r--r--   0        0        0      206 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_indicators.scss
--rw-r--r--   0        0        0     1069 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_menu.scss
--rw-r--r--   0        0        0      298 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_scrollbar.scss
--rw-r--r--   0        0        0     1896 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_sidebar.scss
--rw-r--r--   0        0        0   201232 2023-05-08 12:24:18.034423 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/geoluminate.min.css
--rw-r--r--   0        0        0    76381 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/geoluminate.min.css.map
--rw-r--r--   0        0        0      980 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/geoluminate.scss
--rw-r--r--   0        0        0      271 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/layout/_application.scss
--rw-r--r--   0        0        0      416 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/layout/_main.scss
--rw-r--r--   0        0        0     2525 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/layout/_menu.scss
--rw-r--r--   0        0        0      470 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/layout/_navbar.scss
--rw-r--r--   0        0        0     7355 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/geoluminate/scss/libs/_vendor.scss
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/scss/stylesheet.scss
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/scss/variables.scss
--rw-r--r--   0        0        0    19735 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap.css
--rw-r--r--   0        0        0    17188 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap.min.css
--rw-r--r--   0        0        0    21579 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap4.css
--rw-r--r--   0        0        0    18818 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap4.min.css
--rw-r--r--   0        0        0    21653 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap5.css
--rw-r--r--   0        0        0    18884 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap5.min.css
--rw-r--r--   0        0        0    13118 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bulma.css
--rw-r--r--   0        0        0    11560 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bulma.min.css
--rw-r--r--   0        0        0    40176 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.dataTables.css
--rw-r--r--   0        0        0    35109 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.dataTables.min.css
--rw-r--r--   0        0        0    15928 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.foundation.css
--rw-r--r--   0        0        0    13974 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.foundation.min.css
--rw-r--r--   0        0        0    26109 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.jqueryui.css
--rw-r--r--   0        0        0    23211 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.jqueryui.min.css
--rw-r--r--   0        0        0    16904 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.semanticui.css
--rw-r--r--   0        0        0    14914 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.semanticui.min.css
--rw-r--r--   0        0        0     5266 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/fields.min.css
--rw-r--r--   0        0        0     3533 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/inline.min.css
--rw-r--r--   0        0        0     2869 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/main.min.css
--rw-r--r--   0        0        0       42 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/mixins.min.css
--rw-r--r--   0        0        0     1511 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/processing.min.css
--rw-r--r--   0        0        0     1946 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/upload.min.css
--rw-r--r--   0        0        0   244165 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/dataTables.editor.js
--rw-r--r--   0        0        0    78939 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/dataTables.editor.min.js
--rw-r--r--   0        0        0     5881 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap.js
--rw-r--r--   0        0        0     5556 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap.min.js
--rw-r--r--   0        0        0     5848 2023-05-08 12:24:18.038424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap4.js
--rw-r--r--   0        0        0     5608 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap4.min.js
--rw-r--r--   0        0        0     6134 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap5.js
--rw-r--r--   0        0        0     5820 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap5.min.js
--rw-r--r--   0        0        0     4912 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bulma.js
--rw-r--r--   0        0        0     5364 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bulma.min.js
--rw-r--r--   0        0        0      863 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.dataTables.js
--rw-r--r--   0        0        0      553 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.dataTables.min.js
--rw-r--r--   0        0        0     3189 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.foundation.js
--rw-r--r--   0        0        0     1799 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.foundation.min.js
--rw-r--r--   0        0        0     3818 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.jqueryui.js
--rw-r--r--   0        0        0     4468 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.jqueryui.min.js
--rw-r--r--   0        0        0     5005 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.semanticui.js
--rw-r--r--   0        0        0     2599 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.semanticui.min.js
--rw-r--r--   0        0        0      291 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/403.html
--rw-r--r--   0        0        0      279 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/404.html
--rw-r--r--   0        0        0      324 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/500.html
--rw-r--r--   0        0        0     1219 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/api/map_popup.html
--rw-r--r--   0        0        0     4485 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/base.html
--rw-r--r--   0        0        0      215 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/container.html
--rw-r--r--   0        0        0      204 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/django_social_share/templatetags/post_to_linkedin.html
--rw-r--r--   0        0        0      214 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/django_social_share/templatetags/save_to_pinterest.html
--rw-r--r--   0        0        0     3890 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/forms/checkbox.html
--rw-r--r--   0        0        0      258 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/forms/widgets/array_select2.html
--rw-r--r--   0        0        0     1120 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/forms/widgets/postgres_array_widget.html
--rw-r--r--   0        0        0     1188 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/forms/widgets/quantity_field.html
--rw-r--r--   0        0        0      242 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/fullwidth.html
--rw-r--r--   0        0        0      237 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/base_error.html
--rw-r--r--   0        0        0      496 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/bootstrap/card.html
--rw-r--r--   0        0        0     1057 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/bootstrap/modal.html
--rw-r--r--   0        0        0     1040 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/cms/menu.html
--rw-r--r--   0        0        0     1632 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/app_menu.html
--rw-r--r--   0        0        0      572 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/app_submenu.html
--rw-r--r--   0        0        0      360 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/comments.html
--rw-r--r--   0        0        0      588 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/messages.html
--rw-r--r--   0        0        0      726 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/modal.html
--rw-r--r--   0        0        0      743 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/offcanvas.html
--rw-r--r--   0        0        0     2424 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/paginator.html
--rw-r--r--   0        0        0      561 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/sidebar.html
--rw-r--r--   0        0        0      742 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/components/socials.html
--rw-r--r--   0        0        0      889 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/database/site.html
--rw-r--r--   0        0        0      950 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/layout/navbar.html
--rw-r--r--   0        0        0     1176 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/layout/partials/sidebar_menu.html
--rw-r--r--   0        0        0     1141 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/layout/sidebar.html
--rw-r--r--   0        0        0     5815 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/application.html
--rw-r--r--   0        0        0     1172 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/modals/datasource.html
--rw-r--r--   0        0        0     7159 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/modals/datatable.html
--rw-r--r--   0        0        0     3352 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/modals/layer_settings.html
--rw-r--r--   0        0        0      297 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/modals/snapshot.html
--rw-r--r--   0        0        0     1797 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/sidebars/basemaps.html
--rw-r--r--   0        0        0     2423 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/sidebars/layers.html
--rw-r--r--   0        0        0     1881 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/partials/map.html
--rw-r--r--   0        0        0     2447 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/partials/sidebar.html
--rw-r--r--   0        0        0      716 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/modals/form.html
--rw-r--r--   0        0        0      486 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/modals/header.html
--rw-r--r--   0        0        0     1261 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/spectacular.html
--rw-r--r--   0        0        0       38 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/utils/cms_toolbar.html
--rw-r--r--   0        0        0     5815 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/utils/map.html
--rw-r--r--   0        0        0      438 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/utils/screen-size-indicator.html
--rw-r--r--   0        0        0     2253 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/widgets/nav/theme_switcher.html
--rw-r--r--   0        0        0      998 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/geoluminate/widgets/nav/user_affiliation.html
--rw-r--r--   0        0        0     3523 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/literature/admin/change_list.html
--rw-r--r--   0        0        0     1867 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/literature/admin/search.html
--rw-r--r--   0        0        0      824 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/literature/authors_list.html
--rw-r--r--   0        0        0     1737 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/literature/citation/publication.html
--rw-r--r--   0        0        0     2136 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/literature/literature_list copy.html
--rw-r--r--   0        0        0     6036 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/literature/literature_list.html
--rw-r--r--   0        0        0      463 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/lockdown/form.html
--rw-r--r--   0        0        0      290 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templates/placeholder.html
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templatetags/__init__.py
--rw-r--r--   0        0        0     2325 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/templatetags/geoluminate.py
--rw-r--r--   0        0        0     1810 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/urls.py
--rw-r--r--   0        0        0     1039 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/__init__.py
--rw-r--r--   0        0        0      722 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/drf.py
--rw-r--r--   0        0        0      295 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/generic.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/import_export/__init__.py
--rw-r--r--   0        0        0     4439 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/import_export/mixins.py
--rw-r--r--   0        0        0     1408 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/import_export/widgets.py
--rw-r--r--   0        0        0     3444 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/paginators.py
--rw-r--r--   0        0        0        0 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/select2/__init__.py
--rw-r--r--   0        0        0     1015 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/select2/filters.py
--rw-r--r--   0        0        0     1271 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/utils/select2/widgets.py
--rw-r--r--   0        0        0     1996 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/views.py
--rw-r--r--   0        0        0      580 2023-05-08 12:24:18.042424 geoluminate-0.0.1/geoluminate/widgets.py
--rw-r--r--   0        0        0     6768 2023-05-08 12:24:46.935144 geoluminate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6108 1970-01-01 00:00:00.000000 geoluminate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-13 22:42:19.726753 geoluminate-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2181 2023-05-13 22:42:19.726753 geoluminate-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/__init__.py
+-rw-r--r--   0        0        0     2729 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/admin.py
+-rw-r--r--   0        0        0      107 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/api.py
+-rw-r--r--   0        0        0      472 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/apps.py
+-rw-r--r--   0        0        0        1 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/backends/__init__.py
+-rw-r--r--   0        0        0      739 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/backends/celery.py
+-rw-r--r--   0        0        0     1646 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/backends/storage.py
+-rw-r--r--   0        0        0      942 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/local.py
+-rw-r--r--   0        0        0     3043 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/production.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/__init__.py
+-rw-r--r--   0        0        0     9375 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/admin.py
+-rw-r--r--   0        0        0     3521 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/api.py
+-rw-r--r--   0        0        0     3747 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/authentication.py
+-rw-r--r--   0        0        0      918 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/cache.py
+-rw-r--r--   0        0        0     2166 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/celery.py
+-rw-r--r--   0        0        0     1171 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/cms.py
+-rw-r--r--   0        0        0      235 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/comments.py
+-rw-r--r--   0        0        0      116 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/configuration.py
+-rw-r--r--   0        0        0      816 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/database.py
+-rw-r--r--   0        0        0     1073 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/email.py
+-rw-r--r--   0        0        0    10093 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/general.py
+-rw-r--r--   0        0        0      317 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/invitations.py
+-rw-r--r--   0        0        0      208 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/language.py
+-rw-r--r--   0        0        0      251 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/lockdown.py
+-rw-r--r--   0        0        0     1409 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/logging.py
+-rw-r--r--   0        0        0      545 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/security.py
+-rw-r--r--   0        0        0      177 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/seo.py
+-rw-r--r--   0        0        0     1708 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/staticfiles.py
+-rw-r--r--   0        0        0      703 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/storage.py
+-rw-r--r--   0        0        0      453 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/settings/thumbnailer.py
+-rw-r--r--   0        0        0     1047 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/conf/setup.py
+-rw-r--r--   0        0        0      393 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/apps.py
+-rw-r--r--   0        0        0     3064 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/mixins.py
+-rw-r--r--   0        0        0     4579 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/monkeypatch.py
+-rw-r--r--   0        0        0    21920 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/admin/base.html
+-rw-r--r--   0        0        0       32 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/admin/base_site.html
+-rw-r--r--   0        0        0      547 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/admin/change_list_object_tools.html
+-rw-r--r--   0        0        0     2540 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/admin/includes/fieldset.html
+-rw-r--r--   0        0        0     1041 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/django_spaghetti/plate.html
+-rw-r--r--   0        0        0    15565 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/jazzmin_translate/application.html
+-rw-r--r--   0        0        0     2758 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/jazzmin_translate/base.html
+-rw-r--r--   0        0        0     4519 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/jazzmin_translate/index.html
+-rw-r--r--   0        0        0     3401 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/jazzmin_translate/language.html
+-rw-r--r--   0        0        0     4559 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/templates/postgres_metrics/table.html
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/tests/__init__.py
+-rw-r--r--   0        0        0      910 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/tests/test_urls.py
+-rw-r--r--   0        0        0     1455 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/urls.py
+-rw-r--r--   0        0        0     5744 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/admin/views.py
+-rw-r--r--   0        0        0      183 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/__init__.py
+-rw-r--r--   0        0        0      476 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/access_policies.py
+-rw-r--r--   0        0        0      188 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/apps.py
+-rw-r--r--   0        0        0      282 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/menus.py
+-rw-r--r--   0        0        0      422 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/permissions.py
+-rw-r--r--   0        0        0      333 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/renderers.py
+-rw-r--r--   0        0        0      443 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/throttling.py
+-rw-r--r--   0        0        0      441 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/urls.py
+-rw-r--r--   0        0        0      722 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/utils.py
+-rw-r--r--   0        0        0       51 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/v1/__init__.py
+-rw-r--r--   0        0        0      919 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/v1/serializers.py
+-rw-r--r--   0        0        0      857 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/v1/urls.py
+-rw-r--r--   0        0        0     2716 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/api/v1/views.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/__init__.py
+-rw-r--r--   0        0        0     2281 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/admin.py
+-rw-r--r--   0        0        0     1616 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/apps.py
+-rw-r--r--   0        0        0     1630 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/fields.py
+-rw-r--r--   0        0        0      993 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/migrations/0001_initial.py
+-rw-r--r--   0        0        0    35513 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/migrations/0002_controlledvocabulary_description_af_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/migrations/__init__.py
+-rw-r--r--   0        0        0      675 2023-05-13 22:42:19.734753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/models.py
+-rw-r--r--   0        0        0   141915 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/static/vocabulary/js/jstree.min.js
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/templates/admin/hidden_filter.html
+-rw-r--r--   0        0        0       43 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/templates/vocabulary/change_list.html
+-rw-r--r--   0        0        0      232 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/controlled_vocabulary/translation.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/gis/__init__.py
+-rw-r--r--   0        0        0      497 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/gis/admin.py
+-rw-r--r--   0        0        0      572 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/gis/db_functions.py
+-rw-r--r--   0        0        0     2160 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/gis/managers.py
+-rw-r--r--   0        0        0     1273 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/gis/serializers.py
+-rw-r--r--   0        0        0      271 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/gis/urls.py
+-rw-r--r--   0        0        0     1474 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/gis/views.py
+-rw-r--r--   0        0        0      303 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/admin.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/api/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/api/serialize.py
+-rw-r--r--   0        0        0      356 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/api/urls.py
+-rw-r--r--   0        0        0     2694 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/api/views.py
+-rw-r--r--   0        0        0      242 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/apps.py
+-rw-r--r--   0        0        0     2474 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/filters.py
+-rw-r--r--   0        0        0      609 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/menus.py
+-rw-r--r--   0        0        0      514 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/migrations/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/models.py
+-rw-r--r--   0        0        0      477 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/urls.py
+-rw-r--r--   0        0        0     2466 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/literature/views.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/__init__.py
+-rw-r--r--   0        0        0      595 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/adapters.py
+-rw-r--r--   0        0        0     2029 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/admin.py
+-rw-r--r--   0        0        0      207 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/apps.py
+-rw-r--r--   0        0        0     4618 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/forms.py
+-rw-r--r--   0        0        0     1481 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/managers.py
+-rw-r--r--   0        0        0     2596 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/menus.py
+-rw-r--r--   0        0        0     6017 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/migrations/0001_initial.py
+-rw-r--r--   0        0        0      853 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/migrations/0002_auto_20230301_1346.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/migrations/__init__.py
+-rw-r--r--   0        0        0     1905 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/models.py
+-rw-r--r--   0        0        0      920 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/signals.py
+-rw-r--r--   0        0        0      238 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      192 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/activation_email.html
+-rw-r--r--   0        0        0      413 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/base.html
+-rw-r--r--   0        0        0      249 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email/base_message.txt
+-rw-r--r--   0        0        0      484 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0        0        0       61 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email/email_confirmation_signup_message.txt
+-rw-r--r--   0        0        0       61 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email/email_confirmation_signup_subject.txt
+-rw-r--r--   0        0        0      127 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email/email_confirmation_subject.txt
+-rw-r--r--   0        0        0      530 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email/password_reset_key_message.txt
+-rw-r--r--   0        0        0      114 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email/password_reset_key_subject.txt
+-rw-r--r--   0        0        0     3828 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email.html
+-rw-r--r--   0        0        0      924 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email_confirm.html
+-rw-r--r--   0        0        0      218 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/logged_out.html
+-rw-r--r--   0        0        0      933 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/login.html
+-rw-r--r--   0        0        0      514 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/logout.html
+-rw-r--r--   0        0        0      110 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/cannot_delete_primary_email.txt
+-rw-r--r--   0        0        0      238 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/email_confirmation_resend.txt
+-rw-r--r--   0        0        0       99 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/email_confirmation_sent.txt
+-rw-r--r--   0        0        0       81 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/email_confirmed.txt
+-rw-r--r--   0        0        0       85 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/email_deleted.txt
+-rw-r--r--   0        0        0      138 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/logged_in.txt
+-rw-r--r--   0        0        0       72 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/logged_out.txt
+-rw-r--r--   0        0        0       82 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/password_changed.txt
+-rw-r--r--   0        0        0       78 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/password_set.txt
+-rw-r--r--   0        0        0       79 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/primary_email_set.txt
+-rw-r--r--   0        0        0       97 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/messages/unverified_primary_email.txt
+-rw-r--r--   0        0        0      301 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/orcid/login.html
+-rw-r--r--   0        0        0      521 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_change.html
+-rw-r--r--   0        0        0     1022 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_reset.html
+-rw-r--r--   0        0        0      471 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0      939 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      248 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      418 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_set.html
+-rw-r--r--   0        0        0     1812 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/signup.html
+-rw-r--r--   0        0        0      261 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      432 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      794 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/account/verified_email_required.html
+-rw-r--r--   0        0        0      659 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/base.html
+-rw-r--r--   0        0        0      366 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/components/form_success.html
+-rw-r--r--   0        0        0     1314 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/connected_accounts.html
+-rw-r--r--   0        0        0     1990 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/email.html
+-rw-r--r--   0        0        0      212 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/login_or_register.html
+-rw-r--r--   0        0        0      166 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modal_link.html
+-rw-r--r--   0        0        0     1115 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/add_email.html
+-rw-r--r--   0        0        0     1139 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/change_password.html
+-rw-r--r--   0        0        0     1096 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/deactivate_account.html
+-rw-r--r--   0        0        0     1370 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/forgot_password.html
+-rw-r--r--   0        0        0     1901 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/login.html
+-rw-r--r--   0        0        0     1163 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/register.html
+-rw-r--r--   0        0        0     2705 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/navbar_widget.html
+-rw-r--r--   0        0        0      941 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/settings.html
+-rw-r--r--   0        0        0      402 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/dashboard/panels/projects.html
+-rw-r--r--   0        0        0      567 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/dashboard/panels/publications.html
+-rw-r--r--   0        0        0     1072 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/dashboard/sections/orcid.html
+-rw-r--r--   0        0        0      321 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0     1653 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0      828 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      433 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0        0        0      831 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0      595 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/user/account.html
+-rw-r--r--   0        0        0      532 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/user/community.html
+-rw-r--r--   0        0        0      433 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/user/components/account_sidebar.html
+-rw-r--r--   0        0        0      503 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/user/components/add_email_modal.html
+-rw-r--r--   0        0        0      578 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/user/dashboard.html
+-rw-r--r--   0        0        0      505 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/user/profile.html
+-rw-r--r--   0        0        0      529 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templates/user/why_orcid.html
+-rw-r--r--   0        0        0     1249 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/templatetags/authentication.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/__init__.py
+-rw-r--r--   0        0        0      985 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/factories.py
+-rw-r--r--   0        0        0     1148 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_admin.py
+-rw-r--r--   0        0        0      683 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_drf_urls.py
+-rw-r--r--   0        0        0      912 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_drf_views.py
+-rw-r--r--   0        0        0     1282 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_forms.py
+-rw-r--r--   0        0        0      184 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_models.py
+-rw-r--r--   0        0        0      609 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_swagger.py
+-rw-r--r--   0        0        0      581 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_tasks.py
+-rw-r--r--   0        0        0      680 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_urls.py
+-rw-r--r--   0        0        0     3661 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/tests/test_views.py
+-rw-r--r--   0        0        0      373 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/urls.py
+-rw-r--r--   0        0        0      402 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/utils.py
+-rw-r--r--   0        0        0     2317 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/contrib/user/views.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/core/__init__.py
+-rw-r--r--   0        0        0     1192 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/core/datatables/__init__.py
+-rw-r--r--   0        0        0      937 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/core/datatables/adapters.py
+-rw-r--r--   0        0        0      574 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/core/datatables/apps.py
+-rw-r--r--   0        0        0     1213 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/core/datatables/metadata.py
+-rw-r--r--   0        0        0     4298 2023-05-13 22:42:19.738753 geoluminate-0.0.2/geoluminate/core/datatables/renderers.py
+-rw-r--r--   0        0        0      756 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/core/datatables/spectacular.py
+-rw-r--r--   0        0        0      577 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/core/datatables/urls.py
+-rw-r--r--   0        0        0     3746 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/core/datatables/views.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/core/forms/__init__.py
+-rw-r--r--   0        0        0     2040 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/core/forms/fields.py
+-rw-r--r--   0        0        0     2802 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/core/forms/widgets.py
+-rw-r--r--   0        0        0      818 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/core/mixins.py
+-rw-r--r--   0        0        0     1299 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/core/validators.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/db/__init__.py
+-rw-r--r--   0        0        0     3191 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/db/fields.py
+-rw-r--r--   0        0        0     2012 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/db/models.py
+-rw-r--r--   0        0        0      459 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/forms.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/management/commands/__init__.py
+-rw-r--r--   0        0        0      622 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/management/commands/celery_worker.py
+-rw-r--r--   0        0        0      343 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/management/commands/geoluminate.py
+-rw-r--r--   0        0        0      748 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/management/commands/init_superuser.py
+-rw-r--r--   0        0        0      227 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/management/commands/settings.py
+-rw-r--r--   0        0        0      435 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/menus.py
+-rw-r--r--   0        0        0     6841 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/middleware.py
+-rw-r--r--   0        0        0     7513 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1016 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/migrations/0002_initial.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/migrations/__init__.py
+-rw-r--r--   0        0        0     8415 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/models.py
+-rw-r--r--   0        0        0     1102 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/static/admin/css/custom-admin.min.css
+-rw-r--r--   0        0        0      482 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/static/admin/css/custom-admin.min.css.map
+-rw-r--r--   0        0        0     1329 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/static/admin/css/custom-admin.scss
+-rw-r--r--   0        0        0      152 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/static/admin/js/array_select2_tag.js
+-rw-r--r--   0        0        0     1005 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/static/geoluminate/css/custom-admin.min.css
+-rw-r--r--   0        0        0      523 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/static/geoluminate/css/custom-admin.min.css.map
+-rw-r--r--   0        0        0     1548 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/static/geoluminate/css/custom-admin.scss
+-rw-r--r--   0        0        0   129352 2023-05-13 22:42:19.742754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   689922 2023-05-13 22:42:19.746754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   129048 2023-05-13 22:42:19.746754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    87352 2023-05-13 22:42:19.746754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    74508 2023-05-13 22:42:19.746754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    34388 2023-05-13 22:42:19.746754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   144451 2023-05-13 22:42:19.750753 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    34092 2023-05-13 22:42:19.750753 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    16804 2023-05-13 22:42:19.750753 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    13580 2023-05-13 22:42:19.750753 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   192116 2023-05-13 22:42:19.750753 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   839388 2023-05-13 22:42:19.754754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   191832 2023-05-13 22:42:19.754754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0    98020 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    75440 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    23032 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/brand.svg
+-rw-r--r--   0        0        0    22489 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/icon.svg
+-rw-r--r--   0        0        0    22489 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/icon_original.svg
+-rw-r--r--   0        0        0    59514 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/logo.svg
+-rw-r--r--   0        0        0    45386 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/logo_test.svg
+-rw-r--r--   0        0        0    36930 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/original.svg
+-rw-r--r--   0        0        0     1350 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/audio.svg
+-rw-r--r--   0        0        0     1929 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/ball-triangle.svg
+-rw-r--r--   0        0        0     2322 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/bars.svg
+-rw-r--r--   0        0        0     1926 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/circles.svg
+-rw-r--r--   0        0        0     2051 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/grid.svg
+-rw-r--r--   0        0        0     1360 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/hearts.svg
+-rw-r--r--   0        0        0      697 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/oval.svg
+-rw-r--r--   0        0        0     1463 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/puff.svg
+-rw-r--r--   0        0        0     1787 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/rings.svg
+-rw-r--r--   0        0        0     2809 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/spinning-circles.svg
+-rw-r--r--   0        0        0     1321 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/tail-spin.svg
+-rw-r--r--   0        0        0     1973 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/js/comments.js
+-rw-r--r--   0        0        0     2181 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/js/custom-admin.js
+-rw-r--r--   0        0        0     2554 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/js/custom.js
+-rw-r--r--   0        0        0     2118 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/js/jquery.shave.min.js
+-rw-r--r--   0        0        0     3291 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/js/map.js
+-rw-r--r--   0        0        0     2134 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/js/shave.min.js
+-rw-r--r--   0        0        0     6066 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/js/spin.js
+-rw-r--r--   0        0        0      266 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/_variables.scss
+-rw-r--r--   0        0        0       65 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_dropdown.scss
+-rw-r--r--   0        0        0     1196 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_header.scss
+-rw-r--r--   0        0        0      206 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_indicators.scss
+-rw-r--r--   0        0        0     1069 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_menu.scss
+-rw-r--r--   0        0        0      298 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_scrollbar.scss
+-rw-r--r--   0        0        0     1809 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_sidebar.scss
+-rw-r--r--   0        0        0   201232 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/geoluminate.min.css
+-rw-r--r--   0        0        0    76381 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/geoluminate.min.css.map
+-rw-r--r--   0        0        0      980 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/geoluminate.scss
+-rw-r--r--   0        0        0      271 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/layout/_application.scss
+-rw-r--r--   0        0        0      416 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/layout/_main.scss
+-rw-r--r--   0        0        0     2525 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/layout/_menu.scss
+-rw-r--r--   0        0        0      470 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/layout/_navbar.scss
+-rw-r--r--   0        0        0     7355 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/geoluminate/scss/libs/_vendor.scss
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/scss/stylesheet.scss
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.758754 geoluminate-0.0.2/geoluminate/static/scss/variables.scss
+-rw-r--r--   0        0        0    19735 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap.css
+-rw-r--r--   0        0        0    17188 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap.min.css
+-rw-r--r--   0        0        0    21579 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap4.css
+-rw-r--r--   0        0        0    18818 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap4.min.css
+-rw-r--r--   0        0        0    21653 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap5.css
+-rw-r--r--   0        0        0    18884 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap5.min.css
+-rw-r--r--   0        0        0    13118 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bulma.css
+-rw-r--r--   0        0        0    11560 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bulma.min.css
+-rw-r--r--   0        0        0    40176 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.dataTables.css
+-rw-r--r--   0        0        0    35109 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.dataTables.min.css
+-rw-r--r--   0        0        0    15928 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.foundation.css
+-rw-r--r--   0        0        0    13974 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.foundation.min.css
+-rw-r--r--   0        0        0    26109 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.jqueryui.css
+-rw-r--r--   0        0        0    23211 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.jqueryui.min.css
+-rw-r--r--   0        0        0    16904 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.semanticui.css
+-rw-r--r--   0        0        0    14914 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.semanticui.min.css
+-rw-r--r--   0        0        0     5266 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/fields.min.css
+-rw-r--r--   0        0        0     3533 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/inline.min.css
+-rw-r--r--   0        0        0     2869 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/main.min.css
+-rw-r--r--   0        0        0       42 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/mixins.min.css
+-rw-r--r--   0        0        0     1511 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/processing.min.css
+-rw-r--r--   0        0        0     1946 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/upload.min.css
+-rw-r--r--   0        0        0   244165 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/dataTables.editor.js
+-rw-r--r--   0        0        0    78939 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/dataTables.editor.min.js
+-rw-r--r--   0        0        0     5881 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap.js
+-rw-r--r--   0        0        0     5556 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap.min.js
+-rw-r--r--   0        0        0     5848 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap4.js
+-rw-r--r--   0        0        0     5608 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap4.min.js
+-rw-r--r--   0        0        0     6134 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap5.js
+-rw-r--r--   0        0        0     5820 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap5.min.js
+-rw-r--r--   0        0        0     4912 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bulma.js
+-rw-r--r--   0        0        0     5364 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bulma.min.js
+-rw-r--r--   0        0        0      863 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.dataTables.js
+-rw-r--r--   0        0        0      553 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.dataTables.min.js
+-rw-r--r--   0        0        0     3189 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.foundation.js
+-rw-r--r--   0        0        0     1799 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.foundation.min.js
+-rw-r--r--   0        0        0     3818 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.jqueryui.js
+-rw-r--r--   0        0        0     4468 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.jqueryui.min.js
+-rw-r--r--   0        0        0     5005 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.semanticui.js
+-rw-r--r--   0        0        0     2599 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.semanticui.min.js
+-rw-r--r--   0        0        0      291 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/403.html
+-rw-r--r--   0        0        0      279 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/404.html
+-rw-r--r--   0        0        0      324 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/500.html
+-rw-r--r--   0        0        0     1219 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/api/map_popup.html
+-rw-r--r--   0        0        0     4485 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/base.html
+-rw-r--r--   0        0        0      215 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/container.html
+-rw-r--r--   0        0        0      204 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/django_social_share/templatetags/post_to_linkedin.html
+-rw-r--r--   0        0        0      214 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/django_social_share/templatetags/save_to_pinterest.html
+-rw-r--r--   0        0        0     3890 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/forms/checkbox.html
+-rw-r--r--   0        0        0      258 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/forms/widgets/array_select2.html
+-rw-r--r--   0        0        0     1120 2023-05-13 22:42:19.762754 geoluminate-0.0.2/geoluminate/templates/forms/widgets/postgres_array_widget.html
+-rw-r--r--   0        0        0     1188 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/forms/widgets/quantity_field.html
+-rw-r--r--   0        0        0      242 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/fullwidth.html
+-rw-r--r--   0        0        0      237 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/base_error.html
+-rw-r--r--   0        0        0      496 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/bootstrap/card.html
+-rw-r--r--   0        0        0     1057 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/bootstrap/modal.html
+-rw-r--r--   0        0        0     1040 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/cms/menu.html
+-rw-r--r--   0        0        0     1632 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/app_menu.html
+-rw-r--r--   0        0        0      572 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/app_submenu.html
+-rw-r--r--   0        0        0      360 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/comments.html
+-rw-r--r--   0        0        0      588 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/messages.html
+-rw-r--r--   0        0        0      726 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/modal.html
+-rw-r--r--   0        0        0      743 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/offcanvas.html
+-rw-r--r--   0        0        0     2424 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/paginator.html
+-rw-r--r--   0        0        0      575 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/sidebar.html
+-rw-r--r--   0        0        0      742 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/components/socials.html
+-rw-r--r--   0        0        0      889 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/database/site.html
+-rw-r--r--   0        0        0      950 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/layout/navbar.html
+-rw-r--r--   0        0        0     1176 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/layout/partials/sidebar_menu.html
+-rw-r--r--   0        0        0     1141 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/layout/sidebar.html
+-rw-r--r--   0        0        0     5815 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/application.html
+-rw-r--r--   0        0        0     1172 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/modals/datasource.html
+-rw-r--r--   0        0        0     7159 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/modals/datatable.html
+-rw-r--r--   0        0        0     3352 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/modals/layer_settings.html
+-rw-r--r--   0        0        0      297 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/modals/snapshot.html
+-rw-r--r--   0        0        0     1797 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/sidebars/basemaps.html
+-rw-r--r--   0        0        0     2423 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/sidebars/layers.html
+-rw-r--r--   0        0        0     1948 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/partials/map.html
+-rw-r--r--   0        0        0     2447 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/partials/sidebar.html
+-rw-r--r--   0        0        0      716 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/modals/form.html
+-rw-r--r--   0        0        0      486 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/modals/header.html
+-rw-r--r--   0        0        0     1261 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/spectacular.html
+-rw-r--r--   0        0        0       38 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/utils/cms_toolbar.html
+-rw-r--r--   0        0        0     5815 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/utils/map.html
+-rw-r--r--   0        0        0      438 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/utils/screen-size-indicator.html
+-rw-r--r--   0        0        0     2253 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/widgets/nav/theme_switcher.html
+-rw-r--r--   0        0        0      998 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/geoluminate/widgets/nav/user_affiliation.html
+-rw-r--r--   0        0        0     3523 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/literature/admin/change_list.html
+-rw-r--r--   0        0        0     1867 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/literature/admin/search.html
+-rw-r--r--   0        0        0      824 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/literature/authors_list.html
+-rw-r--r--   0        0        0     1737 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/literature/citation/publication.html
+-rw-r--r--   0        0        0     2136 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/literature/literature_list copy.html
+-rw-r--r--   0        0        0     6191 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/literature/literature_list.html
+-rw-r--r--   0        0        0      463 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/lockdown/form.html
+-rw-r--r--   0        0        0      290 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templates/placeholder.html
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templatetags/__init__.py
+-rw-r--r--   0        0        0     2325 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/templatetags/geoluminate.py
+-rw-r--r--   0        0        0     1856 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/urls.py
+-rw-r--r--   0        0        0     1039 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/drf.py
+-rw-r--r--   0        0        0      295 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/generic.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/import_export/__init__.py
+-rw-r--r--   0        0        0     4439 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/import_export/mixins.py
+-rw-r--r--   0        0        0     1408 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/import_export/widgets.py
+-rw-r--r--   0        0        0     3444 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/paginators.py
+-rw-r--r--   0        0        0        0 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/select2/__init__.py
+-rw-r--r--   0        0        0     1015 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/select2/filters.py
+-rw-r--r--   0        0        0     1271 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/utils/select2/widgets.py
+-rw-r--r--   0        0        0     1996 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/views.py
+-rw-r--r--   0        0        0      580 2023-05-13 22:42:19.766754 geoluminate-0.0.2/geoluminate/widgets.py
+-rw-r--r--   0        0        0     7024 2023-05-13 22:42:19.770754 geoluminate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6219 1970-01-01 00:00:00.000000 geoluminate-0.0.2/PKG-INFO
```

### Comparing `geoluminate-0.0.1/LICENSE` & `geoluminate-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/README.md` & `geoluminate-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 <!-- [![RTD](https://readthedocs.org/projects/geoluminate/badge/?version=latest)](https://geoluminate.readthedocs.io/en/latest/readme.html) -->
 <!-- [![Documentation](https://github.com/Geoluminate/geoluminate/actions/workflows/build-docs.yml/badge.svg)](https://github.com/Geoluminate/geoluminate/actions/workflows/build-docs.yml) -->
 <!-- [![PR](https://img.shields.io/github/issues-pr/Geoluminate/geoluminate)](https://github.com/Geoluminate/geoluminate/pulls)
 [![Issues](https://img.shields.io/github/issues-raw/Geoluminate/geoluminate)](https://github.com/Geoluminate/geoluminate/pulls) -->
 <!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/geoluminate) -->
 <!-- ![PyPI - Status](https://img.shields.io/pypi/status/geoluminate) -->
 
-A Django application for managing collections of scientific instruments
 
 Documentation
 -------------
 
-The full documentation is at https://ssjenny90.github.io/geoluminate/
+The full documentation is at https://geoluminate.github.io/geoluminate/
 
 Quickstart
 ----------
 
 Install Geoluminate::
 
     pip install geoluminate
```

### Comparing `geoluminate-0.0.1/geoluminate/admin.py` & `geoluminate-0.0.2/geoluminate/admin.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/conf/backends/celery.py` & `geoluminate-0.0.2/geoluminate/conf/backends/celery.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/conf/backends/storage.py` & `geoluminate-0.0.2/geoluminate/conf/backends/storage.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/conf/production_defaults.py` & `geoluminate-0.0.2/geoluminate/conf/production.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,37 @@
-from .base import *
+from split_settings.tools import include
+
+# imports all settings defined in the geoluminate/conf/settings/ directory
+include("settings/general.py", "settings/*.py")
+
+# https://docs.djangoproject.com/en/dev/ref/settings/#allowed-hosts
+ALLOWED_HOSTS = env.list("DJANGO_ALLOWED_HOSTS", default=["heatflow.world"])
+
+# DATABASES
+# ------------------------------------------------------------------------------
+DATABASES["default"]["CONN_MAX_AGE"] = env.int("CONN_MAX_AGE", default=60)  # noqa F405
+
+
+CACHES["DEFAULT"]["LOCATION"] = env("REDIS_URL")
 
 # SECURITY
 # ------------------------------------------------------------------------------
+
+# https://docs.djangoproject.com/en/dev/ref/settings/#secure-ssl-redirect
+SECURE_SSL_REDIRECT = env.bool("DJANGO_SECURE_SSL_REDIRECT", default=True)
+
+# https://docs.djangoproject.com/en/dev/ref/settings/#secure-hsts-include-subdomains
+SECURE_HSTS_INCLUDE_SUBDOMAINS = env.bool("DJANGO_SECURE_HSTS_INCLUDE_SUBDOMAINS", default=True)
+
+# https://docs.djangoproject.com/en/dev/ref/settings/#secure-hsts-preload
+SECURE_HSTS_PRELOAD = env.bool("DJANGO_SECURE_HSTS_PRELOAD", default=True)
+
+# https://docs.djangoproject.com/en/dev/ref/middleware/#x-content-type-options-nosniff
+SECURE_CONTENT_TYPE_NOSNIFF = env.bool("DJANGO_SECURE_CONTENT_TYPE_NOSNIFF", default=True)
+
 # https://docs.djangoproject.com/en/dev/ref/settings/#secure-proxy-ssl-header
 SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTO", "https")
 
 # https://docs.djangoproject.com/en/dev/ref/settings/#session-cookie-secure
 SESSION_COOKIE_SECURE = True
 
 # https://docs.djangoproject.com/en/dev/ref/settings/#csrf-cookie-secure
@@ -45,10 +71,7 @@
         "django.security.DisallowedHost": {
             "level": "ERROR",
             "handlers": ["console"],
             "propagate": False,
         },
     },
 }
-
-# https://django-compressor.readthedocs.io/en/latest/settings/#django.conf.settings.COMPRESS_ENABLED
-COMPRESS_ENABLED = env.bool("COMPRESS_ENABLED", default=True)  # type: ignore[name-defined]
```

### Comparing `geoluminate-0.0.1/geoluminate/conf/settings/admin.py` & `geoluminate-0.0.2/geoluminate/conf/settings/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.utils.translation import gettext_lazy as _
 
 JAZZMIN_SETTINGS = {
     # title of the window
-    "site_title": "Geoluminate Admin",
+    "site_title": SITE_NAME,
     # Title on the login screen (19 chars max) (defaults to current_admin_site.site_header if absent or None)
-    "site_header": "Geoluminate",
+    "site_header": SITE_NAME,
     # Title on the brand (19 chars max) (defaults to current_admin_site.site_header if absent or None)
     "site_brand": " ",
     # Logo to use for your site, must be present in static files, used for brand on top left
     "site_logo": "geoluminate/img/brand/logo.svg",
     # Logo to use for your site, must be present in static files, used for login form logo (defaults to site_logo)
     "login_logo": "geoluminate/img/brand/logo.svg",
     # Logo to use for login form in dark themes (defaults to login_logo)
@@ -17,15 +17,15 @@
     # "site_logo_classes": "img-circle",
     "site_logo_classes": "img-thumbnail shadow-none border-0",
     # Relative path to a favicon for your site, will default to site_logo if absent (ideally 32x32 px)
     "site_icon": "geoluminate/img/brand/icon.svg",
     # Welcome text on the login screen
     "welcome_sign": "Welcome to the library",
     # Copyright on the footer
-    "copyright": "Geoluminate Ltd",
+    "copyright": GEOLUMINATE["governance"]["name"],
     # List of model admins to search from the search bar, search bar omitted if excluded
     # If you want to use a single search field you dont need to use a list, you can use a simple string
     # "search_model": ["auth.User", "auth.Group"],
     # Field name on user model that contains avatar ImageField/URLField/Charfield or a callable that receives the user
     "user_avatar": False,
     ############
     # Top Menu #
@@ -101,15 +101,15 @@
         "laboratory",
         # "controlled_vocabulary",
         "literature",
         "fluent_comments",
     ],
     "hide_models": [],
     # List of apps (and/or models) to order the side menu
-    "order_with_respect_to": ["geoluminate"],
+    "order_with_respect_to": ["geoluminate", GEOLUMINATE["database"]["acronym"].lower()],
     # Custom links to append to app groups, keyed on app name
     "custom_links": {
         "geoluminate": [
             {
                 "name": _("Files"),
                 "url": "admin:filer_folder_changelist",
                 "icon": "fas fa-folder",
@@ -248,8 +248,8 @@
         "danger": "btn-danger",
         "success": "btn-success",
     },
     "actions_sticky_top": True,
 }
 
 # Django Admin URL.
-ADMIN_URL = "admin/"
+ADMIN_URL = env("DJANGO_ADMIN_URL", default="admin/")
```

### Comparing `geoluminate-0.0.1/geoluminate/conf/settings/api.py` & `geoluminate-0.0.2/geoluminate/conf/settings/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,31 +39,32 @@
     # 'DEFAULT_METADATA_CLASS': 'datatables.metadata.DatatablesAutoMetadata',
 }
 
 # By Default swagger ui is available only to admin user(s). You can change permission classes to change that
 # See more configuration options at https://drf-spectacular.readthedocs.io/en/latest/settings.html#settings
 SPECTACULAR_SETTINGS = {
     "SCHEMA_PATH_PREFIX": r"/api/v[0-9]",
-    "TITLE": "World Heat Flow Database API",
-    "DESCRIPTION": "Documentation for version 1.0 of the public API of the World Heat Flow Database Project.",
+    "TITLE": f"{SITE_NAME} API",
+    "DESCRIPTION": f"Documentation of API endpoints of {SITE_NAME}",
     "TOS": None,
     "VERSION": "1.0.0",
     "SERVE_INCLUDE_SCHEMA": False,
     "SERVE_PUBLIC": False,
     "SORT_OPERATIONS": False,
     "SORT_OPERATION_PARAMETERS": False,
     "SERVE_PERMISSIONS": ["rest_framework.permissions.IsAdminUser"],
     # OTHER SETTINGS
     # 'AUTHENTICATION_WHITELIST': ['rest_framework.authentication.BasicAuthentication',],
     "PARSER_WHITELIST": [],
     # 'RENDERER_WHITELIST': [
     #     'drf_orjson_renderer.renderers.ORJSONRenderer',
     #     # 'rest_framework_csv.renderers.PaginatedCSVRenderer',
     #     ],
-    "SERVERS": [],
+    # Tools that generate code samples can use SERVERS to point to the correct domain
+    "SERVERS": [{"url": GEOLUMINATE["application"]["domain"], "description": "Production server"}],
     # 'ENUM_NAME_OVERRIDES': {
     #     "TCorrTop/TCorrBot": "database.choices.TempCorrectionMethod",
     #     "TMethodTop/TMethodBot": "database.choices.TempMethod",
     #     },
     "TAGS": [],
     # Tags defined in the global scope
     "SWAGGER_UI_SETTINGS": {
@@ -76,7 +77,10 @@
     },
     "PREPROCESSING_HOOKS": ["geoluminate.core.datatables.spectacular.preprocessing_filter_spec"],
 }  # type: ignore[var-annotated]
 """"""
 
 # django-cors-headers - https://github.com/adamchainz/django-cors-headers#setup
 CORS_URLS_REGEX = r"^/api/.*$"
+
+
+SPECTACULAR_SETTINGS["SERVERS"] = []  # F405
```

### Comparing `geoluminate-0.0.1/geoluminate/conf/settings/authentication.py` & `geoluminate-0.0.2/geoluminate/conf/settings/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,7 +106,10 @@
         "MEMBER_API": False,
     }
 }
 """"""
 
 # https://django-allauth.readthedocs.io/en/latest/configuration.html
 SOCIALACCOUNT_ADAPTER = "geoluminate.contrib.user.adapters.SocialAccountAdapter"
+
+ACCOUNT_ALLOW_REGISTRATION = env.bool("DJANGO_ACCOUNT_ALLOW_REGISTRATION", True)
+"""allow registration"""
```

### Comparing `geoluminate-0.0.1/geoluminate/conf/settings/celery.py` & `geoluminate-0.0.2/geoluminate/conf/settings/celery.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,49 @@
-# Celery
-# ------------------------------------------------------------------------------
-# if USE_TZ:
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#std:setting-timezone
-CELERY_TIMEZONE = True
-
+CELERY_TIMEZONE = TIME_ZONE
 
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#result-extended
 CELERY_RESULT_EXTENDED = True
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#result-backend-always-retry
 # https://github.com/celery/celery/pull/6122
 CELERY_RESULT_BACKEND_ALWAYS_RETRY = True
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#result-backend-max-retries
 CELERY_RESULT_BACKEND_MAX_RETRIES = 10
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#std:setting-accept_content
 CELERY_ACCEPT_CONTENT = ["json"]
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#std:setting-task_serializer
 CELERY_TASK_SERIALIZER = "json"
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#std:setting-result_serializer
 CELERY_RESULT_SERIALIZER = "json"
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#task-time-limit
 # TODO: set to whatever value is adequate in your circumstances
 CELERY_TASK_TIME_LIMIT = 5 * 60
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#task-soft-time-limit
 # TODO: set to whatever value is adequate in your circumstances
 CELERY_TASK_SOFT_TIME_LIMIT = 60
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#beat-scheduler
 CELERY_BEAT_SCHEDULER = "django_celery_beat.schedulers:DatabaseScheduler"
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#worker-send-task-events
 CELERY_WORKER_SEND_TASK_EVENTS = True
+
 # https://docs.celeryq.dev/en/stable/userguide/configuration.html#std-setting-task_send_sent_event
 CELERY_TASK_SEND_SENT_EVENT = True
+
+# https://docs.celeryq.dev/en/stable/userguide/configuration.html#task-eager-propagates
+CELERY_TASK_EAGER_PROPAGATES = True
+
+# https://docs.celeryq.dev/en/stable/userguide/configuration.html#std:setting-broker_url
+CELERY_BROKER_URL = env("REDIS_URL", default="redis://redis:6379/0")
+
+# https://docs.celeryq.dev/en/stable/userguide/configuration.html#std:setting-result_backend
+CELERY_RESULT_BACKEND = CELERY_BROKER_URL
+
+CELERY_TASK_ALWAYS_EAGER = False
```

### Comparing `geoluminate-0.0.1/geoluminate/conf/settings/cms.py` & `geoluminate-0.0.2/geoluminate/conf/settings/cms.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/conf/settings/logging.py` & `geoluminate-0.0.2/geoluminate/conf/settings/logging.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,13 +15,27 @@
             "class": "logging.StreamHandler",
             "formatter": "verbose",
         }
     },
     "root": {"level": "INFO", "handlers": ["console"]},
 }
 
-
 SENTRY_INTEGRATIONS = [
     DjangoIntegration(),
     CeleryIntegration(),
     RedisIntegration(),
 ]
+
+# SENTRY_DSN = env("SENTRY_DSN")
+# SENTRY_LOG_LEVEL = env.int("DJANGO_SENTRY_LOG_LEVEL", logging.INFO)
+
+# sentry_logging = LoggingIntegration(
+#     level=SENTRY_LOG_LEVEL,  # Capture info and above as breadcrumbs
+#     event_level=logging.ERROR,  # Send errors as events
+# )
+
+# sentry_sdk.init(
+#     dsn=SENTRY_DSN,
+#     integrations=sentry_logging + SENTRY_INTEGRATIONS,
+#     environment=env("SENTRY_ENVIRONMENT", default="production"),
+#     traces_sample_rate=env.float("SENTRY_TRACES_SAMPLE_RATE", default=0.0),
+# )
```

### Comparing `geoluminate-0.0.1/geoluminate/conf/settings/security.py` & `geoluminate-0.0.2/geoluminate/conf/settings/security.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/conf/settings/storage.py` & `geoluminate-0.0.2/geoluminate/conf/settings/storage.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/mixins.py` & `geoluminate-0.0.2/geoluminate/contrib/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/monkeypatch.py` & `geoluminate-0.0.2/geoluminate/contrib/admin/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/templates/admin/base.html` & `geoluminate-0.0.2/geoluminate/contrib/admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/templates/admin/change_list_object_tools.html` & `geoluminate-0.0.2/geoluminate/contrib/admin/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/templates/django_spaghetti/plate.html` & `geoluminate-0.0.2/geoluminate/contrib/admin/templates/django_spaghetti/plate.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/templates/jazzmin_translate/application.html` & `geoluminate-0.0.2/geoluminate/contrib/admin/templates/jazzmin_translate/application.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/templates/jazzmin_translate/base.html` & `geoluminate-0.0.2/geoluminate/contrib/admin/templates/jazzmin_translate/base.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/templates/jazzmin_translate/index.html` & `geoluminate-0.0.2/geoluminate/contrib/admin/templates/jazzmin_translate/index.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/templates/jazzmin_translate/language.html` & `geoluminate-0.0.2/geoluminate/contrib/admin/templates/jazzmin_translate/language.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/templates/postgres_metrics/table.html` & `geoluminate-0.0.2/geoluminate/contrib/admin/templates/postgres_metrics/table.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/tests/test_urls.py` & `geoluminate-0.0.2/geoluminate/contrib/admin/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/urls.py` & `geoluminate-0.0.2/geoluminate/contrib/admin/urls.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/admin/views.py` & `geoluminate-0.0.2/geoluminate/contrib/admin/views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/api/utils.py` & `geoluminate-0.0.2/geoluminate/contrib/api/utils.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/api/v1/serializers.py` & `geoluminate-0.0.2/geoluminate/contrib/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/api/v1/urls.py` & `geoluminate-0.0.2/geoluminate/contrib/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/api/v1/views.py` & `geoluminate-0.0.2/geoluminate/contrib/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/gis/db_functions.py` & `geoluminate-0.0.2/geoluminate/contrib/gis/db_functions.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/gis/managers.py` & `geoluminate-0.0.2/geoluminate/contrib/gis/managers.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/gis/serializers.py` & `geoluminate-0.0.2/geoluminate/contrib/gis/serializers.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/gis/views.py` & `geoluminate-0.0.2/geoluminate/contrib/gis/views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/literature/admin.py` & `geoluminate-0.0.2/geoluminate/contrib/literature/admin.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/literature/api/serialize.py` & `geoluminate-0.0.2/geoluminate/contrib/literature/api/serialize.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/literature/api/views.py` & `geoluminate-0.0.2/geoluminate/contrib/literature/api/views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/literature/filters.py` & `geoluminate-0.0.2/geoluminate/contrib/literature/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class Small(Field):
     def __init__(self, *args, **kwargs):
         kwargs.update(css_class="form-control form-control-sm")
         super().__init__(*args, **kwargs)
 
 
 class PublicationFilter(df.FilterSet):
-    DOI = df.CharFilter(label="DOI", lookup_expr="exact")
+    # DOI = df.CharFilter(label="DOI", lookup_expr="exact")
     author = df.ModelMultipleChoiceFilter(
         label="Author/s",
         queryset=Author.objects.all(),
         widget=ModelSelect2MultipleWidget(
             model=Author,
             search_fields=[
                 "family__icontains",
```

### Comparing `geoluminate-0.0.1/geoluminate/contrib/literature/menus.py` & `geoluminate-0.0.2/geoluminate/contrib/literature/menus.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/literature/migrations/0001_initial.py` & `geoluminate-0.0.2/geoluminate/contrib/literature/migrations/0001_initial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 3.2.17 on 2023-02-01 15:19
+# Generated by Django 4.2.1 on 2023-05-10 16:44
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
     initial = True
```

### Comparing `geoluminate-0.0.1/geoluminate/contrib/literature/views.py` & `geoluminate-0.0.2/geoluminate/contrib/literature/views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/adapters.py` & `geoluminate-0.0.2/geoluminate/contrib/user/adapters.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/admin.py` & `geoluminate-0.0.2/geoluminate/contrib/user/admin.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/forms.py` & `geoluminate-0.0.2/geoluminate/contrib/user/forms.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/managers.py` & `geoluminate-0.0.2/geoluminate/contrib/user/managers.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/migrations/0001_initial.py` & `geoluminate-0.0.2/geoluminate/contrib/user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/migrations/0002_auto_20230301_1346.py` & `geoluminate-0.0.2/geoluminate/contrib/user/migrations/0002_auto_20230301_1346.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/models.py` & `geoluminate-0.0.2/geoluminate/contrib/user/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 from django.utils.translation import gettext_lazy as _
 from invitations.base_invitation import AbstractBaseInvitation
 
 from .managers import UserManager
 
 
 class User(AbstractUser):
-    objects = UserManager()
+    objects = UserManager()  # type: ignore[var-annotated]
 
     username = None  # type: ignore[assignment]
     email = models.EmailField(_("email address"), unique=True)
 
     USERNAME_FIELD = "email"
     REQUIRED_FIELDS = ["first_name", "last_name"]
 
     def __str__(self):
         if self.first_name and self.last_name:
             return f"{self.first_name[0]}.{self.last_name}"
+        return ""
 
     # @property
     # def display_name(self):
     #     if self.first_name and self.last_name:
     #         return f"{self.first_name[0]}.{self.last_name}"
 
     def full_name(self) -> str:
```

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/signals.py` & `geoluminate-0.0.2/geoluminate/contrib/user/signals.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email/password_reset_key_message.txt` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email/password_reset_key_message.txt`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/email_confirm.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/login.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/logout.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_change.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_reset.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/password_reset_from_key.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/signup.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/account/verified_email_required.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/account/verified_email_required.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/base.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/base.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/connected_accounts.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/connected_accounts.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/email.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/email.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/add_email.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/add_email.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/change_password.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/change_password.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/deactivate_account.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/deactivate_account.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/forgot_password.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/forgot_password.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/login.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/login.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/modals/register.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/modals/register.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/navbar_widget.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/navbar_widget.html`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   </a>
   <ul class="dropdown-menu dropdown-menu-end" aria-labelledby="navbarDropdown">
       {% if user.is_authenticated %}
       <li>
         <h6 class="dropdown-header">{% trans "User" %}</h6>
       </li>
         <li>
-          <a class="dropdown-item" href="{% url 'user:profile' pk=user.pk %}">
+          <a class="dropdown-item" href="{% url 'user:profile' %}">
             <i class="fas fa-user me-2"></i>
             {% trans "Profile" %}
           </a>
         </li>
         <li>
           <a class="dropdown-item" href="{% url 'user:dashboard' %}">
             <i class="fas fa-th-large me-2"></i>
```

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/authentication/settings.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/authentication/settings.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/dashboard/panels/publications.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/dashboard/panels/publications.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/dashboard/sections/orcid.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/dashboard/sections/orcid.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/socialaccount/connections.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/socialaccount/login.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/socialaccount/signup.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/user/account.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/user/account.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/user/community.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/user/community.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/user/dashboard.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/user/dashboard.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templates/user/why_orcid.html` & `geoluminate-0.0.2/geoluminate/contrib/user/templates/user/why_orcid.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/templatetags/authentication.py` & `geoluminate-0.0.2/geoluminate/contrib/user/templatetags/authentication.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/factories.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/factories.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/test_admin.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/test_drf_urls.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/test_drf_urls.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/test_drf_views.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/test_drf_views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/test_forms.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/test_swagger.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/test_swagger.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/test_tasks.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/test_urls.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/tests/test_views.py` & `geoluminate-0.0.2/geoluminate/contrib/user/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/contrib/user/views.py` & `geoluminate-0.0.2/geoluminate/contrib/user/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 def user_settings(request):
     context = {}
 
     return render(request, "user/account.html", context=context)
 
 
 @login_required
-def profile(request, pk):
+def profile(request):
     context = {
         "can_add_email": EmailAddress.objects.can_add_email(request.user),
         "email_form": AddEmailForm(request),
         "disconnect_form": DisconnectForm(request=request),
     }
 
     return render(request, "user/profile.html", context=context)
```

### Comparing `geoluminate-0.0.1/geoluminate/core/datatables/__init__.py` & `geoluminate-0.0.2/geoluminate/core/datatables/__init__.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/datatables/adapters.py` & `geoluminate-0.0.2/geoluminate/core/datatables/adapters.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/datatables/apps.py` & `geoluminate-0.0.2/geoluminate/core/datatables/apps.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/datatables/metadata.py` & `geoluminate-0.0.2/geoluminate/core/datatables/metadata.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/datatables/renderers.py` & `geoluminate-0.0.2/geoluminate/core/datatables/renderers.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/datatables/spectacular.py` & `geoluminate-0.0.2/geoluminate/core/datatables/spectacular.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/datatables/urls.py` & `geoluminate-0.0.2/geoluminate/core/datatables/urls.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/datatables/views.py` & `geoluminate-0.0.2/geoluminate/core/datatables/views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/forms/fields.py` & `geoluminate-0.0.2/geoluminate/core/forms/fields.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/forms/widgets.py` & `geoluminate-0.0.2/geoluminate/core/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/management/commands/celery_worker.py` & `geoluminate-0.0.2/geoluminate/management/commands/celery_worker.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/mixins.py` & `geoluminate-0.0.2/geoluminate/core/mixins.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/core/validators.py` & `geoluminate-0.0.2/geoluminate/core/validators.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/db/fields.py` & `geoluminate-0.0.2/geoluminate/db/fields.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/db/models.py` & `geoluminate-0.0.2/geoluminate/db/models.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/middleware.py` & `geoluminate-0.0.2/geoluminate/middleware.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/models.py` & `geoluminate-0.0.2/geoluminate/models.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/admin/css/custom-admin.min.css` & `geoluminate-0.0.2/geoluminate/static/admin/css/custom-admin.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/admin/css/custom-admin.scss` & `geoluminate-0.0.2/geoluminate/static/admin/css/custom-admin.scss`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/css/custom-admin.min.css` & `geoluminate-0.0.2/geoluminate/static/geoluminate/css/custom-admin.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/css/custom-admin.min.css.map` & `geoluminate-0.0.2/geoluminate/static/geoluminate/css/custom-admin.min.css.map`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/css/custom-admin.scss` & `geoluminate-0.0.2/geoluminate/static/geoluminate/css/custom-admin.scss`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.eot` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.ttf` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.woff` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-brands-400.woff2` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.eot` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.ttf` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.woff` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-regular-400.woff2` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.eot` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.ttf` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.woff` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/fonts/fa-solid-900.woff2` & `geoluminate-0.0.2/geoluminate/static/geoluminate/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/brand.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/brand.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/icon.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/icon.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/icon_original.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/icon_original.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/logo.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/logo.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/logo_test.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/logo_test.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/brand/original.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/brand/original.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/audio.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/audio.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/ball-triangle.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/ball-triangle.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/bars.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/bars.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/circles.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/circles.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/grid.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/grid.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/hearts.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/hearts.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/oval.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/oval.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/puff.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/puff.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/rings.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/rings.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/spinning-circles.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/spinning-circles.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/img/spinners/tail-spin.svg` & `geoluminate-0.0.2/geoluminate/static/geoluminate/img/spinners/tail-spin.svg`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/js/comments.js` & `geoluminate-0.0.2/geoluminate/static/geoluminate/js/comments.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/js/custom-admin.js` & `geoluminate-0.0.2/geoluminate/static/geoluminate/js/custom-admin.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/js/custom.js` & `geoluminate-0.0.2/geoluminate/static/geoluminate/js/custom.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/js/jquery.shave.min.js` & `geoluminate-0.0.2/geoluminate/static/geoluminate/js/jquery.shave.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/js/shave.min.js` & `geoluminate-0.0.2/geoluminate/static/geoluminate/js/shave.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/js/spin.js` & `geoluminate-0.0.2/geoluminate/static/geoluminate/js/spin.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_header.scss` & `geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_header.scss`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_menu.scss` & `geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_menu.scss`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/scss/components/_sidebar.scss` & `geoluminate-0.0.2/geoluminate/static/geoluminate/scss/components/_sidebar.scss`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 .sidebar {
-  // @extend .offcanvas;
-  // display: flex;
-  // position: relative;
+  @extend .offcanvas;
+  display: flex;
+  position: relative;
   z-index: 100;
   flex: 0 0 $sidebar-width;
   flex-direction: column;
   max-width: 100%;
   color: $offcanvas-color;
   background-color: $offcanvas-bg-color;
   background-clip: padding-box;
   outline: 0;
   @include box-shadow($offcanvas-box-shadow);
   @include transition(transform $offcanvas-transition-duration ease-in-out);
 	transition: .3s;
 
   &-header {
-    display: flex;
-    align-items: center;
-    justify-content: space-between;
-    padding: $offcanvas-padding-y $offcanvas-padding-x;
+    @extend .offcanvas-header;
   
     .btn-close {
       padding: ($offcanvas-padding-y * .5) ($offcanvas-padding-x * .5);
       margin-top: $offcanvas-padding-y * -.5;
       margin-right: $offcanvas-padding-x * -.5;
       margin-bottom: $offcanvas-padding-y * -.5;
     }
@@ -30,20 +27,22 @@
 
   &-title {
     margin-bottom: 0;
     line-height: $offcanvas-title-line-height;
   }
 
   &-body {
+    // @extend .offcanvas-body;
+
     flex-grow: 1;
     // padding: $offcanvas-padding-y $offcanvas-padding-x;
     overflow-y: auto;
-    // overflow: auto;
+    overflow: auto;
     height: 1;
-    // overflow-y: hidden;
+    overflow-y: hidden;
   }
 
   &-start {
     border-right: $offcanvas-border-width solid $offcanvas-border-color;
     margin-left: -1 * $sidebar-width;
   
     &.show {
```

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/scss/geoluminate.min.css` & `geoluminate-0.0.2/geoluminate/static/geoluminate/scss/geoluminate.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/scss/geoluminate.min.css.map` & `geoluminate-0.0.2/geoluminate/static/geoluminate/scss/geoluminate.min.css.map`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/scss/geoluminate.scss` & `geoluminate-0.0.2/geoluminate/static/geoluminate/scss/geoluminate.scss`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/scss/layout/_menu.scss` & `geoluminate-0.0.2/geoluminate/static/geoluminate/scss/layout/_menu.scss`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/geoluminate/scss/libs/_vendor.scss` & `geoluminate-0.0.2/geoluminate/static/geoluminate/scss/libs/_vendor.scss`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap4.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap4.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap5.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bootstrap5.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bulma.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bulma.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.bulma.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.bulma.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.dataTables.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.dataTables.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.dataTables.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.foundation.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.foundation.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.foundation.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.foundation.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.jqueryui.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.jqueryui.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.jqueryui.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.jqueryui.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.semanticui.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.semanticui.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/editor.semanticui.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/editor.semanticui.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/fields.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/fields.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/inline.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/inline.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/main.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/main.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/processing.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/processing.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/css/scss/upload.min.css` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/css/scss/upload.min.css`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/dataTables.editor.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/dataTables.editor.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/dataTables.editor.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/dataTables.editor.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap4.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap4.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap5.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bootstrap5.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bulma.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bulma.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.bulma.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.bulma.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.dataTables.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.dataTables.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.dataTables.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.foundation.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.foundation.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.foundation.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.foundation.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.jqueryui.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.jqueryui.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.jqueryui.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.jqueryui.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.semanticui.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.semanticui.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/static/vendor/dataTables/js/editor.semanticui.min.js` & `geoluminate-0.0.2/geoluminate/static/vendor/dataTables/js/editor.semanticui.min.js`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/api/map_popup.html` & `geoluminate-0.0.2/geoluminate/templates/api/map_popup.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/base.html` & `geoluminate-0.0.2/geoluminate/templates/base.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/forms/checkbox.html` & `geoluminate-0.0.2/geoluminate/templates/forms/checkbox.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/forms/widgets/postgres_array_widget.html` & `geoluminate-0.0.2/geoluminate/templates/forms/widgets/postgres_array_widget.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/forms/widgets/quantity_field.html` & `geoluminate-0.0.2/geoluminate/templates/forms/widgets/quantity_field.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/bootstrap/modal.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/bootstrap/modal.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/cms/menu.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/cms/menu.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/components/app_menu.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/components/app_menu.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/components/app_submenu.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/components/app_submenu.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/components/messages.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/components/messages.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/components/modal.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/components/modal.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/components/offcanvas.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/components/offcanvas.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/components/paginator.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/components/paginator.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/components/sidebar.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/components/sidebar.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 <!-- RIGHT SIDEBAR -->
 <div id='rightSidebar' class="sidebar sidebar-end show">
  <div class="sidebar-header">
   {% block header %}
    <h5 class="sidebar-title">
     {% block title %}
+    {{ title|default:'Sidebar' }}
     {% endblock title %}
    </h5>
    <button type="button"
            class="btn-close text-reset"
            data-bs-dismiss="offcanvas"
            aria-label="Close"
            onclick="$('#rightSidebar').toggleClass('show')">
    </button>
   {% endblock header %}
  </div>
- <div class="sidebar-body" data-select2-id="5">
+ <div class="sidebar-body">
   {% block body %}
   {% endblock body %}
  </div>
 </div>
```

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/components/socials.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/components/socials.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/database/site.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/database/site.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/layout/navbar.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/layout/navbar.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/layout/partials/sidebar_menu.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/layout/partials/sidebar_menu.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/layout/sidebar.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/layout/sidebar.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/application.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/application.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/modals/datasource.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/modals/datasource.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/modals/datatable.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/modals/datatable.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/modals/layer_settings.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/modals/layer_settings.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/sidebars/basemaps.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/sidebars/basemaps.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/components/sidebars/layers.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/components/sidebars/layers.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/partials/map.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/partials/map.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% load static sekizai_tags %}
 <div id='map'
-     url="{% url "sites-list" %}?"
+     {% comment %} url="{% url "sites-list" %}?" {% endcomment %}
+     url="/api/v1/geoluminate?"
      data-format='geojson'
      {% if publication %} data-references='{{ publication.pk }}'{% endif %}
      {% if site %} data-id='{{ site.pk }}'{% endif %}
      class="flex-fill {{ css_class }}">
   <div id='shadow'></div>
 </div>
 {% addtoblock "css" %}
@@ -30,8 +31,8 @@
     {% addtoblock "js" %}
       <script src='https://cdnjs.cloudflare.com/ajax/libs/leaflet.markercluster/1.4.1/leaflet.markercluster.js'></script>{% endaddtoblock %}
       {% addtoblock "js" %}
         <script src="https://unpkg.com/esri-leaflet@2.5.0/dist/esri-leaflet.js"
                 integrity="sha512-ucw7Grpc+iEQZa711gcjgMBnmd9qju1CICsRaryvX7HJklK0pGl/prxKvtHwpgm5ZHdvAil7YPxI1oWPOWK3UQ=="
                 crossorigin=""></script>{% endaddtoblock %}
         {% addtoblock "js" %}
-          <script src="{% static 'mapping/js/map.js' %}"></script>{% endaddtoblock %}
+          <script src="{% static 'geoluminate/js/map.js' %}"></script>{% endaddtoblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% load static sekizai_tags %}
- %}?" data-format='geojson' {% if publication %} data-references='{
+% comment %} url="{% url "sites-list" %}?" {% endcomment %} url="/api/v1/
+geoluminate?" data-format='geojson' {% if publication %} data-references='{
 { publication.pk }}'{% endif %} {% if site %} data-id='{{ site.pk }}'{% endif
 %} class="flex-fill {{ css_class }}">
 {% addtoblock "css" %}
  {% endaddtoblock %} {% addtoblock "css" %}
  {% endaddtoblock %} {% addtoblock "css" %}
  {% endaddtoblock %} {% addtoblock "js" %}
 {% endaddtoblock %} {% addtoblock "js" %}
```

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/mapping/partials/sidebar.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/mapping/partials/sidebar.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/modals/form.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/modals/form.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/spectacular.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/spectacular.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/utils/map.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/utils/map.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/widgets/nav/theme_switcher.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/widgets/nav/theme_switcher.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/geoluminate/widgets/nav/user_affiliation.html` & `geoluminate-0.0.2/geoluminate/templates/geoluminate/widgets/nav/user_affiliation.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/literature/admin/change_list.html` & `geoluminate-0.0.2/geoluminate/templates/literature/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/literature/admin/search.html` & `geoluminate-0.0.2/geoluminate/templates/literature/admin/search.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/literature/authors_list.html` & `geoluminate-0.0.2/geoluminate/templates/literature/authors_list.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/literature/citation/publication.html` & `geoluminate-0.0.2/geoluminate/templates/literature/citation/publication.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/literature/literature_list copy.html` & `geoluminate-0.0.2/geoluminate/templates/literature/literature_list copy.html`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/templates/literature/literature_list.html` & `geoluminate-0.0.2/geoluminate/templates/literature/literature_list.html`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,17 @@
   {{ filter.form.media.css }}
 {% endblock head %}
 {% block style %}
 <link rel="stylesheet" href="{% static 'vendor/DataTables/bootstrap5/datatables.min.css' %}">
 {% endblock style %}
 
 {% block app_menu %}
-<button class='btn btn-sm rounded-pill btn-outline-primary'
+  <button id='rightSidebarToggle' class='btn btn-sm rounded-pill btn-outline-primary'
           onclick="$('#rightSidebar').toggleClass('show')">
-    {% trans "Filter" %}
-  </button>
-  <button class="btn btn-sm rounded-pill btn-outline-primary"
-          type="button"
-          id="dropdownMenuButton"
-          data-bs-toggle="dropdown"
-          aria-expanded="false">
-    {% trans "Years" %}
+    {% trans "Filters" %}
   </button>
   <ul class="dropdown-menu p-2" aria-labelledby="dropdownMenuButton">
     <label for="customRange1" class="form-label" hidden>{% trans "Year range" %}</label>
     <input type="range" class="form-range" id="customRange1">
   </ul>
 {% endblock app_menu %}
 
@@ -90,27 +83,42 @@
          // show new container for data
         $('#new-list').insertBefore('#example');
         $('#new-list').show();
       },
       "rowCallback": function( row, data ) {
          // on each row callback
         var template = $("#template").clone().children().first()
-        
         $.each(data, function(key, val){
           template.find(".data-" + key).text(val);
         });
 
         template.appendTo('#new-list');
       },
       "preDrawCallback": function( settings ) {
          // clear list before draw
         $('#new-list').empty();
       },
       "searchPanes": {
-        layout: 'columns-1'
+        layout: 'columns-1',
+        cascadePanes: true,
+        orderable: false,
+        filterChanged: function (count) {
+          if (count === 0) {
+            $('#rightSidebarToggle').find('span').remove()
+            return
+          }
+          $('#rightSidebarToggle').find('span').remove()
+          $('#rightSidebarToggle').append(`<span class="badge bg-primary">${count}</span>`)
+    
+        },
+        dtOpts: {
+          paging: true,
+          pagingType: 'numbers',
+          searching: true,
+        },
       },
     });
   
   new $.fn.dataTable.Buttons(table, {
        buttons: [
          {
            extend: 'print',
@@ -160,16 +168,13 @@
   table.searchPanes.container().appendTo( $('#rightSidebar>.sidebar-body') );
   });
 
 </script>
 
 
 
-    {% endaddtoblock %}
-  {% endblock content %}
+{% endaddtoblock %}
+{% endblock content %}
+
 {% block sidebar_right %}
-    {% include 'geoluminate/components/sidebar.html' %}
+    {% include 'geoluminate/components/sidebar.html' with title='Filters' %}
 {% endblock sidebar_right %}
-  {% comment %}
-{% block modals %}
-{% include "review/modals/nominate.html" with modal_id='genericModal' %}
-  {% endblock modals %} {% endcomment %}
```

### Comparing `geoluminate-0.0.1/geoluminate/templatetags/geoluminate.py` & `geoluminate-0.0.2/geoluminate/templatetags/geoluminate.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/urls.py` & `geoluminate-0.0.2/geoluminate/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     # path("literature/", include("geoluminate.contrib.literature.urls")),
     path("", include("geoluminate.contrib.user.urls")),
     path("", include("geoluminate.contrib.gis.urls")),
     path("", include("cms.urls")),
 ]
 
 
+GEOLUMINATE_URLS = NON_I18N_URLS + I18N_URLS
+
 # urlpatterns = (
 #     NON_I18N_URLS
 #     + I18N_URLS
 #     + [path("", include("cms.urls"))]  # must be last
 #     + static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 #     + static(settings.STATIC_URL, document_root=settings.STATIC_ROOT)
 # )
```

### Comparing `geoluminate-0.0.1/geoluminate/utils/__init__.py` & `geoluminate-0.0.2/geoluminate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/utils/drf.py` & `geoluminate-0.0.2/geoluminate/utils/drf.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/utils/import_export/mixins.py` & `geoluminate-0.0.2/geoluminate/utils/import_export/mixins.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/utils/import_export/widgets.py` & `geoluminate-0.0.2/geoluminate/utils/import_export/widgets.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/utils/paginators.py` & `geoluminate-0.0.2/geoluminate/utils/paginators.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/utils/select2/filters.py` & `geoluminate-0.0.2/geoluminate/utils/select2/filters.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/utils/select2/widgets.py` & `geoluminate-0.0.2/geoluminate/utils/select2/widgets.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/views.py` & `geoluminate-0.0.2/geoluminate/views.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/geoluminate/widgets.py` & `geoluminate-0.0.2/geoluminate/widgets.py`

 * *Files identical despite different names*

### Comparing `geoluminate-0.0.1/pyproject.toml` & `geoluminate-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geoluminate"
-version = "v0.0.1"
+version = "0.0.2"
 description = ""
 authors = ["Sam Jennings <samuel.scott.jennings@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "geoluminate"}]
 homepage = "https://github.com/Geoluminate/geoluminate"
 keywords = ["research", "database", "research data management", "open data", "geoluminate", "FAIR"]
@@ -74,14 +74,18 @@
 pyyaml = "^6.0"
 celery = "^5.2.7"
 polib = "^1.2.0"
 django-select2 = "^8.1.1"
 django-literature = "^0.1.2"
 django-filer = "^2.2.4"
 django-laboratory = "^0.0.1"
+flower = "^1.2.0"
+django-treebeard = "<4.5"
+django-modeltranslation = "^0.18.9"
+django-redis = "^5.2.0"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.2.1"
 black = "^23.1.0"
 pytest = "^7.2.2"
 factory-boy = "^3.2.1"
 django-coverage-plugin = "^3.0.0"
@@ -150,14 +154,20 @@
 [[tool.mypy.overrides]]
 module = "geoluminate.models"
 disable_error_code = [
     "var-annotated",
 ]
 
 [[tool.mypy.overrides]]
+module = "geoluminate.contrib.controlled_vocabulary.models"
+disable_error_code = [
+    "var-annotated",
+]
+
+[[tool.mypy.overrides]]
 module = "geoluminate.contrib.gis.base"
 disable_error_code = [
     "var-annotated",
 ]
 
 [[tool.mypy.overrides]]
 module = "geoluminate.db.models"
@@ -168,15 +178,15 @@
 [tool.django-stubs]
 django_settings_module = "tests.settings"
 
 [tool.ruff]
 target-version = "py37"
 line-length = 120
 fix = true
-exclude = ['docs/', 'migrations/', 'tests/*.py']
+exclude = ['docs/', 'migrations/', 'tests/*.py','geoluminate/conf/*',]
 select = [
     # flake8-2020
     "YTT",
     # flake8-bandit
     "S",
     # flake8-bugbear
     "B",
```

### Comparing `geoluminate-0.0.1/PKG-INFO` & `geoluminate-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoluminate
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Home-page: https://github.com/Geoluminate/geoluminate
 License: GPL-3.0-or-later
 Keywords: research,database,research data management,open data,geoluminate,FAIR
 Author: Sam Jennings
 Author-email: samuel.scott.jennings@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -44,36 +44,40 @@
 Requires-Dist: django-jazzmin (>=2.6.0,<3.0.0)
 Requires-Dist: django-laboratory (>=0.0.1,<0.0.2)
 Requires-Dist: django-libsass (>=0.9,<0.10)
 Requires-Dist: django-literature (>=0.1.2,<0.2.0)
 Requires-Dist: django-lockdown (>=4.0.0,<5.0.0)
 Requires-Dist: django-meta (>=2.1.0,<3.0.0)
 Requires-Dist: django-model-utils (>=4.3.1,<5.0.0)
+Requires-Dist: django-modeltranslation (>=0.18.9,<0.19.0)
 Requires-Dist: django-nested-admin (>=4.0.2,<5.0.0)
 Requires-Dist: django-pint (>=0.7.1,<0.8.0)
 Requires-Dist: django-postgres-metrics (>=0.13.1,<0.14.0)
+Requires-Dist: django-redis (>=5.2.0,<6.0.0)
 Requires-Dist: django-rosetta (>=0.9.8,<0.10.0)
 Requires-Dist: django-select2 (>=8.1.1,<9.0.0)
 Requires-Dist: django-simple-menu (>=2.1.1,<3.0.0)
 Requires-Dist: django-social-share (>=2.3.0,<3.0.0)
 Requires-Dist: django-solo (>=2.0.0,<3.0.0)
 Requires-Dist: django-spaghetti-and-meatballs (>=0.4.2,<0.5.0)
 Requires-Dist: django-split-settings (>=1.2.0,<2.0.0)
 Requires-Dist: django-storages (>=1.13.2,<2.0.0)
 Requires-Dist: django-tellme (>=0.7.3,<0.8.0)
+Requires-Dist: django-treebeard (<4.5)
 Requires-Dist: django[argon2] (>=3.2)
 Requires-Dist: djangocms-frontend (>=1.1.0,<2.0.0)
 Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
 Requires-Dist: djangorestframework-datatables-editor (>=0.3.3,<0.4.0)
 Requires-Dist: djangorestframework-gis (>=1.0,<2.0)
 Requires-Dist: drf-access-policy (>=1.5.0,<2.0.0)
 Requires-Dist: drf-nested-routers (>=0.93.4,<0.94.0)
 Requires-Dist: drf-orjson-renderer (>=1.7.1,<2.0.0)
 Requires-Dist: drf-schema-adapter (>=3.0.6,<4.0.0)
 Requires-Dist: drf-spectacular[sidecar] (>=0.26.1,<0.27.0)
+Requires-Dist: flower (>=1.2.0,<2.0.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
 Requires-Dist: polib (>=1.2.0,<2.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: redis (>=4.5.2,<5.0.0)
 Requires-Dist: sentry-sdk[django] (>=1.17.0,<2.0.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
@@ -92,20 +96,19 @@
 <!-- [![RTD](https://readthedocs.org/projects/geoluminate/badge/?version=latest)](https://geoluminate.readthedocs.io/en/latest/readme.html) -->
 <!-- [![Documentation](https://github.com/Geoluminate/geoluminate/actions/workflows/build-docs.yml/badge.svg)](https://github.com/Geoluminate/geoluminate/actions/workflows/build-docs.yml) -->
 <!-- [![PR](https://img.shields.io/github/issues-pr/Geoluminate/geoluminate)](https://github.com/Geoluminate/geoluminate/pulls)
 [![Issues](https://img.shields.io/github/issues-raw/Geoluminate/geoluminate)](https://github.com/Geoluminate/geoluminate/pulls) -->
 <!-- ![PyPI - Downloads](https://img.shields.io/pypi/dm/geoluminate) -->
 <!-- ![PyPI - Status](https://img.shields.io/pypi/status/geoluminate) -->
 
-A Django application for managing collections of scientific instruments
 
 Documentation
 -------------
 
-The full documentation is at https://ssjenny90.github.io/geoluminate/
+The full documentation is at https://geoluminate.github.io/geoluminate/
 
 Quickstart
 ----------
 
 Install Geoluminate::
 
     pip install geoluminate
```

