# Comparing `tmp/fief-server-0.8.2.tar.gz` & `tmp/fief-server-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fief-server-0.8.2.tar", last modified: Thu Mar 31 08:47:29 2022, max compression
+gzip compressed data, was "fief-server-0.9.0.tar", last modified: Thu Mar 31 14:17:07 2022, max compression
```

## Comparing `fief-server-0.8.2.tar` & `fief-server-0.9.0.tar`

### file list

```diff
@@ -1,189 +1,191 @@
--rw-r--r--   0        0        0      233 2022-03-31 08:46:44.300332 fief-server-0.8.2/.env.dist
--rw-r--r--   0        0        0      231 2022-03-31 08:46:44.300332 fief-server-0.8.2/babel.cfg
--rw-r--r--   0        0        0       22 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/__init__.py
--rw-r--r--   0        0        0     1397 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic.ini
--rw-r--r--   0        0        0       38 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/README
--rw-r--r--   0        0        0     2466 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/env.py
--rw-r--r--   0        0        0     5964 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/main_versions/274bc650f9a2_initial_migration.py
--rw-r--r--   0        0        0      507 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/script.py.mako
--rw-r--r--   0        0        0    14355 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/workspace_versions/0ba35b227f10_initial_migration.py
--rw-r--r--   0        0        0     1552 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/workspace_versions/0e7f8edd4e21_add_authenticated_at_column_to_.py
--rw-r--r--   0        0        0      879 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/workspace_versions/1df8009b83c5_add_redirect_uris_column_to_client.py
--rw-r--r--   0        0        0      760 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/workspace_versions/cfaa3c85d3d3_update_password_hash_length.py
--rw-r--r--   0        0        0      935 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/alembic/workspace_versions/d3cb52370070_add_nonce_column_to_loginsession_and_.py
--rw-r--r--   0        0        0      802 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/app.py
--rw-r--r--   0        0        0      222 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/__init__.py
--rw-r--r--   0        0        0        0 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/__init__.py
--rw-r--r--   0        0        0     1165 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/app.py
--rw-r--r--   0        0        0        0 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/routers/__init__.py
--rw-r--r--   0        0        0     2103 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/routers/api_keys.py
--rw-r--r--   0        0        0     2358 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/routers/auth.py
--rw-r--r--   0        0        0     2855 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/routers/clients.py
--rw-r--r--   0        0        0      808 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/routers/tenants.py
--rw-r--r--   0        0        0     2414 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/routers/users.py
--rw-r--r--   0        0        0     1872 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin/routers/workspaces.py
--rw-r--r--   0        0        0        0 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin_frontend/__init__.py
--rw-r--r--   0        0        0      998 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/admin_frontend/app.py
--rw-r--r--   0        0        0        0 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/auth/__init__.py
--rw-r--r--   0        0        0     1836 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/auth/app.py
--rw-r--r--   0        0        0     4731 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/auth/exception_handlers.py
--rw-r--r--   0        0        0        0 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/auth/routers/__init__.py
--rw-r--r--   0        0        0     7403 2022-03-31 08:46:44.300332 fief-server-0.8.2/fief/apps/auth/routers/auth.py
--rw-r--r--   0        0        0     2764 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/apps/auth/routers/register.py
--rw-r--r--   0        0        0     4671 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/apps/auth/routers/reset.py
--rw-r--r--   0        0        0     2499 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/apps/auth/routers/token.py
--rw-r--r--   0        0        0      705 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/apps/auth/routers/user.py
--rw-r--r--   0        0        0     2161 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/apps/auth/routers/well_known.py
--rw-r--r--   0        0        0      923 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/apps/auth/templates.py
--rw-r--r--   0        0        0     5804 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/cli.py
--rw-r--r--   0        0        0      722 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/cors.py
--rw-r--r--   0        0        0        0 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/crypto/__init__.py
--rw-r--r--   0        0        0     1269 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/crypto/access_token.py
--rw-r--r--   0        0        0      540 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/crypto/encryption.py
--rw-r--r--   0        0        0     1894 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/crypto/id_token.py
--rw-r--r--   0        0        0      498 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/crypto/jwk.py
--rw-r--r--   0        0        0      206 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/crypto/password.py
--rw-r--r--   0        0        0     2336 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/csrf.py
--rw-r--r--   0        0        0      140 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/db/__init__.py
--rw-r--r--   0        0        0     1400 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/db/engine.py
--rw-r--r--   0        0        0      508 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/db/main.py
--rw-r--r--   0        0        0     1515 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/db/types.py
--rw-r--r--   0        0        0     1689 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/db/workspace.py
--rw-r--r--   0        0        0        0 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/__init__.py
--rw-r--r--   0        0        0     2029 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/admin_api_key.py
--rw-r--r--   0        0        0     1462 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/admin_authentication.py
--rw-r--r--   0        0        0     1236 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/admin_session.py
--rw-r--r--   0        0        0     8374 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/auth.py
--rw-r--r--   0        0        0      962 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/authentication_flow.py
--rw-r--r--   0        0        0     1032 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/client.py
--rw-r--r--   0        0        0     1291 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/current_workspace.py
--rw-r--r--   0        0        0      408 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/fief.py
--rw-r--r--   0        0        0     2034 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/locale.py
--rw-r--r--   0        0        0      982 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/main_managers.py
--rw-r--r--   0        0        0     1113 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/pagination.py
--rw-r--r--   0        0        0      756 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/register.py
--rw-r--r--   0        0        0     1401 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/reset.py
--rw-r--r--   0        0        0      558 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/session_token.py
--rw-r--r--   0        0        0      105 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/tasks.py
--rw-r--r--   0        0        0     1773 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/tenant.py
--rw-r--r--   0        0        0     5423 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/token.py
--rw-r--r--   0        0        0     7555 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/users.py
--rw-r--r--   0        0        0     1024 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/workspace.py
--rw-r--r--   0        0        0      754 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/workspace_creation.py
--rw-r--r--   0        0        0      141 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/workspace_db.py
--rw-r--r--   0        0        0     1783 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/dependencies/workspace_managers.py
--rw-r--r--   0        0        0    10753 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/emails/base.html
--rw-r--r--   0        0        0     1043 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/emails/forgot_password.html
--rw-r--r--   0        0        0      284 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/emails/welcome.html
--rw-r--r--   0        0        0      692 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/errors.py
--rw-r--r--   0        0        0     3224 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/exceptions.py
--rw-r--r--   0        0        0      369 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/fastapi_users.py
--rw-r--r--   0        0        0     1236 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/locale.py
--rw-r--r--   0        0        0     4225 2022-03-31 08:47:27.504958 fief-server-0.8.2/fief/locale/en_US/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     6884 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/locale/en_US/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     4557 2022-03-31 08:47:27.504958 fief-server-0.8.2/fief/locale/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0     7223 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/locale/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      327 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/logging.py
--rw-r--r--   0        0        0     1058 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/__init__.py
--rw-r--r--   0        0        0      465 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/admin_api_key.py
--rw-r--r--   0        0        0      519 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/admin_session_token.py
--rw-r--r--   0        0        0     1042 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/authorization_code.py
--rw-r--r--   0        0        0     5569 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/base.py
--rw-r--r--   0        0        0      747 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/client.py
--rw-r--r--   0        0        0      546 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/grant.py
--rw-r--r--   0        0        0      473 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/login_session.py
--rw-r--r--   0        0        0      693 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/refresh_token.py
--rw-r--r--   0        0        0      693 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/session_token.py
--rw-r--r--   0        0        0      992 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/tenant.py
--rw-r--r--   0        0        0      171 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/user.py
--rw-r--r--   0        0        0     1093 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/workspace.py
--rw-r--r--   0        0        0      630 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/managers/workspace_user.py
--rw-r--r--   0        0        0      960 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/__init__.py
--rw-r--r--   0        0        0      710 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/admin_api_key.py
--rw-r--r--   0        0        0     1061 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/admin_session_token.py
--rw-r--r--   0        0        0     1320 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/authorization_code.py
--rw-r--r--   0        0        0      538 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/base.py
--rw-r--r--   0        0        0     1612 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/client.py
--rw-r--r--   0        0        0     2499 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/generics.py
--rw-r--r--   0        0        0      911 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/grant.py
--rw-r--r--   0        0        0     1223 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/login_session.py
--rw-r--r--   0        0        0     1236 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/refresh_token.py
--rw-r--r--   0        0        0      844 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/session_token.py
--rw-r--r--   0        0        0     1267 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/tenant.py
--rw-r--r--   0        0        0     1221 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/user.py
--rw-r--r--   0        0        0     3550 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/workspace.py
--rw-r--r--   0        0        0      780 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/models/workspace_user.py
--rw-r--r--   0        0        0      283 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/paths.py
--rw-r--r--   0        0        0      300 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/__init__.py
--rw-r--r--   0        0        0      384 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/admin_api_key.py
--rw-r--r--   0        0        0     3648 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/auth.py
--rw-r--r--   0        0        0     1301 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/client.py
--rw-r--r--   0        0        0      456 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/generics.py
--rw-r--r--   0        0        0      700 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/register.py
--rw-r--r--   0        0        0      930 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/reset.py
--rw-r--r--   0        0        0      241 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/tenant.py
--rw-r--r--   0        0        0      848 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/user.py
--rw-r--r--   0        0        0     2174 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/well_known.py
--rw-r--r--   0        0        0     2572 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/schemas/workspace.py
--rw-r--r--   0        0        0        0 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/__init__.py
--rw-r--r--   0        0        0     5622 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/authentication_flow.py
--rw-r--r--   0        0        0      601 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/email/__init__.py
--rw-r--r--   0        0        0      470 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/email/base.py
--rw-r--r--   0        0        0      366 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/email/null.py
--rw-r--r--   0        0        0     1066 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/email/postmark.py
--rw-r--r--   0        0        0     4156 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/main_workspace.py
--rw-r--r--   0        0        0     3934 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/workspace_creation.py
--rw-r--r--   0        0        0     1960 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/services/workspace_db.py
--rw-r--r--   0        0        0     4402 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/settings.py
--rw-r--r--   0        0        0     1189 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/static/favicon.svg
--rw-r--r--   0        0        0     1898 2022-03-31 08:46:44.304332 fief-server-0.8.2/fief/static/fief-logo.svg
--rw-r--r--   0        0        0     1451 2022-03-31 08:47:28.740976 fief-server-0.8.2/fief/static/frontend/asset-manifest.json
--rw-r--r--   0        0        0     1189 2022-03-31 08:47:28.744976 fief-server-0.8.2/fief/static/frontend/favicon.svg
--rw-r--r--   0        0        0      733 2022-03-31 08:47:28.820977 fief-server-0.8.2/fief/static/frontend/index.html
--rw-r--r--   0        0        0      709 2022-03-31 08:47:28.944979 fief-server-0.8.2/fief/static/frontend/locales/en/api-keys.json
--rw-r--r--   0        0        0     1228 2022-03-31 08:47:29.000980 fief-server-0.8.2/fief/static/frontend/locales/en/clients.json
--rw-r--r--   0        0        0     1174 2022-03-31 08:47:29.020980 fief-server-0.8.2/fief/static/frontend/locales/en/common.json
--rw-r--r--   0        0        0      117 2022-03-31 08:47:29.060981 fief-server-0.8.2/fief/static/frontend/locales/en/tenants.json
--rw-r--r--   0        0        0      300 2022-03-31 08:47:29.076981 fief-server-0.8.2/fief/static/frontend/locales/en/users.json
--rw-r--r--   0        0        0     1016 2022-03-31 08:47:29.108981 fief-server-0.8.2/fief/static/frontend/locales/en/workspaces.json
--rw-r--r--   0        0        0     5347 2022-03-31 08:47:28.800977 fief-server-0.8.2/fief/static/frontend/logo192.png
--rw-r--r--   0        0        0     9664 2022-03-31 08:47:28.876978 fief-server-0.8.2/fief/static/frontend/logo512.png
--rw-r--r--   0        0        0      492 2022-03-31 08:47:28.872978 fief-server-0.8.2/fief/static/frontend/manifest.json
--rw-r--r--   0        0        0       67 2022-03-31 08:47:28.936979 fief-server-0.8.2/fief/static/frontend/robots.txt
--rw-r--r--   0        0        0    35836 2022-03-31 08:47:29.164982 fief-server-0.8.2/fief/static/frontend/static/css/main.45cf7c31.css
--rw-r--r--   0        0        0    18184 2022-03-31 08:47:29.136982 fief-server-0.8.2/fief/static/frontend/static/css/main.45cf7c31.css.map
--rw-r--r--   0        0        0     4607 2022-03-31 08:47:29.220983 fief-server-0.8.2/fief/static/frontend/static/js/787.707d1bd1.chunk.js
--rw-r--r--   0        0        0    10281 2022-03-31 08:47:29.196983 fief-server-0.8.2/fief/static/frontend/static/js/787.707d1bd1.chunk.js.map
--rw-r--r--   0        0        0   511557 2022-03-31 08:47:29.412986 fief-server-0.8.2/fief/static/frontend/static/js/main.3b0373f0.js
--rw-r--r--   0        0        0     1493 2022-03-31 08:47:29.256984 fief-server-0.8.2/fief/static/frontend/static/js/main.3b0373f0.js.LICENSE.txt
--rw-r--r--   0        0        0  1596711 2022-03-31 08:47:29.420986 fief-server-0.8.2/fief/static/frontend/static/js/main.3b0373f0.js.map
--rw-r--r--   0        0        0      667 2022-03-31 08:47:29.472987 fief-server-0.8.2/fief/static/frontend/static/media/clients.9b0e9946f3619c28cab1767cc62a22aa.svg
--rw-r--r--   0        0        0      335 2022-03-31 08:47:29.484987 fief-server-0.8.2/fief/static/frontend/static/media/cloud.287167692745095704efd591b87bcaf1.svg
--rw-r--r--   0        0        0     1116 2022-03-31 08:47:29.540988 fief-server-0.8.2/fief/static/frontend/static/media/cogwheel.bbc48a85c6dc5c6dd1eeb294e3afa715.svg
--rw-r--r--   0        0        0      942 2022-03-31 08:47:29.544988 fief-server-0.8.2/fief/static/frontend/static/media/dashboard.580511ccd86590b36f5819c267461ebe.svg
--rw-r--r--   0        0        0     1898 2022-03-31 08:47:29.588988 fief-server-0.8.2/fief/static/frontend/static/media/fief-logo-red.ee09b120c56412b835b2cb57d6adaa58.svg
--rw-r--r--   0        0        0      388 2022-03-31 08:47:29.600989 fief-server-0.8.2/fief/static/frontend/static/media/getFetch.c780682470504fffbd04.cjs
--rw-r--r--   0        0        0      635 2022-03-31 08:47:29.644989 fief-server-0.8.2/fief/static/frontend/static/media/key.69ef1cd7ed8906a8b62c0bb9cb74c731.svg
--rw-r--r--   0        0        0     1926 2022-03-31 08:47:29.660990 fief-server-0.8.2/fief/static/frontend/static/media/tenants.3a942265546a3a2ebbf16aa58f45311f.svg
--rw-r--r--   0        0        0      455 2022-03-31 08:47:29.700990 fief-server-0.8.2/fief/static/frontend/static/media/users.acc3e62b7bc3248222826909f7911672.svg
--rw-r--r--   0        0        0    26633 2022-03-31 08:47:28.428971 fief-server-0.8.2/fief/static/output.css
--rw-r--r--   0        0        0      267 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/tasks/__init__.py
--rw-r--r--   0        0        0     3656 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/tasks/base.py
--rw-r--r--   0        0        0     1299 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/tasks/forgot_password.py
--rw-r--r--   0        0        0     1171 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/tasks/register.py
--rw-r--r--   0        0        0     2996 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/templates/auth_layout.html
--rw-r--r--   0        0        0      181 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/templates/authorize.html
--rw-r--r--   0        0        0      572 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/templates/base.html
--rw-r--r--   0        0        0     1080 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/templates/consent.html
--rw-r--r--   0        0        0     1161 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/templates/forgot_password.html
--rw-r--r--   0        0        0     1556 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/templates/login.html
--rw-r--r--   0        0        0     1695 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/templates/register.html
--rw-r--r--   0        0        0     1194 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/templates/reset_password.html
--rw-r--r--   0        0        0       44 2022-03-31 08:46:44.308332 fief-server-0.8.2/fief/worker.py
--rw-r--r--   0        0        0     1793 2022-03-31 08:46:44.308332 fief-server-0.8.2/justfile
--rw-r--r--   0        0        0    70684 2022-03-31 08:46:44.308332 fief-server-0.8.2/package-lock.json
--rw-r--r--   0        0        0      262 2022-03-31 08:46:44.308332 fief-server-0.8.2/package.json
--rw-r--r--   0        0        0     2492 2022-03-31 08:46:44.308332 fief-server-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      183 2022-03-31 08:46:44.308332 fief-server-0.8.2/setup.cfg
--rw-r--r--   0        0        0     2991 2022-03-31 08:46:44.308332 fief-server-0.8.2/tailwind.config.js
--rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 fief-server-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      233 2022-03-31 14:16:21.476242 fief-server-0.9.0/.env.dist
+-rw-r--r--   0        0        0      231 2022-03-31 14:16:21.476242 fief-server-0.9.0/babel.cfg
+-rw-r--r--   0        0        0       22 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/__init__.py
+-rw-r--r--   0        0        0     1397 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic.ini
+-rw-r--r--   0        0        0       38 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/README
+-rw-r--r--   0        0        0     2466 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/env.py
+-rw-r--r--   0        0        0     5964 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/main_versions/274bc650f9a2_initial_migration.py
+-rw-r--r--   0        0        0      507 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/script.py.mako
+-rw-r--r--   0        0        0    14355 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/workspace_versions/0ba35b227f10_initial_migration.py
+-rw-r--r--   0        0        0     1552 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/workspace_versions/0e7f8edd4e21_add_authenticated_at_column_to_.py
+-rw-r--r--   0        0        0      879 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/workspace_versions/1df8009b83c5_add_redirect_uris_column_to_client.py
+-rw-r--r--   0        0        0     1428 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/workspace_versions/4d0532b3bf16_add_code_challenge_and_code_challenge_.py
+-rw-r--r--   0        0        0      760 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/workspace_versions/cfaa3c85d3d3_update_password_hash_length.py
+-rw-r--r--   0        0        0      935 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/alembic/workspace_versions/d3cb52370070_add_nonce_column_to_loginsession_and_.py
+-rw-r--r--   0        0        0      802 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/app.py
+-rw-r--r--   0        0        0      222 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/__init__.py
+-rw-r--r--   0        0        0     1165 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/app.py
+-rw-r--r--   0        0        0        0 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/routers/__init__.py
+-rw-r--r--   0        0        0     2103 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/routers/api_keys.py
+-rw-r--r--   0        0        0     2358 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/routers/auth.py
+-rw-r--r--   0        0        0     2855 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/routers/clients.py
+-rw-r--r--   0        0        0      808 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/routers/tenants.py
+-rw-r--r--   0        0        0     2414 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/routers/users.py
+-rw-r--r--   0        0        0     1872 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin/routers/workspaces.py
+-rw-r--r--   0        0        0        0 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin_frontend/__init__.py
+-rw-r--r--   0        0        0      998 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/admin_frontend/app.py
+-rw-r--r--   0        0        0        0 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/__init__.py
+-rw-r--r--   0        0        0     1836 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/app.py
+-rw-r--r--   0        0        0     4731 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/exception_handlers.py
+-rw-r--r--   0        0        0        0 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/routers/__init__.py
+-rw-r--r--   0        0        0     7827 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/routers/auth.py
+-rw-r--r--   0        0        0     2764 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/routers/register.py
+-rw-r--r--   0        0        0     4671 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/routers/reset.py
+-rw-r--r--   0        0        0     2628 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/routers/token.py
+-rw-r--r--   0        0        0      705 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/routers/user.py
+-rw-r--r--   0        0        0     2270 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/routers/well_known.py
+-rw-r--r--   0        0        0      923 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/apps/auth/templates.py
+-rw-r--r--   0        0        0     5804 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/cli.py
+-rw-r--r--   0        0        0      722 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/cors.py
+-rw-r--r--   0        0        0        0 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/crypto/__init__.py
+-rw-r--r--   0        0        0     1269 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/crypto/access_token.py
+-rw-r--r--   0        0        0      679 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/crypto/code_challenge.py
+-rw-r--r--   0        0        0      540 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/crypto/encryption.py
+-rw-r--r--   0        0        0     1894 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/crypto/id_token.py
+-rw-r--r--   0        0        0      498 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/crypto/jwk.py
+-rw-r--r--   0        0        0      206 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/crypto/password.py
+-rw-r--r--   0        0        0     2336 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/csrf.py
+-rw-r--r--   0        0        0      140 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/db/__init__.py
+-rw-r--r--   0        0        0     1400 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/db/engine.py
+-rw-r--r--   0        0        0      508 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/db/main.py
+-rw-r--r--   0        0        0     1515 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/db/types.py
+-rw-r--r--   0        0        0     1689 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/db/workspace.py
+-rw-r--r--   0        0        0        0 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/__init__.py
+-rw-r--r--   0        0        0     2029 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/admin_api_key.py
+-rw-r--r--   0        0        0     1462 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/admin_authentication.py
+-rw-r--r--   0        0        0     1236 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/admin_session.py
+-rw-r--r--   0        0        0     9632 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/auth.py
+-rw-r--r--   0        0        0      962 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/authentication_flow.py
+-rw-r--r--   0        0        0     1032 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/client.py
+-rw-r--r--   0        0        0     1291 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/current_workspace.py
+-rw-r--r--   0        0        0      408 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/fief.py
+-rw-r--r--   0        0        0     2034 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/locale.py
+-rw-r--r--   0        0        0      982 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/main_managers.py
+-rw-r--r--   0        0        0     1113 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/pagination.py
+-rw-r--r--   0        0        0      756 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/register.py
+-rw-r--r--   0        0        0     1401 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/reset.py
+-rw-r--r--   0        0        0      558 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/session_token.py
+-rw-r--r--   0        0        0      105 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/tasks.py
+-rw-r--r--   0        0        0     1773 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/tenant.py
+-rw-r--r--   0        0        0     5890 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/token.py
+-rw-r--r--   0        0        0     7555 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/users.py
+-rw-r--r--   0        0        0     1024 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/workspace.py
+-rw-r--r--   0        0        0      754 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/workspace_creation.py
+-rw-r--r--   0        0        0      141 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/workspace_db.py
+-rw-r--r--   0        0        0     1783 2022-03-31 14:16:21.476242 fief-server-0.9.0/fief/dependencies/workspace_managers.py
+-rw-r--r--   0        0        0    10753 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/emails/base.html
+-rw-r--r--   0        0        0     1043 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/emails/forgot_password.html
+-rw-r--r--   0        0        0      284 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/emails/welcome.html
+-rw-r--r--   0        0        0      692 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/errors.py
+-rw-r--r--   0        0        0     3224 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/exceptions.py
+-rw-r--r--   0        0        0      369 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/fastapi_users.py
+-rw-r--r--   0        0        0     1236 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/locale.py
+-rw-r--r--   0        0        0     4805 2022-03-31 14:17:05.775437 fief-server-0.9.0/fief/locale/en_US/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     6949 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/locale/en_US/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     5194 2022-03-31 14:17:05.771437 fief-server-0.9.0/fief/locale/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0     7342 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/locale/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      327 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/logging.py
+-rw-r--r--   0        0        0     1058 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/__init__.py
+-rw-r--r--   0        0        0      465 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/admin_api_key.py
+-rw-r--r--   0        0        0      519 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/admin_session_token.py
+-rw-r--r--   0        0        0     1042 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/authorization_code.py
+-rw-r--r--   0        0        0     5569 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/base.py
+-rw-r--r--   0        0        0      747 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/client.py
+-rw-r--r--   0        0        0      546 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/grant.py
+-rw-r--r--   0        0        0      473 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/login_session.py
+-rw-r--r--   0        0        0      693 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/refresh_token.py
+-rw-r--r--   0        0        0      693 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/session_token.py
+-rw-r--r--   0        0        0      992 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/tenant.py
+-rw-r--r--   0        0        0      171 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/user.py
+-rw-r--r--   0        0        0     1093 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/workspace.py
+-rw-r--r--   0        0        0      630 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/managers/workspace_user.py
+-rw-r--r--   0        0        0      960 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/__init__.py
+-rw-r--r--   0        0        0      710 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/admin_api_key.py
+-rw-r--r--   0        0        0     1061 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/admin_session_token.py
+-rw-r--r--   0        0        0     1710 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/authorization_code.py
+-rw-r--r--   0        0        0      538 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/base.py
+-rw-r--r--   0        0        0     1612 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/client.py
+-rw-r--r--   0        0        0     2499 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/generics.py
+-rw-r--r--   0        0        0      911 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/grant.py
+-rw-r--r--   0        0        0     1596 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/login_session.py
+-rw-r--r--   0        0        0     1236 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/refresh_token.py
+-rw-r--r--   0        0        0      844 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/session_token.py
+-rw-r--r--   0        0        0     1267 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/tenant.py
+-rw-r--r--   0        0        0     1221 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/user.py
+-rw-r--r--   0        0        0     3550 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/workspace.py
+-rw-r--r--   0        0        0      780 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/models/workspace_user.py
+-rw-r--r--   0        0        0      283 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/paths.py
+-rw-r--r--   0        0        0      300 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/__init__.py
+-rw-r--r--   0        0        0      384 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/admin_api_key.py
+-rw-r--r--   0        0        0     3834 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/auth.py
+-rw-r--r--   0        0        0     1301 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/client.py
+-rw-r--r--   0        0        0      456 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/generics.py
+-rw-r--r--   0        0        0      700 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/register.py
+-rw-r--r--   0        0        0      930 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/reset.py
+-rw-r--r--   0        0        0      241 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/tenant.py
+-rw-r--r--   0        0        0      848 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/user.py
+-rw-r--r--   0        0        0     3037 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/well_known.py
+-rw-r--r--   0        0        0     2572 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/schemas/workspace.py
+-rw-r--r--   0        0        0        0 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/__init__.py
+-rw-r--r--   0        0        0     6250 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/authentication_flow.py
+-rw-r--r--   0        0        0      601 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/email/__init__.py
+-rw-r--r--   0        0        0      470 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/email/base.py
+-rw-r--r--   0        0        0      366 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/email/null.py
+-rw-r--r--   0        0        0     1066 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/email/postmark.py
+-rw-r--r--   0        0        0     4156 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/main_workspace.py
+-rw-r--r--   0        0        0     3934 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/workspace_creation.py
+-rw-r--r--   0        0        0     1960 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/services/workspace_db.py
+-rw-r--r--   0        0        0     4402 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/settings.py
+-rw-r--r--   0        0        0     1189 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/static/favicon.svg
+-rw-r--r--   0        0        0     1898 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/static/fief-logo.svg
+-rw-r--r--   0        0        0     1451 2022-03-31 14:17:07.031527 fief-server-0.9.0/fief/static/frontend/asset-manifest.json
+-rw-r--r--   0        0        0     1189 2022-03-31 14:17:07.023527 fief-server-0.9.0/fief/static/frontend/favicon.svg
+-rw-r--r--   0        0        0      733 2022-03-31 14:17:07.075530 fief-server-0.9.0/fief/static/frontend/index.html
+-rw-r--r--   0        0        0      709 2022-03-31 14:17:07.179538 fief-server-0.9.0/fief/static/frontend/locales/en/api-keys.json
+-rw-r--r--   0        0        0     1228 2022-03-31 14:17:07.215540 fief-server-0.9.0/fief/static/frontend/locales/en/clients.json
+-rw-r--r--   0        0        0     1174 2022-03-31 14:17:07.219540 fief-server-0.9.0/fief/static/frontend/locales/en/common.json
+-rw-r--r--   0        0        0      117 2022-03-31 14:17:07.271544 fief-server-0.9.0/fief/static/frontend/locales/en/tenants.json
+-rw-r--r--   0        0        0      300 2022-03-31 14:17:07.259543 fief-server-0.9.0/fief/static/frontend/locales/en/users.json
+-rw-r--r--   0        0        0     1016 2022-03-31 14:17:07.307547 fief-server-0.9.0/fief/static/frontend/locales/en/workspaces.json
+-rw-r--r--   0        0        0     5347 2022-03-31 14:17:07.091531 fief-server-0.9.0/fief/static/frontend/logo192.png
+-rw-r--r--   0        0        0     9664 2022-03-31 14:17:07.115533 fief-server-0.9.0/fief/static/frontend/logo512.png
+-rw-r--r--   0        0        0      492 2022-03-31 14:17:07.135534 fief-server-0.9.0/fief/static/frontend/manifest.json
+-rw-r--r--   0        0        0       67 2022-03-31 14:17:07.159536 fief-server-0.9.0/fief/static/frontend/robots.txt
+-rw-r--r--   0        0        0    35836 2022-03-31 14:17:07.347550 fief-server-0.9.0/fief/static/frontend/static/css/main.45cf7c31.css
+-rw-r--r--   0        0        0    18184 2022-03-31 14:17:07.319548 fief-server-0.9.0/fief/static/frontend/static/css/main.45cf7c31.css.map
+-rw-r--r--   0        0        0     4607 2022-03-31 14:17:07.391553 fief-server-0.9.0/fief/static/frontend/static/js/787.707d1bd1.chunk.js
+-rw-r--r--   0        0        0    10281 2022-03-31 14:17:07.363551 fief-server-0.9.0/fief/static/frontend/static/js/787.707d1bd1.chunk.js.map
+-rw-r--r--   0        0        0   511557 2022-03-31 14:17:07.463558 fief-server-0.9.0/fief/static/frontend/static/js/main.3b0373f0.js
+-rw-r--r--   0        0        0     1493 2022-03-31 14:17:07.407554 fief-server-0.9.0/fief/static/frontend/static/js/main.3b0373f0.js.LICENSE.txt
+-rw-r--r--   0        0        0  1596711 2022-03-31 14:17:07.483559 fief-server-0.9.0/fief/static/frontend/static/js/main.3b0373f0.js.map
+-rw-r--r--   0        0        0      667 2022-03-31 14:17:07.511561 fief-server-0.9.0/fief/static/frontend/static/media/clients.9b0e9946f3619c28cab1767cc62a22aa.svg
+-rw-r--r--   0        0        0      335 2022-03-31 14:17:07.539564 fief-server-0.9.0/fief/static/frontend/static/media/cloud.287167692745095704efd591b87bcaf1.svg
+-rw-r--r--   0        0        0     1116 2022-03-31 14:17:07.551564 fief-server-0.9.0/fief/static/frontend/static/media/cogwheel.bbc48a85c6dc5c6dd1eeb294e3afa715.svg
+-rw-r--r--   0        0        0      942 2022-03-31 14:17:07.579566 fief-server-0.9.0/fief/static/frontend/static/media/dashboard.580511ccd86590b36f5819c267461ebe.svg
+-rw-r--r--   0        0        0     1898 2022-03-31 14:17:07.587567 fief-server-0.9.0/fief/static/frontend/static/media/fief-logo-red.ee09b120c56412b835b2cb57d6adaa58.svg
+-rw-r--r--   0        0        0      388 2022-03-31 14:17:07.619569 fief-server-0.9.0/fief/static/frontend/static/media/getFetch.c780682470504fffbd04.cjs
+-rw-r--r--   0        0        0      635 2022-03-31 14:17:07.631570 fief-server-0.9.0/fief/static/frontend/static/media/key.69ef1cd7ed8906a8b62c0bb9cb74c731.svg
+-rw-r--r--   0        0        0     1926 2022-03-31 14:17:07.655572 fief-server-0.9.0/fief/static/frontend/static/media/tenants.3a942265546a3a2ebbf16aa58f45311f.svg
+-rw-r--r--   0        0        0      455 2022-03-31 14:17:07.679573 fief-server-0.9.0/fief/static/frontend/static/media/users.acc3e62b7bc3248222826909f7911672.svg
+-rw-r--r--   0        0        0    26633 2022-03-31 14:17:06.803511 fief-server-0.9.0/fief/static/output.css
+-rw-r--r--   0        0        0      267 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/tasks/__init__.py
+-rw-r--r--   0        0        0     3656 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/tasks/base.py
+-rw-r--r--   0        0        0     1299 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/tasks/forgot_password.py
+-rw-r--r--   0        0        0     1171 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/tasks/register.py
+-rw-r--r--   0        0        0     2996 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/templates/auth_layout.html
+-rw-r--r--   0        0        0      181 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/templates/authorize.html
+-rw-r--r--   0        0        0      572 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/templates/base.html
+-rw-r--r--   0        0        0     1080 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/templates/consent.html
+-rw-r--r--   0        0        0     1161 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/templates/forgot_password.html
+-rw-r--r--   0        0        0     1556 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/templates/login.html
+-rw-r--r--   0        0        0     1695 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/templates/register.html
+-rw-r--r--   0        0        0     1194 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/templates/reset_password.html
+-rw-r--r--   0        0        0       44 2022-03-31 14:16:21.480242 fief-server-0.9.0/fief/worker.py
+-rw-r--r--   0        0        0     1793 2022-03-31 14:16:21.480242 fief-server-0.9.0/justfile
+-rw-r--r--   0        0        0    70684 2022-03-31 14:16:21.484243 fief-server-0.9.0/package-lock.json
+-rw-r--r--   0        0        0      262 2022-03-31 14:16:21.484243 fief-server-0.9.0/package.json
+-rw-r--r--   0        0        0     2492 2022-03-31 14:16:21.484243 fief-server-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      183 2022-03-31 14:16:21.484243 fief-server-0.9.0/setup.cfg
+-rw-r--r--   0        0        0     2991 2022-03-31 14:16:21.484243 fief-server-0.9.0/tailwind.config.js
+-rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 fief-server-0.9.0/PKG-INFO
```

### Comparing `fief-server-0.8.2/fief/alembic.ini` & `fief-server-0.9.0/fief/alembic.ini`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/alembic/env.py` & `fief-server-0.9.0/fief/alembic/env.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/alembic/main_versions/274bc650f9a2_initial_migration.py` & `fief-server-0.9.0/fief/alembic/main_versions/274bc650f9a2_initial_migration.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/alembic/workspace_versions/0ba35b227f10_initial_migration.py` & `fief-server-0.9.0/fief/alembic/workspace_versions/0ba35b227f10_initial_migration.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/alembic/workspace_versions/0e7f8edd4e21_add_authenticated_at_column_to_.py` & `fief-server-0.9.0/fief/alembic/workspace_versions/0e7f8edd4e21_add_authenticated_at_column_to_.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/alembic/workspace_versions/1df8009b83c5_add_redirect_uris_column_to_client.py` & `fief-server-0.9.0/fief/alembic/workspace_versions/1df8009b83c5_add_redirect_uris_column_to_client.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/alembic/workspace_versions/cfaa3c85d3d3_update_password_hash_length.py` & `fief-server-0.9.0/fief/alembic/workspace_versions/cfaa3c85d3d3_update_password_hash_length.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/alembic/workspace_versions/d3cb52370070_add_nonce_column_to_loginsession_and_.py` & `fief-server-0.9.0/fief/alembic/workspace_versions/d3cb52370070_add_nonce_column_to_loginsession_and_.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/app.py` & `fief-server-0.9.0/fief/app.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/admin/app.py` & `fief-server-0.9.0/fief/apps/admin/app.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/admin/routers/api_keys.py` & `fief-server-0.9.0/fief/apps/admin/routers/api_keys.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/admin/routers/auth.py` & `fief-server-0.9.0/fief/apps/admin/routers/auth.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/admin/routers/clients.py` & `fief-server-0.9.0/fief/apps/admin/routers/clients.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/admin/routers/tenants.py` & `fief-server-0.9.0/fief/apps/admin/routers/tenants.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/admin/routers/users.py` & `fief-server-0.9.0/fief/apps/admin/routers/users.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/admin/routers/workspaces.py` & `fief-server-0.9.0/fief/apps/admin/routers/workspaces.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/admin_frontend/app.py` & `fief-server-0.9.0/fief/apps/admin_frontend/app.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/auth/app.py` & `fief-server-0.9.0/fief/apps/auth/app.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/auth/exception_handlers.py` & `fief-server-0.9.0/fief/apps/auth/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/auth/routers/auth.py` & `fief-server-0.9.0/fief/apps/auth/routers/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 from fastapi import APIRouter, Depends, Query, Request, status
 from fastapi.responses import RedirectResponse
 from fastapi.security.oauth2 import OAuth2PasswordRequestForm
 
 from fief.apps.auth.templates import templates
 from fief.csrf import check_csrf
 from fief.dependencies.auth import (
+    check_unsupported_request_parameter,
     get_authorize_client,
+    get_authorize_code_challenge,
     get_authorize_prompt,
     get_authorize_redirect_uri,
     get_authorize_response_type,
     get_authorize_scope,
     get_authorize_screen,
     get_consent_action,
     get_consent_prompt,
@@ -30,23 +32,30 @@
 from fief.models.session_token import SessionToken
 from fief.schemas.auth import LoginError
 from fief.services.authentication_flow import AuthenticationFlow
 
 router = APIRouter(dependencies=[Depends(check_csrf), Depends(get_translations)])
 
 
-@router.get("/authorize", name="auth:authorize")
+@router.get(
+    "/authorize",
+    name="auth:authorize",
+    dependencies=[Depends(check_unsupported_request_parameter)],
+)
 async def authorize(
     request: Request,
     response_type: str = Depends(get_authorize_response_type),
     client: Client = Depends(get_authorize_client),
     redirect_uri: str = Depends(get_authorize_redirect_uri),
     scope: List[str] = Depends(get_authorize_scope),
     prompt: Optional[str] = Depends(get_authorize_prompt),
     screen: str = Depends(get_authorize_screen),
+    code_challenge_tuple: Optional[Tuple[str, str]] = Depends(
+        get_authorize_code_challenge
+    ),
     state: Optional[str] = Query(None),
     nonce: Optional[str] = Query(None),
     authentication_flow: AuthenticationFlow = Depends(get_authentication_flow),
     has_valid_session_token: bool = Depends(has_valid_session_token),
 ):
     tenant = client.tenant
 
@@ -61,14 +70,15 @@
     response = await authentication_flow.create_login_session(
         response,
         response_type=response_type,
         redirect_uri=redirect_uri,
         scope=scope,
         state=state,
         nonce=nonce,
+        code_challenge_tuple=code_challenge_tuple,
         client=client,
     )
 
     return response
 
 
 @router.get("/login", name="auth:login.get")
@@ -139,14 +149,15 @@
         user_id = session_token.user_id
         response = await authentication_flow.get_authorization_code_success_redirect(
             login_session.redirect_uri,
             login_session.scope,
             session_token.created_at,
             login_session.state,
             login_session.nonce,
+            login_session.get_code_challenge_tuple(),
             login_session.client,
             user_id,
         )
         response = await authentication_flow.delete_login_session(
             response, login_session
         )
         return response
@@ -185,14 +196,15 @@
         )
         response = await authentication_flow.get_authorization_code_success_redirect(
             login_session.redirect_uri,
             login_session.scope,
             session_token.created_at,
             login_session.state,
             login_session.nonce,
+            login_session.get_code_challenge_tuple(),
             login_session.client,
             user_id,
         )
     elif action == "deny":
         response = AuthenticationFlow.get_authorization_code_error_redirect(
             login_session.redirect_uri,
             "access_denied",
```

### Comparing `fief-server-0.8.2/fief/apps/auth/routers/register.py` & `fief-server-0.9.0/fief/apps/auth/routers/register.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/auth/routers/reset.py` & `fief-server-0.9.0/fief/apps/auth/routers/reset.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/auth/routers/token.py` & `fief-server-0.9.0/fief/apps/auth/routers/token.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime, timedelta, timezone
 from typing import List, Optional, Tuple
 
-from fastapi import APIRouter, Depends
+from fastapi import APIRouter, Depends, Response
 from pydantic import UUID4
 
 from fief.crypto.access_token import generate_access_token
 from fief.crypto.id_token import generate_id_token
 from fief.dependencies.current_workspace import get_current_workspace
 from fief.dependencies.tenant import get_current_tenant
 from fief.dependencies.token import (
@@ -23,14 +23,15 @@
 REFRESH_TOKEN_LIFETIME = 3600 * 24 * 30
 
 router = APIRouter()
 
 
 @router.post("/token", name="auth:token")
 async def token(
+    response: Response,
     grant_request: GrantRequest = Depends(validate_grant_request),
     user: UserDB = Depends(get_user_from_grant_request),
     refresh_token_manager: RefreshTokenManager = Depends(get_refresh_token_manager),
     workspace: Workspace = Depends(get_current_workspace),
     tenant: Tenant = Depends(get_current_tenant),
 ):
     scope = grant_request["scope"]
@@ -66,8 +67,10 @@
             user_id=user.id,
             client_id=client.id,
             authenticated_at=authenticated_at,
         )
         refresh_token = await refresh_token_manager.create(refresh_token)
         token_response.refresh_token = refresh_token.token
 
+    response.headers["Cache-Control"] = "no-store"
+    response.headers["Pragma"] = "no-cache"
     return token_response.dict(exclude_none=True)
```

### Comparing `fief-server-0.8.2/fief/apps/auth/routers/user.py` & `fief-server-0.9.0/fief/apps/auth/routers/user.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/apps/auth/routers/well_known.py` & `fief-server-0.9.0/fief/apps/auth/routers/well_known.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from fastapi import APIRouter, Request
 from fastapi.param_functions import Depends
 from jwcrypto import jwk
 
 from fief.dependencies.current_workspace import get_current_workspace
 from fief.dependencies.tenant import get_current_tenant
 from fief.models import Tenant, Workspace
-from fief.schemas.well_known import OpenIDConfiguration
+from fief.schemas.well_known import OpenIDProviderMetadata
 from fief.settings import settings
 
 router = APIRouter()
 
 
 @router.get("/openid-configuration", name="well_known:openid_configuration")
 async def get_openid_configuration(
@@ -20,15 +20,15 @@
     url_for_params = {}
     if not tenant.default:
         url_for_params["tenant_slug"] = tenant.slug
 
     def _url_for(name: str) -> str:
         return request.url_for(name, **url_for_params)
 
-    configuration = OpenIDConfiguration(
+    configuration = OpenIDProviderMetadata(
         issuer=tenant.get_host(workspace.domain),
         authorization_endpoint=_url_for("auth:authorize"),
         token_endpoint=_url_for("auth:token"),
         userinfo_endpoint=_url_for("user:userinfo.get"),
         jwks_uri=_url_for("well_known:jwks"),
         registration_endpoint=_url_for("register:get"),
         scopes_supported=["openid", "offline_access"],
@@ -40,14 +40,16 @@
         id_token_encryption_enc_values_supported=["A256CBC-HS512"],
         userinfo_signing_alg_values_supported=["none"],
         token_endpoint_auth_methods_supported=[
             "client_secret_basic",
             "client_secret_post",
         ],
         claims_supported=["email", "tenant_id"],
+        request_parameter_supported=False,
+        code_challenge_methods_supported=["plain", "S256"],
         service_documentation=settings.fief_documentation_url,
     )
 
     return configuration.dict(exclude_unset=True)
 
 
 @router.get("/jwks.json", name="well_known:jwks")
```

### Comparing `fief-server-0.8.2/fief/apps/auth/templates.py` & `fief-server-0.9.0/fief/apps/auth/templates.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/cli.py` & `fief-server-0.9.0/fief/cli.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/cors.py` & `fief-server-0.9.0/fief/cors.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/crypto/access_token.py` & `fief-server-0.9.0/fief/crypto/access_token.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/crypto/encryption.py` & `fief-server-0.9.0/fief/crypto/encryption.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/crypto/id_token.py` & `fief-server-0.9.0/fief/crypto/id_token.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/csrf.py` & `fief-server-0.9.0/fief/csrf.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/db/engine.py` & `fief-server-0.9.0/fief/db/engine.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/db/types.py` & `fief-server-0.9.0/fief/db/types.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/db/workspace.py` & `fief-server-0.9.0/fief/db/workspace.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/admin_api_key.py` & `fief-server-0.9.0/fief/dependencies/admin_api_key.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/admin_authentication.py` & `fief-server-0.9.0/fief/dependencies/admin_authentication.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/admin_session.py` & `fief-server-0.9.0/fief/dependencies/admin_session.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/auth.py` & `fief-server-0.9.0/fief/dependencies/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timezone
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 from fastapi import Cookie, Depends, Form, Query, Response
 from pydantic import UUID4
 
 from fief.dependencies.authentication_flow import get_authentication_flow
 from fief.dependencies.locale import get_gettext
 from fief.dependencies.session_token import get_session_token
@@ -69,14 +69,30 @@
     return redirect_uri
 
 
 async def get_authorize_state(state: Optional[str] = Query(None)) -> Optional[str]:
     return state
 
 
+async def check_unsupported_request_parameter(
+    request_parameter: Optional[str] = Query(None, alias="request"),
+    redirect_uri: str = Depends(get_authorize_redirect_uri),
+    state: Optional[str] = Depends(get_authorize_state),
+    _=Depends(get_gettext),
+) -> None:
+    if request_parameter is not None:
+        raise AuthorizeRedirectException(
+            AuthorizeRedirectError.get_request_not_supported(
+                _("request parameter is not supported")
+            ),
+            redirect_uri,
+            state,
+        )
+
+
 async def get_authorize_response_type(
     response_type: Optional[str] = Query(None),
     redirect_uri: str = Depends(get_authorize_redirect_uri),
     state: Optional[str] = Depends(get_authorize_state),
     _=Depends(get_gettext),
 ) -> str:
     if response_type is None:
@@ -165,14 +181,36 @@
             redirect_uri,
             state,
         )
 
     return screen
 
 
+async def get_authorize_code_challenge(
+    code_challenge: Optional[str] = Query(None),
+    code_challenge_method: Optional[str] = Query("plain"),
+    redirect_uri: str = Depends(get_authorize_redirect_uri),
+    state: Optional[str] = Depends(get_authorize_state),
+    _=Depends(get_gettext),
+) -> Optional[Tuple[str, str]]:
+    if code_challenge is None:
+        return None
+
+    if code_challenge_method not in ["plain", "S256"]:
+        raise AuthorizeRedirectException(
+            AuthorizeRedirectError.get_invalid_request(
+                _("Unsupported code_challenge_method")
+            ),
+            redirect_uri,
+            state,
+        )
+
+    return code_challenge, code_challenge_method
+
+
 async def has_valid_session_token(
     max_age: Optional[int] = Query(None),
     session_token: Optional[SessionToken] = Depends(get_session_token),
 ) -> bool:
     if session_token is None:
         return False
```

### Comparing `fief-server-0.8.2/fief/dependencies/authentication_flow.py` & `fief-server-0.9.0/fief/dependencies/authentication_flow.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/client.py` & `fief-server-0.9.0/fief/dependencies/client.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/current_workspace.py` & `fief-server-0.9.0/fief/dependencies/current_workspace.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/locale.py` & `fief-server-0.9.0/fief/dependencies/locale.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/main_managers.py` & `fief-server-0.9.0/fief/dependencies/main_managers.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/pagination.py` & `fief-server-0.9.0/fief/dependencies/pagination.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/register.py` & `fief-server-0.9.0/fief/dependencies/register.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/reset.py` & `fief-server-0.9.0/fief/dependencies/reset.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/session_token.py` & `fief-server-0.9.0/fief/dependencies/session_token.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/tenant.py` & `fief-server-0.9.0/fief/dependencies/tenant.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/token.py` & `fief-server-0.9.0/fief/dependencies/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import AsyncGenerator, List, Optional, TypedDict
 
 from fastapi import Depends, Form
 from fastapi.security import HTTPBasic, HTTPBasicCredentials
 from fastapi_users.manager import UserNotExists
 from pydantic import UUID4
 
+from fief.crypto.code_challenge import verify_code_verifier
 from fief.dependencies.users import UserManager, get_user_manager
 from fief.dependencies.workspace_managers import (
     get_authorization_code_manager,
     get_client_manager,
     get_refresh_token_manager,
 )
 from fief.exceptions import TokenRequestException
@@ -70,14 +71,15 @@
         raise TokenRequestException(TokenError.get_invalid_request())
 
     return grant_type
 
 
 async def validate_grant_request(
     code: Optional[str] = Form(None),
+    code_verifier: Optional[str] = Form(None),
     redirect_uri: Optional[str] = Form(None),
     refresh_token_token: Optional[str] = Form(None, alias="refresh_token"),
     scope: Optional[str] = Form(None),
     grant_type: str = Depends(get_grant_type),
     client: Client = Depends(authenticate_client_secret),
     authorization_code_manager: AuthorizationCodeManager = Depends(
         get_authorization_code_manager
@@ -97,14 +99,21 @@
 
         if authorization_code.client.id != client.id:
             raise TokenRequestException(TokenError.get_invalid_grant())
 
         if authorization_code.redirect_uri != redirect_uri:
             raise TokenRequestException(TokenError.get_invalid_grant())
 
+        code_challenge_tuple = authorization_code.get_code_challenge_tuple()
+        if code_challenge_tuple is not None:
+            if code_verifier is None or not verify_code_verifier(
+                code_verifier, code_challenge_tuple[0], code_challenge_tuple[1]
+            ):
+                raise TokenRequestException(TokenError.get_invalid_grant())
+
         yield {
             "user_id": authorization_code.user_id,
             "scope": authorization_code.scope,
             "authenticated_at": authorization_code.authenticated_at,
             "nonce": authorization_code.nonce,
             "client": client,
         }
```

### Comparing `fief-server-0.8.2/fief/dependencies/users.py` & `fief-server-0.9.0/fief/dependencies/users.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/workspace.py` & `fief-server-0.9.0/fief/dependencies/workspace.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/workspace_creation.py` & `fief-server-0.9.0/fief/dependencies/workspace_creation.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/dependencies/workspace_managers.py` & `fief-server-0.9.0/fief/dependencies/workspace_managers.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/emails/base.html` & `fief-server-0.9.0/fief/emails/base.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/emails/forgot_password.html` & `fief-server-0.9.0/fief/emails/forgot_password.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/errors.py` & `fief-server-0.9.0/fief/errors.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/exceptions.py` & `fief-server-0.9.0/fief/exceptions.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/locale.py` & `fief-server-0.9.0/fief/locale.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,26 @@
     try:
         TRANSLATIONS[TERRITORY_FALLBACKS[locale]] = translation
     except KeyError:
         pass
 
 
 def get_preferred_locale(
-    preffered: List[str],
+    preferred: List[str],
     *,
     supported: List[str] = SUPPORTED_LOCALES,
     fallback: str = FALLBACK
 ) -> str:
-    locale = core.negotiate_locale(preffered, supported)
+    locale = core.negotiate_locale(preferred, supported)
     if locale is None:
         return fallback
     return locale
 
 
 def get_preferred_translations(
-    preffered: List[str],
+    preferred: List[str],
     *,
     supported: List[str] = SUPPORTED_LOCALES,
     fallback: str = FALLBACK
 ) -> Translations:
-    locale = get_preferred_locale(preffered, supported=supported, fallback=fallback)
+    locale = get_preferred_locale(preferred, supported=supported, fallback=fallback)
     return TRANSLATIONS[locale]
```

### Comparing `fief-server-0.8.2/fief/locale/en_US/LC_MESSAGES/messages.mo` & `fief-server-0.9.0/fief/locale/en_US/LC_MESSAGES/messages.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Fief\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-02-13 15:49+0100\n"
+"POT-Creation-Date: 2022-03-31 14:17+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: en_us\n"
 "Language-Team: en_us <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -121,26 +121,37 @@
 
 msgid "This will allow %(name)s to:"
 msgstr "This will allow %(name)s to:"
 
 msgid "Unknown client"
 msgstr "Unknown client"
 
+msgid "Unsupported code_challenge_method"
+msgstr "Unsupported code_challenge_method"
+
+msgid ""
+"Use this link to reset your password. This link is only valid for 1 hour."
+msgstr ""
+"Use this link to reset your password. This link is only valid for 1 hour."
+
 msgid "User consent is required for this scope"
 msgstr "User consent is required for this scope"
 
 msgid "User is not logged in"
 msgstr "User is not logged in"
 
 msgid "Welcome back!"
 msgstr "Welcome back!"
 
 msgid "Welcome to %(tenant)s!"
 msgstr "Welcome to %(tenant)s!"
 
+msgid "Welcome to %(tenant)s! We're thrilled to have you on board."
+msgstr "Welcome to %(tenant)s! We're thrilled to have you on board."
+
 msgid ""
 "You recently requested to reset your password for your %(tenant)s account. "
 "Use the button below to reset it."
 msgstr ""
 "You recently requested to reset your password for your %(tenant)s account. "
 "Use the button below to reset it."
 
@@ -155,14 +166,20 @@
 
 msgid "prompt should either be \"none\", \"login\" or \"register\""
 msgstr "prompt should either be \"none\", \"login\" or \"register\""
 
 msgid "redirect_uri is missing"
 msgstr "redirect_uri is missing"
 
+msgid "redirect_uri is not authorized for this client"
+msgstr "redirect_uri is not authorized for this client"
+
+msgid "request parameter is not supported"
+msgstr "request parameter is not supported"
+
 msgid "response_type is missing"
 msgstr "response_type is missing"
 
 msgid "response_type should be \"code\""
 msgstr "response_type should be \"code\""
 
 msgid "scope is missing"
```

### Comparing `fief-server-0.8.2/fief/locale/en_US/LC_MESSAGES/messages.po` & `fief-server-0.9.0/fief/locale/en_US/LC_MESSAGES/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,249 +1,238 @@
-
 msgid ""
 msgstr ""
-"Project-Id-Version:  Fief\n"
-"Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-02-13 15:49+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language: en_us\n"
-"Language-Team: en_us <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1)\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"X-Generator: POEditor.com\n"
+"Project-Id-Version: Fief\n"
+"Language: en-us\n"
+
+#: fief/templates/auth_layout.html:49
+msgid "Powered by"
+msgstr "Powered by"
+
+#: fief/templates/login.html:3
+msgid "Login"
+msgstr "Login"
+
+#: fief/templates/login.html:5
+msgid "Welcome back!"
+msgstr "Welcome back!"
+
+#: fief/templates/forgot_password.html:11 fief/templates/login.html:11
+#: fief/templates/register.html:11
+msgid "Email address"
+msgstr "Email address"
+
+#: fief/templates/login.html:18 fief/templates/register.html:18
+msgid "Password"
+msgstr "Password"
+
+#: fief/templates/login.html:30
+msgid "Sign in"
+msgstr "Sign in"
 
-#: fief/errors.py:30
+#: fief/exceptions.py:20
 msgid "This field is required."
 msgstr "This field is required."
 
-#: fief/errors.py:31
+#: fief/exceptions.py:21
 msgid "This email address is invalid."
 msgstr "This email address is invalid."
 
-#: fief/errors.py:47
-msgid "type"
-msgstr "type"
-
-#: fief/apps/auth/routers/auth.py:99
+#: fief/apps/auth/routers/auth.py:112
 msgid "Invalid email or password"
 msgstr "Invalid email or password"
 
-#: fief/apps/auth/routers/auth.py:191
-msgid "The user denied access to their data."
-msgstr "The user denied access to their data."
-
-#: fief/apps/auth/routers/register.py:51
+#: fief/apps/auth/routers/register.py:54
 msgid "A user with the same email address already exists."
 msgstr "A user with the same email address already exists."
 
-#: fief/apps/auth/routers/reset.py:62
-msgid ""
-"Check your inbox! If an account associated with this email address exists"
-" in our system, you'll receive a link to reset your password."
-msgstr ""
-"Check your inbox! If an account associated with this email address exists"
-" in our system, you'll receive a link to reset your password."
-
-#: fief/apps/auth/routers/reset.py:84
-msgid "The reset password token is missing."
-msgstr "The reset password token is missing."
-
-#: fief/apps/auth/routers/reset.py:114
-msgid "The reset password token is invalid or expired."
-msgstr "The reset password token is invalid or expired."
+#: fief/dependencies/auth.py:100
+msgid "response_type is missing"
+msgstr "response_type is missing"
 
-#: fief/apps/auth/routers/reset.py:135
-msgid "Your password has been changed!"
-msgstr "Your password has been changed!"
+#: fief/dependencies/auth.py:108
+msgid "response_type should be \"code\""
+msgstr "response_type should be \"code\""
 
-#: fief/dependencies/auth.py:40
+#: fief/dependencies/auth.py:41
 msgid "client_id is missing"
 msgstr "client_id is missing"
 
-#: fief/dependencies/auth.py:46
+#: fief/dependencies/auth.py:47
 msgid "Unknown client"
 msgstr "Unknown client"
 
-#: fief/dependencies/auth.py:57
+#: fief/dependencies/auth.py:59
 msgid "redirect_uri is missing"
 msgstr "redirect_uri is missing"
 
-#: fief/dependencies/auth.py:75
-msgid "response_type is missing"
-msgstr "response_type is missing"
-
-#: fief/dependencies/auth.py:83
-msgid "response_type should be \"code\""
-msgstr "response_type should be \"code\""
-
-#: fief/dependencies/auth.py:100
+#: fief/dependencies/auth.py:125
 msgid "scope is missing"
 msgstr "scope is missing"
 
-#: fief/dependencies/auth.py:110
+#: fief/dependencies/auth.py:135
 msgid "scope should contain \"openid\""
 msgstr "scope should contain \"openid\""
 
-#: fief/dependencies/auth.py:129
-msgid "prompt should either be \"none\", \"login\" or \"register\""
-msgstr "prompt should either be \"none\", \"login\" or \"register\""
-
-#: fief/dependencies/auth.py:137
-msgid "User is not logged in"
-msgstr "User is not logged in"
-
-#: fief/dependencies/auth.py:154
+#: fief/dependencies/auth.py:179
 msgid "screen should either be \"login\" or \"register\""
 msgstr "screen should either be \"login\" or \"register\""
 
-#: fief/dependencies/auth.py:187
+#: fief/dependencies/auth.py:250
 msgid "Invalid login session"
 msgstr "Invalid login session"
 
-#: fief/dependencies/auth.py:202
-msgid "action should either be \"allow\" or \"deny\""
-msgstr "action should either be \"allow\" or \"deny\""
-
-#: fief/dependencies/auth.py:242
-msgid "User consent is required for this scope"
-msgstr "User consent is required for this scope"
-
-#: fief/dependencies/users.py:57
+#: fief/dependencies/users.py:79
 msgid "The password should be at least 8 characters."
 msgstr "The password should be at least 8 characters."
 
-#: fief/emails/base.html:496
-#, python-format
-msgid "&copy; %(year)d %(tenant)s. All rights reserved."
-msgstr "&copy; %(year)d %(tenant)s. All rights reserved."
+#: fief/templates/authorize.html:3 fief/templates/authorize.html:5
+msgid "Authorize"
+msgstr "Authorize"
 
-#: fief/emails/forgot_password.html:3
-#, fuzzy
-msgid "Use this link to reset your password. This link is only valid for 1 hour."
-msgstr "This password reset is only valid for the next hour."
+#: fief/templates/register.html:3 fief/templates/register.html:5
+msgid "Register"
+msgstr "Register"
 
-#: fief/emails/forgot_password.html:6
-#, python-format
-msgid ""
-"You recently requested to reset your password for your %(tenant)s "
-"account. Use the button below to reset it."
-msgstr ""
-"You recently requested to reset your password for your %(tenant)s "
-"account. Use the button below to reset it."
+#: fief/templates/register.html:28
+msgid "I already have an account"
+msgstr "I already have an account"
 
-#: fief/emails/forgot_password.html:6
-msgid "This password reset is only valid for the next hour."
-msgstr "This password reset is only valid for the next hour."
+#: fief/templates/register.html:30
+msgid "Sign up"
+msgstr "Sign up"
 
-#: fief/emails/forgot_password.html:15
-msgid "Reset your password"
-msgstr "Reset your password"
+#: fief/exceptions.py:37
+msgid "type"
+msgstr "type"
 
-#: fief/emails/welcome.html:3 fief/emails/welcome.html:6
-#, python-format
-msgid "Welcome to %(tenant)s! We're thrilled to have you on board."
-msgstr ""
+#: fief/apps/auth/routers/auth.py:211
+msgid "The user denied access to their data."
+msgstr "The user denied access to their data."
 
-#: fief/tasks/forgot_password.py:19
-#, python-format
-msgid "Reset your %(tenant)s's password"
-msgstr "Reset your %(tenant)s's password"
+#: fief/dependencies/auth.py:154
+msgid "prompt should either be \"none\", \"login\" or \"register\""
+msgstr "prompt should either be \"none\", \"login\" or \"register\""
 
-#: fief/tasks/register.py:19
-#, python-format
-msgid "Welcome to %(tenant)s!"
-msgstr "Welcome to %(tenant)s!"
+#: fief/dependencies/auth.py:162
+msgid "User is not logged in"
+msgstr "User is not logged in"
 
-#: fief/templates/auth_layout.html:50
-msgid "Powered by"
-msgstr "Powered by"
+#: fief/dependencies/auth.py:265
+msgid "action should either be \"allow\" or \"deny\""
+msgstr "action should either be \"allow\" or \"deny\""
 
-#: fief/templates/authorize.html:3 fief/templates/authorize.html:5
-msgid "Authorize"
-msgstr "Authorize"
+#: fief/dependencies/auth.py:310
+msgid "User consent is required for this scope"
+msgstr "User consent is required for this scope"
 
 #: fief/templates/consent.html:3
 msgid "Consent"
 msgstr "Consent"
 
 #: fief/templates/consent.html:5
-#, python-format
 msgid "%(name)s wants to access your account"
 msgstr "%(name)s wants to access your account"
 
 #: fief/templates/consent.html:10
-#, python-format
 msgid "This will allow %(name)s to:"
 msgstr "This will allow %(name)s to:"
 
 #: fief/templates/consent.html:21
 msgid "Deny"
 msgstr "Deny"
 
 #: fief/templates/consent.html:22
 msgid "Allow"
 msgstr "Allow"
 
+#: fief/apps/auth/routers/reset.py:62
+msgid "Check your inbox! If an account associated with this email address exists in our system, you'll receive a link to reset your password."
+msgstr "Check your inbox! If an account associated with this email address exists in our system, you'll receive a link to reset your password."
+
+#: fief/apps/auth/routers/reset.py:84
+msgid "The reset password token is missing."
+msgstr "The reset password token is missing."
+
+#: fief/apps/auth/routers/reset.py:114
+msgid "The reset password token is invalid or expired."
+msgstr "The reset password token is invalid or expired."
+
+#: fief/apps/auth/routers/reset.py:135
+msgid "Your password has been changed!"
+msgstr "Your password has been changed!"
+
+#: fief/emails/base.html:496
+msgid "&copy; %(year)d %(tenant)s. All rights reserved."
+msgstr "&copy; %(year)d %(tenant)s. All rights reserved."
+
+#: fief/emails/forgot_password.html:6
+msgid "You recently requested to reset your password for your %(tenant)s account. Use the button below to reset it."
+msgstr "You recently requested to reset your password for your %(tenant)s account. Use the button below to reset it."
+
+#: fief/emails/forgot_password.html:6
+msgid "This password reset is only valid for the next hour."
+msgstr "This password reset is only valid for the next hour."
+
+#: fief/emails/forgot_password.html:15
+msgid "Reset your password"
+msgstr "Reset your password"
+
+#: fief/tasks/forgot_password.py:20
+msgid "Reset your %(tenant)s's password"
+msgstr "Reset your %(tenant)s's password"
+
+#: fief/tasks/register.py:20
+msgid "Welcome to %(tenant)s!"
+msgstr "Welcome to %(tenant)s!"
+
 #: fief/templates/forgot_password.html:3 fief/templates/forgot_password.html:5
 msgid "Forgot password"
 msgstr "Forgot password"
 
-#: fief/templates/forgot_password.html:11 fief/templates/login.html:11
-#: fief/templates/register.html:11
-msgid "Email address"
-msgstr "Email address"
-
 #: fief/templates/forgot_password.html:21
 msgid "I remember my password"
 msgstr "I remember my password"
 
 #: fief/templates/forgot_password.html:23
 msgid "Send me a reset link"
 msgstr "Send me a reset link"
 
-#: fief/templates/login.html:3
-msgid "Login"
-msgstr "Login"
-
-#: fief/templates/login.html:5
-msgid "Welcome back!"
-msgstr "Welcome back!"
-
-#: fief/templates/login.html:18 fief/templates/register.html:18
-msgid "Password"
-msgstr "Password"
-
 #: fief/templates/login.html:28
 msgid "I forgot my password"
 msgstr "I forgot my password"
 
-#: fief/templates/login.html:30
-msgid "Sign in"
-msgstr "Sign in"
-
-#: fief/templates/register.html:3 fief/templates/register.html:5
-msgid "Register"
-msgstr "Register"
-
-#: fief/templates/register.html:28
-msgid "I already have an account"
-msgstr "I already have an account"
-
-#: fief/templates/register.html:30
-msgid "Sign up"
-msgstr "Sign up"
-
 #: fief/templates/reset_password.html:3 fief/templates/reset_password.html:5
 msgid "Reset password"
 msgstr "Reset password"
 
 #: fief/templates/reset_password.html:11
 msgid "New password"
 msgstr "New password"
 
 #: fief/templates/reset_password.html:22
 msgid "Reset my password"
 msgstr "Reset my password"
 
+#: fief/dependencies/auth.py:65
+msgid "redirect_uri is not authorized for this client"
+msgstr "redirect_uri is not authorized for this client"
+
+#: fief/dependencies/auth.py:85
+msgid "request parameter is not supported"
+msgstr "request parameter is not supported"
+
+#: fief/emails/forgot_password.html:3
+msgid "Use this link to reset your password. This link is only valid for 1 hour."
+msgstr "Use this link to reset your password. This link is only valid for 1 hour."
+
+#: fief/emails/welcome.html:3 fief/emails/welcome.html:6
+msgid "Welcome to %(tenant)s! We're thrilled to have you on board."
+msgstr "Welcome to %(tenant)s! We're thrilled to have you on board."
+
+#: fief/dependencies/auth.py:201
+msgid "Unsupported code_challenge_method"
+msgstr "Unsupported code_challenge_method"
+
```

### Comparing `fief-server-0.8.2/fief/locale/fr_FR/LC_MESSAGES/messages.mo` & `fief-server-0.9.0/fief/locale/fr_FR/LC_MESSAGES/messages.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  Fief\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-02-13 15:49+0100\n"
+"POT-Creation-Date: 2022-03-31 14:17+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: fr\n"
 "Language-Team: fr <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n > 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -28,15 +28,15 @@
 msgid "Authorize"
 msgstr "Autoriser"
 
 msgid ""
 "Check your inbox! If an account associated with this email address exists in "
 "our system, you'll receive a link to reset your password."
 msgstr ""
-"Vérifiez votre boîte de réception! Si un compte associé à cette adresse e-"
+"Vérifiez votre boîte de réception ! Si un compte associé à cette adresse e-"
 "mail existe dans notre système, vous allez recevoir un lien pour "
 "réinitialiser votre mot de passe."
 
 msgid "Consent"
 msgstr "Consentement"
 
 msgid "Deny"
@@ -122,26 +122,39 @@
 
 msgid "This will allow %(name)s to:"
 msgstr "Cela permettra à %(name)s de :"
 
 msgid "Unknown client"
 msgstr "Client inconnu"
 
+msgid "Unsupported code_challenge_method"
+msgstr "Méthode de code_challenge non supportée"
+
+msgid ""
+"Use this link to reset your password. This link is only valid for 1 hour."
+msgstr ""
+"Utilisez ce lien pour réinitialiser votre mot de passe. Ce lien n'est valide "
+"qu'une heure."
+
 msgid "User consent is required for this scope"
 msgstr "Le consentement de l'utilisateur est requis pour ce scope"
 
 msgid "User is not logged in"
 msgstr "L'utilisateur n'est pas connecté"
 
 msgid "Welcome back!"
 msgstr "Ravi de vous revoir !"
 
 msgid "Welcome to %(tenant)s!"
 msgstr "Bienvenue sur %(tenant)s !"
 
+msgid "Welcome to %(tenant)s! We're thrilled to have you on board."
+msgstr ""
+"Bienvenue sur %(tenant)s ! Nous sommes heureux de vous compter parmi nous."
+
 msgid ""
 "You recently requested to reset your password for your %(tenant)s account. "
 "Use the button below to reset it."
 msgstr ""
 "Vous avez demandé à réinitialiser le mot de passe de votre compte "
 "%(tenant)s. Utilisez le bouton ci-dessous pour le réinitialiser."
 
@@ -156,14 +169,20 @@
 
 msgid "prompt should either be \"none\", \"login\" or \"register\""
 msgstr "prompt doit être \"none\", \"login\" ou \"register\""
 
 msgid "redirect_uri is missing"
 msgstr "redirect_uri manquant"
 
+msgid "redirect_uri is not authorized for this client"
+msgstr "Cette redirect_uri n'est pas autorisée pour ce client"
+
+msgid "request parameter is not supported"
+msgstr "Le paramètre request n'est pas supporté"
+
 msgid "response_type is missing"
 msgstr "response_type manquant"
 
 msgid "response_type should be \"code\""
 msgstr "response_type doit être \"code\""
 
 msgid "scope is missing"
```

### Comparing `fief-server-0.8.2/fief/locale/fr_FR/LC_MESSAGES/messages.po` & `fief-server-0.9.0/fief/locale/fr_FR/LC_MESSAGES/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,250 +1,238 @@
-
 msgid ""
 msgstr ""
-"Project-Id-Version:  Fief\n"
-"Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-02-13 15:49+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language: fr\n"
-"Language-Team: fr <LL@li.org>\n"
-"Plural-Forms: nplurals=2; plural=(n > 1)\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=utf-8\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"X-Generator: POEditor.com\n"
+"Project-Id-Version: Fief\n"
+"Language: fr\n"
+
+#: fief/templates/auth_layout.html:49
+msgid "Powered by"
+msgstr "Propulsé et sécurisé par"
+
+#: fief/templates/login.html:3
+msgid "Login"
+msgstr "Connexion"
+
+#: fief/templates/login.html:5
+msgid "Welcome back!"
+msgstr "Ravi de vous revoir !"
+
+#: fief/templates/forgot_password.html:11 fief/templates/login.html:11
+#: fief/templates/register.html:11
+msgid "Email address"
+msgstr "Adresse e-mail"
+
+#: fief/templates/login.html:18 fief/templates/register.html:18
+msgid "Password"
+msgstr "Mot de passe"
+
+#: fief/templates/login.html:30
+msgid "Sign in"
+msgstr "Connexion"
 
-#: fief/errors.py:30
+#: fief/exceptions.py:20
 msgid "This field is required."
 msgstr "Ce champ est requis."
 
-#: fief/errors.py:31
+#: fief/exceptions.py:21
 msgid "This email address is invalid."
 msgstr "Cette adresse e-mail est invalide."
 
-#: fief/errors.py:47
-msgid "type"
-msgstr "type"
-
-#: fief/apps/auth/routers/auth.py:99
+#: fief/apps/auth/routers/auth.py:112
 msgid "Invalid email or password"
 msgstr "L'e-mail ou le mot de passe est invalide"
 
-#: fief/apps/auth/routers/auth.py:191
-msgid "The user denied access to their data."
-msgstr "L'utilisateur a refusé l'accès à ses données."
-
-#: fief/apps/auth/routers/register.py:51
+#: fief/apps/auth/routers/register.py:54
 msgid "A user with the same email address already exists."
 msgstr "Un utilisateur avec la même adresse e-mail existe déjà."
 
-#: fief/apps/auth/routers/reset.py:62
-msgid ""
-"Check your inbox! If an account associated with this email address exists"
-" in our system, you'll receive a link to reset your password."
-msgstr ""
-"Vérifiez votre boîte de réception! Si un compte associé à cette adresse "
-"e-mail existe dans notre système, vous allez recevoir un lien pour "
-"réinitialiser votre mot de passe."
-
-#: fief/apps/auth/routers/reset.py:84
-msgid "The reset password token is missing."
-msgstr "Le jeton de réinitialisation de mot de passe est manquant."
-
-#: fief/apps/auth/routers/reset.py:114
-msgid "The reset password token is invalid or expired."
-msgstr "Le jeton de réinitialisation de mot de passe est invalide ou a expiré."
+#: fief/dependencies/auth.py:100
+msgid "response_type is missing"
+msgstr "response_type manquant"
 
-#: fief/apps/auth/routers/reset.py:135
-msgid "Your password has been changed!"
-msgstr "Votre mot de passe a été modifié !"
+#: fief/dependencies/auth.py:108
+msgid "response_type should be \"code\""
+msgstr "response_type doit être \"code\""
 
-#: fief/dependencies/auth.py:40
+#: fief/dependencies/auth.py:41
 msgid "client_id is missing"
 msgstr "client_id manquant"
 
-#: fief/dependencies/auth.py:46
+#: fief/dependencies/auth.py:47
 msgid "Unknown client"
 msgstr "Client inconnu"
 
-#: fief/dependencies/auth.py:57
+#: fief/dependencies/auth.py:59
 msgid "redirect_uri is missing"
 msgstr "redirect_uri manquant"
 
-#: fief/dependencies/auth.py:75
-msgid "response_type is missing"
-msgstr "response_type manquant"
-
-#: fief/dependencies/auth.py:83
-msgid "response_type should be \"code\""
-msgstr "response_type doit être \"code\""
-
-#: fief/dependencies/auth.py:100
+#: fief/dependencies/auth.py:125
 msgid "scope is missing"
 msgstr "scope manquant"
 
-#: fief/dependencies/auth.py:110
+#: fief/dependencies/auth.py:135
 msgid "scope should contain \"openid\""
 msgstr "scope doit contenir \"openid\""
 
-#: fief/dependencies/auth.py:129
-msgid "prompt should either be \"none\", \"login\" or \"register\""
-msgstr "prompt doit être \"none\", \"login\" ou \"register\""
-
-#: fief/dependencies/auth.py:137
-msgid "User is not logged in"
-msgstr "L'utilisateur n'est pas connecté"
-
-#: fief/dependencies/auth.py:154
+#: fief/dependencies/auth.py:179
 msgid "screen should either be \"login\" or \"register\""
 msgstr "screen doit être \"login\" ou \"register\""
 
-#: fief/dependencies/auth.py:187
+#: fief/dependencies/auth.py:250
 msgid "Invalid login session"
 msgstr "Session invalide"
 
-#: fief/dependencies/auth.py:202
-msgid "action should either be \"allow\" or \"deny\""
-msgstr "action doit être \"allow\" ou \"deny\""
-
-#: fief/dependencies/auth.py:242
-msgid "User consent is required for this scope"
-msgstr "Le consentement de l'utilisateur est requis pour ce scope"
-
-#: fief/dependencies/users.py:57
+#: fief/dependencies/users.py:79
 msgid "The password should be at least 8 characters."
 msgstr "Le mot de passe doit avoir au moins 8 caractères."
 
-#: fief/emails/base.html:496
-#, python-format
-msgid "&copy; %(year)d %(tenant)s. All rights reserved."
-msgstr "&copy; %(year)d %(tenant)s. Tous droits réservés."
+#: fief/templates/authorize.html:3 fief/templates/authorize.html:5
+msgid "Authorize"
+msgstr "Autoriser"
 
-#: fief/emails/forgot_password.html:3
-#, fuzzy
-msgid "Use this link to reset your password. This link is only valid for 1 hour."
-msgstr "Cette réinitialisation n'est valide que pour une heure."
+#: fief/templates/register.html:3 fief/templates/register.html:5
+msgid "Register"
+msgstr "Inscription"
 
-#: fief/emails/forgot_password.html:6
-#, python-format
-msgid ""
-"You recently requested to reset your password for your %(tenant)s "
-"account. Use the button below to reset it."
-msgstr ""
-"Vous avez demandé à réinitialiser le mot de passe de votre compte "
-"%(tenant)s. Utilisez le bouton ci-dessous pour le réinitialiser."
+#: fief/templates/register.html:28
+msgid "I already have an account"
+msgstr "J'ai déjà un compte"
 
-#: fief/emails/forgot_password.html:6
-msgid "This password reset is only valid for the next hour."
-msgstr "Cette réinitialisation n'est valide que pour une heure."
+#: fief/templates/register.html:30
+msgid "Sign up"
+msgstr "S'inscrire"
 
-#: fief/emails/forgot_password.html:15
-msgid "Reset your password"
-msgstr "Réinitialiser votre mot de passe"
+#: fief/exceptions.py:37
+msgid "type"
+msgstr "type"
 
-#: fief/emails/welcome.html:3 fief/emails/welcome.html:6
-#, python-format
-msgid "Welcome to %(tenant)s! We're thrilled to have you on board."
-msgstr ""
+#: fief/apps/auth/routers/auth.py:211
+msgid "The user denied access to their data."
+msgstr "L'utilisateur a refusé l'accès à ses données."
 
-#: fief/tasks/forgot_password.py:19
-#, python-format
-msgid "Reset your %(tenant)s's password"
-msgstr "Réinitialiser votre mot de passe %(tenant)s"
+#: fief/dependencies/auth.py:154
+msgid "prompt should either be \"none\", \"login\" or \"register\""
+msgstr "prompt doit être \"none\", \"login\" ou \"register\""
 
-#: fief/tasks/register.py:19
-#, python-format
-msgid "Welcome to %(tenant)s!"
-msgstr "Bienvenue sur %(tenant)s !"
+#: fief/dependencies/auth.py:162
+msgid "User is not logged in"
+msgstr "L'utilisateur n'est pas connecté"
 
-#: fief/templates/auth_layout.html:50
-msgid "Powered by"
-msgstr "Propulsé et sécurisé par"
+#: fief/dependencies/auth.py:265
+msgid "action should either be \"allow\" or \"deny\""
+msgstr "action doit être \"allow\" ou \"deny\""
 
-#: fief/templates/authorize.html:3 fief/templates/authorize.html:5
-msgid "Authorize"
-msgstr "Autoriser"
+#: fief/dependencies/auth.py:310
+msgid "User consent is required for this scope"
+msgstr "Le consentement de l'utilisateur est requis pour ce scope"
 
 #: fief/templates/consent.html:3
 msgid "Consent"
 msgstr "Consentement"
 
 #: fief/templates/consent.html:5
-#, python-format
 msgid "%(name)s wants to access your account"
 msgstr "%(name)s veut accéder à votre compte"
 
 #: fief/templates/consent.html:10
-#, python-format
 msgid "This will allow %(name)s to:"
 msgstr "Cela permettra à %(name)s de :"
 
 #: fief/templates/consent.html:21
 msgid "Deny"
 msgstr "Refuser"
 
 #: fief/templates/consent.html:22
 msgid "Allow"
 msgstr "Autoriser"
 
+#: fief/apps/auth/routers/reset.py:62
+msgid "Check your inbox! If an account associated with this email address exists in our system, you'll receive a link to reset your password."
+msgstr "Vérifiez votre boîte de réception ! Si un compte associé à cette adresse e-mail existe dans notre système, vous allez recevoir un lien pour réinitialiser votre mot de passe."
+
+#: fief/apps/auth/routers/reset.py:84
+msgid "The reset password token is missing."
+msgstr "Le jeton de réinitialisation de mot de passe est manquant."
+
+#: fief/apps/auth/routers/reset.py:114
+msgid "The reset password token is invalid or expired."
+msgstr "Le jeton de réinitialisation de mot de passe est invalide ou a expiré."
+
+#: fief/apps/auth/routers/reset.py:135
+msgid "Your password has been changed!"
+msgstr "Votre mot de passe a été modifié !"
+
+#: fief/emails/base.html:496
+msgid "&copy; %(year)d %(tenant)s. All rights reserved."
+msgstr "&copy; %(year)d %(tenant)s. Tous droits réservés."
+
+#: fief/emails/forgot_password.html:6
+msgid "You recently requested to reset your password for your %(tenant)s account. Use the button below to reset it."
+msgstr "Vous avez demandé à réinitialiser le mot de passe de votre compte %(tenant)s. Utilisez le bouton ci-dessous pour le réinitialiser."
+
+#: fief/emails/forgot_password.html:6
+msgid "This password reset is only valid for the next hour."
+msgstr "Cette réinitialisation n'est valide que pour une heure."
+
+#: fief/emails/forgot_password.html:15
+msgid "Reset your password"
+msgstr "Réinitialiser votre mot de passe"
+
+#: fief/tasks/forgot_password.py:20
+msgid "Reset your %(tenant)s's password"
+msgstr "Réinitialiser votre mot de passe %(tenant)s"
+
+#: fief/tasks/register.py:20
+msgid "Welcome to %(tenant)s!"
+msgstr "Bienvenue sur %(tenant)s !"
+
 #: fief/templates/forgot_password.html:3 fief/templates/forgot_password.html:5
 msgid "Forgot password"
 msgstr "Mot de passe oublié"
 
-#: fief/templates/forgot_password.html:11 fief/templates/login.html:11
-#: fief/templates/register.html:11
-msgid "Email address"
-msgstr "Adresse e-mail"
-
 #: fief/templates/forgot_password.html:21
 msgid "I remember my password"
 msgstr "Je me souviens de mon mot de passe"
 
 #: fief/templates/forgot_password.html:23
 msgid "Send me a reset link"
 msgstr "Envoyer un lien de réinitialisation"
 
-#: fief/templates/login.html:3
-msgid "Login"
-msgstr "Connexion"
-
-#: fief/templates/login.html:5
-msgid "Welcome back!"
-msgstr "Ravi de vous revoir !"
-
-#: fief/templates/login.html:18 fief/templates/register.html:18
-msgid "Password"
-msgstr "Mot de passe"
-
 #: fief/templates/login.html:28
 msgid "I forgot my password"
 msgstr "J'ai oublié mon mot de passe"
 
-#: fief/templates/login.html:30
-msgid "Sign in"
-msgstr "Connexion"
-
-#: fief/templates/register.html:3 fief/templates/register.html:5
-msgid "Register"
-msgstr "Inscription"
-
-#: fief/templates/register.html:28
-msgid "I already have an account"
-msgstr "J'ai déjà un compte"
-
-#: fief/templates/register.html:30
-msgid "Sign up"
-msgstr "S'inscrire"
-
 #: fief/templates/reset_password.html:3 fief/templates/reset_password.html:5
 msgid "Reset password"
 msgstr "Réinitialisation du mot de passe"
 
 #: fief/templates/reset_password.html:11
 msgid "New password"
 msgstr "Nouveau mot de passe"
 
 #: fief/templates/reset_password.html:22
 msgid "Reset my password"
 msgstr "Réinitialiser mon mot de passe"
 
+#: fief/dependencies/auth.py:65
+msgid "redirect_uri is not authorized for this client"
+msgstr "Cette redirect_uri n'est pas autorisée pour ce client"
+
+#: fief/dependencies/auth.py:85
+msgid "request parameter is not supported"
+msgstr "Le paramètre request n'est pas supporté"
+
+#: fief/emails/forgot_password.html:3
+msgid "Use this link to reset your password. This link is only valid for 1 hour."
+msgstr "Utilisez ce lien pour réinitialiser votre mot de passe. Ce lien n'est valide qu'une heure."
+
+#: fief/emails/welcome.html:3 fief/emails/welcome.html:6
+msgid "Welcome to %(tenant)s! We're thrilled to have you on board."
+msgstr "Bienvenue sur %(tenant)s ! Nous sommes heureux de vous compter parmi nous."
+
+#: fief/dependencies/auth.py:201
+msgid "Unsupported code_challenge_method"
+msgstr "Méthode de code_challenge non supportée"
+
```

### Comparing `fief-server-0.8.2/fief/managers/__init__.py` & `fief-server-0.9.0/fief/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/admin_session_token.py` & `fief-server-0.9.0/fief/managers/admin_session_token.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/authorization_code.py` & `fief-server-0.9.0/fief/managers/authorization_code.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/base.py` & `fief-server-0.9.0/fief/managers/base.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/client.py` & `fief-server-0.9.0/fief/managers/client.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/grant.py` & `fief-server-0.9.0/fief/managers/grant.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/refresh_token.py` & `fief-server-0.9.0/fief/managers/refresh_token.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/session_token.py` & `fief-server-0.9.0/fief/managers/session_token.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/tenant.py` & `fief-server-0.9.0/fief/managers/tenant.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/workspace.py` & `fief-server-0.9.0/fief/managers/workspace.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/managers/workspace_user.py` & `fief-server-0.9.0/fief/managers/workspace_user.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/__init__.py` & `fief-server-0.9.0/fief/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/admin_api_key.py` & `fief-server-0.9.0/fief/models/admin_api_key.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/admin_session_token.py` & `fief-server-0.9.0/fief/models/admin_session_token.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/authorization_code.py` & `fief-server-0.9.0/fief/models/refresh_token.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import secrets
 from datetime import datetime
-from typing import List, Optional
+from typing import List
 
 from pydantic import UUID4
-from sqlalchemy import Column, ForeignKey
+from sqlalchemy import JSON, Column, ForeignKey, String
 from sqlalchemy.orm import relationship
-from sqlalchemy.sql.sqltypes import JSON, String
 
 from fief.models.base import WorkspaceBase
 from fief.models.client import Client
 from fief.models.generics import GUID, CreatedUpdatedAt, TIMESTAMPAware, UUIDModel
 from fief.models.user import User
 
 
-class AuthorizationCode(UUIDModel, CreatedUpdatedAt, WorkspaceBase):
-    __tablename__ = "authorization_codes"
+class RefreshToken(UUIDModel, CreatedUpdatedAt, WorkspaceBase):
+    __tablename__ = "refresh_tokens"
 
-    code: str = Column(
+    token: str = Column(
         String(length=255),
         default=secrets.token_urlsafe,
         nullable=False,
         index=True,
         unique=True,
     )
-    redirect_uri: str = Column(String(length=2048), nullable=False)
+    expires_at: datetime = Column(
+        TIMESTAMPAware(timezone=True), nullable=False, index=True
+    )
     scope: List[str] = Column(JSON, nullable=False, default=list)
     authenticated_at: datetime = Column(TIMESTAMPAware(timezone=True), nullable=False)
-    nonce: Optional[str] = Column(String(length=255), nullable=True)
 
     user_id: UUID4 = Column(GUID, ForeignKey(User.id, ondelete="CASCADE"), nullable=False)  # type: ignore
     user: User = relationship("User")
 
     client_id: UUID4 = Column(GUID, ForeignKey(Client.id, ondelete="CASCADE"), nullable=False)  # type: ignore
     client: Client = relationship("Client", lazy="joined")
```

### Comparing `fief-server-0.8.2/fief/models/base.py` & `fief-server-0.9.0/fief/models/base.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/client.py` & `fief-server-0.9.0/fief/models/client.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/generics.py` & `fief-server-0.9.0/fief/models/generics.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/grant.py` & `fief-server-0.9.0/fief/models/grant.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/login_session.py` & `fief-server-0.9.0/fief/models/authorization_code.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 import secrets
-from re import L
-from typing import List, Optional
+from datetime import datetime
+from typing import List, Optional, Tuple, cast
 
 from pydantic import UUID4
 from sqlalchemy import Column, ForeignKey
 from sqlalchemy.orm import relationship
 from sqlalchemy.sql.sqltypes import JSON, String
 
 from fief.models.base import WorkspaceBase
 from fief.models.client import Client
-from fief.models.generics import GUID, CreatedUpdatedAt, UUIDModel
+from fief.models.generics import GUID, CreatedUpdatedAt, TIMESTAMPAware, UUIDModel
+from fief.models.user import User
 
 
-class LoginSession(UUIDModel, CreatedUpdatedAt, WorkspaceBase):
-    __tablename__ = "login_sessions"
+class AuthorizationCode(UUIDModel, CreatedUpdatedAt, WorkspaceBase):
+    __tablename__ = "authorization_codes"
 
-    token: str = Column(
+    code: str = Column(
         String(length=255),
         default=secrets.token_urlsafe,
         nullable=False,
         index=True,
         unique=True,
     )
-    response_type: str = Column(String(length=255), nullable=False)
     redirect_uri: str = Column(String(length=2048), nullable=False)
     scope: List[str] = Column(JSON, nullable=False, default=list)
-    prompt: Optional[str] = Column(String(length=255), nullable=True)
-    state: Optional[str] = Column(String(length=2048), nullable=True)
+    authenticated_at: datetime = Column(TIMESTAMPAware(timezone=True), nullable=False)
     nonce: Optional[str] = Column(String(length=255), nullable=True)
+    code_challenge: Optional[str] = Column(String(length=255), nullable=True)
+    code_challenge_method: Optional[str] = Column(String(length=255), nullable=True)
+
+    user_id: UUID4 = Column(GUID, ForeignKey(User.id, ondelete="CASCADE"), nullable=False)  # type: ignore
+    user: User = relationship("User")
 
     client_id: UUID4 = Column(GUID, ForeignKey(Client.id, ondelete="CASCADE"), nullable=False)  # type: ignore
     client: Client = relationship("Client", lazy="joined")
+
+    def get_code_challenge_tuple(self) -> Optional[Tuple[str, str]]:
+        if self.code_challenge is not None:
+            return (self.code_challenge, cast(str, self.code_challenge_method))
+        return None
```

### Comparing `fief-server-0.8.2/fief/models/refresh_token.py` & `fief-server-0.9.0/fief/models/session_token.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 import secrets
 from datetime import datetime
-from typing import List
 
 from pydantic import UUID4
-from sqlalchemy import JSON, Column, ForeignKey, String
+from sqlalchemy import Column, ForeignKey, String
 from sqlalchemy.orm import relationship
 
 from fief.models.base import WorkspaceBase
-from fief.models.client import Client
 from fief.models.generics import GUID, CreatedUpdatedAt, TIMESTAMPAware, UUIDModel
 from fief.models.user import User
 
 
-class RefreshToken(UUIDModel, CreatedUpdatedAt, WorkspaceBase):
-    __tablename__ = "refresh_tokens"
+class SessionToken(UUIDModel, CreatedUpdatedAt, WorkspaceBase):
+    __tablename__ = "session_tokens"
 
     token: str = Column(
         String(length=255),
         default=secrets.token_urlsafe,
         nullable=False,
         index=True,
         unique=True,
     )
     expires_at: datetime = Column(
         TIMESTAMPAware(timezone=True), nullable=False, index=True
     )
-    scope: List[str] = Column(JSON, nullable=False, default=list)
-    authenticated_at: datetime = Column(TIMESTAMPAware(timezone=True), nullable=False)
 
     user_id: UUID4 = Column(GUID, ForeignKey(User.id, ondelete="CASCADE"), nullable=False)  # type: ignore
     user: User = relationship("User")
-
-    client_id: UUID4 = Column(GUID, ForeignKey(Client.id, ondelete="CASCADE"), nullable=False)  # type: ignore
-    client: Client = relationship("Client", lazy="joined")
```

### Comparing `fief-server-0.8.2/fief/models/tenant.py` & `fief-server-0.9.0/fief/models/tenant.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/user.py` & `fief-server-0.9.0/fief/models/user.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/workspace.py` & `fief-server-0.9.0/fief/models/workspace.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/models/workspace_user.py` & `fief-server-0.9.0/fief/models/workspace_user.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/schemas/auth.py` & `fief-server-0.9.0/fief/schemas/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     def get_login_required(cls, error_description: Optional[str] = None):
         return cls(error="login_required", error_description=error_description)
 
     @classmethod
     def get_consent_required(cls, error_description: Optional[str] = None):
         return cls(error="consent_required", error_description=error_description)
 
+    @classmethod
+    def get_request_not_supported(cls, error_description: Optional[str] = None):
+        return cls(error="request_not_supported", error_description=error_description)
+
 
 class LoginError(BaseModel):
     error: str = Field(..., regex="invalid_session|bad_credentials")
     error_description: Optional[str] = None
     error_uri: Optional[str] = None
 
     @classmethod
```

### Comparing `fief-server-0.8.2/fief/schemas/client.py` & `fief-server-0.9.0/fief/schemas/client.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/schemas/register.py` & `fief-server-0.9.0/fief/schemas/register.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/schemas/reset.py` & `fief-server-0.9.0/fief/schemas/reset.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/schemas/user.py` & `fief-server-0.9.0/fief/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/schemas/workspace.py` & `fief-server-0.9.0/fief/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/services/authentication_flow.py` & `fief-server-0.9.0/fief/services/authentication_flow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timedelta, timezone
-from typing import List, Optional, TypeVar
+from typing import List, Optional, Tuple, TypeVar
 
 from fastapi import Response, status
 from fastapi.responses import RedirectResponse
 from furl import furl
 from pydantic import UUID4
 
 from fief.managers import (
@@ -36,24 +36,30 @@
         response: ResponseType,
         *,
         response_type: str,
         redirect_uri: str,
         scope: List[str],
         state: Optional[str],
         nonce: Optional[str],
+        code_challenge_tuple: Optional[Tuple[str, str]],
         client: Client,
     ) -> ResponseType:
         login_session = LoginSession(
             response_type=response_type,
             redirect_uri=redirect_uri,
             scope=scope,
             state=state,
             nonce=nonce,
             client_id=client.id,
         )
+        if code_challenge_tuple is not None:
+            code_challenge, code_challenge_method = code_challenge_tuple
+            login_session.code_challenge = code_challenge
+            login_session.code_challenge_method = code_challenge_method
+
         login_session = await self.login_session_manager.create(login_session)
 
         response.set_cookie(
             settings.login_session_cookie_name,
             login_session.token,
             domain=settings.login_session_cookie_domain,
             secure=settings.login_session_cookie_secure,
@@ -118,27 +124,32 @@
     async def get_authorization_code_success_redirect(
         self,
         redirect_uri: str,
         scope: List[str],
         authenticated_at: datetime,
         state: Optional[str],
         nonce: Optional[str],
+        code_challenge_tuple: Optional[Tuple[str, str]],
         client: Client,
         user_id: UUID4,
     ) -> RedirectResponse:
         authorization_code = await self.authorization_code_manager.create(
             AuthorizationCode(
                 redirect_uri=redirect_uri,
                 scope=scope,
                 authenticated_at=authenticated_at,
                 nonce=nonce,
                 user_id=user_id,
                 client_id=client.id,
             )
         )
+        if code_challenge_tuple is not None:
+            code_challenge, code_challenge_method = code_challenge_tuple
+            authorization_code.code_challenge = code_challenge
+            authorization_code.code_challenge_method = code_challenge_method
 
         parsed_redirect_uri = furl(redirect_uri)
         parsed_redirect_uri.add(query_params={"code": authorization_code.code})
         if state is not None:
             parsed_redirect_uri.add(query_params={"state": state})
 
         return RedirectResponse(
```

### Comparing `fief-server-0.8.2/fief/services/email/__init__.py` & `fief-server-0.9.0/fief/services/email/__init__.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/services/email/postmark.py` & `fief-server-0.9.0/fief/services/email/postmark.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/services/main_workspace.py` & `fief-server-0.9.0/fief/services/main_workspace.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/services/workspace_creation.py` & `fief-server-0.9.0/fief/services/workspace_creation.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/services/workspace_db.py` & `fief-server-0.9.0/fief/services/workspace_db.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/settings.py` & `fief-server-0.9.0/fief/settings.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/favicon.svg` & `fief-server-0.9.0/fief/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/fief-logo.svg` & `fief-server-0.9.0/fief/static/fief-logo.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/asset-manifest.json` & `fief-server-0.9.0/fief/static/frontend/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/favicon.svg` & `fief-server-0.9.0/fief/static/frontend/favicon.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/index.html` & `fief-server-0.9.0/fief/static/frontend/index.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/locales/en/api-keys.json` & `fief-server-0.9.0/fief/static/frontend/locales/en/api-keys.json`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/locales/en/clients.json` & `fief-server-0.9.0/fief/static/frontend/locales/en/clients.json`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/locales/en/common.json` & `fief-server-0.9.0/fief/static/frontend/locales/en/common.json`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/locales/en/workspaces.json` & `fief-server-0.9.0/fief/static/frontend/locales/en/workspaces.json`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/logo192.png` & `fief-server-0.9.0/fief/static/frontend/logo192.png`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/logo512.png` & `fief-server-0.9.0/fief/static/frontend/logo512.png`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/css/main.45cf7c31.css` & `fief-server-0.9.0/fief/static/frontend/static/css/main.45cf7c31.css`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/css/main.45cf7c31.css.map` & `fief-server-0.9.0/fief/static/frontend/static/css/main.45cf7c31.css.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.979591836734694%*

 * *Differences: {"'sources'": "{insert: [(1, '%3Cinput%20css%20vApJ0T%3E')], delete: [1]}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "file": "static/css/main.45cf7c31.css",
     "mappings": ";AAEA;;CAAA,kBCSE,sBAAwD,CAHxD,qBDNF,gBCcE,eDdF,MC0BE,6BAA8B,CAG9B,gMAAsP,CAJtP,eAAgB,CAGhB,UD5BF,MCuCE,mBAAoB,CADpB,QDtCF,ICmDE,oBAAqB,CADrB,aAAc,CADd,QDjDF,qBC2DE,wCAAiC,CAAjC,gCD3DF,mBCwEE,iBAAkB,CAClB,mBDzEF,GCiFE,aAAc,CACd,uBDlFF,UC2FE,kBD3FF,mBCuGE,mGAAyI,CACzI,aDxGF,OCgHE,aDhHF,SCyHE,aAAc,CACd,aAAc,CACd,iBAAkB,CAClB,uBD5HF,KCgIE,aDhIF,KCoIE,SDpIF,OCgJE,wBAAyB,CADzB,oBAAqB,CADrB,aD9IF,uCCiKE,aAAc,CAHd,mBAAoB,CACpB,cAAe,CACf,mBAAoB,CAEpB,QAAS,CACT,SDnKF,eC4KE,mBD5KF,iDCwLE,yBAA0B,CAC1B,4BAA6B,CAC7B,qBD1LF,iBCkME,YDlMF,kBC0ME,eD1MF,UCkNE,uBDlNF,yDC2NE,WD3NF,eCoOE,4BAA6B,CAC7B,mBDrOF,6BC6OE,uBD7OF,8BCsPE,yBAA0B,CAC1B,YDvPF,SC+PE,iBD/PF,oDCmRE,QDnRF,UCuRE,QDvRF,iBCwRE,SDxRF,YCkSE,eAAgB,CAChB,QAAS,CACT,SDpSF,UC4SE,eD5SF,sECuTE,aDvTF,4DCuTE,aDvTF,0CCuTE,aDvTF,sBCgUE,cDhUF,WCuUE,cDvUF,gDCwVE,aAAc,CACd,qBDzVF,WCmWE,WAAY,CADZ,cDlWF,UC2WE,YD3WF,8LEFA,gMFEA,wREFA,meFEA,sEEFA,uBFEA,4DEFA,uBFEA,0CEFA,uBFEA,wCEFA,SFEA,+BEFA,gBFEA,gUEFA,8BFEA,QEFA,waFEA,YEFA,gMFEA,8BEFA,iXFEA,iBEFA,eFEA,cEFA,kBFEA,0CEFA,8cFEA,8CEFA,oIFEA,yBEFA,2RFEA,sBEFA,kLFEA,mHEFA,sDFEA,+BEFA,0XFEA,yEEFA,sDFEA,aEFA,kHFEA,mBEFA,yCFEA,CEFA,i4B,CAAA,qOFGA,mFEHA,meFGA,kFEHA,uBFGA,wEEHA,uBFGA,sDEHA,uBFGA,mDEHA,SFGA,0CEHA,gBFGA,maEHA,8BFGA,cEHA,+VFGA,yCEHA,mDFGA,4BEHA,4SFGA,gBEHA,eFGA,wCEHA,8cFGA,4CEHA,oIFGA,wBEHA,2RFGA,+GEHA,sDFGA,8BEHA,0XFGA,uEEHA,sDFGA,CEHA,4E,CAAA,yB,CAAA,0D,CAAA,yB,CAAA,4E,CAAA,2C,CAAA,8C,CAAA,qB,CAAA,kkC,CAAA,yB,CAAA,2B,CAAA,4B,CAAA,6B,CAAA,uMCwDE,wBDxDF,kR,CAAA,6F,CAAA,ia,CAAA,8J,CAAA,4I,CAAA,gK,CAAA,sJ,CAAA,oI,CAAA,iC,CAAA,qK,CAAA,iCCmGE,aAGF,cACE,wBACA,qBCrGF,kBAOI,kBANA,wCACA,gBACA,kBACA,WAEA,mBADA,eAEA,CAEA,wCACI,gBACA,wBACA,sBACA,8LAWA,wBACA,uDACA,2BACA,gDAGA,qBACA,+LAYA,wBAEA,4BAGJ,YACI,kBFpDR,miB,CAAA,kG,CAAA,uEGWY,YAEA,SHbZ,kBGcY,UAFA,QAGA,6BHfZ,U,CAAA,kH,CAAA,iEG2BoB,UH3BpB,0O,CAAA,0I,CAAA,ue,CAAA,0IFWA,sBEXA,mBFWA,SEXA,eFWA,QEXA,cFWA,WEXA,iBFWA,WEXA,iBFWA,SEXA,uCFWA,UEXA,cFWA,qBEXA,cFWA,UEXA,OFWA,QEXA,KFWA,SEXA,MFWA,WEXA,OFWA,OEXA,UFWA,OEXA,UFWA,aEXA,yBFWA,aEXA,yBFWA,OEXA,oCFWA,OEXA,sCFWA,UEXA,kCFWA,OEXA,oBFWA,OEXA,iBFWA,OEXA,iBFWA,OEXA,oBFWA,OEXA,mBFWA,OEXA,kBFWA,OEXA,iBFWA,OEXA,oBFWA,OEXA,eFWA,aEXA,cFWA,OEXA,mBFWA,SEXA,kBFWA,OEXA,kBFWA,SEXA,eFWA,OEXA,kBFWA,OEXA,mBFWA,OEXA,kBFWA,QEXA,oBFWA,UEXA,qBFWA,OEXA,eFWA,OEXA,gBFWA,OEXA,kBFWA,UEXA,gBFWA,QEXA,aFWA,eEXA,oBFWA,OEXA,YFWA,cEXA,mBFWA,QEXA,aFWA,OEXA,YFWA,WEXA,gBFWA,SEXA,YFWA,MEXA,WFWA,OEXA,WFWA,MEXA,aFWA,WEXA,YFWA,SEXA,WFWA,SEXA,cFWA,MEXA,QFWA,MEXA,WFWA,OEXA,aFWA,eEXA,gBFWA,SEXA,UFWA,MEXA,UFWA,MEXA,YFWA,OEXA,SFWA,aEXA,UFWA,OEXA,WFWA,MEXA,UFWA,OEXA,WFWA,OEXA,YFWA,YEXA,eFWA,WEXA,eFWA,WEXA,eFWA,SEXA,QFWA,WEXA,aFWA,aEXA,iBFWA,mBEXA,6DFWA,gBEXA,oBFWA,iCEXA,mYFWA,kBEXA,uBFWA,WEXA,iCFWA,sBEXA,mYFWA,YEXA,6BFWA,YEXA,mYFWA,yBEXA,0D,CFWA,iBEXA,0D,CFWA,eEXA,2EFWA,qBEXA,kBFWA,iBEXA,cFWA,gBEXA,qBFWA,cEXA,6CFWA,WEXA,qBFWA,YEXA,cFWA,cEXA,sBFWA,eEXA,kBFWA,gBEXA,0BFWA,cEXA,wBFWA,iBEXA,sBFWA,kBEXA,6BFWA,QEXA,SFWA,QEXA,QFWA,0CEXA,+HFWA,0CEXA,mIFWA,0CEXA,iIFWA,0CEXA,+HFWA,0CEXA,mIFWA,yCEXA,4IFWA,iDEXA,4EFWA,gDEXA,4EFWA,kBEXA,eFWA,kBEXA,eFWA,kBEXA,eFWA,kBEXA,eFWA,oBEXA,iBFWA,oBEXA,iBFWA,WEXA,sCFWA,8BEXA,kBFWA,UEXA,oBFWA,aEXA,qBFWA,eEXA,oBFWA,SEXA,gBFWA,WEXA,gBFWA,WEXA,uBFWA,WEXA,oBFWA,mBEXA,4EFWA,mBEXA,4EFWA,iBEXA,4EFWA,oBEXA,4EFWA,qBEXA,wBFWA,eEXA,wEFWA,iBEXA,kEFWA,WEXA,wEFWA,cEXA,wEFWA,aEXA,sEFWA,aEXA,wEFWA,eEXA,wEFWA,eEXA,qEFWA,aEXA,kEFWA,eEXA,qEFWA,gBEXA,wEFWA,eEXA,wEFWA,gBEXA,mBFWA,eEXA,iBFWA,iBEXA,YFWA,MEXA,cFWA,MEXA,aFWA,MEXA,eFWA,MEXA,YFWA,OEXA,wCFWA,OEXA,wCFWA,OEXA,wCFWA,OEXA,0CFWA,OEXA,oCFWA,OEXA,sCFWA,OEXA,oCFWA,OEXA,sCFWA,OEXA,oCFWA,OEXA,wCFWA,UEXA,0CFWA,UEXA,0CFWA,OEXA,8BFWA,OEXA,wCFWA,OEXA,mBFWA,OEXA,mBFWA,QEXA,gBFWA,OEXA,mBFWA,OEXA,oBFWA,YEXA,eFWA,cEXA,iBFWA,eEXA,kBFWA,eEXA,qBFWA,aEXA,4BFWA,UEXA,oCFWA,UEXA,gCFWA,WEXA,gBFWA,qBEXA,sCFWA,WEXA,iBFWA,gBEXA,eFWA,cEXA,eFWA,YEXA,eFWA,YEXA,wBFWA,iBEXA,+DFWA,aEXA,iEFWA,iBEXA,8DFWA,mBEXA,4CFWA,iBEXA,iEFWA,iBEXA,iEFWA,eEXA,+DFWA,eEXA,+DFWA,iBEXA,iEFWA,iBEXA,iEFWA,kBEXA,+DFWA,iBEXA,+DFWA,eEXA,4CFWA,YEXA,qEFWA,cEXA,oEFWA,aEXA,UFWA,aEXA,WFWA,aEXA,WFWA,YEXA,SFWA,cEXA,SFWA,YEXA,6KFWA,uBEXA,kJFWA,YEXA,8FFWA,SEXA,oXFWA,aEXA,qEFWA,iBEXA,sBFWA,iBEXA,mGFWA,qBEXA,uGFWA,aEXA,4mBFWA,eEXA,uBFWA,eEXA,uBFWA,eEXA,wBFWA,eEXA,uBFWA,cEXA,wBFWA,WEXA,iDFWA,UEXA,iDFWA,cEXA,kDFWA,CAGA,aACI,aAGJ,qCACI,2BAGJ,MACE,0BAA2B,CAC3B,2BAA4B,CAC5B,2BAA4B,CAC5B,2BAA4B,CAC5B,2BAA4B,CAC5B,2BAA4B,CAC5B,2BAA4B,CAC5B,2BAA4B,CAC5B,2BAA4B,CAC5B,2BAA4B,CAhCtB,qBEAR,kC,CAAA,sC,CAAA,6C,CAAA,sC,CAAA,4C,CAAA,2G,CAAA,+F,CAAA,+F,CAAA,4F,CAAA,8F,CAAA,8F,CAAA,0F,CAAA,8F,CAAA,2F,CAAA,sF,CAAA,2E,CAAA,yD,CAAA,iH,CAAA,yG,CAAA,oG,CAAA,wG,CAAA,0G,CAAA,6C,CAAA,yB,CAAA,sB,CAAA,sF,CAAA,gC,CAAA,oC,CAAA,yC,CAAA,kD,CAAA,0K,CAAA,4K,CAAA,kD,CAAA,gD,CAAA,8B,EAAA,8C,CAAA,sE,EAAA,qD,CAAA,+B,CAAA,mD,CAAA,oB,CAAA,wB,CAAA,sB,CAAA,wB,CAAA,sB,CAAA,wB,CAAA,uD,CAAA,4B,CAAA,oB,CAAA,8B,CAAA,2B,CAAA,2a,CAAA,0C,CAAA,oC,CAAA,wC,CAAA,kC,CAAA,mC,CAAA,8C,CAAA,wB,CAAA,qE,CAAA,8D,EAAA,8D,CAAA,6B,EAAA,iD",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../../styles/globals.scss",
-        "%3Cinput%20css%20eAzREk%3E",
+        "%3Cinput%20css%20vApJ0T%3E",
         "../<no source>",
         "../../styles/additional-styles/utility-patterns.scss",
         "../../styles/additional-styles/range-slider.scss",
         "../../styles/additional-styles/toggle-switch.scss"
     ],
     "sourcesContent": [
         "@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=fallback');\n\n@tailwind base;\n@tailwind components;\n\n// Additional styles\n@import 'additional-styles/utility-patterns.scss';\n@import 'additional-styles/range-slider.scss';\n@import 'additional-styles/toggle-switch.scss';\n@import 'additional-styles/theme.scss';\n\n@tailwind utilities;\n\n// See Alpine.js: https://github.com/alpinejs/alpine#x-cloak\n[x-cloak=\"\"] {\n    display: none;\n}\n\n@media screen and (max-width: theme('screens.lg')) {\n    [x-cloak=\"lg\"] { display: none; }\n}\n\n:root {\n  --color-primary-50: #fff1f2;\n  --color-primary-100: #ffe4e6;\n  --color-primary-200: #fecdd3;\n  --color-primary-300: #fda4af;\n  --color-primary-400: #fb7185;\n  --color-primary-500: #f43f5e;\n  --color-primary-600: #e11d48;\n  --color-primary-700: #be123c;\n  --color-primary-800: #9f1239;\n  --color-primary-900: #881337;\n}\n",
```

### Comparing `fief-server-0.8.2/fief/static/frontend/static/js/787.707d1bd1.chunk.js` & `fief-server-0.9.0/fief/static/frontend/static/js/787.707d1bd1.chunk.js`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/js/787.707d1bd1.chunk.js.map` & `fief-server-0.9.0/fief/static/frontend/static/js/787.707d1bd1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/js/main.3b0373f0.js` & `fief-server-0.9.0/fief/static/frontend/static/js/main.3b0373f0.js`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/js/main.3b0373f0.js.LICENSE.txt` & `fief-server-0.9.0/fief/static/frontend/static/js/main.3b0373f0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/js/main.3b0373f0.js.map` & `fief-server-0.9.0/fief/static/frontend/static/js/main.3b0373f0.js.map`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/media/clients.9b0e9946f3619c28cab1767cc62a22aa.svg` & `fief-server-0.9.0/fief/static/frontend/static/media/clients.9b0e9946f3619c28cab1767cc62a22aa.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/media/cogwheel.bbc48a85c6dc5c6dd1eeb294e3afa715.svg` & `fief-server-0.9.0/fief/static/frontend/static/media/cogwheel.bbc48a85c6dc5c6dd1eeb294e3afa715.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/media/dashboard.580511ccd86590b36f5819c267461ebe.svg` & `fief-server-0.9.0/fief/static/frontend/static/media/dashboard.580511ccd86590b36f5819c267461ebe.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/media/fief-logo-red.ee09b120c56412b835b2cb57d6adaa58.svg` & `fief-server-0.9.0/fief/static/frontend/static/media/fief-logo-red.ee09b120c56412b835b2cb57d6adaa58.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/media/key.69ef1cd7ed8906a8b62c0bb9cb74c731.svg` & `fief-server-0.9.0/fief/static/frontend/static/media/key.69ef1cd7ed8906a8b62c0bb9cb74c731.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/frontend/static/media/tenants.3a942265546a3a2ebbf16aa58f45311f.svg` & `fief-server-0.9.0/fief/static/frontend/static/media/tenants.3a942265546a3a2ebbf16aa58f45311f.svg`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/static/output.css` & `fief-server-0.9.0/fief/static/output.css`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/tasks/base.py` & `fief-server-0.9.0/fief/tasks/base.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/tasks/forgot_password.py` & `fief-server-0.9.0/fief/tasks/forgot_password.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/tasks/register.py` & `fief-server-0.9.0/fief/tasks/register.py`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/templates/auth_layout.html` & `fief-server-0.9.0/fief/templates/auth_layout.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/templates/base.html` & `fief-server-0.9.0/fief/templates/base.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/templates/consent.html` & `fief-server-0.9.0/fief/templates/consent.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/templates/forgot_password.html` & `fief-server-0.9.0/fief/templates/forgot_password.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/templates/login.html` & `fief-server-0.9.0/fief/templates/login.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/templates/register.html` & `fief-server-0.9.0/fief/templates/register.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/fief/templates/reset_password.html` & `fief-server-0.9.0/fief/templates/reset_password.html`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/justfile` & `fief-server-0.9.0/justfile`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/package-lock.json` & `fief-server-0.9.0/package-lock.json`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/pyproject.toml` & `fief-server-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/tailwind.config.js` & `fief-server-0.9.0/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `fief-server-0.8.2/PKG-INFO` & `fief-server-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fief-server
-Version: 0.8.2
+Version: 0.9.0
 Summary: Users and authentication management SaaS
 Author-email: François Voron <contact@fief.dev>
 Requires-Python: >=3.10
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: aiomysql ==0.0.22
```

