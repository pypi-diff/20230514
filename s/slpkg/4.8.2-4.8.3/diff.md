# Comparing `tmp/slpkg-4.8.2.tar.gz` & `tmp/slpkg-4.8.3.tar.gz`

## Comparing `slpkg-4.8.2.tar` & `slpkg-4.8.3.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:51:40.000000 slpkg-4.8.2/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-04-28 14:28:20.000000 slpkg-4.8.2/filelists/README
--rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-04-28 14:28:20.000000 slpkg-4.8.2/repositories.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4195 2023-04-28 14:28:20.000000 slpkg-4.8.2/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-04-28 14:28:20.000000 slpkg-4.8.2/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-04-28 14:28:20.000000 slpkg-4.8.2/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8545 2023-04-28 14:28:20.000000 slpkg-4.8.2/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-04-28 14:28:20.000000 slpkg-4.8.2/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     3813 2023-04-28 14:28:20.000000 slpkg-4.8.2/configs/slpkg.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      770 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1891 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1455 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      890 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/check_updates_test.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1567 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1787 2023-04-28 14:28:20.000000 slpkg-4.8.2/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-04-28 14:28:20.000000 slpkg-4.8.2/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-04-28 14:28:20.000000 slpkg-4.8.2/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    45800 2023-04-28 14:28:20.000000 slpkg-4.8.2/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     9291 2023-04-28 14:28:20.000000 slpkg-4.8.2/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-04-28 14:28:20.000000 slpkg-4.8.2/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-04-28 14:28:20.000000 slpkg-4.8.2/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-04-28 14:28:20.000000 slpkg-4.8.2/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     4126 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1623 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2110 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     8326 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    63301 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    26741 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2016 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1368 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    13735 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)      974 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    30343 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1524 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2518 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2630 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/models/models.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6208 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5053 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/ascii.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3810 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    10363 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/error_messages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3595 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1443 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/logging_deps.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11552 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/new_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3277 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/cleanings.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1916 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2584 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4460 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6888 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3592 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/toml_error_message.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5595 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5458 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      939 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2593 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2818 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      456 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    30502 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1117 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3371 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2605 2023-04-28 14:28:20.000000 slpkg-4.8.2/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1471 2023-04-28 14:28:20.000000 slpkg-4.8.2/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/entry_points.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1233 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-04-28 14:51:34.000000 slpkg-4.8.2/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8684 2023-04-28 14:28:20.000000 slpkg-4.8.2/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-04-28 14:28:20.000000 slpkg-4.8.2/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-04-28 14:28:20.000000 slpkg-4.8.2/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:21:35.000000 slpkg-4.8.3/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-05-14 17:18:17.000000 slpkg-4.8.3/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-05-14 17:18:17.000000 slpkg-4.8.3/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4195 2023-05-14 17:18:17.000000 slpkg-4.8.3/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-05-14 17:18:17.000000 slpkg-4.8.3/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-05-14 17:18:17.000000 slpkg-4.8.3/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8822 2023-05-14 17:18:17.000000 slpkg-4.8.3/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-05-14 17:18:17.000000 slpkg-4.8.3/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     3813 2023-05-14 17:18:17.000000 slpkg-4.8.3/configs/slpkg.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      753 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      255 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-05-14 17:18:17.000000 slpkg-4.8.3/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-05-14 17:18:17.000000 slpkg-4.8.3/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-05-14 17:18:17.000000 slpkg-4.8.3/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    46097 2023-05-14 17:18:17.000000 slpkg-4.8.3/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9164 2023-05-14 17:18:17.000000 slpkg-4.8.3/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)     9919 2023-05-14 17:18:17.000000 slpkg-4.8.3/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-05-14 17:18:17.000000 slpkg-4.8.3/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-05-14 17:18:17.000000 slpkg-4.8.3/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4208 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1901 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7477 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    65522 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4370 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11741 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1160 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    34064 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2066 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3156 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/models/models.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     5945 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6212 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4898 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/asciibox.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3801 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     9651 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3649 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1334 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/logging_deps.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11666 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/new_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1819 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/multi_process.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3256 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/cleanings.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2196 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4460 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7274 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3715 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6020 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6025 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      939 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3339 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3965 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    29842 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3609 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2731 2023-05-14 17:18:17.000000 slpkg-4.8.3/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1471 2023-05-14 17:18:17.000000 slpkg-4.8.3/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/entry_points.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1286 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1262 2023-05-14 17:21:31.000000 slpkg-4.8.3/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     8493 2023-05-14 17:18:17.000000 slpkg-4.8.3/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-14 17:18:17.000000 slpkg-4.8.3/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-05-14 17:18:17.000000 slpkg-4.8.3/tools/gen_sbo_txt.sh
```

### Comparing `slpkg-4.8.2/filelists/multilib/README.ERIC` & `slpkg-4.8.3/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/filelists/multilib/README` & `slpkg-4.8.3/filelists/multilib/README`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/filelists/multilib/compat32.pkgs` & `slpkg-4.8.3/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/repositories.txt` & `slpkg-4.8.3/repositories.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/slackbuild/slack-desc` & `slpkg-4.8.3/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/slackbuild/slpkg.SlackBuild` & `slpkg-4.8.3/slackbuild/slpkg.SlackBuild`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/configs/repositories.toml` & `slpkg-4.8.3/configs/repositories.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,214 +1,232 @@
 # This is the general repositories configuration file of slpkg:
 # /etc/slpkg/repositories.toml
 # Date: 26/04/2023, Version: 4.8.2
 
-# The philosophy behind this is to have two repositories for
-# Slackbuilds one for the Slackware stable and one for the -current
-# and many binaries for all versions.
-# Set 'true' to 'PONCE_REPO' to switch with the ponce repository.
-# Set 'true' to the binary repositories you want to enable.
-# Default is the 'sbo' Slackbuilds.org repository.
+# Set 'true' to the variable {NAME}_REPO to enable a repository.
 
-# If you are going to use a local repository, set the mirror:
-# Example: ["file:///path/to/alien/repository/" ,"15.0/", "x86_64/"]
+# If you are going to use a local repository, set the repository:
+# as the example bellow:
+# ALIEN_REPO_LOCAL = ["file:///path/to/alien/repository/" ,"15.0/", "x86_64/"]
 # A binary local repository will must contain the files:
-# ChangeLog.txt, PACKAGES.TXT and CHECKSUMS.md5
+#   ChangeLog.txt, PACKAGES.TXT and CHECKSUMS.md5
 # A SlackBuilds repository will must contain the files:
-# SLACKBUILDS.TXT and ChangeLog.txt
-
-# After the mirror changed, you should update the database:
-# slpkg update or apply the option --bin-repo=<repo_name> for
-# binary repositories.
+#   SLACKBUILDS.TXT and ChangeLog.txt
+# After the mirror changed, you should update the database, run:
+# slpkg update
 
 # DO NOT CHANGE THE PATTERN OF THE MIRRORS, CHANGE ONLY WHAT YOU WANT.
-# Example: ["https://slackware.nl/people/alien/sbrepos/", "15.0/", "x86_64/"]
-# For Slackware -current users should be:
-# ["https://slackware.nl/people/alien/sbrepos/", "current/", "x86_64/"]
-# and NOT: ["https://slackware.nl/people/alien/sbrepos/current/x86_64/"]
+# For alien and Slackware -current users should be:
+#  ["https://slackware.nl/people/alien/sbrepos/", "current/", "x86_64/"]
+# and NOT:
+#  ["https://slackware.nl/people/alien/sbrepos/current/x86_64/"]
 
 # Note: Before using a repository, make sure you have read about it.
 #       Some repositories are for -current only. Change the mirror
 #       if it is necessary. The mirror or every part of the mirror
 #       should end with a slash '/'.
 
 [REPOSITORIES]
 
+# This is the DEFAULT REPOSITORY.
+# You can change it with one that you see below.
+# Make sure you have enabled it before.
+DEFAULT_REPOSITORY = "sbo"
+
 # SBo Repository for Slackware 15.0 stable.
+SBO_REPO = true
 SBO_REPO_NAME = "sbo"
+SBO_REPO_LOCAL = [""]
 SBO_REPO_MIRROR = ["https://slackbuilds.org/slackbuilds/15.0/"]
 SBO_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
 SBO_REPO_CHANGELOG = "ChangeLog.txt"
-SBO_REPO_TAR_SUFFIX = ".tar.gz"
 SBO_REPO_TAG = "_SBo"  # Default repo TAG.
 SBO_REPO_PATCH_TAG = ""  # Patch the TAG.
+SBO_REPO_TAR_SUFFIX = ".tar.gz"
 
 # Ponce Repository for Slackware -current.
 PONCE_REPO = false
 PONCE_REPO_NAME = "ponce"
+PONCE_REPO_LOCAL = [""]
 PONCE_REPO_MIRROR = ["https://cgit.ponce.cc/slackbuilds/plain/"]
 PONCE_REPO_SLACKBUILDS = "SLACKBUILDS.TXT"
 PONCE_REPO_CHANGELOG = "ChangeLog.txt"
 PONCE_REPO_TAG = "_SBo"  # Default repo TAG.
 PONCE_REPO_PATCH_TAG = ""  # Patch the TAG.
 
 # Official repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["https://slackware.uk/slackware/slackware64-current/"]
 SLACK_REPO = false
 SLACK_REPO_NAME = "slack"
+SLACK_REPO_LOCAL = [""]
 SLACK_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/"]
 SLACK_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_REPO_CHANGELOG = "ChangeLog.txt"
 SLACK_REPO_TAG = ""
 
 # Official repository for Slackware patches x86_64 15.0 stable.
 # For Slackware patches x86_64 -current:
 # ["https://slackware.uk/slackware/slackware64-current/", "extra/"]
 SLACK_EXTRA_REPO = false
 SLACK_EXTRA_REPO_NAME = "slack_extra"
+SLACK_EXTRA_REPO_LOCAL = [""]
 SLACK_EXTRA_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/", "extra/"]
 SLACK_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
 SLACK_EXTRA_REPO_TAG = ""
 
 # Official repository for Slackware patches x86_64 15.0 stable.
 SLACK_PATCHES_REPO = false
 SLACK_PATCHES_REPO_NAME = "slack_patches"
+SLACK_PATCHES_REPO_LOCAL = [""]
 SLACK_PATCHES_REPO_MIRROR = ["https://slackware.uk/slackware/slackware64-15.0/", "patches/"]
 SLACK_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
 SLACK_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACK_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
 SLACK_PATCHES_REPO_TAG = "_slack15.0"
 
 # AlienBob Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["http://slackware.uk/people/alien/sbrepos/", "current/", "x86_64/"]
 ALIEN_REPO = false
 ALIEN_REPO_NAME = "alien"
+ALIEN_REPO_LOCAL = [""]
 ALIEN_REPO_MIRROR = ["https://slackware.nl/people/alien/sbrepos/", "15.0/", "x86_64/"]
 ALIEN_REPO_PACKAGES = "PACKAGES.TXT"
 ALIEN_REPO_CHECKSUMS = "CHECKSUMS.md5"
 ALIEN_REPO_CHANGELOG = "ChangeLog.txt"
 ALIEN_REPO_TAG = "alien"
 
 # Multilib Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["https://slackware.nl/people/alien/multilib/", current/"]
 MULTILIB_REPO = false
 MULTILIB_REPO_NAME = "multilib"
+MULTILIB_REPO_LOCAL = [""]
 MULTILIB_REPO_MIRROR = ["https://slackware.nl/people/alien/multilib/", "15.0/"]
 MULTILIB_REPO_PACKAGES = "PACKAGES.TXT"
 MULTILIB_REPO_CHECKSUMS = "CHECKSUMS.md5"
 MULTILIB_REPO_CHANGELOG = "ChangeLog.txt"
 MULTILIB_REPO_TAG = "alien"
 
 # Restricted Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["https://slackware.nl/people/alien/restricted_sbrepos/", "current/", "x86_64/"]
 RESTRICTED_REPO = false
 RESTRICTED_REPO_NAME = "restricted"
+RESTRICTED_REPO_LOCAL = [""]
 RESTRICTED_REPO_MIRROR = ["https://slackware.nl/people/alien/restricted_sbrepos/", "15.0/", "x86_64/"]
 RESTRICTED_REPO_PACKAGES = "PACKAGES.TXT"
 RESTRICTED_REPO_CHECKSUMS = "CHECKSUMS.md5"
 RESTRICTED_REPO_CHANGELOG = "ChangeLog.txt"
 RESTRICTED_REPO_TAG = "alien"
 
 # Gnome Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["https://reddoglinux.ddns.net/linux/gnome/43.x/x86_64/"]
 GNOME_REPO = false
 GNOME_REPO_NAME = "gnome"
+GNOME_REPO_LOCAL = [""]
 GNOME_REPO_MIRROR = ["https://reddoglinux.ddns.net/linux/gnome/41.x/x86_64/"]
 GNOME_REPO_PACKAGES = "PACKAGES.TXT"
 GNOME_REPO_CHECKSUMS = "CHECKSUMS.md5"
 GNOME_REPO_CHANGELOG = "ChangeLog.txt"
 GNOME_REPO_TAG = "gfs"
 
 # MATE Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["https://slackware.uk/msb/current/", "1.26/", "x86_64/"]
 MSB_REPO = false
 MSB_REPO_NAME = "msb"
+MSB_REPO_LOCAL = [""]
 MSB_REPO_MIRROR = ["https://slackware.uk/msb/", "15.0/", "1.26/", "x86_64/"]
 MSB_REPO_PACKAGES = "PACKAGES.TXT"
 MSB_REPO_CHECKSUMS = "CHECKSUMS.md5"
 MSB_REPO_CHANGELOG = "ChangeLog.txt"
 MSB_REPO_TAG = "msb"
 
 # Cinnamon Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["https://slackware.uk/csb/", "current/", "x86_64/"]
 CSB_REPO = false
 CSB_REPO_NAME = "csb"
+CSB_REPO_LOCAL = [""]
 CSB_REPO_MIRROR = ["https://slackware.uk/csb/", "15.0/", "x86_64/"]
 CSB_REPO_PACKAGES = "PACKAGES.TXT"
 CSB_REPO_CHECKSUMS = "CHECKSUMS.md5"
 CSB_REPO_CHANGELOG = "ChangeLog.txt"
 CSB_REPO_TAG = "csb"
 
 # Conraid Repository for Slackware x86_64 -current.
 CONRAID_REPO = false
 CONRAID_REPO_NAME = "conraid"
+CONRAID_REPO_LOCAL = [""]
 CONRAID_REPO_MIRROR = ["https://slack.conraid.net/repository/slackware64-current/"]
 CONRAID_REPO_PACKAGES = "PACKAGES.TXT"
 CONRAID_REPO_CHECKSUMS = "CHECKSUMS.md5"
 CONRAID_REPO_CHANGELOG = "ChangeLog.txt"
 CONRAID_REPO_TAG = "cf"
 
 # Slackonly Repository for Slackware x86_64 15.0 stable.
 # For Slackware x86_64 -current:
 # ["https://packages.slackonly.com/pub/packages/current-x86_64/"]
 SLACKONLY_REPO = false
 SLACKONLY_REPO_NAME = "slackonly"
+SLACKONLY_REPO_LOCAL = [""]
 SLACKONLY_REPO_MIRROR = ["https://packages.slackonly.com/pub/packages/15.0-x86_64/"]
 SLACKONLY_REPO_PACKAGES = "PACKAGES.TXT"
 SLACKONLY_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACKONLY_REPO_CHANGELOG = "ChangeLog.txt"
 SLACKONLY_REPO_TAG = "slonly"
 
 # Repository for Salix OS x86_64 15.0 stable.
 SALIXOS_REPO = false
 SALIXOS_REPO_NAME = "salixos"
+SALIXOS_REPO_LOCAL = [""]
 SALIXOS_REPO_MIRROR = ["https://download.salixos.org/x86_64/slackware-15.0/"]
 SALIXOS_REPO_PACKAGES = "PACKAGES.TXT"
 SALIXOS_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SALIXOS_REPO_CHANGELOG = "ChangeLog.txt"
 SALIXOS_REPO_TAG = ""
 
 # Repository for Salix OS x86_64 15.0 stable.
 SALIXOS_EXTRA_REPO = false
 SALIXOS_EXTRA_REPO_NAME = "salixos_extra"
+SALIXOS_EXTRA_REPO_LOCAL = [""]
 SALIXOS_EXTRA_REPO_MIRROR = ["https://download.salixos.org/x86_64/slackware-15.0/", "extra/"]
 SALIXOS_EXTRA_REPO_PACKAGES = "PACKAGES.TXT"
 SALIXOS_EXTRA_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SALIXOS_EXTRA_REPO_CHANGELOG = "ChangeLog.txt"
 SALIXOS_EXTRA_REPO_TAG = ""
 
 # Repository for Salix OS x86_64 15.0 stable.
 SALIXOS_PATCHES_REPO = false
 SALIXOS_PATCHES_REPO_NAME = "salixos_patches"
+SALIXOS_PATCHES_REPO_LOCAL = [""]
 SALIXOS_PATCHES_REPO_MIRROR = ["https://download.salixos.org/x86_64/slackware-15.0/", "patches/"]
 SALIXOS_PATCHES_REPO_PACKAGES = "PACKAGES.TXT"
 SALIXOS_PATCHES_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SALIXOS_PATCHES_REPO_CHANGELOG = "ChangeLog.txt"
 SALIXOS_PATCHES_REPO_TAG = "_slack15.0"
 
 # Repository for Slackel OS x86_64 -current.
 SLACKEL_REPO = false
 SLACKEL_REPO_NAME = "slackel"
+SLACKEL_REPO_LOCAL = [""]
 SLACKEL_REPO_MIRROR = ["http://www.slackel.gr/repo/x86_64/current/"]
 SLACKEL_REPO_PACKAGES = "PACKAGES.TXT"
 SLACKEL_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLACKEL_REPO_CHANGELOG = "ChangeLog.txt"
 SLACKEL_REPO_TAG = "dj"
 
 # Slint Repository for Slackware x86_64 15.0 stable.
 SLINT_REPO = false
 SLINT_REPO_NAME = "slint"
+SLINT_REPO_LOCAL = [""]
 SLINT_REPO_MIRROR = ["https://slackware.uk/slint/x86_64/slint-15.0/"]
 SLINT_REPO_PACKAGES = "PACKAGES.TXT"
 SLINT_REPO_CHECKSUMS = "CHECKSUMS.md5"
 SLINT_REPO_CHANGELOG = "ChangeLog.txt"
 SLINT_REPO_TAG = "slint"
```

### Comparing `slpkg-4.8.2/configs/slpkg.toml` & `slpkg-4.8.3/configs/slpkg.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/tests/test_configs.py` & `slpkg-4.8.3/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/tests/test_checks.py` & `slpkg-4.8.3/tests/test_checks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import unittest
 from slpkg.checks import Check
-from slpkg.binaries.queries import BinQueries
+from slpkg.sbos.queries import SBoQueries
 
 
 class TestPkgInstalled(unittest.TestCase):
 
     def setUp(self):
-        self.bin_queries = BinQueries('alien')
+        self.bin_queries = SBoQueries('sbo')
         self.data = self.bin_queries.repository_data()
-        self.check = Check(['-B', '--bin-repo='], self.data)
-        self.packages = ['audacity', 'vlc', 'dnspython']
+        self.check = Check('sbo', self.data)
+        self.packages = ['audacity', 'Flask', 'awscli']
 
     def test_check_exists(self):
-        self.assertIsNone(self.check.exists_in_the_database(self.packages))
+        self.assertIsNone(self.check.package_exists_in_the_database(self.packages))
 
     def test_check_unsupported(self):
         self.assertIsNone(self.check.is_package_unsupported(self.packages))
 
     def test_check_is_installed(self):
-        self.assertIsNone(self.check.is_package_unsupported(self.packages))
+        self.assertIsNone(self.check.is_package_installed(self.packages))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `slpkg-4.8.2/tests/test_utilities.py` & `slpkg-4.8.3/tests/test_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 import unittest
 
 from pathlib import Path
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
-from slpkg.sbos.queries import SBoQueries
+from slpkg.binaries.queries import BinQueries
 
 
 class TestUtilities(unittest.TestCase):
 
     def setUp(self):
         self.utils = Utilities()
-        self.sbo_queries = SBoQueries()
-        self.data: dict = self.sbo_queries.repository_data()
+        self.repository: str = 'slack'
+        self.queries = BinQueries('slack')
+        self.data: dict = self.queries.repository_data()
         self.build_path = Configs.build_path
         self.package = 'aaa_base-15.0-x86_64-4_slack15.0'
 
     def test_ins_installed(self):
         self.assertEqual(self.package, self.utils.is_package_installed('aaa_base'))
 
     def test_split_name(self):
-        self.assertEqual('aaa_base', self.utils.split_binary_pkg(self.package)[0])
+        self.assertEqual('aaa_base', self.utils.split_package(self.package)['name'])
 
     def test_split_version(self):
-        self.assertEqual('15.0', self.utils.split_binary_pkg(self.package)[1])
+        self.assertEqual('15.0', self.utils.split_package(self.package)['version'])
 
     def test_split_arch(self):
-        self.assertEqual('x86_64', self.utils.split_binary_pkg(self.package)[2])
+        self.assertEqual('x86_64', self.utils.split_package(self.package)['arch'])
 
     def test_split_build(self):
-        self.assertEqual('4', self.utils.split_binary_pkg(self.package)[3])
+        self.assertEqual('4', self.utils.split_package(self.package)['build'])
 
     def test_is_installed(self):
         self.assertEqual(self.package, self.utils.is_package_installed('aaa_base'))
 
     def test_all_installed(self):
         self.assertIn(self.package, self.utils.installed_packages.values())
 
     def test_read_build_tag(self):
-        self.assertEqual('1', self.utils.read_sbo_build_tag('slpkg', 'system'))
+        self.assertEqual('1', self.utils.read_slackbuild_build_tag('slpkg', 'system', 'sbo'))
 
     def test_is_option(self):
         self.assertTrue(True, self.utils.is_option(['-P', '--parallel'],
-                                                   ['-k', '-p', '-P', '--parallel', '--bin-repo']))
+                                                   ['-k', '-p', '-P', '--parallel', '--repository']))
 
     def test_get_file_size(self):
         self.assertEqual('2 MB', self.utils.get_file_size(Path('/var/log/packages/', self.package)))
 
     def test_apply_package_pattern(self):
         self.assertGreater(len(self.utils.apply_package_pattern(self.data, ['*'])), 1)
```

### Comparing `slpkg-4.8.2/tests/test_sbo_queries.py` & `slpkg-4.8.3/tests/test_sbo_queries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 import unittest
 from slpkg.sbos.queries import SBoQueries
 
 
 class TestSBoQueries(unittest.TestCase):
 
     def setUp(self):
-        self.sbo_queries = SBoQueries()
+        self.sbo_queries = SBoQueries('sbo')
         self.data: dict = self.sbo_queries.repository_data()
         self.name: str = 'slpkg'
 
     def test_slackbuild(self):
         self.assertTrue(True, self.data[self.name])
 
     def test_location(self):
-        self.assertEqual('system', self.data[self.name][0])
+        self.assertEqual('system', self.data[self.name]['location'])
 
     def test_sources_x86(self):
         self.assertEqual(['https://gitlab.com/dslackw/slpkg/-/archive'
-                         '/4.8.0/slpkg-4.8.0.tar.gz'], self.data[self.name][3].split())
+                         '/4.8.2/slpkg-4.8.2.tar.gz'], self.data[self.name]['download'].split())
 
     def test_sources_x86_64(self):
-        self.assertEqual([], self.data[self.name][4].split())
+        self.assertEqual([], self.data[self.name]['download64'].split())
 
     def test_requires(self):
-        self.assertEqual(['SQLAlchemy', 'python3-pythondialog', 'python3-progress'], self.data[self.name][7].split())
+        self.assertEqual(['SQLAlchemy', 'python3-pythondialog', 'python3-progress'],
+                         self.data[self.name]['requires'].split())
 
     def test_version(self):
-        self.assertEqual('4.8.0', self.data[self.name][2])
+        self.assertEqual('4.8.2', self.data[self.name]['version'])
 
     def test_checksum_x86(self):
-        self.assertListEqual(['75af7a43379407b8428dc6053fac470c'], self.data[self.name][5].split())
+        self.assertListEqual(['96197dd92a2cc70e163eacdf83909252'], self.data[self.name]['md5sum'].split())
 
     def test_checksum_x86_64(self):
-        self.assertListEqual([], self.data[self.name][6].split())
+        self.assertListEqual([], self.data[self.name]['md5sum64'].split())
 
     def test_files(self):
-        self.assertEqual(5, len(self.data[self.name][1].split()))
+        self.assertEqual(5, len(self.data[self.name]['files'].split()))
 
     def test_description(self):
-        self.assertEqual('slpkg (Slackware Packaging Tool)', self.data[self.name][8])
+        self.assertEqual('slpkg (Slackware Packaging Tool)', self.data[self.name]['description'])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `slpkg-4.8.2/tests/test_colors.py` & `slpkg-4.8.3/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/tests/check_updates_test.py` & `slpkg-4.8.3/tests/check_updates_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         self.repos = Repositories()
         self.repositories = Repositories().repositories
 
     def test(self):
         local_size: int = 0
         for name, data in self.repositories.items():
 
-            local_chg_txt: Path = Path(data[1], 'ChangeLog.txt')
-            repo_chg_txt: str = f'{data[2][0]}ChangeLog.txt'
+            local_chg_txt: Path = Path(data['path'], 'ChangeLog.txt')
+            repo_chg_txt: str = f"{data['mirror'][0]}ChangeLog.txt"
 
             http = PoolManager()
             repo = http.request('GET', repo_chg_txt)
             repo_size: int = int(repo.headers['Content-Length'])
 
             if local_chg_txt.is_file():
                 local_size: int = int(os.stat(local_chg_txt).st_size)
```

### Comparing `slpkg-4.8.2/tests/test_upgrade.py` & `slpkg-4.8.3/tests/test_upgrade.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,40 +6,34 @@
 from slpkg.binaries.queries import BinQueries
 
 
 class TestUtilities(unittest.TestCase):
 
     def setUp(self):
         self.utils = Utilities()
-        self.sbo_queries = SBoQueries()
+        self.sbo_queries = SBoQueries('sbo')
         self.data: dict = self.sbo_queries.repository_data()
 
     def test_installed_is_upgradable_for_sbo_repository(self):
-        flags: list = []
         packages: list = ['sbo-create', 'ptpython', 'pycharm', 'powerline-status']
-
         for pkg in packages:
-            self.assertFalse(False, Upgrade(flags, self.data).is_package_upgradeable(pkg))
+            self.assertFalse(False, Upgrade('sbo', self.data).is_package_upgradeable(pkg))
 
     def test_installed_is_upgradable_for_slack_patches_repository(self):
         repo: str = 'slack_patches'
         bin_queries = BinQueries(repo)
         data: dict = bin_queries.repository_data()
-        flags: list = ['-B', '--bin-repo=']
         packages: list = ['vim', 'httpd', 'seamonkey', 'sudo', 'python3', 'qt5', 'php']
-
         for pkg in packages:
-            self.assertFalse(False, Upgrade(flags, data).is_package_upgradeable(pkg))
+            self.assertFalse(False, Upgrade('slack', data).is_package_upgradeable(pkg))
 
     def test_installed_is_upgradable_for_alien_repository(self):
         repo: str = 'alien'
         bin_queries = BinQueries(repo)
         data: dict = bin_queries.repository_data()
-        flags: list = ['-B', '--bin-repo=']
         packages: list = ['audacity', 'vlc', 'dnspython']
-
         for pkg in packages:
-            self.assertFalse(False, Upgrade(flags, data).is_package_upgradeable(pkg))
+            self.assertFalse(False, Upgrade('alien', data).is_package_upgradeable(pkg))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `slpkg-4.8.2/tests/test_bin_queries.py` & `slpkg-4.8.3/tests/test_bin_queries.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,54 +3,50 @@
 
 
 class TestBinQueries(unittest.TestCase):
 
     def setUp(self):
         self.bin_queries = BinQueries('slack')
         self.repo_data = self.bin_queries.repository_data()
-        self.repos_data = self.bin_queries.repositories_data()
 
     def test_repository_data(self):
         self.assertGreater(len(list(self.repo_data.keys())), 1)
 
-    def test_repositories_data(self):
-        self.assertGreater(len(list(self.repos_data.keys())), 1)
-
     def test_package_name(self):
         self.assertTrue(True, self.repo_data.get('aaa_base'))
 
     def test_version(self):
-        self.assertEqual('15.0', self.repo_data['aaa_base'][0])
+        self.assertEqual('15.0', self.repo_data['aaa_base']['version'])
 
     def test_package_bin(self):
-        self.assertEqual('aaa_base-15.0-x86_64-3.txz', self.repo_data['aaa_base'][1])
+        self.assertEqual('aaa_base-15.0-x86_64-3.txz', self.repo_data['aaa_base']['package'])
 
     def test_mirror(self):
-        self.assertEqual('https://slackware.uk/slackware/slackware64-15.0/', self.repo_data['aaa_base'][2])
+        self.assertEqual('https://slackware.uk/slackware/slackware64-15.0/', self.repo_data['aaa_base']['mirror'])
 
     def test_location(self):
-        self.assertEqual('slackware64/a', self.repo_data['aaa_base'][3])
+        self.assertEqual('slackware64/a', self.repo_data['aaa_base']['location'])
 
     def test_size_comp(self):
-        self.assertEqual('12 KB', self.repo_data['aaa_base'][4])
+        self.assertEqual('12', self.repo_data['aaa_base']['size_comp'])
 
     def test_size_uncomp(self):
-        self.assertEqual('90 KB', self.repo_data['aaa_base'][5])
+        self.assertEqual('90', self.repo_data['aaa_base']['size_uncomp'])
 
     def test_required(self):
-        self.assertEqual('', self.repo_data['aaa_base'][6])
+        self.assertEqual('', self.repo_data['aaa_base']['requires'])
 
     def test_conflicts(self):
-        self.assertEqual('', self.repo_data['aaa_base'][7])
+        self.assertEqual('', self.repo_data['aaa_base']['conflicts'])
 
     def test_suggests(self):
-        self.assertEqual('', self.repo_data['aaa_base'][8])
+        self.assertEqual('', self.repo_data['aaa_base']['suggests'])
 
     def test_description(self):
-        self.assertEqual('', self.repo_data['aaa_base'][9])
+        self.assertEqual('', self.repo_data['aaa_base']['description'])
 
     def test_package_checksum(self):
-        self.assertEqual('ee674755e75a3f9cb3c7cfc0039f376d', self.repo_data['aaa_base'][10])
+        self.assertEqual('ee674755e75a3f9cb3c7cfc0039f376d', self.repo_data['aaa_base']['checksum'])
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `slpkg-4.8.2/LICENSE` & `slpkg-4.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/install.sh` & `slpkg-4.8.3/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/ChangeLog.txt` & `slpkg-4.8.3/ChangeLog.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+4.8.3 - 29/04/2023
+Updated:
+- For synchronization with the local repository (Thanks to Christopher Schrauben) #166
+- Renamed the option --bin-repo with --repository
+Added:
+- Options --install-data to install only data into the database
+- Column for package installed version (Thanks to tpiszcze)
+
 4.8.2 - 25/04/2023
 Updated:
 - For exit status code
 - Packages summary for calculating the file sizes
 Added:
 - Disable or enable the spinning bar
 Fixed:
```

### Comparing `slpkg-4.8.2/man/slpkg.1` & `slpkg-4.8.3/man/slpkg.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-.TH slpkg 1 "Orestiada, Greece" "slpkg 4.8.2" dslackw
+.TH slpkg 1 "Orestiada, Greece" "slpkg 4.8.3" dslackw
 .SH NAME
 .P
 slpkg \- Package manager utility for Slackware.
 .SH SYNOPSIS
 .P
 slpkg \c
 [\fICOMMAND\fR] [\fIOPTIONS\fR] [\fIFILELIST|PACKAGES...\fR]
 .P
 slpkg [-h|-v] [-u, update] [-U, upgrade] [-c, check-updates] [-I, repo-info] [-g, configs]
 [-L, clean-logs] [-D, clean-tmp] [-T, clean-data] [-b, build] [-i, install] [-d, download]
-[-R, remove] [-f, find] [-w, view] [-s, search] [-e, dependees] [-t, tracking] -y, --yes, -j, --jobs, -o, --resolve-off,
--r, --reinstall, -k, --skip-installed, -E, --full-reverse, -S, --search, -n, --no-silent, -p, --pkg-version, -z,
--G, --generate-only, -P, --parallel, -B, --bin-repo=[\fIREPO\fR], -z, --directory=[\fIPATH\fR]
+[-R, remove] [-f, find] [-w, view] [-s, search] [-e, dependees] [-t, tracking] -y, --yes, -j, --jobs, -O, --resolve-off,
+-r, --reinstall, -k, --skip-installed, -a, --install-data, -E, --full-reverse, -S, --search, -n, --no-silent, -p, --pkg-version,
+-P, --parallel, -o, --repository=\fINAME\fR, -z, --directory=\fIPATH\fR
 .SH DESCRIPTION
 .P
 Slpkg is a software package manager that installs, updates, and removes packages on Slackware based systems.
 It automatically computes dependencies and figures out what things should occur to install packages.
 Slpkg makes it easier to maintain groups of machines without having to manually update.
 .P
 Slpkg works in accordance with the standards of the organization SlackBuilds.org to build packages.
@@ -62,15 +62,15 @@
 .B -g, configs
 .RS
 Edit the configuration /etc/slpkg/slpkg.toml file.
 .RE
 .P
 .B -b, build
 .RS
-Builds the Slackbuilds scripts and adds them to the /tmp directory.
+Builds the Slackbuilds scripts and add the packages to the '/tmp' directory.
 .RE
 .P
 .B -i, install
 .RS
 Builds and installs the packages in the correct order, and also logs the packages with the dependencies for removal.
 .RE
 .P
@@ -83,15 +83,15 @@
 .RS
 Removes packages with dependencies if the packages was installed with '\fIslpkg install\fR' method.
 Slpkg looks at the 'REPO_TAG' configuration to find packages for removal by default, except if you are using \fB--file-pattern\fR option.
 .RE
 .P
 .B -f, find
 .RS
-Find your installed packages on your system..
+Find your installed packages on your system.
 .RE
 .P
 .B -w, view
 .RS
 View information packages from the repository and get everything in your terminal.
 .RE
 .P
@@ -120,15 +120,15 @@
 .B -j, --jobs
 .RS
 Acceleration of SlackBuild scripts. When the \fB--jobs\fR flag is set, slpkg automatically detects the number
 of processors and enters it into the MAKEFLAGS variable. Some SlackBuilds fail when MAKEFLAGS is declared or
 the number of processors (-j) is greater than one. (to be used with: -U, upgrade, -b, build, -i, install)
 .RE
 .P
-.B -o, --resolve-off
+.B -O, --resolve-off
 .RS
 Turns off dependency resolving. (to be used with: -U, upgrade, -b, build, -i, install)
 .RE
 .P
 .B -r, --reinstall
 .RS
 Use this option if you want to upgrade all packages even if the same version is already installed.
@@ -137,14 +137,22 @@
 .P
 .B -k, --skip-installed
 .RS
 This a helpful option if you want to avoid building and reinstalling packages.
 Note: This option affects only the dependencies. (to be used with: -i, install)
 .RE
 .P
+.B -a, --install-data
+.RS
+Install the data into the database only, if when you don't want to re-download or re-synchronize the package lists,
+and you have already downloaded the repository, you can apply this options to install the data into the database.
+This is a helpful especially for locals repositories and for those who download the repositories manually.
+(to be used with: -u, update)
+.RE
+.P
 .B -E, --full-reverse
 .RS
 Full reverse dependency. Works only with -e, dependees command and show the requires too.
 (to be used with: -e, dependees)
 .RE
 .P
 .B -S, --search
@@ -162,37 +170,30 @@
 .RE
 .P
 .B -p, --pkg-version
 .RS
 Print the repository package version. (to be used with: -e, dependees, -t, tracking, -w, view)
 .RE
 .P
-.B -G, --generate-only
-.RS
-It is used only with the ponce repository and when you want to generate only the SLACKBUILDS.TXT
-file and update the database, without downloading the whole repository if you have already
-downloaded it. (to be used with: -u, update)
-.RE
-.P
 .B -P, --parallel
 .RS
 Download files in parallel to speed up the process.
 (to be used with: -u, update, -U, upgrade, -b, build, -i, install, -d, download)
 .RE
 .P
-.BI "-B," "" " \-\-bin-repo=[" REPO "]
+.BI "-o," "" " \-\--repository=" NAME "
 .RS
-Switch to binaries repositories and select a repository.
-Example: '\fIslpkg -i audacity --bin-repo=alien\fR'. Options update, check, and search support the asterisk '*' to apply
-it in all repositories, like search a package to all binaries repositories '\fIslpkg -s libreoffice --bin-repo='*'\fR'.
-Repo pattern '*' supported only with: -s, search, -u, update and -c, check-updates options.
-(to be used with: -u, update, -c, check-updates, -U, upgrade, -i, install, -d, download, -s, search, -t, tracking, -e, dependees, -w, view)
+Switches the default repository and set the repository you want to work with.
+Make sure that you have been enabling the repository in the file '/etc/slpkg/repositories.toml'.
+Repo pattern '*' supported only with: '-s, search' option.
+(to be used with: -u, update, -U, upgrade, -c, check-updates, -I, repo-info, -b, build, -i, install, -d, download, -s, search,
+-t, tracking, -e, dependees, -w, view)
 .RE
 .P
-.BI "-z," "" " \-\-directory=[" PATH "]
+.BI "-z," "" " \-\-directory=" PATH "
 .RS
 The directory is the path where the files will be saved. (to be used with: -d, download)
 .RE
 .P
 .B -h | --help
 .RS
 Show help information and exit.
@@ -232,27 +233,25 @@
 For the upgrade command, you should know, that you can upgrade packages from different repositories, if you edit
 the '\fI/etc/slpkg/repositories.toml\fR' file and remove the repository tag. Then the slpkg can't recognize the repository of the packages.
 
 With the remove command, it's going to remove the dependencies if the package had installed with the '\fIslpkg install\fR' command,
 otherwise, the slpkg does not know the dependencies that are installed with the packages that going to remove.
 
 You can apply the asterisk '*' instead of a package, to matching all the packages from a repository. You can't apply
-an asterisk to the '\fB-B, --bin-repos=\fR' option, except for the '\fB-s, search\fR', '\fB-u, update\fR' and '\fB-c, check-updates\fR' commands.
-
-Command clean-data, removes the local repository data and the database data.
+an asterisk to the '\fB-o, --repository=\fR' option, except for the '\fB-s, search\fR', command.
 
 Note: There is currently no function to indicate the packages if the colors are disabled.
 .RE
 .SH EXIT STATUS
 .P
 0 Successful slpkg execution.
 .P
 1 Something wrong happened.
 .P
-20 No package found to be  downloaded,  installed,  reinstalled,  up‐graded, or removed.
+20 No package found to be  downloaded,  installed,  reinstalled,  upgraded, or removed.
 .RE
 .SH CONFIGURATION FILES
 .P
 Configuration file in the /etc/slpkg/slpkg.toml file.
 .P
 Repositories file in the /etc/slpkg/repositories.toml file.
 .P
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `slpkg-4.8.2/man/slpkg-fr.1` & `slpkg-4.8.3/man/slpkg-fr.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/completion/slpkg` & `slpkg-4.8.3/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/slpkg/dialog_configs.py` & `slpkg-4.8.3/slpkg/dialog_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 
         # Creating the elements for the dialog form.
         for i, (key, value) in enumerate(self.configs['CONFIGS'].items(), start=1):
             if value is True:
                 value: str = 'true'
             elif value is False:
                 value: str = 'false'
-            elements += [
-                (key, i, 1, value, i, 21, 47, 200, '0x0', f'Config: {key} = {value}')
-            ]
+            elements.extend(
+                [(key, i, 1, value, i, 21, 47, 200, '0x0', f'Config: {key} = {value}')]
+            )
 
         code, tags = self.dialogbox.mixedform(text, title, elements, height, width)
 
         os.system('clear')
 
         if code == 'help':
             tags = self.configs.values()
@@ -79,34 +79,35 @@
             'SPINNING_BAR'
         ]
         values: list = ['true', 'false']
 
         for key, value in zip(self.configs['CONFIGS'].keys(), tags):
 
             if key in keys and value not in values:
-                self.dialogbox.msgbox(f"\nError value for {key}. It must be 'true' or 'false'\n", height=7, width=60)
+                self.dialogbox.msgbox(f"\nError: Value for '{key}', it must be 'true' or 'false.'\n",
+                                      height=7, width=60)
                 return False
 
-            if key in ['DOWNLOADER'] and value not in ['wget', 'curl', 'lftp']:
-                self.dialogbox.msgbox(f"\nError value for {key}. It must be 'wget' or 'curl'\n", height=7, width=60)
+            if key in ['DOWNLOADER'] and value not in ['wget2', 'wget', 'curl', 'lftp']:
+                self.dialogbox.msgbox(f"\nError: Value for '{key}' not supported.\n",
+                                      height=7, width=60)
                 return False
 
         return True
 
     def read_configs(self) -> None:
         """ Read the original config file. """
         with open(self.config_file, 'r') as toml_file:
             self.orig_configs: list = toml_file.readlines()
 
     def write_file(self, tags: list) -> None:
         """ Write the new values to the config file. """
         self.read_configs()
 
         with open(self.config_file, 'w') as patch_toml:
-
             for line in self.orig_configs:
                 for key, value in zip(self.configs['CONFIGS'].keys(), tags):
 
                     if line.lstrip().startswith(f'{key} ='):
                         line = f'  {key} = "{value}"\n'
 
                     if line.lstrip().startswith(
```

### Comparing `slpkg-4.8.2/slpkg/binaries/required.py` & `slpkg-4.8.3/slpkg/sbos/dependencies.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,38 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from typing import Generator
 
-from slpkg.repositories import Repositories
 
-
-class Required:
-    """ Creates a list of dependencies with
+class Requires:
+    """ Creates a tuple of dependencies with
     the right order to install. """
+    __slots__ = ('data', 'name', 'repository_packages')
 
     def __init__(self, data: dict, name: str):
-        __slots__ = 'data', 'name,'
         self.data: dict = data
         self.name: str = name
-        self.repos = Repositories()
-
-        self.special_repos: list = [
-            self.repos.salixos_repo_name,
-            self.repos.salixos_patches_repo_name,
-            self.repos.salixos_extra_repo_name,
-            self.repos.slackel_repo_name,
-            self.repos.slint_repo_name
-        ]
-
-        self.repo: str = data[name][11]
+        self.repository_packages: tuple = tuple(data.keys())
 
-    def resolve(self) -> list:
+    def resolve(self) -> tuple:
         """ Resolve the dependencies. """
-        required: list[str] = list(self.remove_deps(self.data[self.name][6].split()))
+        requires: list[str] = list(
+            self.remove_deps(self.data[self.name]['requires'].split())
+        )
+
+        for require in requires:
+            sub_requires: list[str] = list(
+                self.remove_deps(self.data[require]['requires'].split())
+            )
+            for sub in sub_requires:
+                requires.append(sub)
 
-        # Resolve dependencies for some special repos.
-        if self.repo in self.special_repos:
-            for req in required:
-                if req not in list(self.data.keys()):
-                    required.remove(req)
-
-        else:
-            for req in required:
-                sub_required: list[str] = list(self.remove_deps(self.data[req][6].split()))
-                for sub in sub_required:
-                    required.append(sub)
+        requires.reverse()
 
-        required.reverse()
-        return list(dict.fromkeys(required))
+        return tuple(dict.fromkeys(requires))
 
     def remove_deps(self, requires: list) -> Generator:
         """ Remove requires that not in the repository or blacklisted. """
-        for dep in requires:
-            if dep in list(self.data.keys()):
-                yield dep
+        for dependency in requires:
+            if dependency in self.repository_packages:
+                yield dependency
```

### Comparing `slpkg-4.8.2/slpkg/binaries/install.py` & `slpkg-4.8.3/slpkg/binaries/install.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,136 +1,135 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
 import time
-import subprocess
 from pathlib import Path
 from collections import OrderedDict
-from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.checksum import Md5sum
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
-from slpkg.progress_bar import ProgressBar
 from slpkg.logging_deps import LoggingDeps
 from slpkg.repositories import Repositories
+from slpkg.multi_process import MultiProcess
 from slpkg.binaries.required import Required
-from slpkg.models.models import session as Session
 
 
 class Packages(Configs):
 
-    def __init__(self, data: dict, packages: list, flags: list, mode: str):
-        __slots__ = 'data', 'packages', 'flags', 'mode'
+    def __init__(self, repository: str, data: dict, packages: list, flags: list, mode: str):
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
         self.mode: str = mode
 
-        self.progress = ProgressBar()
         self.utils = Utilities()
         self.repos = Repositories()
         self.dialogbox = DialogBox()
-        self.logs_deps = LoggingDeps(flags, data)
-        self.upgrade = Upgrade(flags, data)
-        self.view_message = ViewMessage(flags, data)
-        self.session = Session
-
-        self.stderr = None
-        self.stdout = None
-        self.process_message: str = ''
+        self.multi_proc = MultiProcess(flags)
+        self.logs_deps = LoggingDeps(repository, data)
+        self.upgrade = Upgrade(repository, data)
+        self.view_message = ViewMessage(flags, repository, data)
+        self.check_md5 = Md5sum(flags)
 
-        self.packages_requires: list = []
+        self.dependencies: list = []
         self.install_order: list = []
         self.binary_packages: list = []
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ['-r', '--reinstall'], flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ['-k', '--skip-installed'], flags)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-o', '--resolve-off'], flags)
-
-        self.option_for_no_silent: bool = self.utils.is_option(
-            ['-n', '--no-silent'], flags)
+            ['-O', '--resolve-off'], flags)
 
         self.packages: list = self.utils.apply_package_pattern(data, packages)
 
     def execute(self) -> None:
-        self.dependencies()
+        # self.creating_dependencies_list()
+        self.creating_dependencies_list()
+        self.remove_duplicate_from_dependencies_list()
+        self.choose_package_dependencies()
+        self.add_dependencies_to_install_order()
+        self.clean_the_main_slackbuilds()
+        self.add_main_packages_to_install_order()
 
-        self.view_message.install_packages(self.packages, self.packages_requires, self.mode)
+        self.view_message.install_upgrade_packages(self.packages, self.dependencies, self.mode)
         self.view_message.question()
 
         start: float = time.time()
-        self.download()
-        self.checksum()
+        self.crating_the_package_urls_list()
+        self.checksum_binary_packages()
         self.install_packages()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
-    def dependencies(self):
-        """ Creating the dependencies list and the order for install. """
+    def creating_dependencies_list(self) -> None:
         if not self.option_for_resolve_off:
+            for package in self.packages:
+                dependencies: tuple = Required(self.data, package).resolve()
 
-            for pkg in self.packages:
-
-                # Skip installed package when the option --skip-installed is applied.
-                if self.option_for_skip_installed and self.utils.is_package_installed(pkg):
-                    continue
+                for dependency in dependencies:
+                    # Skip installed package when the option --skip-installed is applied.
+                    if self.option_for_skip_installed and self.utils.is_package_installed(dependency):
+                        continue
 
-                self.packages_requires += Required(self.data, pkg).resolve()
+                    self.dependencies.append(dependency)
 
-            # Clean dependencies from the dependencies list if already added with main packages.
-            requires = list(OrderedDict.fromkeys(self.packages_requires))
+    def remove_duplicate_from_dependencies_list(self) -> None:
+        if self.dependencies:
+            self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
-            if requires:
-                self.packages_requires = self.choose_dependencies(requires)
+    def add_dependencies_to_install_order(self) -> None:
+        self.install_order.extend(self.dependencies)
 
-        # Clean up the main packages if they were selected for dependencies.
-        for dep in self.packages_requires:
-            if dep in self.packages:
-                self.packages.remove(dep)
+    def clean_the_main_slackbuilds(self) -> None:
+        for dependency in self.dependencies:
+            if dependency in self.packages:
+                self.packages.remove(dependency)
 
-        self.install_order = [*self.packages_requires, *self.packages]
+    def add_main_packages_to_install_order(self) -> None:
+        self.install_order.extend(self.packages)
 
-    def download(self) -> None:
-        """ Download packages from the repositories. """
-        pkg_urls: list = []
+    def crating_the_package_urls_list(self) -> None:
+        package_urls: list = []
 
         for pkg in self.install_order:
+            if self.continue_to_install(pkg):
+                package: str = self.data[pkg]['package']
+                mirror: str = self.data[pkg]['mirror']
+                location: str = self.data[pkg]['location']
 
-            if self.continue_install(pkg):
-                package: str = self.data[pkg][1]
-                mirror: str = self.data[pkg][2]
-                location: str = self.data[pkg][3]
-
-                pkg_urls.append(f'{mirror}{location}/{package}')
+                package_urls.append(f'{mirror}{location}/{package}')
 
                 self.binary_packages.append(package)
                 self.utils.remove_file_if_exists(self.tmp_slpkg, package)
             else:
-                version: str = self.data[pkg][0]
-                self.view_message.view_skipping_packages(pkg, version)
-
-        if pkg_urls:
-            down = Downloader(self.tmp_slpkg, pkg_urls, self.flags)
+                installed_package: str = self.utils.is_package_installed(pkg)
+                installed_version: str = self.utils.split_package(installed_package)['version']
+                self.view_message.view_skipping_packages(pkg, installed_version)
+
+        self.download_the_binary_packages(package_urls)
+
+    def download_the_binary_packages(self, package_urls: list) -> None:
+        if package_urls:
+            down = Downloader(self.tmp_slpkg, package_urls, self.flags)
             down.download()
             print()
 
-    def continue_install(self, name) -> bool:
+    def continue_to_install(self, name: str) -> bool:
         """ Skip installed package when the option --skip-installed is applied
             and continue to install if the package is upgradable or the --reinstall option
             applied.
          """
         if not self.utils.is_package_installed(name):
             return True
 
@@ -138,105 +137,58 @@
             return True
 
         if self.utils.is_package_installed(name) and self.option_for_reinstall:
             return True
 
         return False
 
-    def checksum(self) -> None:
-        """ Packages checksums. """
-        md5 = Md5sum(self.flags)
+    def checksum_binary_packages(self) -> None:
         for package in self.binary_packages:
-            name: str = self.utils.split_binary_pkg(Path(package).stem)[0]
-            pkg_checksum: str = self.data[name][10]
-            md5.check(self.tmp_slpkg, package, pkg_checksum)
+            name: str = self.utils.split_package(Path(package).stem)['name']
+            pkg_checksum: str = self.data[name]['checksum']
+            self.check_md5.md5sum(self.tmp_slpkg, package, pkg_checksum)
 
     def install_packages(self) -> None:
-        """ Install the packages. """
         for package in self.binary_packages:
-
-            message: str = f'{self.cyan}Installing{self.endc}'
+            progress_message: str = f'{self.cyan}Installing{self.endc}'
             slack_command: str = self.installpkg
 
             if (self.option_for_reinstall or self.utils.is_package_installed(package)
                     or self.mode == 'upgrade'):
-
-                message: str = f'{self.cyan}Upgrade{self.endc}'
+                progress_message: str = f'{self.cyan}Upgrading{self.endc}'
                 slack_command: str = self.reinstall
 
             command: str = f'{slack_command} {self.tmp_slpkg}/{package}'
-            self.process_message: str = f"package '{package}' to install"
-            self.multi_process(command, package, message)
+            process_message: str = f"package '{package}' to install"
+            self.multi_proc.process(command, package, process_message, progress_message)
 
             if not self.option_for_resolve_off:
-                name: str = self.utils.split_binary_pkg(Path(package).stem)[0]
+                name: str = self.utils.split_package(Path(package).stem)['name']
                 self.logs_deps.logging(name)
 
-    def multi_process(self, command: str, filename: str, message: str) -> None:
-        """ Starting multiprocessing install/upgrade process. """
-        if self.silent_mode and not self.option_for_no_silent:
-
-            done: str = f' {self.byellow} Done{self.endc}'
-            self.stderr = subprocess.DEVNULL
-            self.stdout = subprocess.DEVNULL
-
-            # Starting multiprocessing
-            p1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
-            p2 = Process(target=self.progress.bar, args=(f'{message}:', filename))
-
-            p1.start()
-            p2.start()
-
-            # Wait until process 1 finish
-            p1.join()
+    def choose_package_dependencies(self) -> None:
+        if self.dependencies:
+            height: int = 10
+            width: int = 70
+            list_height: int = 0
+            choices: list = []
+            title: str = ' Choose dependencies you want to install '
 
-            # Terminate process 2 if process 1 finished
-            if not p1.is_alive():
-
-                if p1.exitcode != 0:
-                    done: str = f'{self.bred}Failed: {self.endc}{self.process_message}.'
-
-                print(f'{self.endc}{done}', end='')
-                p2.terminate()
-
-            # Wait until process 2 finish
-            p2.join()
-
-            # Restore the terminal cursor
-            print('\x1b[?25h', self.endc)
-        else:
-            self.utils.process(command, self.stderr, self.stdout)
-
-    def choose_dependencies(self, dependencies: list) -> list:
-        """ Choose packages for install. """
-        height: int = 10
-        width: int = 70
-        list_height: int = 0
-        choices: list = []
-        title: str = ' Choose dependencies you want to install '
-
-        for package in dependencies:
-            status: bool = True
-
-            repo_ver: str = self.data[package][0]
-            help_text: str = f'Package: {package} {repo_ver}'
-            installed: str = self.utils.is_package_installed(package)
-
-            if installed:
-                status: bool = False
-
-            if self.option_for_reinstall:
+            for package in self.dependencies:
                 status: bool = True
+                repo_ver: str = self.data[package]['version']
+                help_text: str = f'Package: {package} {repo_ver}'
+                installed: str = self.utils.is_package_installed(package)
 
-            choices += [(package, repo_ver, status, help_text)]
-
-        text: str = f'There are {len(choices)} dependencies:'
+                if installed:
+                    status: bool = False
 
-        code, tags = self.dialogbox.checklist(text, dependencies, title, height,
-                                              width, list_height, choices)
+                if self.option_for_reinstall:
+                    status: bool = True
 
-        if not code:
-            return dependencies
+                choices.extend([(package, repo_ver, status, help_text)])
 
-        os.system('clear')
+            text: str = f'There are {len(choices)} dependencies:'
+            code, self.dependencies = self.dialogbox.checklist(
+                text, self.dependencies, title, height, width, list_height, choices)
 
-        return tags
+            os.system('clear')
```

### Comparing `slpkg-4.8.2/slpkg/install_data.py` & `slpkg-4.8.3/slpkg/install_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+import re
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.repositories import Repositories
 from slpkg.models.models import session as Session
 from slpkg.models.models import (SBoTable, PonceTable,
@@ -17,73 +18,115 @@
         super(Configs, self).__init__()
         self.session = Session
         self.utils = Utilities()
         self.repos = Repositories()
 
     def last_updated(self, repo_file: Path) -> str:
         """ Reads the first date of the changelog file."""
-        lines: list = self.utils.read_file(repo_file)
+        lines: list = self.utils.read_text_file(repo_file)
         days = ('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
         for line in lines:
             if line.startswith(days):
                 return line.replace('\n', '')
 
-    def install_sbos_data(self) -> None:
+    def install_sbo_data(self) -> None:
         """ Install the data for SBo repository. """
         sbo_tags = [
             'SLACKBUILD NAME:',
             'SLACKBUILD LOCATION:',
             'SLACKBUILD FILES:',
             'SLACKBUILD VERSION:',
             'SLACKBUILD DOWNLOAD:',
             'SLACKBUILD DOWNLOAD_x86_64:',
             'SLACKBUILD MD5SUM:',
             'SLACKBUILD MD5SUM_x86_64:',
             'SLACKBUILD REQUIRES:',
             'SLACKBUILD SHORT DESCRIPTION:'
         ]
-        sbo_table = SBoTable
-        sbo_name: str = self.repos.sbo_repo_name
+
         path_slackbuilds: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
         path_changelog: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
 
-        if self.repos.ponce_repo:
-            sbo_table = PonceTable
-            sbo_name: str = self.repos.ponce_repo_name
-            path_slackbuilds = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
-            path_changelog: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
+        slackbuilds_txt: list = self.utils.read_text_file(path_slackbuilds)
+
+        cache: list = []  # init cache
+
+        print(f"Updating the database for '{self.cyan}{self.repos.sbo_repo_name}{self.endc}'... ", end='', flush=True)
+
+        for i, line in enumerate(slackbuilds_txt, 1):
+
+            for tag in sbo_tags:
+                if line.startswith(tag):
+                    line = line.replace(tag, '').strip()
+                    cache.append(line)
+
+            if (i % 11) == 0:
+                data: str = SBoTable(name=cache[0], location=cache[1].split('/')[1],
+                                     files=cache[2], version=cache[3],
+                                     download=cache[4], download64=cache[5],
+                                     md5sum=cache[6], md5sum64=cache[7],
+                                     requires=cache[8], short_description=cache[9])
+                self.session.add(data)
+
+                cache: list = []  # reset cache after 11 lines
+
+        last_updated: str = self.last_updated(path_changelog)
+        date: str = LastRepoUpdated(repo=self.repos.sbo_repo_name, date=last_updated)
+        self.session.add(date)
+
+        print(f'{self.byellow}Done{self.endc}\n')
+
+        self.session.commit()
+
+    def install_ponce_data(self) -> None:
+        """ Install the data for SBo repository. """
+        sbo_tags = [
+            'SLACKBUILD NAME:',
+            'SLACKBUILD LOCATION:',
+            'SLACKBUILD FILES:',
+            'SLACKBUILD VERSION:',
+            'SLACKBUILD DOWNLOAD:',
+            'SLACKBUILD DOWNLOAD_x86_64:',
+            'SLACKBUILD MD5SUM:',
+            'SLACKBUILD MD5SUM_x86_64:',
+            'SLACKBUILD REQUIRES:',
+            'SLACKBUILD SHORT DESCRIPTION:'
+        ]
+
+        path_slackbuilds = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
+        path_changelog: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
 
-        slackbuilds_txt: list = self.utils.read_file(path_slackbuilds)
+        slackbuilds_txt: list = self.utils.read_text_file(path_slackbuilds)
 
         cache: list = []  # init cache
 
-        print(f"Updating the database for '{self.cyan}{sbo_name}{self.endc}'... ", end='', flush=True)
+        print(f"Updating the database for '{self.cyan}{self.repos.ponce_repo_name}{self.endc}'... ", end='', flush=True)
 
         for i, line in enumerate(slackbuilds_txt, 1):
 
             for tag in sbo_tags:
                 if line.startswith(tag):
                     line = line.replace(tag, '').strip()
                     cache.append(line)
 
             if (i % 11) == 0:
-                data: str = sbo_table(name=cache[0], location=cache[1].split('/')[1],
-                                      files=cache[2], version=cache[3],
-                                      download=cache[4], download64=cache[5],
-                                      md5sum=cache[6], md5sum64=cache[7],
-                                      requires=cache[8], short_description=cache[9])
+                data: str = PonceTable(name=cache[0], location=cache[1].split('/')[1],
+                                       files=cache[2], version=cache[3],
+                                       download=cache[4], download64=cache[5],
+                                       md5sum=cache[6], md5sum64=cache[7],
+                                       requires=cache[8], short_description=cache[9])
                 self.session.add(data)
 
                 cache: list = []  # reset cache after 11 lines
 
         last_updated: str = self.last_updated(path_changelog)
-        date: str = LastRepoUpdated(repo=sbo_name, date=last_updated)
+        date: str = LastRepoUpdated(repo=self.repos.ponce_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_slack_data(self) -> None:
         """ Install the data for slackware repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slack_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -96,51 +139,54 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.slack_repo_path, self.repos.slack_repo_packages)
         path_checksums: Path = Path(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
         path_changelog: Path = Path(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.slack_repo_mirror[0]
+        if self.repos.slack_repo_local[0].startswith('file'):
+            mirror: str = self.repos.slack_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.slack_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location = line.replace(pkg_tag[2], '').strip()
                 cache.append(package_location[2:])  # Do not install (.) dot
 
             if line.startswith(pkg_tag[3]):
-                package_size_comp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
-                package_size_uncomp = line.replace(pkg_tag[4], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -163,15 +209,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slack_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_slack_extra_data(self) -> None:
         """ Install the data for slackware extra repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slack_extra_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -184,51 +230,54 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_packages)
         path_checksums: Path = Path(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_checksums)
         path_changelog: Path = Path(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.slack_extra_repo_mirror[0]
+        if self.repos.slack_extra_repo_local[0].startswith('file'):
+            mirror: str = self.repos.slack_extra_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.slack_extra_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location = line.replace(pkg_tag[2], '').strip()
                 cache.append(package_location[2:])  # Do not install (.) dot
 
             if line.startswith(pkg_tag[3]):
-                package_size_comp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
-                package_size_uncomp = line.replace(pkg_tag[4], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -251,15 +300,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slack_extra_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_slack_patches_data(self) -> None:
         """ Install the data for slackware patches repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slack_patches_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -272,51 +321,54 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.slack_patches_repo_path, self.repos.slack_patches_repo_packages)
         path_checksums: Path = Path(self.repos.slack_patches_repo_path, self.repos.slack_patches_repo_checksums)
         path_changelog: Path = Path(self.repos.slack_patches_repo_path, self.repos.slack_patches_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.slack_patches_repo_mirror[0]
+        if self.repos.slack_patches_repo_local[0].startswith('file'):
+            mirror: str = self.repos.slack_patches_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.slack_patches_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location = line.replace(pkg_tag[2], '').strip()
                 cache.append(package_location[2:])  # Do not install (.) dot
 
             if line.startswith(pkg_tag[3]):
-                package_size_comp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
-                package_size_uncomp = line.replace(pkg_tag[4], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -339,15 +391,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slack_patches_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_alien_data(self) -> None:
         """ Install the data for alien repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.alien_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -360,52 +412,55 @@
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.alien_repo_path, self.repos.alien_repo_packages)
         path_checksums: Path = Path(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
         path_changelog: Path = Path(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = ''.join(self.repos.alien_repo_mirror)
+        if self.repos.alien_repo_local[0].startswith('file'):
+            mirror: str = ''.join(self.repos.alien_repo_local)
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append("".join(self.repos.alien_repo_mirror))
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (.) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 required = line.replace(pkg_tag[4], '').strip()
                 package_required = required.replace(',', ' ').strip()
                 cache.append(package_required)
 
             if line.startswith(pkg_tag[5]):
@@ -433,15 +488,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.alien_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_multilib_data(self) -> None:
         """ Install the data for multilib repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.multilib_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -453,52 +508,55 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
         path_checksums: Path = Path(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
         path_changelog: Path = Path(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = ''.join(self.repos.multilib_repo_mirror)
+        if self.repos.multilib_repo_local[0].startswith('file'):
+            mirror: str = ''.join(self.repos.multilib_repo_local)
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append("".join(self.repos.multilib_repo_mirror))
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)  # package name
+                cache.append(version)  # package version
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 package_description = line.replace(pkg_tag[4], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -521,15 +579,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.multilib_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_restricted_data(self) -> None:
         """ Install the data for multilib repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.restricted_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -541,52 +599,55 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
         path_checksums: Path = Path(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
         path_changelog: Path = Path(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = ''.join(self.repos.restricted_repo_mirror)
+        if self.repos.restricted_repo_local[0].startswith('file'):
+            mirror: str = ''.join(self.repos.restricted_repo_local)
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append("".join(self.repos.restricted_repo_mirror))
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 package_description = line.replace(pkg_tag[4], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -609,15 +670,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.restricted_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_gnome_data(self) -> None:
         """ Install the data for gnome repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.gnome_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -630,52 +691,55 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
         path_checksums: Path = Path(self.repos.gnome_repo_path, self.repos.gnome_repo_checksums)
         path_changelog: Path = Path(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.gnome_repo_mirror[0]
+        if self.repos.gnome_repo_local[0].startswith('file'):
+            mirror: str = self.repos.gnome_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.gnome_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location = line.replace(pkg_tag[2], '').strip()
                 cache.append(package_location[1:])  # Do not install (.) dot
 
             if line.startswith(pkg_tag[3]):
-                package_size_comp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
-                package_size_uncomp = line.replace(pkg_tag[4], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -698,15 +762,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.gnome_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_msb_data(self) -> None:
         """ Install the data for msb repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.msb_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -718,52 +782,55 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.msb_repo_path, self.repos.msb_repo_packages)
         path_checksums: Path = Path(self.repos.msb_repo_path, self.repos.msb_repo_checksums)
         path_changelog: Path = Path(self.repos.msb_repo_path, self.repos.msb_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = ''.join(self.repos.msb_repo_mirror)
+        if self.repos.msb_repo_local[0].startswith('file'):
+            mirror: str = ''.join(self.repos.msb_repo_local)
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append("".join(self.repos.msb_repo_mirror))
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 package_description = line.replace(pkg_tag[4], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -786,15 +853,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.msb_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_csb_data(self) -> None:
         """ Install the data for csb repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.csb_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -806,52 +873,55 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.csb_repo_path, self.repos.csb_repo_packages)
         path_checksums: Path = Path(self.repos.csb_repo_path, self.repos.csb_repo_checksums)
         path_changelog: Path = Path(self.repos.csb_repo_path, self.repos.csb_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = ''.join(self.repos.csb_repo_mirror)
+        if self.repos.csb_repo_local[0].startswith('file'):
+            mirror: str = ''.join(self.repos.csb_repo_local)
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append("".join(self.repos.csb_repo_mirror))
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 package_description = line.replace(pkg_tag[4], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -874,15 +944,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.csb_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_conraid_data(self) -> None:
         """ Install the data for conraid repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.conraid_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -895,53 +965,55 @@
             'PACKAGE SIZE (compressed):',
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
         path_checksums: Path = Path(self.repos.conraid_repo_path, self.repos.conraid_repo_checksums)
         path_changelog: Path = Path(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
 
-        packages_txt: list = self.utils.read_file(path_packages)
+        mirror: str = self.repos.conraid_repo_mirror[0]
+        if self.repos.conraid_repo_local[0].startswith('file'):
+            mirror: str = self.repos.conraid_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name: str = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.conraid_repo_mirror[0])
+                package: str = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[2]):
                 package_location: str = line.replace(pkg_tag[2], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[3]):
-                package_size_comp: str = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
-                package_size_uncomp: str = line.replace(pkg_tag[4], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[5]):
                 package_description: str = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
             if len(cache) == 9:
                 data: str = BinariesTable(
@@ -964,15 +1036,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.conraid_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_slackonly_data(self) -> None:
         """ Install the data for slackonly repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slackonly_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -985,52 +1057,55 @@
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
         path_checksums: Path = Path(self.repos.slackonly_repo_path, self.repos.slackonly_repo_checksums)
         path_changelog: Path = Path(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.slackonly_repo_mirror[0]
+        if self.repos.slackonly_repo_local[0].startswith('file'):
+            mirror: str = self.repos.slackonly_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.slackonly_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 required = line.replace(pkg_tag[4], '').strip()
                 package_required = required.replace(',', ' ').strip()
                 cache.append(package_required)
 
             if line.startswith(pkg_tag[5]):
@@ -1058,15 +1133,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slackonly_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_salixos_data(self) -> None:
         """ Install the data for salixos repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.salixos_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -1079,63 +1154,66 @@
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
         path_checksums: Path = Path(self.repos.salixos_repo_path, self.repos.salixos_repo_checksums)
         path_changelog: Path = Path(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.salixos_repo_mirror[0]
+        if self.repos.salixos_repo_local[0].startswith('file'):
+            mirror: str = self.repos.salixos_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.salixos_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 deps: list = []
                 required = line.replace(pkg_tag[4], '').strip()
 
                 for req in required.split(','):
                     dep = req.split('|')
                     if len(dep) > 1:
                         deps.append(dep[1])
                     else:
-                        deps += dep
+                        deps.extend(dep)
 
                 cache.append(' '.join(deps))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
@@ -1160,15 +1238,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.salixos_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_salixos_extra_data(self) -> None:
         """ Install the data for salixos_extra repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.salixos_extra_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -1182,63 +1260,66 @@
             'PACKAGE REQUIRED:',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.salixos_extra_repo_path, self.repos.salixos_extra_repo_packages)
         path_checksums: Path = Path(self.repos.salixos_extra_repo_path, self.repos.salixos_extra_repo_checksums)
         path_changelog: Path = Path(self.repos.salixos_extra_repo_path,
                                     self.repos.salixos_extra_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.salixos_extra_repo_mirror[0]
+        if self.repos.salixos_extra_repo_local[0].startswith('file'):
+            mirror: str = self.repos.salixos_extra_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.salixos_extra_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 deps: list = []
                 required = line.replace(pkg_tag[4], '').strip()
 
                 for req in required.split(','):
                     dep = req.split('|')
                     if len(dep) > 1:
                         deps.append(dep[1])
                     else:
-                        deps += dep
+                        deps.extend(dep)
 
                 cache.append(' '.join(deps))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
@@ -1263,15 +1344,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.salixos_extra_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_salixos_patches_data(self) -> None:
         """ Install the data for salixos_patches repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.salixos_patches_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -1285,63 +1366,66 @@
             'PACKAGE REQUIRED:',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.salixos_patches_repo_path, self.repos.salixos_patches_repo_packages)
         path_checksums: Path = Path(self.repos.salixos_patches_repo_path, self.repos.salixos_patches_repo_checksums)
         path_changelog: Path = Path(self.repos.salixos_patches_repo_path,
                                     self.repos.salixos_patches_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.salixos_patches_repo_mirror[0]
+        if self.repos.salixos_patches_repo_local[0].startswith('file'):
+            mirror: str = self.repos.salixos_patches_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.salixos_patches_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 deps: list = []
                 required = line.replace(pkg_tag[4], '').strip()
 
                 for req in required.split(','):
                     dep = req.split('|')
                     if len(dep) > 1:
                         deps.append(dep[1])
                     else:
-                        deps += dep
+                        deps.extend(dep)
 
                 cache.append(' '.join(deps))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
@@ -1366,15 +1450,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.salixos_patches_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_slackel_data(self) -> None:
         """ Install the data for slackel repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slackel_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -1387,63 +1471,66 @@
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
         path_checksums: Path = Path(self.repos.slackel_repo_path, self.repos.slackel_repo_checksums)
         path_changelog: Path = Path(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.slackel_repo_mirror[0]
+        if self.repos.slackel_repo_local[0].startswith('file'):
+            mirror: str = self.repos.slackel_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.slackel_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)
+                cache.append(version)
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 deps: list = []
                 required = line.replace(pkg_tag[4], '').strip()
 
                 for req in required.split(','):
                     dep = req.split('|')
                     if len(dep) > 1:
                         deps.append(dep[1])
                     else:
-                        deps += dep
+                        deps.extend(dep)
 
                 cache.append(' '.join(deps))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
@@ -1468,15 +1555,15 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slackel_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
 
     def install_slint_data(self) -> None:
         """ Install the data for slint repository. """
         print(f"Updating the database for '{self.cyan}{self.repos.slint_repo_name}{self.endc}'... ",
               end='', flush=True)
@@ -1489,63 +1576,66 @@
             'PACKAGE SIZE (uncompressed):',
             'PACKAGE REQUIRED:',
             'PACKAGE DESCRIPTION:'
         ]
         path_packages: Path = Path(self.repos.slint_repo_path, self.repos.slint_repo_packages)
         path_checksums: Path = Path(self.repos.slint_repo_path, self.repos.slint_repo_checksums)
         path_changelog: Path = Path(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
-        packages_txt: list = self.utils.read_file(path_packages)
-        checksums_md5: list = self.utils.read_file(path_checksums)
+        packages_txt: list = self.utils.read_text_file(path_packages)
+        checksums_md5: list = self.utils.read_text_file(path_checksums)
+
+        mirror: str = self.repos.slint_repo_mirror[0]
+        if self.repos.slint_repo_local[0].startswith('file'):
+            mirror: str = self.repos.slint_repo_local[0]
 
         for line in checksums_md5:
             line = line.strip()
 
             if line.endswith(('.txz', '.tgz')):
                 file: str = line.split('./')[1].split('/')[-1].strip()
                 checksum: str = line.split('./')[0].strip()
                 checksums_dict[file] = checksum
 
         cache: list = []  # init cache
 
         for line in packages_txt:
 
             if line.startswith(pkg_tag[0]):
-                package_name = line.replace(pkg_tag[0], '').strip()
-                split_package: list = self.utils.split_binary_pkg(package_name)
-                cache.append(split_package[0])  # package name
-                cache.append(split_package[1])  # package version
-                cache.append(package_name)
-                cache.append(self.repos.slint_repo_mirror[0])
+                package = line.replace(pkg_tag[0], '').strip()
+                name: str = self.utils.split_package(package)['name']
+                version: str = self.utils.split_package(package)['version']
+                cache.append(name)  # package name
+                cache.append(version)  # package version
+                cache.append(package)
+                cache.append(mirror)
                 try:
-                    cache.append(checksums_dict[package_name])
+                    cache.append(checksums_dict[package])
                 except KeyError:
                     cache.append('error checksum')
 
             if line.startswith(pkg_tag[1]):
                 package_location = line.replace(pkg_tag[1], '').strip()
                 cache.append(package_location[2:])  # Do not install (./) dot
 
             if line.startswith(pkg_tag[2]):
-                package_size_comp = line.replace(pkg_tag[2], '').strip()
-                cache.append(f'{package_size_comp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[3]):
-                package_size_uncomp = line.replace(pkg_tag[3], '').strip()
-                cache.append(f'{package_size_uncomp}B')
+                cache.append(''.join(re.findall(r'\d+', line)))
 
             if line.startswith(pkg_tag[4]):
                 deps: list = []
                 required = line.replace(pkg_tag[4], '').strip()
 
                 for req in required.split(','):
                     dep = req.split('|')
                     if len(dep) > 1:
                         deps.append(dep[1])
                     else:
-                        deps += dep
+                        deps.extend(dep)
 
                 cache.append(' '.join(deps))
 
             if line.startswith(pkg_tag[5]):
                 package_description = line.replace(pkg_tag[5], '').strip()
                 cache.append(package_description)
 
@@ -1570,10 +1660,10 @@
 
                 cache: list = []  # reset cache
 
         last_updated: str = self.last_updated(path_changelog)
         date: str = LastRepoUpdated(repo=self.repos.slint_repo_name, date=last_updated)
         self.session.add(date)
 
-        print(f'{self.byellow}Done{self.endc}')
+        print(f'{self.byellow}Done{self.endc}\n')
 
         self.session.commit()
```

### Comparing `slpkg-4.8.2/slpkg/sbos/queries.py` & `slpkg-4.8.3/slpkg/sbos/queries.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,38 +7,42 @@
 from slpkg.models.models import session as Session
 from slpkg.models.models import SBoTable, PonceTable
 
 
 class SBoQueries(Configs):
     """ Queries class for the sbo repository. """
 
-    def __init__(self):
+    def __init__(self, repository: str):
         super(Configs, self).__init__()
         self.session = Session
 
         self.repos = Repositories()
         self.utils = Utilities()
 
-        # Switch between sbo and ponce repository.
-        self.sbo_table = SBoTable
-        if self.repos.ponce_repo:
-            self.sbo_table = PonceTable
+        table: dict = {
+            self.repos.sbo_repo_name: SBoTable,
+            self.repos.ponce_repo_name: PonceTable
+        }
+
+        if repository == '*':
+            repository = self.repos.default_repository
+
+        self.sbo_table: str = table[repository]
 
     def repository_data(self) -> dict:
         """ Returns a dictionary with the repository data. """
         repository_data: tuple = self.session.query(self.sbo_table).all()
 
-        repos_dict: dict = {
-            data.name: (data.location,
-                        data.files,
-                        data.version,
-                        data.download,
-                        data.download64,
-                        data.md5sum,
-                        data.md5sum64,
-                        data.requires,
-                        data.short_description)
+        repos_dict: dict[str] = {
+            data.name: {'location': data.location,
+                        'files': data.files,
+                        'version': data.version,
+                        'download': data.download,
+                        'download64': data.download64,
+                        'md5sum': data.md5sum,
+                        'md5sum64': data.md5sum64,
+                        'requires': data.requires,
+                        'description': data.short_description}
             for data in repository_data
             if not self.utils.blacklist_pattern(data.name)
         }
-
         return repos_dict
```

### Comparing `slpkg-4.8.2/slpkg/sbos/slackbuild.py` & `slpkg-4.8.3/slpkg/sbos/slackbuild.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,152 +1,136 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 import os
 import time
 import shutil
 import logging
-import subprocess
 
 from pathlib import Path
 from collections import OrderedDict
-from multiprocessing import Process, cpu_count
+from multiprocessing import cpu_count
 
 from slpkg.checksum import Md5sum
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
 from slpkg.downloader import Downloader
 from slpkg.error_messages import Errors
 from slpkg.views.views import ViewMessage
-from slpkg.progress_bar import ProgressBar
 from slpkg.logging_deps import LoggingDeps
 from slpkg.repositories import Repositories
+from slpkg.multi_process import MultiProcess
 from slpkg.sbos.dependencies import Requires
 from slpkg.logging_config import LoggingConfig
-from slpkg.models.models import session as Session
 
 
 class Slackbuilds(Configs):
     """ Download build and install the SlackBuilds. """
 
-    def __init__(self, data: dict, slackbuilds: list, flags: list, mode: str):
-        __slots__ = 'data', 'slackbuilds', 'flags', 'mode'
+    def __init__(self, repository: str, data: dict, slackbuilds: list, flags: list, mode: str):
         super(Configs, self).__init__()
-        self.data = data
+        self.repository: str = repository
+        self.data: dict = data
         self.slackbuilds: list = slackbuilds
         self.flags: list = flags
         self.mode: str = mode
 
-        self.session = Session
         self.errors = Errors()
         self.repos = Repositories()
         self.utils = Utilities()
-        self.progress = ProgressBar()
         self.dialogbox = DialogBox()
-        self.logs_deps = LoggingDeps(flags, data)
-        self.upgrade = Upgrade(flags, data)
-        self.view_message = ViewMessage(flags, data)
-
-        self.stderr = None
-        self.stdout = None
-        self.sbos: dict = {}
+        self.multi_proc = MultiProcess(flags)
+        self.logs_deps = LoggingDeps(repository, data)
+        self.upgrade = Upgrade(repository, data)
+        self.view_message = ViewMessage(flags, repository, data)
+        self.check_md5 = Md5sum(self.flags)
+
+        self.sources: dict = {}
         self.install_order: list = []
         self.dependencies: list = []
-        self.process_message: str = ''
+        self.slackware_command: str = str()
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ['-r', '--reinstall'], flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
             ['-k', '--skip-installed'], flags)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-o', '--resolve-off'], flags)
+            ['-O', '--resolve-off'], flags)
 
         self.option_for_jobs: bool = self.utils.is_option(
             ['-j', '--jobs'], flags)
 
-        self.option_for_no_silent: bool = self.utils.is_option(
-            ['-n', '--no-silent'], flags)
-
         self.slackbuilds: list = self.utils.apply_package_pattern(data, slackbuilds)
 
-        # Patch the TAG from configs.
-        if self.repos.patch_repo_tag:
-            self.repos.repo_tag = self.repos.patch_repo_tag
+        # Patch the TAG from configs if changed.
+        self.repo_tag: str = self.repos.repositories[repository]['repo_tag']
+        if self.repos.repositories[repository]['patch_tag']:
+            self.repo_tag: str = self.repos.repositories[repository]['repo_tag']
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
     def execute(self) -> None:
-        """ Starting build or install the slackbuilds. """
-        self.creating_dictionary()
-        self.creating_dependencies_for_build()
-        self.creating_main_for_build()
-        self.view_before_build()
+        self.creating_dependencies_list()
+        self.remove_duplicate_from_dependencies_list()
+        self.choose_package_dependencies()
+        self.add_dependencies_to_install_order()
+        self.clean_the_main_slackbuilds()
+        self.add_main_packages_to_install_order()
+        self.view_slackbuilds_before_build()
 
         start: float = time.time()
         self.prepare_slackbuilds_for_build()
-        self.build_and_install()
+        self.download_the_sources()
+        self.build_and_install_the_slackbuilds()
         elapsed_time: float = time.time() - start
 
         self.utils.finished_time(elapsed_time)
 
-    def creating_dictionary(self) -> None:
-        """ Dictionary with the main slackbuilds and dependencies. """
-        for sbo in self.slackbuilds:
-            if self.option_for_resolve_off:
-                self.sbos[sbo] = []
-            else:
-                self.sbos[sbo] = Requires(self.data, sbo).resolve()
-
-    def creating_dependencies_for_build(self) -> None:
-        """ List with the dependencies. """
-        for deps in self.sbos.values():
-            for dep in deps:
-
-                # Skip installed package when the option --skip-installed is applied.
-                if self.option_for_skip_installed and self.utils.is_package_installed(dep):
-                    continue
+    def creating_dependencies_list(self) -> None:
+        if not self.option_for_resolve_off:
+            for slackbuild in self.slackbuilds:
+                dependencies: tuple = Requires(self.data, slackbuild).resolve()
+
+                for dependency in dependencies:
+                    # Skip installed package when the option --skip-installed is applied.
+                    if self.option_for_skip_installed and self.utils.is_package_installed(dependency):
+                        continue
 
-                self.dependencies.append(dep)
+                    self.dependencies.append(dependency)
 
-        # Remove duplicate packages and keeps the order.
-        dependencies = list(OrderedDict.fromkeys(self.dependencies))
+    def remove_duplicate_from_dependencies_list(self) -> None:
+        self.dependencies: list = list(OrderedDict.fromkeys(self.dependencies))
 
-        if dependencies:
-            self.dependencies: list = self.choose_dependencies(dependencies)
+    def add_dependencies_to_install_order(self) -> None:
+        self.install_order.extend(self.dependencies)
 
-            # Clean up the main packages if they were selected for dependencies.
-            for dep in self.dependencies:
-                if dep in self.slackbuilds:
-                    self.slackbuilds.remove(dep)
+    def clean_the_main_slackbuilds(self) -> None:
+        for dep in self.dependencies:
+            if dep in self.slackbuilds:
+                self.slackbuilds.remove(dep)
 
-        self.install_order.extend(self.dependencies)
+    def add_main_packages_to_install_order(self) -> None:
+        self.install_order.extend(self.slackbuilds)
 
-    def creating_main_for_build(self) -> None:
-        """ List with the main slackbuilds. """
-        [self.install_order.append(main) for main in self.sbos.keys() if main not in self.install_order]
-
-    def view_before_build(self) -> None:
-        """ View slackbuilds before proceed. """
-        if not self.mode == 'build':
-            self.view_message.install_packages(self.slackbuilds, self.dependencies, self.mode)
-        else:
+    def view_slackbuilds_before_build(self) -> None:
+        if self.mode == 'build':
             self.view_message.build_packages(self.slackbuilds, self.dependencies)
-
-        del self.dependencies  # no more needed
+        else:
+            self.view_message.install_upgrade_packages(self.slackbuilds, self.dependencies, self.mode)
 
         self.view_message.question()
 
-    def continue_build_or_install(self, name) -> bool:
+    def continue_build_or_install(self, name: str) -> bool:
         """ Skip installed package when the option --skip-installed is applied
             and continue to install if the package is upgradable or the --reinstall option
             applied.
         """
         if self.mode == 'build':
             return True
 
@@ -158,224 +142,155 @@
 
         if self.utils.is_package_installed(name) and self.option_for_reinstall:
             return True
 
         return False
 
     def prepare_slackbuilds_for_build(self) -> None:
-        """ Downloads files and sources. """
-        sources: dict = {}
-
         for sbo in self.install_order:
             if self.continue_build_or_install(sbo):
-
                 build_path: Path = Path(self.build_path, sbo)
 
                 self.utils.remove_folder_if_exists(build_path)
-                location: str = self.data[sbo][0]
-                slackbuild = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
+                location: str = self.data[sbo]['location']
+                slackbuild: Path = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
 
                 # Copy slackbuilds to the build folder.
-                if self.repos.ponce_repo:
-                    path_ponce_repo_package = Path(self.repos.ponce_repo_path, location, sbo)
-                    shutil.copytree(path_ponce_repo_package, build_path)
-                else:
-                    path_sbo_repo_package = Path(self.repos.sbo_repo_path, location, sbo)
-                    shutil.copytree(path_sbo_repo_package, build_path)
+                path_repo_package: Path = Path(self.repos.repositories[self.repository]['path'], location, sbo)
+                shutil.copytree(path_repo_package, build_path)
 
                 os.chmod(slackbuild, 0o775)
 
-                if self.os_arch == 'x86_64' and self.data[sbo][4]:
-                    sources[sbo] = self.data[sbo][4].split()
+                if self.os_arch == 'x86_64' and self.data[sbo]['download64']:
+                    self.sources[sbo] = self.data[sbo]['download64'].split()
                 else:
-                    sources[sbo] = self.data[sbo][3].split()
+                    self.sources[sbo] = self.data[sbo]['download'].split()
 
-        if sources:
-            for pkg, sbo_sources in sources.items():
-                down_urls = Downloader(Path(self.build_path, pkg), sbo_sources, self.flags)
+    def download_the_sources(self) -> None:
+        if self.sources:
+            for package, sbo_sources in self.sources.items():
+                down_urls = Downloader(Path(self.build_path, package), sbo_sources, self.flags)
                 down_urls.download()
+            print()
 
-            self.checksum_downloads()
-        print()  # New line here.
+            self.checksum_downloaded_sources()
 
-    def checksum_downloads(self) -> None:
-        """ Checking the correct checksums. """
+    def checksum_downloaded_sources(self) -> None:
         for sbo in self.install_order:
-            path = Path(self.build_path, sbo)
+            path: Path = Path(self.build_path, sbo)
 
-            if self.os_arch == 'x86_64' and self.data[sbo][6]:
-                checksums: list = self.data[sbo][6].split()
-                sources: list = self.data[sbo][4].split()
+            if self.os_arch == 'x86_64' and self.data[sbo]['md5sum64']:
+                checksums: list = self.data[sbo]['md5sum64'].split()
+                sources: list = self.data[sbo]['download64'].split()
             else:
-                checksums: list = self.data[sbo][5].split()
-                sources: list = self.data[sbo][3].split()
+                checksums: list = self.data[sbo]['md5sum'].split()
+                sources: list = self.data[sbo]['download'].split()
 
             for source, checksum in zip(sources, checksums):
-                md5sum = Md5sum(self.flags)
-                md5sum.check(path, source, checksum)
+                self.check_md5.md5sum(path, source, checksum)
 
-    def build_and_install(self) -> None:
-        """ Build the slackbuilds and install. """
+    def build_and_install_the_slackbuilds(self) -> None:
         for sbo in self.install_order:
-
             if self.continue_build_or_install(sbo):
-
-                self.patch_sbo_tag(sbo)
-
+                self.patch_slackbuild_tag(sbo)
                 self.build_the_script(self.build_path, sbo)
 
-                if self.mode in ['install', 'upgrade']:
-
-                    pkg: str = self.package_for_install(sbo)
-                    self.install_package(pkg)
+                if self.mode in ('install', 'upgrade'):
+                    self.install_package(sbo)
 
                     if not self.option_for_resolve_off:
                         self.logs_deps.logging(sbo)
             else:
-                package: str = self.utils.is_package_installed(sbo)
-                version: str = self.utils.split_binary_pkg(package)[1]
-                self.view_message.view_skipping_packages(sbo, version)
+                installed_package: str = self.utils.is_package_installed(sbo)
+                installed_version: str = self.utils.split_package(installed_package)['version']
+                self.view_message.view_skipping_packages(sbo, installed_version)
 
-    def patch_sbo_tag(self, sbo: str) -> None:
-        """ Patching SBo TAG from the configuration file. """
+    def patch_slackbuild_tag(self, sbo: str) -> None:
         sbo_script: Path = Path(self.build_path, sbo, f'{sbo}.SlackBuild')
-
-        if sbo_script.is_file() and self.repos.patch_repo_tag:
-
-            lines: list = self.utils.read_file(sbo_script)
+        if sbo_script.is_file() and self.repo_tag:
+            lines: list = self.utils.read_text_file(sbo_script)
 
             with open(sbo_script, 'w') as script:
                 for line in lines:
                     if line.startswith('TAG=$'):
-                        line: str = f'TAG=${{TAG:-{self.repos.patch_repo_tag}}}\n'
+                        line: str = f'TAG=${{TAG:-{self.repo_tag}}}\n'
                     script.write(line)
 
-    def install_package(self, package: str) -> None:
-        """ Install the packages that before created in the tmp directory. """
-        pkg: str = self.utils.split_binary_pkg(package)[0]
-
-        execute: str = self.installpkg
-        if self.option_for_reinstall and self.utils.is_package_installed(pkg):
-            execute: str = self.reinstall
+    def install_package(self, name: str) -> None:
+        package: str = self.find_package_for_install(name)
+        self.set_slackware_command(name)
 
-        message: str = f'{self.cyan}Installing{self.endc}'
-        self.process_message: str = f"package '{pkg}' to install"
+        progress_message: str = f'{self.cyan}Installing{self.endc}'
+        process_message: str = f"package '{name}' to install"
 
         if self.mode == 'upgrade':
-            self.process_message: str = f"package '{pkg}' to upgrade"
-            message: str = f'{self.cyan}Upgrade{self.endc}'
+            progress_message: str = f'{self.cyan}Upgrading{self.endc}'
+            process_message: str = f"package '{name}' to upgrade"
 
-        command: str = f'{execute} {self.tmp_path}/{package}'
+        command: str = f'{self.slackware_command} {self.tmp_path}/{package}'
 
-        self.multi_process(command, package, message)
+        self.multi_proc.process(command, package, process_message, progress_message)
 
-    def package_for_install(self, name: str) -> str:
-        """ Returns the package for install. """
-        package: str = ''
-        version: str = self.data[name][2]
-        pattern: str = f'{name}-{version}*{self.repos.repo_tag}*'
+    def set_slackware_command(self, name: str) -> None:
+        self.slackware_command: str = self.installpkg
+        if self.option_for_reinstall and self.utils.is_package_installed(name):
+            self.slackware_command: str = self.reinstall
 
+    def find_package_for_install(self, name: str) -> str:
+        version: str = self.data[name]['version']
+        pattern: str = f'{name}-{version}*{self.repo_tag}*'
         packages: list = [file.name for file in self.tmp_path.glob(pattern)]
-
         try:
-            package: str = max(packages)
+            return max(packages)
         except ValueError:
-            logger = logging.getLogger(LoggingConfig.date)
+            logger = logging.getLogger(LoggingConfig.date_time)
             logger.exception(f'{self.__class__.__name__}: '
-                             f'{self.__class__.package_for_install.__name__}')
+                             f'{self.__class__.find_package_for_install.__name__}')
             self.errors.raise_error_message(f"Package '{name}' not found for install", exit_status=20)
 
-        return package
-
     def build_the_script(self, path: Path, name: str) -> None:
-        """ Run the .SlackBuild script. """
-        folder: str = f'{Path(path, name)}/'
-        execute: str = f'{folder}./{name}.SlackBuild'
-
-        # Change to root privileges
-        os.chown(folder, 0, 0)
-        for file in os.listdir(folder):
-            os.chown(f'{folder}{file}', 0, 0)
-
-        if self.option_for_jobs:
-            self.set_makeflags()
-
-        name: str = f'{name}.SlackBuild'
-        message: str = f'{self.red}Build{self.endc}'
-        self.process_message: str = f"package '{name}' to build"
-
-        self.multi_process(execute, name, message)
-
-    @staticmethod
-    def set_makeflags() -> None:
-        """ Set number of processors. """
-        os.environ['MAKEFLAGS'] = f'-j {cpu_count()}'
-
-    def multi_process(self, command: str, filename: str, message: str) -> None:
-        """ Starting multiprocessing install/upgrade process. """
-        if self.silent_mode and not self.option_for_no_silent:
-
-            done: str = f' {self.byellow} Done{self.endc}'
-            self.stderr = subprocess.DEVNULL
-            self.stdout = subprocess.DEVNULL
-
-            # Starting multiprocessing
-            p1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
-            p2 = Process(target=self.progress.bar, args=(f'{self.bold}{message}:', filename))
+        self.set_makeflags()
+        folder: Path = Path(path, name)
+        filename: str = f'{name}.SlackBuild'
+        command: str = f'{folder}/./{filename}'
 
-            p1.start()
-            p2.start()
+        self.utils.change_owner_privileges(folder)
 
-            # Wait until process 1 finish
-            p1.join()
+        progress_message: str = f'{self.red}Build{self.endc}'
+        process_message: str = f"package '{name}' to build"
 
-            # Terminate process 2 if process 1 finished
-            if not p1.is_alive():
+        self.multi_proc.process(command, filename, process_message, progress_message)
 
-                if p1.exitcode != 0:
-                    done: str = f'{self.bred}Failed: {self.endc}{self.process_message}.'
-
-                p2.terminate()
-                print(f'{self.endc}{done}', end='')
-
-            # Wait until process 2 finish
-            p2.join()
-
-            # Restore the terminal cursor
-            print('\x1b[?25h', self.endc)
-        else:
-            self.utils.process(command, self.stderr, self.stdout)
-
-    def choose_dependencies(self, dependencies: list) -> list:
-        """ Choose packages for install. """
-        height: int = 10
-        width: int = 70
-        list_height: int = 0
-        choices: list = []
-        title: str = ' Choose dependencies you want to install '
-
-        for package in dependencies:
-            status: bool = True
-
-            repo_ver: str = self.data[package][2]
-            description: str = self.data[package][8]
-            help_text: str = f'Description: {description}'
-            installed: str = self.utils.is_package_installed(package)
+    def set_makeflags(self) -> None:
+        if self.option_for_jobs:
+            os.environ['MAKEFLAGS'] = f'-j {cpu_count()}'
 
-            if installed:
-                status: bool = False
+    def choose_package_dependencies(self) -> None:
+        if self.dependencies:
+            height: int = 10
+            width: int = 70
+            list_height: int = 0
+            choices: list = []
+            title: str = ' Choose dependencies you want to install '
 
-            if self.option_for_reinstall:
+            for package in self.dependencies:
                 status: bool = True
+                repo_ver: str = self.data[package]['version']
+                description: str = self.data[package]['description']
+                help_text: str = f'Description: {description}'
+                installed: str = self.utils.is_package_installed(package)
+
+                if installed:
+                    status: bool = False
+
+                if self.option_for_reinstall:
+                    status: bool = True
+
+                choices.extend(
+                    [(package, repo_ver, status, help_text)]
+                )
+            text: str = f'There are {len(choices)} dependencies:'
 
-            choices += [(package, repo_ver, status, help_text)]
-
-        text: str = f'There are {len(choices)} dependencies:'
-
-        code, tags = self.dialogbox.checklist(text, dependencies, title, height,
-                                              width, list_height, choices)
-        if not code:
-            return dependencies
-
-        os.system('clear')
+            code, self.dependencies = self.dialogbox.checklist(
+                text, self.dependencies, title, height, width, list_height, choices)
 
-        return tags
+            os.system('clear')
```

### Comparing `slpkg-4.8.2/slpkg/update_repository.py` & `slpkg-4.8.3/slpkg/update_repository.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,67 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-import os
 from pathlib import Path
 from multiprocessing import Process, Queue
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
 from slpkg.progress_bar import ProgressBar
 from slpkg.install_data import InstallData
 from slpkg.repositories import Repositories
 from slpkg.check_updates import CheckUpdates
+from slpkg.sbos.sbo_generate import SBoGenerate
 from slpkg.models.models import session as Session
 from slpkg.models.models import (SBoTable, PonceTable,
                                  BinariesTable, LastRepoUpdated)
 
 
 class UpdateRepository(Configs):
-    """ Deletes and install the data. """
+    """ Updates the local repositories and install the data
+        into the database.
+    """
 
-    def __init__(self, flags: list, repo: str):
-        __slots__ = 'flags', 'repo'
+    def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
         self.flags: list = flags
-        self.repo: str = repo
+        self.repository: str = repository
 
         self.session = Session
         self.view = ViewMessage(flags)
         self.repos = Repositories()
         self.progress = ProgressBar()
         self.utils = Utilities()
         self.data = InstallData()
-
-        self.check_updates = CheckUpdates(flags, repo)
+        self.generate = SBoGenerate()
+        self.check_updates = CheckUpdates(flags, repository)
 
         self.repos_for_update: dict = {}
 
-        self.option_for_generate: bool = self.utils.is_option(
-            ['-G', '--generate-only'], flags)
+        self.is_binary: bool = self.utils.is_binary_repo(repository)
+
+        self.option_for_repository: bool = self.utils.is_option(
+            ['-o', '--repository='], flags)
 
-        self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], flags)
+        self.option_for_install_data: bool = self.utils.is_option(
+            ['-a', '--install-data'], flags)
 
     def update_the_repositories(self) -> None:
-        if not any(list(self.repos_for_update.values())) or self.repo == '*':
+        if not any(list(self.repos_for_update.values())):
             self.view.question()
+            for repo in self.repos_for_update:
+                self.repos_for_update[repo] = True
         else:
             print()
 
-        bin_repositories: dict = {
+        repositories: dict = {
+            self.repos.sbo_repo_name: self.sbo_repository,
+            self.repos.ponce_repo_name: self.ponce_repository,
             self.repos.slack_repo_name: self.slack_repository,
             self.repos.slack_extra_repo_name: self.slack_extra_repository,
             self.repos.slack_patches_repo_name: self.slack_patches_repository,
             self.repos.alien_repo_name: self.alien_repository,
             self.repos.multilib_repo_name: self.multilib_repository,
             self.repos.restricted_repo_name: self.restricted_repository,
             self.repos.gnome_repo_name: self.gnome_repository,
@@ -65,506 +72,555 @@
             self.repos.salixos_repo_name: self.salixos_repository,
             self.repos.salixos_extra_repo_name: self.salixos_extra_repository,
             self.repos.salixos_patches_repo_name: self.salixos_patches_repository,
             self.repos.slackel_repo_name: self.slackel_repository,
             self.repos.slint_repo_name: self.slint_repository
         }
 
-        if self.option_for_binaries:
-
-            for repo in bin_repositories.keys():
-                if self.repos.repositories[repo][0]:
-
-                    if repo == self.repo:
-                        bin_repositories[repo]()
-                        break
-
-                    if self.repo == '*':
-                        bin_repositories[repo]()
+        if self.option_for_repository:
+            print(f"Downloading the '{self.green}{self.repository}{self.endc}' repository "
+                  f"in the '{self.repos.repositories[self.repository]['path']}' folder, please wait...\n")
+            repositories[self.repository]()
         else:
-            self.slackbuild_repositories()
+            for repo, value in self.repos_for_update.items():
+                if value:
+                    print(f"Downloading the '{self.green}{repo}{self.endc}' repository "
+                          f"in the '{self.repos.repositories[repo]['path']}' folder, please wait...\n")
+                    repositories[repo]()
         print()
 
     def slack_repository(self):
-        if not self.repos.slack_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.slack_repo_name}{self.endc}"
-                  f"' repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.slack_repo_path)
 
-            urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}')
-            urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}')
-            urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}')
-
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slack_repo_path, self.repos.slack_repo_checksums)
 
-            down = Downloader(self.repos.slack_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if self.repos.slack_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {self.repos.slack_repo_mirror[0]} '
+                    f'{self.repos.slack_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_changelog}')
+                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_packages}')
+                urls.append(f'{self.repos.slack_repo_mirror[0]}{self.repos.slack_repo_checksums}')
+
+                down = Downloader(self.repos.slack_repo_path, urls, self.flags)
+                down.download()
+                print()
 
         self.delete_bin_database_data(self.repos.slack_repo_name)
         self.delete_last_updated(self.repos.slack_repo_name)
         self.data.install_slack_data()
-        print()
 
     def slack_extra_repository(self):
-        if not self.repos.slack_extra_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.slack_extra_repo_name}{self.endc}"
-                  f"' repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.slack_extra_repo_path)
 
-            urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}')
+            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path, self.repos.slack_extra_repo_checksums)
+
             urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_changelog}')
-            urls.append(f'{self.repos.slack_extra_repo_mirror[0]}{self.repos.slack_extra_repo_checksums}')
 
-            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                             self.repos.slack_extra_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                             self.repos.slack_extra_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.slack_extra_repo_path,
-                                             self.repos.slack_extra_repo_checksums)
+            if self.repos.slack_extra_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.slack_extra_repo_mirror)} '
+                    f'{self.repos.slack_extra_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_packages}')
+                urls.append(f'{"".join(self.repos.slack_extra_repo_mirror)}{self.repos.slack_extra_repo_checksums}')
 
             down = Downloader(self.repos.slack_extra_repo_path, urls, self.flags)
             down.download()
             print()
 
         self.delete_bin_database_data(self.repos.slack_extra_repo_name)
         self.delete_last_updated(self.repos.slack_extra_repo_name)
         self.data.install_slack_extra_data()
-        print()
 
     def slack_patches_repository(self):
-        if not self.repos.slack_patches_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.slack_patches_repo_name}{self.endc}"
-                  f"' repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.slack_patches_repo_path)
 
-            urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_packages}')
-            urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}')
-            urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
-                                             self.repos.slack_patches_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
+                                             self.repos.slack_patches_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.slack_patches_repo_path,
                                              self.repos.slack_patches_repo_checksums)
 
+            urls.append(f'{self.repos.slack_patches_repo_mirror[0]}{self.repos.slack_patches_repo_changelog}')
+
+            if self.repos.slack_patches_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.slack_patches_repo_mirror)} '
+                    f'{self.repos.slack_patches_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_packages}')
+                urls.append(f'{"".join(self.repos.slack_patches_repo_mirror)}{self.repos.slack_patches_repo_checksums}')
+
             down = Downloader(self.repos.slack_patches_repo_path, urls, self.flags)
             down.download()
             print()
 
         self.delete_bin_database_data(self.repos.slack_patches_repo_name)
         self.delete_last_updated(self.repos.slack_patches_repo_name)
         self.data.install_slack_patches_data()
-        print()
 
     def alien_repository(self):
-        if not self.repos.alien_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.alien_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.alien_repo_path)
 
-            urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}')
-            urls.append(f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}')
-            urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_packages)
             self.utils.remove_file_if_exists(self.repos.alien_repo_path, self.repos.alien_repo_checksums)
 
+            urls.append(f'{self.repos.alien_repo_mirror[0]}{self.repos.alien_repo_changelog}')
+
+            if self.repos.alien_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.alien_repo_mirror)} '
+                    f'{self.repos.alien_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_packages}')
+                urls.append(f'{"".join(self.repos.alien_repo_mirror)}{self.repos.alien_repo_checksums}')
+
             down = Downloader(self.repos.alien_repo_path, urls, self.flags)
             down.download()
             print()
 
         self.delete_bin_database_data(self.repos.alien_repo_name)
         self.delete_last_updated(self.repos.alien_repo_name)
         self.data.install_alien_data()
-        print()
 
     def multilib_repository(self) -> None:
-        if not self.repos.multilib_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.multilib_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.multilib_repo_path)
 
-            urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}')
-            urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}')
-            urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_packages)
             self.utils.remove_file_if_exists(self.repos.multilib_repo_path, self.repos.multilib_repo_checksums)
 
+            urls.append(f'{self.repos.multilib_repo_mirror[0]}{self.repos.multilib_repo_changelog}')
+
+            if self.repos.multilib_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.multilib_repo_mirror)} '
+                    f'{self.repos.multilib_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_packages}')
+                urls.append(f'{"".join(self.repos.multilib_repo_mirror)}{self.repos.multilib_repo_checksums}')
+
             down = Downloader(self.repos.multilib_repo_path, urls, self.flags)
             down.download()
             print()
 
         self.delete_bin_database_data(self.repos.multilib_repo_name)
         self.delete_last_updated(self.repos.multilib_repo_name)
         self.data.install_multilib_data()
-        print()
 
     def restricted_repository(self) -> None:
-        if not self.repos.restricted_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.restricted_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.restricted_repo_path)
 
-            urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}')
-            urls.append(f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}')
-            urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_packages)
             self.utils.remove_file_if_exists(self.repos.restricted_repo_path, self.repos.restricted_repo_checksums)
 
+            urls.append(f'{self.repos.restricted_repo_mirror[0]}{self.repos.restricted_repo_changelog}')
+
+            if self.repos.restricted_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.restricted_repo_mirror)} '
+                    f'{self.repos.restricted_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_packages}')
+                urls.append(f'{"".join(self.repos.restricted_repo_mirror)}{self.repos.restricted_repo_checksums}')
+
             down = Downloader(self.repos.restricted_repo_path, urls, self.flags)
             down.download()
             print()
 
         self.delete_bin_database_data(self.repos.restricted_repo_name)
         self.delete_last_updated(self.repos.restricted_repo_name)
         self.data.install_restricted_data()
-        print()
 
     def gnome_repository(self) -> None:
-        if not self.repos.gnome_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.gnome_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.gnome_repo_path)
 
-            urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}')
-            urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}')
-            urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
             self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_packages)
             self.utils.remove_file_if_exists(self.repos.gnome_repo_path, self.repos.gnome_repo_checksums)
 
-            down = Downloader(self.repos.gnome_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if self.repos.gnome_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {self.repos.gnome_repo_mirror[0]} '
+                    f'{self.repos.gnome_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_changelog}')
+                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_packages}')
+                urls.append(f'{self.repos.gnome_repo_mirror[0]}{self.repos.gnome_repo_checksums}')
+
+                down = Downloader(self.repos.gnome_repo_path, urls, self.flags)
+                down.download()
+                print()
 
         self.delete_bin_database_data(self.repos.gnome_repo_name)
         self.delete_last_updated(self.repos.gnome_repo_name)
         self.data.install_gnome_data()
-        print()
 
     def msb_repository(self) -> None:
-        if not self.repos.msb_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.msb_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.msb_repo_path)
 
-            urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}')
+            self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.msb_repo_path, self.repos.msb_repo_checksums)
+
             urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_changelog}')
-            urls.append(f'{self.repos.msb_repo_mirror[0]}{self.repos.msb_repo_checksums}')
 
-            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                             self.repos.msb_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                             self.repos.msb_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.msb_repo_path,
-                                             self.repos.msb_repo_checksums)
+            if self.repos.msb_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.msb_repo_mirror)} '
+                    f'{self.repos.msb_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_packages}')
+                urls.append(f'{"".join(self.repos.msb_repo_mirror)}{self.repos.msb_repo_checksums}')
 
             down = Downloader(self.repos.msb_repo_path, urls, self.flags)
             down.download()
             print()
 
         self.delete_bin_database_data(self.repos.msb_repo_name)
         self.delete_last_updated(self.repos.msb_repo_name)
         self.data.install_msb_data()
-        print()
 
     def csb_repository(self) -> None:
-        if not self.repos.csb_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.csb_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.csb_repo_path)
 
-            urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}')
-            urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_changelog}')
-            urls.append(f'{self.repos.csb_repo_mirror[0]}{self.repos.csb_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                             self.repos.csb_repo_packages)
-            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                             self.repos.csb_repo_changelog)
-            self.utils.remove_file_if_exists(self.repos.csb_repo_path,
-                                             self.repos.csb_repo_checksums)
-
-            down = Downloader(self.repos.csb_repo_path, urls, self.flags)
-            down.download()
-            print()
+            self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.csb_repo_path, self.repos.csb_repo_checksums)
+
+            if self.repos.csb_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.csb_repo_mirror)} '
+                    f'{self.repos.csb_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_changelog}')
+                urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_packages}')
+                urls.append(f'{"".join(self.repos.csb_repo_mirror)}{self.repos.csb_repo_checksums}')
+
+                down = Downloader(self.repos.csb_repo_path, urls, self.flags)
+                down.download()
+                print()
 
         self.delete_bin_database_data(self.repos.csb_repo_name)
         self.delete_last_updated(self.repos.csb_repo_name)
         self.data.install_csb_data()
-        print()
 
     def conraid_repository(self) -> None:
-        if not self.repos.conraid_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.conraid_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.conraid_repo_path)
 
-            urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}')
-            urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}')
-            urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
             self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_packages)
             self.utils.remove_file_if_exists(self.repos.conraid_repo_path, self.repos.conraid_repo_checksums)
 
-            down = Downloader(self.repos.conraid_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if self.repos.conraid_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {self.repos.conraid_repo_mirror[0]} '
+                    f'{self.repos.conraid_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_changelog}')
+                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_packages}')
+                urls.append(f'{self.repos.conraid_repo_mirror[0]}{self.repos.conraid_repo_checksums}')
+
+                down = Downloader(self.repos.conraid_repo_path, urls, self.flags)
+                down.download()
+                print()
 
         self.delete_bin_database_data(self.repos.conraid_repo_name)
         self.delete_last_updated(self.repos.conraid_repo_name)
         self.data.install_conraid_data()
-        print()
 
     def slackonly_repository(self) -> None:
-        if not self.repos.slackonly_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.slackonly_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.slackonly_repo_path)
 
-            urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}')
-            urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}')
-            urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slackonly_repo_path, self.repos.slackonly_repo_checksums)
 
-            down = Downloader(self.repos.slackonly_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if self.repos.slackonly_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {self.repos.slackonly_repo_mirror[0]} '
+                    f'{self.repos.slackonly_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_changelog}')
+                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_packages}')
+                urls.append(f'{self.repos.slackonly_repo_mirror[0]}{self.repos.slackonly_repo_checksums}')
+
+                down = Downloader(self.repos.slackonly_repo_path, urls, self.flags)
+                down.download()
+                print()
 
         self.delete_bin_database_data(self.repos.slackonly_repo_name)
         self.delete_last_updated(self.repos.slackonly_repo_name)
         self.data.install_slackonly_data()
-        print()
 
     def salixos_repository(self) -> None:
-        if not self.repos.salixos_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.salixos_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.salixos_repo_path)
 
-            urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}')
-            urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}')
-            urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_repo_path, self.repos.salixos_repo_checksums)
 
-            down = Downloader(self.repos.salixos_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if self.repos.salixos_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {self.repos.salixos_repo_mirror[0]} '
+                    f'{self.repos.salixos_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_changelog}')
+                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_packages}')
+                urls.append(f'{self.repos.salixos_repo_mirror[0]}{self.repos.salixos_repo_checksums}')
+
+                down = Downloader(self.repos.salixos_repo_path, urls, self.flags)
+                down.download()
+                print()
 
         self.delete_bin_database_data(self.repos.salixos_repo_name)
         self.delete_last_updated(self.repos.salixos_repo_name)
         self.data.install_salixos_data()
-        print()
 
     def salixos_extra_repository(self) -> None:
-        if not self.repos.salixos_extra_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.salixos_extra_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.salixos_extra_repo_path)
 
-            urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_packages}')
-            urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}')
-            urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
-                                             self.repos.salixos_extra_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
                                              self.repos.salixos_extra_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
+                                             self.repos.salixos_extra_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.salixos_extra_repo_path,
                                              self.repos.salixos_extra_repo_checksums)
 
+            urls.append(f'{self.repos.salixos_extra_repo_mirror[0]}{self.repos.salixos_extra_repo_changelog}')
+
+            if self.repos.salixos_extra_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.salixos_extra_repo_mirror)} '
+                    f'{self.repos.salixos_extra_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_packages}')
+                urls.append(f'{"".join(self.repos.salixos_extra_repo_mirror)}{self.repos.salixos_extra_repo_checksums}')
+
             down = Downloader(self.repos.salixos_extra_repo_path, urls, self.flags)
             down.download()
-            print()
 
         self.delete_bin_database_data(self.repos.salixos_extra_repo_name)
         self.delete_last_updated(self.repos.salixos_extra_repo_name)
         self.data.install_salixos_extra_data()
-        print()
 
     def salixos_patches_repository(self) -> None:
-        if not self.repos.salixos_patches_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.salixos_patches_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.slack_patches_repo_path)
 
-            urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
-                        f'{self.repos.salixos_patches_repo_packages}')
-            urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}')
-            urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
-                                             self.repos.salixos_patches_repo_packages)
             self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
                                              self.repos.salixos_patches_repo_changelog)
             self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
+                                             self.repos.salixos_patches_repo_packages)
+            self.utils.remove_file_if_exists(self.repos.salixos_patches_repo_path,
                                              self.repos.salixos_patches_repo_checksums)
 
+            urls.append(f'{self.repos.salixos_patches_repo_mirror[0]}{self.repos.salixos_patches_repo_changelog}')
+
+            if self.repos.salixos_patches_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {"".join(self.repos.salixos_patches_repo_mirror)} '
+                    f'{self.repos.salixos_patches_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
+                            f'{self.repos.salixos_patches_repo_packages}')
+                urls.append(f'{"".join(self.repos.salixos_patches_repo_mirror)}'
+                            f'{self.repos.salixos_patches_repo_checksums}')
+
             down = Downloader(self.repos.salixos_patches_repo_path, urls, self.flags)
             down.download()
             print()
 
         self.delete_bin_database_data(self.repos.salixos_patches_repo_name)
         self.delete_last_updated(self.repos.salixos_patches_repo_name)
         self.data.install_salixos_patches_data()
-        print()
 
     def slackel_repository(self) -> None:
-        if not self.repos.slackel_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.slackel_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.slackel_repo_path)
 
-            urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}')
-            urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}')
-            urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slackel_repo_path, self.repos.slackel_repo_checksums)
 
-            down = Downloader(self.repos.slackel_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if self.repos.slackel_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {self.repos.slackel_repo_mirror[0]} '
+                    f'{self.repos.slackel_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_changelog}')
+                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_packages}')
+                urls.append(f'{self.repos.slackel_repo_mirror[0]}{self.repos.slackel_repo_checksums}')
+
+                down = Downloader(self.repos.slackel_repo_path, urls, self.flags)
+                down.download()
+                print()
 
         self.delete_bin_database_data(self.repos.slackel_repo_name)
         self.delete_last_updated(self.repos.slackel_repo_name)
         self.data.install_slackel_data()
-        print()
 
     def slint_repository(self) -> None:
-        if not self.repos.slint_repo_mirror[0].startswith('file'):
-            print(f"Downloading the '{self.green}{self.repos.slint_repo_name}{self.endc}' "
-                  f"repository, please wait...\n")
+        if not self.option_for_install_data:
             urls: list = []
             self.utils.create_directory(self.repos.slint_repo_path)
 
-            urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}')
-            urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}')
-            urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}')
-
-            self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_changelog)
+            self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_packages)
             self.utils.remove_file_if_exists(self.repos.slint_repo_path, self.repos.slint_repo_checksums)
 
-            down = Downloader(self.repos.slint_repo_path, urls, self.flags)
-            down.download()
-            print()
+            if self.repos.slint_repo_local[0].startswith('file'):
+                lftp_command: str = (
+                    f'lftp {self.lftp_mirror_options} {self.repos.slint_repo_mirror[0]} '
+                    f'{self.repos.slint_repo_path}'
+                )
+                self.utils.process(lftp_command)
+            else:
+                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_changelog}')
+                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_packages}')
+                urls.append(f'{self.repos.slint_repo_mirror[0]}{self.repos.slint_repo_checksums}')
+
+                down = Downloader(self.repos.slint_repo_path, urls, self.flags)
+                down.download()
+                print()
 
         self.delete_bin_database_data(self.repos.slint_repo_name)
         self.delete_last_updated(self.repos.slint_repo_name)
         self.data.install_slint_data()
-        print()
 
-    def slackbuild_repositories(self) -> None:
+    def ponce_repository(self) -> None:
         """ Update the slackbuild repositories. """
-        if self.repos.ponce_repo:
+        if not self.option_for_install_data:
+            self.utils.create_directory(self.repos.ponce_repo_path)
+            self.utils.remove_file_if_exists(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
+            self.utils.remove_file_if_exists(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
 
-            if not self.option_for_generate or self.repos.ponce_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.ponce_repo_name}"
-                      f"{self.endc}' repository, please wait...\n")
+            lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.ponce_repo_mirror[0]} '
+                                 f'{self.repos.ponce_repo_path}')
 
-                self.utils.create_directory(self.repos.ponce_repo_path)
-                self.utils.remove_file_if_exists(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
+            self.utils.process(lftp_command)
 
-                lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.ponce_repo_mirror[0]} '
-                                     f'{self.repos.ponce_repo_path}')
+        # It checks if there is the SLACKBUILDS.TXT file, otherwise going to create it.
+        if not Path(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds).is_file():
+            self.generate.slackbuild_file(self.repos.ponce_repo_path, self.repos.ponce_repo_slackbuilds)
 
-                self.utils.process(lftp_command)
+        self.delete_last_updated(self.repos.ponce_repo_name)
+        self.delete_ponce_database_data()
+        self.data.install_ponce_data()
 
-            gen_script: Path = Path(self.repos.ponce_repo_path, 'gen_sbo_txt.sh')
-            if not gen_script.is_file():
-                with open(gen_script, 'w') as file:
-                    file.write(self.__class__.gen_sbo_script.__doc__)
+    def sbo_repository(self) -> None:
+        if not self.option_for_install_data:
+            self.utils.create_directory(self.repos.sbo_repo_path)
+            self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
+            self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
 
-                os.chmod(gen_script, 0o775)
+            lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.sbo_repo_mirror[0]} '
+                                 f'{self.repos.sbo_repo_path}')
 
-            # Generating the ponce SLACKBUILDS.TXT file.
-            print(f'Generating the {self.repos.ponce_repo_slackbuilds} file... ', end='', flush=True)
-            os.chdir(self.repos.ponce_repo_path)
-            gen_command: str = f'./gen_sbo_txt.sh > {self.repos.ponce_repo_slackbuilds}'
+            self.utils.process(lftp_command)
 
-            self.utils.process(gen_command)
-            self.delete_last_updated(self.repos.ponce_repo_name)
-            print('\n')
-
-        else:
-
-            if not self.repos.sbo_repo_mirror[0].startswith('file'):
-                print(f"Downloading the '{self.green}{self.repos.sbo_repo_name}{self.endc}' "
-                      f"repository, please wait...\n")
-
-                self.utils.create_directory(self.repos.sbo_repo_path)
-
-                self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
-                self.utils.remove_file_if_exists(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
-
-                lftp_command: str = (f'lftp {self.lftp_mirror_options} {self.repos.sbo_repo_mirror[0]} '
-                                     f'{self.repos.sbo_repo_path}')
-
-                self.utils.process(lftp_command)
-            self.delete_last_updated(self.repos.sbo_repo_name)
+        # It checks if there is the SLACKBUILDS.TXT file, otherwise going to create it.
+        if not Path(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds).is_file():
+            self.generate.slackbuild_file(self.repos.sbo_repo_path, self.repos.sbo_repo_slackbuilds)
 
+        self.delete_last_updated(self.repos.sbo_repo_name)
         self.delete_sbo_database_data()
-        self.data.install_sbos_data()
+        self.data.install_sbo_data()
 
-    def check(self, queue) -> None:
-        compare: dict = self.check_updates.check()
+    def check_for_updates(self, queue) -> None:
+        compare: dict = self.check_updates.check_the_repositories()
+        self.print_the_messages(compare)
 
+        return queue.put(compare)
+
+    def print_the_messages(self, compare: dict) -> None:
         print()
         for repo, comp in compare.items():
             if comp:
                 print(f"\n{self.endc}There are new updates available for the "
                       f"'{self.bgreen}{repo}{self.endc}' repository!")
 
         if not any(list(compare.values())):
             print(f'\n{self.endc}{self.yellow}No changes in ChangeLog.txt between your '
                   f'last update and now.{self.endc}')
 
-        return queue.put(compare)
-
     def repositories(self) -> None:
         queue = Queue()
         message = f'Checking for news, please wait...'
 
         # Starting multiprocessing
-        p1 = Process(target=self.check, args=(queue,))
-        p2 = Process(target=self.progress.bar, args=(message, ''))
+        p1 = Process(target=self.check_for_updates, args=(queue,))
+        p2 = Process(target=self.progress.progress_bar, args=(message, ''))
 
         p1.start()
         p2.start()
 
         # Wait until process 1 finish
         p1.join()
 
@@ -579,50 +635,71 @@
         print('\x1b[?25h', self.endc, end='')
 
         self.repos_for_update: dict = queue.get()
         self.update_the_repositories()
 
     def delete_sbo_database_data(self) -> None:
         """ Delete all the data from a table of the database. """
-        if self.repos.ponce_repo:
-            self.session.query(PonceTable).delete()
-        else:
-            self.session.query(SBoTable).delete()
+        self.session.query(SBoTable).delete()
         self.session.commit()
 
-    def delete_bin_database_data(self, repo) -> None:
+    def delete_ponce_database_data(self) -> None:
+        self.session.query(PonceTable).delete()
+        self.session.commit()
+
+    def delete_bin_database_data(self, repo: str) -> None:
         """ Delete the repository data from a table of the database. """
         self.session.query(BinariesTable).where(BinariesTable.repo == repo).delete()
         self.session.commit()
 
-    def delete_last_updated(self, repo) -> None:
+    def delete_last_updated(self, repo: str) -> None:
         """ Deletes the last updated date. """
         self.session.query(LastRepoUpdated).where(LastRepoUpdated.repo == repo).delete()
         self.session.commit()
 
-    def gen_sbo_script(self):
-        """#!/bin/bash
-
-# gen_sbo_txt.sh is a script to build a SLACKBUILDS.TXT file.
-# Thanks to bassmadrigal from LQ forum.
-# https://www.linuxquestions.org/questions/slackware-14/script-for-building-a-slackbuilds-txt-4175598436/
-
-for i in */*; do
-
-  NAME=$(echo $i | cut -d "/" -f2)
-  FILES=$(ls $i)
-  source $i/${NAME}.info
-  DESCRIPTION=$(grep -m 1 $NAME $i/slack-desc | cut -d " " -f2-)
-
-  echo SLACKBUILD NAME: $NAME
-  echo SLACKBUILD LOCATION: ./$i
-  echo SLACKBUILD FILES: $FILES
-  echo SLACKBUILD VERSION: $VERSION
-  echo SLACKBUILD DOWNLOAD: $DOWNLOAD
-  echo SLACKBUILD DOWNLOAD_x86_64: $DOWNLOAD_x86_64
-  echo SLACKBUILD MD5SUM: $MD5SUM
-  echo SLACKBUILD MD5SUM_x86_64: $MD5SUM_x86_64
-  echo SLACKBUILD REQUIRES: $REQUIRES
-  echo SLACKBUILD SHORT DESCRIPTION: $DESCRIPTION
-  echo
-
-done"""
+#     def generate_the_slackbuilds_txt(self, path: Path, slackbuilds_txt: str) -> None:
+#         """ Generates the SLACKBUILDS.TXT file. """
+#
+#         sbo_txt: Path = Path(path, slackbuilds_txt)
+#         gen_script: Path = Path(path, 'gen_sbo_txt.sh')
+#
+#         if not sbo_txt.is_file():
+#
+#             if not gen_script.is_file():
+#                 with open(gen_script, 'w') as file:
+#                     file.write(self.__class__.gen_sbo_script.__doc__)
+#                 os.chmod(gen_script, 0o775)
+#
+#             # Generating the SLACKBUILDS.TXT file.
+#             print(f'Generating the {slackbuilds_txt} file... ', end='', flush=True)
+#             os.chdir(path)
+#             self.utils.process(f'./gen_sbo_txt.sh > {slackbuilds_txt}')
+#
+#             print(f'{self.byellow}Done{self.endc}\n')
+#
+#     def gen_sbo_script(self) -> None:
+#         """#!/bin/bash
+#
+# # gen_sbo_txt.sh is a script to build a SLACKBUILDS.TXT file.
+# # Thanks to bassmadrigal from LQ forum.
+# # https://www.linuxquestions.org/questions/slackware-14/script-for-building-a-slackbuilds-txt-4175598436/
+#
+# for i in */*; do
+#
+#   NAME=$(echo $i | cut -d "/" -f2)
+#   FILES=$(ls $i)
+#   source $i/${NAME}.info
+#   DESCRIPTION=$(grep -m 1 $NAME $i/slack-desc | cut -d " " -f2-)
+#
+#   echo SLACKBUILD NAME: $NAME
+#   echo SLACKBUILD LOCATION: ./$i
+#   echo SLACKBUILD FILES: $FILES
+#   echo SLACKBUILD VERSION: $VERSION
+#   echo SLACKBUILD DOWNLOAD: $DOWNLOAD
+#   echo SLACKBUILD DOWNLOAD_x86_64: $DOWNLOAD_x86_64
+#   echo SLACKBUILD MD5SUM: $MD5SUM
+#   echo SLACKBUILD MD5SUM_x86_64: $MD5SUM_x86_64
+#   echo SLACKBUILD REQUIRES: $REQUIRES
+#   echo SLACKBUILD SHORT DESCRIPTION: $DESCRIPTION
+#   echo
+#
+# done"""
```

### Comparing `slpkg-4.8.2/slpkg/progress_bar.py` & `slpkg-4.8.3/slpkg/progress_bar.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,46 +8,63 @@
 from slpkg.configs import Configs
 
 
 class ProgressBar(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
+        self.spinner = PixelSpinner
+        self.color: str = self.endc
+        self.spinners: dict = {}
+        self.spinners_color: dict = {}
 
-    def bar(self, message: str, filename: str) -> None:
+    def progress_bar(self, message: str, filename: str) -> None:
         """ Creating progress bar. """
-        spinners: dict = {
+        self.assign_spinners()
+        self.assign_spinner_colors()
+        self.set_spinner()
+        self.set_color()
+
+        if self.spinning_bar:
+            bar_spinner = self.spinner(f'{self.endc}{message} {filename} {self.color}')
+            # print('\033[F', end='', flush=True)
+            try:
+                while True:
+                    time.sleep(0.1)
+                    bar_spinner.next()
+            except KeyboardInterrupt:
+                raise SystemExit(1)
+        else:
+            print(f'{message} ', end='', flush=True)
+
+    def assign_spinners(self) -> None:
+        self.spinners: dict[str] = {
             'pixel': PixelSpinner,
             'line': LineSpinner,
             'moon': MoonSpinner,
             'pie': PieSpinner,
             'spinner': Spinner
         }
-        colors: dict = {
+
+    def assign_spinner_colors(self) -> None:
+        self.spinners_color: dict[str] = {
             'green': self.green,
             'violet': self.violet,
             'yellow': self.yellow,
             'blue': self.blue,
             'cyan': self.cyan,
             'grey': self.grey,
             'red': self.red,
             '': self.endc
         }
 
+    def set_spinner(self) -> None:
         try:
-            spinner = spinners[self.progress_spinner]
-            color: str = colors[self.spinner_color]
+            self.spinner = self.spinners[self.progress_spinner]
         except KeyError:
-            spinner = PixelSpinner
-            color: str = self.endc
+            self.spinner = PixelSpinner
 
-        if self.spinning_bar:
-            bar_spinner = spinner(f'{self.endc}{message} {filename} {color}')
-            # print('\033[F', end='', flush=True)
-            try:
-                while True:
-                    time.sleep(0.1)
-                    bar_spinner.next()
-            except KeyboardInterrupt:
-                raise SystemExit(1)
-        else:
-            print(f'{message} ', end='', flush=True)
+    def set_color(self) -> None:
+        try:
+            self.color: str = self.spinners_color[self.spinner_color]
+        except KeyError:
+            self.color: str = self.endc
```

### Comparing `slpkg-4.8.2/slpkg/downloader.py` & `slpkg-4.8.3/slpkg/downloader.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,65 +11,78 @@
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 
 
 class Downloader(Configs):
 
     def __init__(self, path: Union[str, Path], urls: list, flags: list):
-        __slots__ = 'path', 'urls', 'flags'
         super(Configs, self).__init__()
         self.path: Path = path
         self.urls: list = urls
         self.flags: list = flags
 
         self.errors = Errors()
         self.utils = Utilities()
 
+        self.filename = None
+        self.downloader_command: str = str()
+        self.downloader_tools: dict = {
+            'wget': self.wget_downloader,
+            'wget2': self.wget_downloader,
+            'curl': self.curl_downloader,
+            'lftp': self.lftp_downloader
+        }
         self.option_for_parallel: bool = self.utils.is_option(
             ['-P', '--parallel'], flags)
 
     def download(self) -> None:
         """ Starting the processing for downloading. """
         process: list = []
 
         if self.parallel_downloads or self.option_for_parallel:
             for url in self.urls:
-                p1 = Process(target=self.tool, args=(url,))
+                p1 = Process(target=self.tools, args=(url,))
                 process.append(p1)
                 p1.start()
 
             for proc in process:
                 proc.join()
         else:
             for url in self.urls:
-                self.tool(url)
+                self.tools(url)
 
-    def tool(self, url: str) -> None:
-        """ Downloader tools wget, wget2, curl and lftp. """
-        command: str = ''
+    def tools(self, url: str) -> None:
         path: str = urlparse(url).path
-        filename: str = unquote(Path(path).name)
+        self.filename: str = unquote(Path(path).name)
 
         if url.startswith('file'):
-            shutil.copy2(url[7:], self.tmp_slpkg)
+            self.copy_local_binary_file(url)
         else:
-            if self.downloader in ['wget', 'wget2']:
-                command: str = f'{self.downloader} {self.wget_options} --directory-prefix={self.path} "{url}"'
-
-            elif self.downloader == 'curl':
-                command: str = f'{self.downloader} {self.curl_options} "{url}" --output {self.path}/{filename}'
-
-            elif self.downloader == 'lftp':
-                command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {self.path}'
-
-            else:
+            try:
+                self.downloader_tools[self.downloader](url)
+            except KeyError:
                 self.errors.raise_error_message(f"Downloader '{self.downloader}' not supported", exit_status=1)
 
-        self.utils.process(command)
-        self.check_if_downloaded(url, filename)
+            self.utils.process(self.downloader_command)
+            self.check_if_downloaded(url)
+
+    def copy_local_binary_file(self, url: str) -> None:
+        try:
+            shutil.copy2(Path(url.replace('file:', '')), self.tmp_slpkg)
+            print(f"{self.byellow}Copying{self.endc}: {Path(url.replace('file:', ''))} -> {self.tmp_slpkg}")
+        except FileNotFoundError as error:
+            self.errors.raise_error_message(f'{error}', 1)
+
+    def wget_downloader(self, url: str) -> None:
+        self.downloader_command: str = f'{self.downloader} {self.wget_options} --directory-prefix={self.path} "{url}"'
+
+    def curl_downloader(self, url: str) -> None:
+        self.downloader_command: str = (f'{self.downloader} {self.curl_options} "{url}" '
+                                        f'--output {self.path}/{self.filename}')
 
-    def check_if_downloaded(self, url: str, filename: str) -> None:
-        """ Checks if the file downloaded. """
-        path_file: Path = Path(self.path, filename)
+    def lftp_downloader(self, url: str) -> None:
+        self.downloader_command: str = f'{self.downloader} {self.lftp_get_options} {url} -o {self.path}'
 
+    def check_if_downloaded(self, url: str) -> None:
+        path_file: Path = Path(self.path, self.filename)
         if not path_file.exists():
-            self.errors.raise_error_message(f"Download the '{url}' file", exit_status=20)
+            self.errors.raise_error_message(f"Download the '{url}'", exit_status=20)
```

### Comparing `slpkg-4.8.2/slpkg/models/models.py` & `slpkg-4.8.3/slpkg/models/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import create_engine, Column, Integer, Text
 
 from slpkg.configs import Configs
 
 
 DATABASE_URI: str = os.path.join(f'sqlite:///{Configs.db_path}', Configs.database_name)
-
 engine = create_engine(DATABASE_URI)
-
 session = sessionmaker(engine)()
 Base = declarative_base()
 
 
 @dataclass
 class SBoTable(Base):
     """ The main table for the SBo repository. """
@@ -36,17 +34,17 @@
     md5sum64: str = Column(Text)
     requires: str = Column(Text)
     short_description: str = Column(Text)
 
 
 @dataclass
 class PonceTable(Base):
-    """ The main table for the SBo repository. """
+    """ The main table for the ponce repository. """
 
-    __tablename__ = 'poncetable'
+    __tablename__: str = 'poncetable'
 
     id: int = Column(Integer, primary_key=True)
     name: str = Column(Text)
     location: str = Column(Text)
     files: str = Column(Text)
     version: str = Column(Text)
     download: str = Column(Text)
@@ -55,17 +53,17 @@
     md5sum64: str = Column(Text)
     requires: str = Column(Text)
     short_description: str = Column(Text)
 
 
 @dataclass
 class BinariesTable(Base):
-    """ The main table for the SBo repository. """
+    """ The main table for the binary repositories. """
 
-    __tablename__ = 'binariestable'
+    __tablename__: str = 'binariestable'
 
     id: int = Column(Integer, primary_key=True)
     repo: str = Column(Text)
     name: str = Column(Text)
     version: str = Column(Text)
     package: str = Column(Text)
     mirror: str = Column(Text)
@@ -79,26 +77,26 @@
     checksum: str = Column(Text)
 
 
 @dataclass
 class LogsDependencies(Base):
     """ The table that stores the dependencies after installing a package. """
 
-    __tablename__ = 'logsdependencies'
+    __tablename__: str = 'logsdependencies'
 
     id: int = Column(Integer, primary_key=True)    
     name: str = Column(Text)    
     requires: str = Column(Text)    
 
 
 @dataclass
 class LastRepoUpdated(Base):
     """ The table that saves the last updated date. """
 
-    __tablename__ = 'lastupdated'
+    __tablename__: str = 'lastupdated'
 
     id: int = Column(Integer, primary_key=True)
     repo: str = Column(Text)
     date: str = Column(Text)
 
 
 Base.metadata.create_all(engine)
```

### Comparing `slpkg-4.8.2/slpkg/views/version.py` & `slpkg-4.8.3/slpkg/views/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 2)
+        self.version_info: tuple = (4, 8, 3)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.2/slpkg/views/cli_menu.py` & `slpkg-4.8.3/slpkg/views/cli_menu.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,22 +25,22 @@
     def help_short(self, status: int) -> NoReturn:
         """ Prints the short menu. """
         args: str = (
             f'USAGE: {self.prog_name} [{self.cyan}COMMAND{self.endc}] [{self.yellow}OPTIONS{self.endc}] '
             f'[FILELIST|PACKAGES...]\n'
             f'\n  slpkg [{self.cyan}COMMAND{self.endc}] [-u, update, -U, upgrade, -c, check-updates, -I, repo-info]\n'
             f'  slpkg [{self.cyan}COMMAND{self.endc}] [-g, configs, -L, clean-logs, -T, clean-data, -D, clean-tmp]\n'
-            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-b, build, -i, install, -R, remove [packages...]]\n'
-            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-d, download, -f, find, -w, view [packages...]]\n'
-            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-s, search, -e, dependees, -t, tracking  [packages...]]\n'
-            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-y, --yes, -j, --jobs, -o, --resolve-off, -r, --reinstall]\n'
-            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-k, --skip-installed, -E, --full-reverse, -S, --search]\n'
-            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-n, --no-silent, -p, --pkg-version, -G, --generate-only]\n'
-            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-P, --parallel, -B, --bin-repo=[REPO]]\n'
-            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-z, --directory=[PATH]]\n'
+            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-b, build, -i, install, -R, remove [PACKAGES...]]\n'
+            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-d, download, -f, find, -w, view [PACKAGES...]]\n'
+            f'  slpkg [{self.cyan}COMMAND{self.endc}] [-s, search, -e, dependees, -t, tracking  [PACKAGES...]]\n'
+            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-y, --yes, -j, --jobs, -O, --resolve-off, -r, --reinstall]\n'
+            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-k, --skip-installed, -a, --install-data]\n'
+            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-E, --full-reverse, -S, --search, -n, --no-silent]\n'
+            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-p, --pkg-version, -P, --parallel]\n'
+            f'  slpkg [{self.yellow}OPTIONS{self.endc}] [-o, --repository=NAME, -z, --directory=PATH]\n'
             "  \nIf you need more information please try 'slpkg --help'.")
 
         print(args)
         raise SystemExit(status)
 
     def help(self, status: int) -> NoReturn:
         """ Prints the main menu. """
@@ -54,38 +54,38 @@
             f'  {self.cyan}-U, upgrade{self.endc}                   Upgrade all the packages.\n'
             f'  {self.cyan}-c, check-updates{self.endc}             Check for news on ChangeLog.txt.\n'
             f'  {self.cyan}-I, repo-info{self.endc}                 Prints the repositories information.\n'
             f'  {self.cyan}-g, configs{self.endc}                   Edit the configuration file.\n'
             f'  {self.cyan}-L, clean-logs{self.endc}                Clean dependencies log tracking.\n'
             f'  {self.cyan}-T, clean-data{self.endc}                Clean all the repositories data.\n'
             f'  {self.cyan}-D, clean-tmp{self.endc}                 Delete all the downloaded sources.\n'
-            f'  {self.cyan}-b, build{self.endc} [packages...]       Build only the packages.\n'
-            f'  {self.cyan}-i, install{self.endc} [packages...]     Build and install the packages.\n'
-            f'  {self.cyan}-R, remove{self.endc} [packages...]      Remove installed packages.\n'
-            f'  {self.cyan}-d, download{self.endc} [packages...]    Download only the scripts and sources.\n'
-            f'  {self.cyan}-f, find{self.endc} [packages...]        Find installed packages.\n'
-            f'  {self.cyan}-w, view{self.endc} [packages...]        View packages from the repository.\n'
-            f'  {self.cyan}-s, search{self.endc} [packages...]      Search packages from the repository.\n'
-            f'  {self.cyan}-e, dependees{self.endc} [packages...]   Show which packages depend on.\n'
-            f'  {self.cyan}-t, tracking{self.endc} [packages...]    Tracking the packages dependencies.\n'
+            f'  {self.cyan}-b, build{self.endc} [PACKAGES...]       Build only the packages.\n'
+            f'  {self.cyan}-i, install{self.endc} [PACKAGES...]     Build and install the packages.\n'
+            f'  {self.cyan}-R, remove{self.endc} [PACKAGES...]      Remove installed packages.\n'
+            f'  {self.cyan}-d, download{self.endc} [PACKAGES...]    Download only the scripts and sources.\n'
+            f'  {self.cyan}-f, find{self.endc} [PACKAGES...]        Find installed packages.\n'
+            f'  {self.cyan}-w, view{self.endc} [PACKAGES...]        View packages from the repository.\n'
+            f'  {self.cyan}-s, search{self.endc} [PACKAGES...]      Search packages from the repository.\n'
+            f'  {self.cyan}-e, dependees{self.endc} [PACKAGES...]   Show which packages depend on.\n'
+            f'  {self.cyan}-t, tracking{self.endc} [PACKAGES...]    Tracking the packages dependencies.\n'
             f'\n{self.bold}OPTIONS:{self.endc}\n'
             f'  {self.yellow}-y, --yes{self.endc}                     Answer Yes to all questions.\n'
             f'  {self.yellow}-j, --jobs{self.endc}                    Set it for multicore systems.\n'
-            f'  {self.yellow}-o, --resolve-off{self.endc}             Turns off dependency resolving.\n'
+            f'  {self.yellow}-O, --resolve-off{self.endc}             Turns off dependency resolving.\n'
             f'  {self.yellow}-r, --reinstall{self.endc}               Upgrade packages of the same version.\n'
             f'  {self.yellow}-k, --skip-installed{self.endc}          Skip installed packages.\n'
+            f'  {self.yellow}-a, --install-data{self.endc}            Install data into the database only.\n'
             f'  {self.yellow}-E, --full-reverse{self.endc}            Full reverse dependency.\n'
             f'  {self.yellow}-S, --search{self.endc}                  Search packages from the repository.\n'
             f'  {self.yellow}-n, --no-silent{self.endc}               Disable silent mode.\n'
             f'  {self.yellow}-p, --pkg-version{self.endc}             Print the repository package version.\n'
-            f'  {self.yellow}-G, --generate-only{self.endc}           Generates only the SLACKBUILDS.TXT file.\n'
             f'  {self.yellow}-P, --parallel{self.endc}                Download files in parallel.\n'
-            f'  {self.yellow}-B, --bin-repo={self.endc}[REPO]         Set a binary repository.\n'
-            f'  {self.yellow}-z, --directory={self.endc}[PATH]        Download files to a specific path.\n'
+            f'  {self.yellow}-o, --repository={self.endc}NAME         Change repository you want to work.\n'
+            f'  {self.yellow}-z, --directory={self.endc}PATH          Download files to a specific path.\n'
             '\n  -h, --help                    Show this message and exit.\n'
             '  -v, --version                 Print version and exit.\n'
             "\nIf you need more information try to use slpkg manpage.\n"
-            "Extra help for the commands, use: 'slpkg help [command]'.\n"
+            "Extra help for the commands, use: 'slpkg help [COMMAND]'.\n"
             "Edit the config file in the /etc/slpkg/slpkg.toml or 'slpkg configs'.")
 
         print(args)
         raise SystemExit(status)
```

### Comparing `slpkg-4.8.2/slpkg/views/ascii.py` & `slpkg-4.8.3/slpkg/views/asciibox.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 # -*- coding: utf-8 -*-
 
 import shutil
 
 from slpkg.configs import Configs
 
 
-class Ascii(Configs):
-    """ ascii characters. """
+class AsciiBox(Configs):
+
     def __init__(self):
         super(Configs, self).__init__()
         self.columns, self.rows = shutil.get_terminal_size()
+        self.package_alignment: int = self.columns - 61
+        self.version_alignment: int = 29
+        self.size_alignment: int = 14
+        self.repo_alignment: int = 14
+
+        if self.package_alignment < 1:
+            self.package_alignment = 1
 
         self.vertical_line: str = '|'
         self.horizontal_line: str = '='
         self.horizontal_vertical: str = '+'
         self.upper_right_corner: str = '+'
         self.lower_left_corner: str = '+'
         self.lower_right_corner: str = '+'
@@ -33,76 +40,57 @@
             self.lower_right_corner: str = '┘'
             self.upper_left_corner: str = '┌'
             self.horizontal_and_up: str = '┴'
             self.horizontal_and_down: str = '┬'
             self.vertical_and_right: str = '├'
             self.vertical_and_left: str = '┤'
 
-    def draw_package_title_box(self, message: str, title: str) -> None:
-        """ Drawing package title box. """
+    def draw_package_title(self, message: str, title: str) -> None:
         title = title.title()
-        middle_title: int = int((self.columns / 2) - len(title) + 10)
-
-        print(f'{self.bgreen}{self.upper_left_corner}' + f'{self.horizontal_line}' * (self.columns - 2) +
-              f'{self.upper_right_corner}')
-
-        print(f'{self.vertical_line}' + ' ' * middle_title + f'{title}' + ' ' *
-              (self.columns - middle_title - len(title) - 2) + f'{self.vertical_line}')
-
+        print(f"{self.bgreen}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
+              f"{self.upper_right_corner}")
+        print(f"{self.vertical_line}{title.center(self.columns - 2, ' ')}{self.vertical_line}")
         self.draw_middle_line()
-
-        print(f'{self.vertical_line}{self.endc} {message}' + ' ' * (self.columns - len(message) - 3) +
-              f'{self.bgreen}{self.vertical_line}')
-
+        print(f"{self.vertical_line} {self.endc}{message.ljust(self.columns - 3, ' ')}"
+              f"{self.bgreen}{self.vertical_line}")
         self.draw_middle_line()
-
-        print(f'{self.bgreen}{self.vertical_line}{self.endc} Package:' + ' ' * 22 + 'Version:' +
-              ' ' * (self.columns - 66) + 'Size:' + ' ' * 14 + f'Repo:{self.bgreen} {self.vertical_line}{self.endc}')
-
-    def draw_view_package(self, package: str, version: str, size: str, color: str, repo: str) -> None:
-        """ Draw nad print the packages. """
-        if len(version) >= 11 and self.columns <= 80:
-            version: str = f'{version[:10]}...'
-        if len(package) >= 25:
-            package: str = f'{package[:24]}...'
-        print(f'{self.bgreen}{self.vertical_line} {self.bold}{color}{package}{self.endc}' + ' ' * (30 - len(package)) +
-              f'{self.bgreen}{version}' + ' ' * ((self.columns - 53) - len(version) - len(size)) +
-              f'{self.endc}{size}' + ' ' * (19 - len(repo)) +
-              f'{self.blue}{repo} {self.bgreen}{self.vertical_line}{self.endc}')
-
-    def draw_log_package(self, package: str) -> None:
-        """ Drawing and print logs packages. """
-        print(f'  {self.lower_left_corner}{self.horizontal_line}{self.cyan} {package}{self.endc}\n')
+        print(f"{self.bgreen}{self.vertical_line}{self.endc} {'Package:':<{self.package_alignment}}"
+              f"{'Version:':<{self.version_alignment}}{'Size:':<{self.size_alignment}}{'Repo:':>{self.repo_alignment}} "
+              f"{self.bgreen}{self.vertical_line}{self.endc}")
+
+    def draw_package_line(self, package: str, version: str, size: str, color: str, repo: str) -> None:
+        if len(version) >= 20 and self.columns <= 80:
+            version: str = f'{version[:self.version_alignment - 5]}...'
+        if len(package) >= 15 and self.columns <= 80:
+            package: str = f'{package[:self.package_alignment - 5]}...'
+        print(f"{self.bgreen}{self.vertical_line} {self.bold}{color}{package:<{self.package_alignment}}{self.endc}"
+              f"{self.bgreen}{version:<{self.version_alignment}}{self.endc}{size:<{self.size_alignment}}{self.blue}"
+              f"{repo:>{self.repo_alignment}}{self.bgreen} {self.vertical_line}{self.endc}")
 
     def draw_middle_line(self) -> None:
-        """ Drawing a middle line. """
-        print(f'{self.bgreen}{self.vertical_and_right}' + f'{self.horizontal_line}' *
-              (self.columns - 2) + f'{self.vertical_and_left}')
+        print(f"{self.bgreen}{self.vertical_and_right}{self.horizontal_line * (self.columns - 2)}"
+              f"{self.vertical_and_left}")
 
     def draw_dependency_line(self) -> None:
-        """ Drawing  the dependencies line. """
-        print(f'{self.bgreen}{self.vertical_line}{self.endc} Dependencies:' + ' ' * (self.columns - 16) +
-              f'{self.bgreen}{self.vertical_line}{self.endc}')
+        print(f"{self.bgreen}{self.vertical_line}{self.endc} Dependencies:{' ' * (self.columns - 16)}"
+              f"{self.bgreen}{self.vertical_line}{self.endc}")
 
     def draw_bottom_line(self) -> None:
-        """ Drawing the bottom line. """
-        print(f'{self.bold}{self.green}{self.lower_left_corner}' + f'{self.horizontal_line}' *
-              (self.columns - 2) + f'{self.lower_right_corner}{self.endc}')
+        print(f"{self.bold}{self.green}{self.lower_left_corner}{self.horizontal_line * (self.columns - 2)}"
+              f"{self.lower_right_corner}{self.endc}")
 
     def draw_checksum_error_box(self, name: str, checksum: str, file_check: str) -> None:
-        """ Drawing checksum error box. """
-        print('\n' + self.bred + self.upper_left_corner + self.horizontal_line * (self.columns - 2) +
-              self.upper_right_corner)
-
-        print(f"{self.bred}{self.vertical_line}{self.bred} Error:{self.endc} MD5SUM check for "
-              f"'{self.cyan}{name}'{self.red} FAILED!" + ' ' * (self.columns - (len(name)) - 37) + self.vertical_line)
+        print(f"{self.bred}{self.upper_left_corner}{self.horizontal_line * (self.columns - 2)}"
+              f"{self.upper_right_corner}")
+        print(f"{self.bred}{self.vertical_line}{self.bred} FAILED:{self.endc} MD5SUM check for "
+              f"'{self.cyan}{name}'{' ' * (self.columns - len(name) - 30)}{self.red}{self.vertical_line}")
+        print(f"{self.bred}{self.vertical_and_right}{self.horizontal_line * (self.columns - 2)}"
+              f"{self.vertical_and_left}")
+        print(f"{self.bred}{self.vertical_line}{self.yellow} Expected:{self.endc} {checksum}{self.bred}"
+              f"{' ' * (self.columns - (len(checksum)) - 13)}{self.vertical_line}")
+        print(f"{self.bred}{self.vertical_line}{self.violet} Found:{self.endc} {file_check}{self.bred}"
+              f"{' ' * (self.columns - (len(file_check)) - 10)}{self.vertical_line}")
+        print(f"{self.bred}{self.lower_left_corner}{self.horizontal_line * (self.columns - 2)}"
+              f"{self.lower_right_corner}{self.endc}")
 
-        print(self.bred + self.vertical_and_right + self.horizontal_line * (self.columns - 2) + self.vertical_and_left)
-
-        print(f'{self.bred}{self.vertical_line}{self.yellow} Expected:{self.endc} {checksum}{self.bred}'
-              + ' ' * (self.columns - (len(checksum)) - 13) + self.vertical_line)
-
-        print(f'{self.bred}{self.vertical_line}{self.violet} Found:{self.endc} {file_check}{self.bred}'
-              + ' ' * (self.columns - (len(file_check)) - 10) + self.vertical_line)
-
-        print(self.bred + self.lower_left_corner + self.horizontal_line * (self.columns - 2) +
-              self.lower_right_corner + self.endc)
+    def draw_log_package(self, package: str) -> None:
+        print(f"{'':>2}{self.lower_left_corner}{self.horizontal_line}{self.cyan} {package}{self.endc}\n")
```

### Comparing `slpkg-4.8.2/slpkg/views/help_commands.py` & `slpkg-4.8.3/slpkg/views/help_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from slpkg.configs import Configs
 
 
 class Help(Configs):
 
     def __init__(self, command: str, flags: list):
-        __slots__ = 'command', 'flags'
         super(Configs, self).__init__()
         self.command: str = command
         self.flags: list = flags
 
     def view(self) -> None:
         self.flags.reverse()  # Put first the short options.
 
@@ -20,29 +19,29 @@
             'upgrade': "Upgrade all the installed packages if the newer version exists in the repository.",
             'check-updates': "Check if there is any news on the repositories ChangeLog.txt file.",
             'repo-info': "View information related to repositories, such as which repositories are active, "
                          "when they were upgraded, and how many packages they contain.",
             'configs': "Edit the configuration '/etc/slpkg/slpkg.toml' file.",
             'clean-logs': "Cleans dependencies log tracking. After that procedure you should remove dependencies "
                           "by hand.",
-            'clean-tmp': "Deletes all the downloaded SlackBuilds scripts and sources.",
+            'clean-tmp': "Deletes all the downloaded SlackBuilds scripts, packages and sources from the /tmp folder.",
             'clean-data': "Sometimes is necessary to clean all the data from the database. Run this command to drop "
                           "all the tables from the database and run 'slpkg update' to recreate.",
             'build': "Builds the Slackbuilds scripts and adds them to the /tmp directory.",
             'install': "Builds and installs the packages in the correct order, and also logs the packages with the "
                        "dependencies for removal.",
             'download': "Download the SlackBuilds scripts and the sources without building or installing it.",
             'remove': "Removes packages with dependencies if the packages was installed with 'slpkg install' method. "
                       "Slpkg looks at the 'REPO_TAG' configuration to find packages for removal by default, except "
                       "if you are using '--file-pattern=' option.",
             'find': "Find your installed packages on your system.",
             'view': "View information packages from the repository and get everything in your terminal.",
             'search': "Search and match packages from the repository.",
             'dependees': "Show which packages depend on.",
-            'tracking': "Tracking the packages dependencies."
+            'tracking': "Tracking the package dependencies."
         }
 
         help_commands['-u'] = help_commands['update']
         help_commands['-U'] = help_commands['upgrade']
         help_commands['-c'] = help_commands['check-updates']
         help_commands['-I'] = help_commands['repo-info']
         help_commands['-g'] = help_commands['configs']
```

### Comparing `slpkg-4.8.2/slpkg/views/views.py` & `slpkg-4.8.3/slpkg/views/views.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,283 +1,242 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-import os
 import re
 from typing import Any
 from pathlib import Path
 
 from slpkg.configs import Configs
 from slpkg.upgrade import Upgrade
-from slpkg.views.ascii import Ascii
 from slpkg.utilities import Utilities
 from slpkg.dialog_box import DialogBox
-from slpkg.repositories import Repositories
-from slpkg.models.models import LogsDependencies
-from slpkg.models.models import session as Session
+from slpkg.views.asciibox import AsciiBox
 
 
 class ViewMessage(Configs):
 
-    def __init__(self, flags: list, data=None):
-        __slots__ = 'flags', 'data'
+    def __init__(self, flags: list, repository=None, data=None):
         super(Configs, self).__init__()
         self.flags: list = flags
+        self.repository = repository
         self.data: dict = data
 
-        self.session = Session
         self.utils = Utilities()
         self.dialogbox = DialogBox()
-        self.ascii = Ascii()
-        self.upgrade = Upgrade(flags, data)
-        self.repos = Repositories()
+        self.ascii = AsciiBox()
+        self.upgrade = Upgrade(repository, data)
 
-        self.download_only: Path = self.tmp_slpkg
-        self.installed_packages: list = []
+        self.download_only = None
+        self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
-            ['-o', '--resolve-off'], flags)
+            ['-O', '--resolve-off'], flags)
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ['-r', '--reinstall'], flags)
 
         self.option_for_yes: bool = self.utils.is_option(
             ['-y', '--yes'], flags)
 
-        self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], flags)
-
-        self.repo: str = self.utils.repository_name(data)
-
-    def view_packages(self, package: str, mode: str) -> None:
-        """ Printing the main packages. """
-        size: str = ''
-        color: str = self.red
-
-        if self.option_for_binaries:
-            version: str = self.data[package][0]
-            size: str = self.utils.convert_file_sizes(
-                int(''.join(re.findall(r'\d+', self.data[package][4])))
-            )
-        else:
-            version: str = self.data[package][2]
-
-        if mode in ['install', 'download']:
-            color: str = self.cyan
-        if mode == 'build':
-            color: str = self.yellow
-        if mode == 'upgrade':
-            color: str = self.violet
-
-        # If the package is installed and change the color to gray.
-        if package in self.utils.installed_packages.keys() and mode == 'install':
-            color: str = self.grey
-
-        if self.upgrade.is_package_upgradeable(package) and mode == 'install':
-            color: str = self.violet
-
-        if (package in self.utils.installed_packages.keys() and mode == 'install'
-                and self.option_for_reinstall):
-            color: str = self.violet
-
-        self.ascii.draw_view_package(package, version, size, color, self.repo)
-
-    def view_skipping_packages(self, package: str, version: str) -> None:
-        """ Print the skipping packages. """
-        print(f'{self.yellow}Skipping{self.endc}: {package}-{version} {self.red}(already installed){self.endc}')
-
     def build_packages(self, slackbuilds: list, dependencies: list) -> None:
-        """ View packages for build only. """
-        self.ascii.draw_package_title_box('The following packages will be build:', 'slpkg build packages')
+        mode: str = 'build'
+        self.ascii.draw_package_title('The following packages will be build:',
+                                      'slpkg build packages')
 
-        for sbo in slackbuilds:
-            self.view_packages(sbo, mode='build')
+        for slackbuild in slackbuilds:
+            self.view_build_package(slackbuild)
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
-            for sbo in dependencies:
-                self.view_packages(sbo, mode='build')
-
-        self.summary(slackbuilds, dependencies, option='build')
+            for dependency in dependencies:
+                self.view_build_package(dependency)
 
-    def install_packages(self, packages: list, dependencies: list, mode: str) -> None:
-        """ View packages for install. """
-        if dependencies is None:
-            dependencies: list = []
+        self.view_summary(slackbuilds, dependencies, option=mode)
 
+    def install_upgrade_packages(self, packages: list, dependencies: list, mode: str) -> None:
         title: str = 'slpkg install packages'
         if mode == 'upgrade':
             title: str = 'slpkg upgrade packages'
+        self.ascii.draw_package_title('The following packages will be installed or upgraded:', title)
 
-        self.ascii.draw_package_title_box('The following packages will be installed or upgraded:', title)
-
-        for pkg in packages:
-            self.view_packages(pkg, mode)
+        for package in packages:
+            self.view_install_upgrade_package(package)
 
         if dependencies:
             self.ascii.draw_middle_line()
             self.ascii.draw_dependency_line()
 
-            for pkg in dependencies:
-                self.view_packages(pkg, mode)
+            for dependency in dependencies:
+                self.view_install_upgrade_package(dependency)
 
-        self.summary(packages, dependencies, option=mode)
+        self.view_summary(packages, dependencies, option=mode)
 
-    def download_packages(self, slackbuilds: list, directory: Path) -> None:
-        """ View downloaded packages. """
-        mode = 'download'
+    def download_packages(self, packages: list, directory: Path) -> None:
+        mode: str = 'download'
+        self.download_only: Path = directory
+        self.ascii.draw_package_title('The following packages will be downloaded:',
+                                      'slpkg download packages')
+
+        for package in packages:
+            self.view_download_package(package)
+
+        self.view_summary(packages, dependencies=[], option=mode)
+
+    def remove_packages(self, packages: list, dependencies: list) -> Any:
+        mode: str = 'remove'
+        self.ascii.draw_package_title('The following packages will be removed:',
+                                      'slpkg remove packages')
+        for package in packages:
+            self.view_remove_package(package)
 
-        self.ascii.draw_package_title_box('The following packages will be downloaded:', 'slpkg download packages')
+        if dependencies:
+            self.ascii.draw_middle_line()
+            self.ascii.draw_dependency_line()
 
-        if directory:
-            self.download_only: Path = directory
+            for dependency in dependencies:
+                self.view_remove_package(dependency)
 
-        for sbo in slackbuilds:
-            self.view_packages(sbo, mode)
+        self.view_summary(packages, dependencies, option=mode)
 
-        self.summary(slackbuilds, dependencies=[], option='download')
+    def view_build_package(self, package: str) -> None:
+        size: str = str()
+        color: str = self.yellow
+        version: str = self.data[package]['version']
 
-    def remove_packages(self, packages: list) -> Any:
-        """ View remove packages. """
-        pkgs, dependencies = [], []
+        if self.is_binary:
+            # size: str = self.utils.convert_file_sizes(int(self.data[package][4])) <- It's going to replace with this
+            size: str = self.utils.convert_file_sizes(
+                int(''.join(re.findall(r'\d+', self.data[package]['size_comp']))))
 
-        for pkg in packages:
-            pkgs.append(pkg)
+        self.ascii.draw_package_line(package, version, size, color, self.repository)
+
+    def view_install_upgrade_package(self, package: str) -> None:
+        size: str = str()
+        color: str = self.cyan
+        version: str = self.data[package]['version']
+        installed: str = self.utils.is_package_installed(package)
+        upgradable: bool = self.upgrade.is_package_upgradeable(package)
 
-            requires = self.session.query(
-                LogsDependencies.requires).filter(
-                    LogsDependencies.name == pkg).first()
+        if self.is_binary:
+            # size: str = self.utils.convert_file_sizes(int(self.data[package][4])) <- It's going to replace with this
+            size: str = self.utils.convert_file_sizes(
+                int(''.join(re.findall(r'\d+', self.data[package]['size_comp']))))
 
-            if requires:
-                dependencies += requires[0].split()
+        if installed:
+            color: str = self.grey
 
-        if dependencies and not self.option_for_resolve_off:
-            dependencies: list = self.choose_dependencies_for_remove(list(set(dependencies)))
+        if upgradable:
+            color: str = self.violet
+            package: str = self.build_package_and_version(package)
 
-        self.ascii.draw_package_title_box('The following packages will be removed:', 'slpkg remove packages')
+        if installed and self.option_for_reinstall and not upgradable:
+            color: str = self.violet
+            package: str = self.build_package_and_version(package)
 
-        for pkg in pkgs:
-            if pkg not in dependencies:
-                self._view_removed(pkg)
+        self.ascii.draw_package_line(package, version, size, color, self.repository)
 
-        if dependencies and not self.option_for_resolve_off:
-            self.ascii.draw_middle_line()
-            self.ascii.draw_dependency_line()
+    def view_download_package(self, package: str) -> None:
+        size: str = str()
+        color: str = self.cyan
+        version: str = self.data[package]['version']
 
-            for pkg in dependencies:
-                self._view_removed(pkg)
-        else:
-            dependencies: list = []
-
-        self.summary(pkgs, dependencies, option='remove')
-
-        return self.installed_packages, dependencies
-
-    def _view_removed(self, name: str) -> None:
-        """ View and creates list with packages for remove. """
-        installed = self.utils.is_package_installed(name)
+        if self.is_binary:
+            # size: str = self.utils.convert_file_sizes(int(self.data[package][4])) <- It's going to replace with this
+            size: str = self.utils.convert_file_sizes(
+                int(''.join(re.findall(r'\d+', self.data[package]['size_comp']))))
 
-        if installed:
-            pkg: list = self.utils.split_binary_pkg(installed)
-            self.installed_packages.append(installed)
-            size: str = self.utils.get_file_size(Path(self.log_packages, installed))
-
-            self.ascii.draw_view_package(pkg[0], pkg[1], size, self.red,
-                                         repo=pkg[4].lower().replace('_', ''))
-
-    def choose_dependencies_for_remove(self, dependencies: list) -> list:
-        """ Choose packages for remove using the dialog box. """
-        height: int = 10
-        width: int = 70
-        list_height: int = 0
-        choices: list = []
-        title: str = " Choose dependencies you want to remove "
-
-        for package in dependencies:
-            inst_pkg: str = self.utils.is_package_installed(package)
-            inst_ver: str = self.utils.split_binary_pkg(inst_pkg)[1]
-            choices += [(package, inst_ver, True, f'Package: {inst_pkg}')]
-
-        text: str = f'There are {len(choices)} dependencies:'
-
-        code, tags = self.dialogbox.checklist(text, dependencies, title, height,
-                                              width, list_height, choices)
+        self.ascii.draw_package_line(package, version, size, color, self.repository)
+
+    def view_remove_package(self, package: str) -> None:
+        installed: str = self.utils.is_package_installed(package)
+        version: str = self.utils.split_package(installed)['version']
+        repo_tag: str = self.utils.split_package(installed)['tag']
+        size: str = self.utils.get_file_size(Path(self.log_packages, installed))
+        repository: str = repo_tag.lower().replace('_', '')
+
+        self.ascii.draw_package_line(package, version, size, self.red, repository)
 
-        if not code:
-            return dependencies
+    def logs_dependencies(self, dependencies: list) -> None:
+        print('The following logs will be removed:\n')
+        for dep in dependencies:
+            print(f'{self.yellow}{dep[0]}{self.endc}')
+            self.ascii.draw_log_package(dep[1])
 
-        os.system('clear')
-        return tags
+        print('Note: After cleaning you should remove them one by one.')
 
-    def summary(self, packages: list, dependencies: list, option: str) -> None:
-        """ View the status of the packages action. """
+    def view_summary(self, packages: list, dependencies: list, option: str) -> None:
         packages.extend(dependencies)
-        install = upgrade = remove = size_comp = size_uncomp = size_rmv = 0
+        summary_message: str = str()
+        install = upgrade = remove = size_comp = size_uncomp = size_rmv = int()
 
         for pkg in packages:
             installed: str = self.utils.is_package_installed(pkg)
 
-            if self.option_for_binaries:
-                size_comp += int(''.join(re.findall(r'\d+', self.data[pkg][4])))
-                size_uncomp += int(''.join(re.findall(r'\d+', self.data[pkg][5])))
+            if self.is_binary:
+                # size_comp += int(self.data[pkg][4]) <- It's going to replace with this
+                size_comp += int(''.join(re.findall(r'\d+', self.data[pkg]['size_comp'])))
+                # size_uncomp += int(self.data[pkg][5]) <- It's going to replace with this
+                size_uncomp += int(''.join(re.findall(r'\d+', self.data[pkg]['size_uncomp'])))
 
             if installed and option == 'remove':
                 size_rmv += Path(self.log_packages, installed).stat().st_size
 
             upgradeable: bool = False
             if option != 'remove':
                 upgradeable: bool = self.upgrade.is_package_upgradeable(pkg)
 
             if not installed:
                 install += 1
             elif installed and self.option_for_reinstall:
                 upgrade += 1
-            elif installed and upgradeable and self.option_for_reinstall:
-                upgrade += 1
-            elif installed and upgradeable:
+            elif upgradeable:
                 upgrade += 1
             elif installed and option == 'remove':
                 remove += 1
 
         self.ascii.draw_bottom_line()
 
         if option in ['install', 'upgrade']:
-            print(f'{self.grey}Total {install} packages will be '
-                  f'installed and {upgrade} will be upgraded, and total '
-                  f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
-                  f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc} ')
+            summary_message: str = (
+                f'{self.grey}Total {install} packages will be '
+                f'installed and {upgrade} will be upgraded, and total '
+                f'{self.utils.convert_file_sizes(size_comp)} will be downloaded and '
+                f'{self.utils.convert_file_sizes(size_uncomp)} will be installed.{self.endc} '
+            )
 
         elif option == 'build':
-            print(f'{self.grey}Total {len(packages)} packages '
-                  f'will be build in {self.tmp_path} folder.{self.endc}')
+            summary_message: str = (
+                f'{self.grey}Total {len(packages)} packages '
+                f'will be build in {self.tmp_path} folder.{self.endc}'
+            )
 
         elif option == 'remove':
-            print(f'{self.grey}Total {remove} packages '
-                  f'will be removed and {self.utils.convert_file_sizes(size_rmv)} '
-                  f'of space will be freed up.{self.endc}')
+            summary_message: str = (
+                f'{self.grey}Total {remove} packages '
+                f'will be removed and {self.utils.convert_file_sizes(size_rmv)} '
+                f'of space will be freed up.{self.endc}'
+            )
 
         elif option == 'download':
-            print(f'{self.grey}Total {len(packages)} packages and {self.utils.convert_file_sizes(size_comp)} '
-                  f'will be downloaded in {self.download_only} folder.{self.endc}')
+            summary_message: str = (
+                f'{self.grey}Total {len(packages)} packages and {self.utils.convert_file_sizes(size_comp)} '
+                f'will be downloaded in {self.download_only} folder.{self.endc}'
+            )
 
-    def logs_packages(self, dependencies: list) -> None:
-        """ View the logging packages. """
-        print('The following logs will be removed:\n')
+        print(summary_message)
 
-        for dep in dependencies:
-            print(f'{self.yellow}{dep[0]}{self.endc}')
-            self.ascii.draw_log_package(dep[1])
+    def build_package_and_version(self, package: str) -> str:
+        installed_package: str = self.utils.is_package_installed(package)
+        version: str = self.utils.split_package(installed_package)['version']
+        return f'{package}-{version}'
 
-        print('Note: After cleaning you should remove them one by one.')
+    def view_skipping_packages(self, package: str, version: str) -> None:
+        print(f'{self.yellow}Skipping{self.endc}: {package}-{version} {self.red}(already installed){self.endc}')
 
     def question(self) -> None:
-        """ Manage to proceed. """
-        try:
-            if not self.option_for_yes and self.ask_question:
-                answer: str = input('\nDo you want to continue? [y/N] ')
-                if answer not in ['Y', 'y']:
-                    raise SystemExit()
-            print()
-        except KeyboardInterrupt:
-            raise SystemExit()
+        if not self.option_for_yes and self.ask_question:
+            answer: str = input('\nDo you want to continue? [y/N] ')
+            if answer not in ['Y', 'y']:
+                raise SystemExit()
+        print()
```

### Comparing `slpkg-4.8.2/slpkg/checks.py` & `slpkg-4.8.3/slpkg/checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,95 +1,94 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
-
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 from slpkg.repositories import Repositories
 from slpkg.models.models import session as Session
 
 from slpkg.models.models import SBoTable, PonceTable, BinariesTable
 
 
 class Check(Configs):
     """ Some checks before proceed. """
 
-    def __init__(self, flags: list, data: dict):
-        __slots__ = 'flags', 'data'
+    def __init__(self, repository: str, data: dict):
         super(Configs, self).__init__()
-        self.flags: list = flags
         self.data: dict = data
+        self.repository = repository
 
         self.errors = Errors()
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.session = Session
 
-        self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], flags)
-
-        if self.option_for_binaries:
-            self.repo_table = BinariesTable
-        else:
-            self.repo_table = SBoTable
-            if self.repos.ponce_repo:
-                self.repo_table = PonceTable
+        self.is_binary: bool = self.utils.is_binary_repo(repository)
 
-    def exists_in_the_database(self, packages: list) -> None:
-        """ Checking if the slackbuild exists in the database. """
+    def package_exists_in_the_database(self, packages: list) -> None:
         not_packages: list = []
 
         for pkg in packages:
-
-            if self.option_for_binaries:
+            if self.is_binary:
                 if not self.data.get(pkg) and pkg != '*':
                     not_packages.append(pkg)
             else:
                 if not self.data.get(pkg) and pkg != '*':
                     not_packages.append(pkg)
 
         if not_packages:
             self.errors.raise_error_message(f"Packages '{', '.join(not_packages)}' does not exists",
                                             exit_status=1)
 
     def is_package_unsupported(self, slackbuilds: list) -> None:
         """ Checking for unsupported slackbuilds. """
         for sbo in slackbuilds:
             if sbo != '*':
-                if self.os_arch == 'x86_64' and self.data[sbo][4]:
-                    sources: list = self.data[sbo][4].split()
+                if self.os_arch == 'x86_64' and self.data[sbo]['download64']:
+                    sources: list = self.data[sbo]['download64'].split()
                 else:
-                    sources: list = self.data[sbo][3].split()
+                    sources: list = self.data[sbo]['download'].split()
 
                 if 'UNSUPPORTED' in sources:
                     self.errors.raise_error_message(f"Package '{sbo}' unsupported by arch",
                                                     exit_status=1)
 
-    def is_installed(self, packages: list) -> None:
+    def is_package_installed(self, packages: list) -> None:
         """ Checking for installed packages. """
         not_found: list = []
 
         for pkg in packages:
             if not self.utils.is_package_installed(pkg):
                 not_found.append(pkg)
 
         if not_found:
             self.errors.raise_error_message(f'Not found \'{", ".join(not_found)}\' installed packages',
                                             exit_status=1)
 
-    def is_empty_database(self, repo: str) -> None:
+    def is_database_empty(self) -> None:
         """ Checking for empty table and database file. """
-        db = Path(self.db_path, self.database_name)
-
-        if self.option_for_binaries and repo != '*':
-            count: int = self.session.query(self.repo_table.id).where(self.repo_table.repo == repo).count()
+        count: int = 0
+        sbo_table: dict = {
+            self.repos.sbo_repo_name: SBoTable,
+            self.repos.ponce_repo_name: PonceTable
+        }
+
+        if self.repository == '*':
+            for repository, item in self.repos.repositories.items():
+                if item['path']:
+                    if self.utils.is_binary_repo(repository):
+                        count += self.session.query(BinariesTable.id).where(
+                            BinariesTable.repo == repository).count()
+                    else:
+                        count += self.session.query(sbo_table[repository].id).count()
         else:
-            count: int = self.session.query(self.repo_table.id).count()
+            if self.is_binary:
+                count: int = self.session.query(BinariesTable.id).where(BinariesTable.repo == self.repository).count()
+            else:
+                count: int = self.session.query(sbo_table[self.repository].id).count()
 
-        if not self.session.query(self.repo_table).first() or not db.is_file() or count == 0:
+        if count == 0:
             self.errors.raise_error_message("You need to update the package lists first, run:\n\n"
-                                            "              $ slpkg update\n"
-                                            "              $ slpkg update --bin-repo=[repo_name] for binaries",
+                                            "              $ slpkg update",
                                             exit_status=1)
```

### Comparing `slpkg-4.8.2/slpkg/logging_deps.py` & `slpkg-4.8.3/slpkg/logging_deps.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,33 +7,30 @@
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class LoggingDeps:
     """ Logging installed dependencies. """
 
-    def __init__(self, flags: list, data: dict):
-        __slots__ = 'flags', 'data'
-        self.flags: list = flags
+    def __init__(self, repository: str, data: dict):
         self.data: dict = data
 
         self.utils = Utilities()
         self.session = Session
 
-        self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], flags)
+        self.is_binary: bool = self.utils.is_binary_repo(repository)
 
     def logging(self, name: str) -> None:
         exist = self.session.query(LogsDependencies.name).filter(
             LogsDependencies.name == name).first()
 
-        if self.option_for_binaries:
-            requires: list = Required(self.data, name).resolve()
+        if self.is_binary:
+            requires: tuple = Required(self.data, name).resolve()
         else:
-            requires: list = Requires(self.data, name).resolve()
+            requires: tuple = Requires(self.data, name).resolve()
 
         # Update the dependencies if exist else create it.
         if exist:
             self.session.query(
                 LogsDependencies).filter(
                 LogsDependencies.name == name).update(
                 {LogsDependencies.requires: ' '.join(requires)})
```

### Comparing `slpkg-4.8.2/slpkg/new_configs.py` & `slpkg-4.8.3/slpkg/new_configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import Any
 from pathlib import Path
 
 
 class NewConfigs:
 
     def __init__(self, options: list):
-        __slots__ = 'options'
         self.options: list = options
         self.etc_path: Path = Path('/etc/slpkg')
         self.slpkg_config: Path = Path(self.etc_path, 'slpkg.toml')
         self.repositories_config: Path = Path(self.etc_path, 'repositories.toml')
         self.blacklist_config: Path = Path(self.etc_path, 'blacklist.toml')
         self.slpkg_config_new: Path = Path(self.etc_path, 'slpkg.toml.new')
         self.repositories_config_new: Path = Path(self.etc_path, 'repositories.toml.new')
@@ -37,26 +36,26 @@
 
         self.set_no_colors()
 
         self.choice = None
 
     def set_no_colors(self) -> None:
         if '--no-colors' in self.options:
-            self.bold: str = ''
-            self.red: str = ''
-            self.bred: str = ''
-            self.green: str = ''
-            self.bgreen: str = ''
-            self.yellow: str = ''
-            self.byellow: str = ''
-            self.cyan: str = ''
-            self.blue: str = ''
-            self.grey: str = ''
-            self.violet: str = ''
-            self.endc: str = ''
+            self.bold: str = str()
+            self.red: str = str()
+            self.bred: str = str()
+            self.green: str = str()
+            self.bgreen: str = str()
+            self.yellow: str = str()
+            self.byellow: str = str()
+            self.cyan: str = str()
+            self.blue: str = str()
+            self.grey: str = str()
+            self.violet: str = str()
+            self.endc: str = str()
 
     def check(self) -> None:
         """ Checks for .new files. """
         print('\nChecking for NEW configuration files...')
         if (self.slpkg_config_new.is_file() or self.blacklist_config_new.is_file()
                 or self.repositories_config_new.is_file()):
             print('\nThere are NEW files:\n')
@@ -87,15 +86,15 @@
 
     def menu(self) -> None:
         """ Menu of choices. """
         choice: str = input('Choice: ')
 
         choice: str = choice.lower()
 
-        arguments: dict = {
+        arguments: dict[str] = {
             'k': self.keep,
             'o': self.overwrite,
             'r': self.remove,
             'p': self.prompt
         }
 
         try:
@@ -175,72 +174,81 @@
     def prompt(self) -> None:
         """ Prompt K, O, R selection for every single file. """
         print(f"\n{'':>2}({self.byellow}K{self.endc})eep, ({self.byellow}O{self.endc})verwrite, "
               f"({self.byellow}R{self.endc})emove, ({self.byellow}D{self.endc})iff, "
               f"({self.byellow}V{self.endc})imdiff\n")
 
         if self.slpkg_config_new.is_file():
-            make = input(f'{self.bgreen}{self.slpkg_config_new}{self.endc} - '
-                         f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
-                         f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
-                         f'{self.byellow}V{self.endc}): ')
-
-            if make.lower() == 'k':
-                pass
-            if make.lower() == 'o':
-                self.overwrite_config_file()
-                print()  # new line
-            if make.lower() == 'r':
-                print()  # new line
-                self.remove_config_new_file()
-                print()  # new line
-            if make.lower() == 'd':
-                self.diff_files(self.slpkg_config_new, self.slpkg_config)
-            if make.lower() == 'v':
-                self.vimdiff(self.slpkg_config_new, self.slpkg_config)
+            self.prompt_slpkg_config()
 
         if self.repositories_config_new.is_file():
-            make = input(f'{self.bgreen}{self.repositories_config_new}{self.endc} - '
-                         f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
-                         f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
-                         f'{self.byellow}V{self.endc}): ')
-
-            if make.lower() == 'k':
-                pass
-            if make.lower() == 'o':
-                self.overwrite_repositories_file()
-                print()  # new line
-            if make.lower() == 'r':
-                print()  # new line
-                self.remove_repositories_new_file()
-                print()  # new line
-            if make.lower() == 'd':
-                self.diff_files(self.repositories_config_new, self.repositories_config)
-            if make.lower() == 'v':
-                self.vimdiff(self.repositories_config_new, self.repositories_config)
+            self.prompt_repositories_config()
 
         if self.blacklist_config_new.is_file():
-            make = input(f'{self.bgreen}{self.blacklist_config_new}{self.endc} - '
-                         f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
-                         f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
-                         f'{self.byellow}V{self.endc}): ')
-
-            if make.lower() == 'k':
-                pass
-            if make.lower() == 'o':
-                self.overwrite_blacklist_file()
-                print()  # new line
-            if make.lower() == 'r':
-                print()  # new line
-                self.remove_blacklist_new_file()
-                print()  # new line
-            if make.lower() == 'd':
-                self.diff_files(self.blacklist_config_new, self.blacklist_config)
-            if make.lower() == 'v':
-                self.vimdiff(self.blacklist_config_new, self.blacklist_config)
+            self.prompt_blacklist_config()
+
+    def prompt_slpkg_config(self):
+        make: str = input(f'{self.bgreen}{self.slpkg_config_new}{self.endc} - '
+                          f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
+                          f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
+                          f'{self.byellow}V{self.endc}): ')
+
+        if make.lower() == 'k':
+            pass
+        if make.lower() == 'o':
+            self.overwrite_config_file()
+            print()  # new line
+        if make.lower() == 'r':
+            print()  # new line
+            self.remove_config_new_file()
+            print()  # new line
+        if make.lower() == 'd':
+            self.diff_files(self.slpkg_config_new, self.slpkg_config)
+        if make.lower() == 'v':
+            self.vimdiff(self.slpkg_config_new, self.slpkg_config)
+
+    def prompt_repositories_config(self):
+        make: str = input(f'{self.bgreen}{self.repositories_config_new}{self.endc} - '
+                          f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
+                          f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
+                          f'{self.byellow}V{self.endc}): ')
+
+        if make.lower() == 'k':
+            pass
+        if make.lower() == 'o':
+            self.overwrite_repositories_file()
+            print()  # new line
+        if make.lower() == 'r':
+            print()  # new line
+            self.remove_repositories_new_file()
+            print()  # new line
+        if make.lower() == 'd':
+            self.diff_files(self.repositories_config_new, self.repositories_config)
+        if make.lower() == 'v':
+            self.vimdiff(self.repositories_config_new, self.repositories_config)
+
+    def prompt_blacklist_config(self):
+        make: str = input(f'{self.bgreen}{self.blacklist_config_new}{self.endc} - '
+                          f'({self.byellow}K{self.endc}/{self.byellow}O{self.endc}/'
+                          f'{self.byellow}R{self.endc}/{self.byellow}D{self.endc}/'
+                          f'{self.byellow}V{self.endc}): ')
+
+        if make.lower() == 'k':
+            pass
+        if make.lower() == 'o':
+            self.overwrite_blacklist_file()
+            print()  # new line
+        if make.lower() == 'r':
+            print()  # new line
+            self.remove_blacklist_new_file()
+            print()  # new line
+        if make.lower() == 'd':
+            self.diff_files(self.blacklist_config_new, self.blacklist_config)
+        if make.lower() == 'v':
+            self.vimdiff(self.blacklist_config_new, self.blacklist_config)
 
     @staticmethod
     def diff_files(file2: Any, file1: Any) -> None:
         """ Diff the .new and the current file. """
         with open(file1, 'r') as f1:
             with open(file2, 'r') as f2:
                 diff = difflib.context_diff(
```

### Comparing `slpkg-4.8.2/slpkg/cleanings.py` & `slpkg-4.8.3/slpkg/cleanings.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,59 +14,59 @@
                                  LastRepoUpdated)
 
 
 class Cleanings(Configs):
     """ Cleans the logs from packages. """
 
     def __init__(self, flags: list):
-        __slots__ = 'flags'
         super(Configs, self).__init__()
         self.flags: list = flags
         self.session = Session
 
         self.view = ViewMessage(flags)
         self.repos = Repositories()
         self.utils = Utilities()
 
-    def tmp(self):
+    def tmp(self) -> None:
         print('Deleting of local data:\n')
 
         for file in self.tmp_slpkg.glob('*'):
             print(f"  {self.bred}>{self.endc} '{file}'")
 
         print(f"\n{self.prog_name}: {self.blink}{self.bold}{self.bred}WARNING!{self.endc}: All the files and "
               f"folders will delete!")
 
-        views = ViewMessage(self.flags)
-        views.question()
+        self.view.question()
 
         self.utils.remove_folder_if_exists(self.tmp_slpkg)
         self.utils.create_directory(self.build_path)
         print(f'{self.byellow}Successfully cleared!{self.endc}\n')
 
-    def logs_deps(self) -> None:
+    def logs_dependencies(self) -> None:
         """ Deletes the log table from the database. """
         dependencies: list = self.session.query(
             LogsDependencies.name, LogsDependencies.requires).all()  # type: ignore
 
         if dependencies:
-            self.view.logs_packages(dependencies)
+            self.view.logs_dependencies(dependencies)
             self.view.question()
-
-            self.session.query(LogsDependencies).delete()
-            self.session.commit()
+            self.delete_logs_of_dependencies()
         else:
             print('\nNothing to clean.\n')
 
+    def delete_logs_of_dependencies(self):
+        self.session.query(LogsDependencies).delete()
+        self.session.commit()
+
     def db_tables(self) -> None:
         """ Drop all the tables from the database. """
         print('Deleting repositories of local data and the database:\n')
-        for repo, values in self.repos.repositories.items():
-            if values[1].exists() and isinstance(values[1], PosixPath):
-                print(f"  {self.bred}>{self.endc} '{values[1]}'")
+        for item in self.repos.repositories.values():
+            if item['path'].exists() and isinstance(item['path'], PosixPath):
+                print(f"  {self.bred}>{self.endc} '{item['path']}'")
 
         print(f'\n{self.prog_name}: {self.blink}{self.bold}{self.bred}WARNING!{self.endc}: '
               f'All the data from the database will be deleted!')
         self.view.question()
 
         tables: list = [
             PonceTable.__table__,
@@ -78,15 +78,14 @@
         Base.metadata.drop_all(bind=engine, tables=tables)
 
         # Deletes local downloaded data.
         self.delete_repositories_data()
 
         print(f"{self.byellow}Successfully cleared!{self.endc}\n\n"
               "You need to update the package lists now:\n\n"
-              "  $ slpkg update\n"
-              "  $ slpkg update --bin-repo=[repo_name] for binaries\n")
+              "  $ slpkg update\n")
 
-    def delete_repositories_data(self):
+    def delete_repositories_data(self) -> None:
         """ Deletes local folders with the repository downloaded data. """
-        for repo, values in self.repos.repositories.items():
-            if values[1].exists() and isinstance(values[1], PosixPath):
-                shutil.rmtree(values[1])
+        for item in self.repos.repositories.values():
+            if item['path'].exists() and isinstance(item['path'], PosixPath):
+                shutil.rmtree(item['path'])
```

### Comparing `slpkg-4.8.2/slpkg/checksum.py` & `slpkg-4.8.3/slpkg/checksum.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,56 +3,51 @@
 
 import hashlib
 import logging
 from pathlib import Path
 from typing import Union
 from urllib.parse import unquote
 
-from slpkg.views.ascii import Ascii
 from slpkg.utilities import Utilities
 from slpkg.error_messages import Errors
 from slpkg.views.views import ViewMessage
+from slpkg.views.asciibox import AsciiBox
 from slpkg.logging_config import LoggingConfig
 
 
 class Md5sum:
     """ Checksum the sources. """
 
     def __init__(self, flags: list):
-        __slots__ = 'flags'
-        self.flags: list = flags
-        self.ascii = Ascii()
+        self.ascii = AsciiBox()
         self.errors = Errors()
         self.utils = Utilities()
+        self.view = ViewMessage(flags)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
-    def check(self, path: Union[str, Path], source: str, checksum: str) -> None:
+    def md5sum(self, path: Union[str, Path], source: str, checksum: str) -> None:
         """ Checksum the source. """
         source_file = unquote(source)
         filename = source_file.split('/')[-1]
         source_path = Path(path, filename)
 
-        md5 = self.read_file(source_path)
-
-        file_check = hashlib.md5(md5).hexdigest()
-
-        checksum = "".join(checksum)
+        md5: bytes = self.read_binary_file(source_path)
+        file_check: str = hashlib.md5(md5).hexdigest()
+        checksum: str = "".join(checksum)
 
         if file_check != checksum:
             self.ascii.draw_checksum_error_box(filename, checksum, file_check)
-            view = ViewMessage(self.flags)
-            view.question()
+            self.view.question()
 
-    def read_file(self, filename: Union[str, Path]) -> bytes:
-        """ Reads the file. """
+    def read_binary_file(self, filename: Union[str, Path]) -> bytes:
         try:
-            with open(filename, 'rb') as f:
-                return f.read()
+            with open(filename, 'rb') as file:
+                return file.read()
         except FileNotFoundError:
-            logger = logging.getLogger(LoggingConfig.date)
+            logger = logging.getLogger(LoggingConfig.date_time)
             logger.exception(f'{self.__class__.__name__}: '
-                             f'{self.__class__.read_file.__name__}')
+                             f'{self.__class__.read_binary_file.__name__}')
             self.errors.raise_error_message(f"No such file or directory: '{filename}'", exit_status=20)
```

### Comparing `slpkg-4.8.2/slpkg/configs.py` & `slpkg-4.8.3/slpkg/configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/slpkg/utilities.py` & `slpkg-4.8.3/slpkg/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+import os
 import re
 import time
 import shutil
 import fnmatch
 import logging
 import subprocess
 from pathlib import Path
@@ -16,44 +17,46 @@
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
 
 
 class Utilities(Configs):
 
     def __init__(self):
+        super(Configs, self).__init__()
+
         self.black = Blacklist()
         self.errors = Errors()
         self.repos = Repositories()
 
-        self.installed_packages: dict = dict(self.all_installed())
+        self.installed_packages: dict[str] = dict(self.all_installed())
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
     def is_package_installed(self, name: str) -> str:
         """ Returns the installed package binary. """
         try:
             return self.installed_packages[name]
         except KeyError:
             return ''
 
-    def all_installed(self) -> dict:
+    def all_installed(self) -> tuple:
         """ Return all installed packages from /val/log/packages folder. """
         for file in self.log_packages.glob(self.file_pattern):
-            name: str = self.split_binary_pkg(file.name)[0]
+            name: str = self.split_package(file.name)['name']
 
             if not name.startswith('.') and not self.blacklist_pattern(name):
                 yield name, file.name
 
     @staticmethod
     def remove_file_if_exists(path: Path, file: str) -> None:
         """ Clean the old files. """
-        archive = Path(path, file)
+        archive: Path = Path(path, file)
         if archive.is_file():
             archive.unlink()
 
     @staticmethod
     def remove_folder_if_exists(folder: Path) -> None:
         """ Clean the old folders. """
         if folder.exists():
@@ -62,131 +65,131 @@
     @staticmethod
     def create_directory(directory: Path) -> None:
         """ Creates folder like mkdir -p. """
         if not directory.is_dir():
             directory.mkdir(parents=True, exist_ok=True)
 
     @staticmethod
-    def split_binary_pkg(package: str) -> list:
+    def split_package(package: str) -> dict:
         """ Split the package by the name, version, arch, build and tag. """
         name: str = '-'.join(package.split('-')[:-3])
         version: str = ''.join(package[len(name):].split('-')[:-2])
         arch: str = ''.join(package[len(name + version) + 2:].split('-')[:-1])
         build_tag: str = package.split('-')[-1]
         build: str = ''.join(re.findall(r'\d+', build_tag[:2]))
         pkg_tag: str = build_tag[len(build):]
 
-        return [name, version, arch, build, pkg_tag]
+        split: dict[str] = {
+            'name': name,
+            'version': version,
+            'arch': arch,
+            'build': build,
+            'tag': pkg_tag
+        }
+        return split
 
     def finished_time(self, elapsed_time: float) -> None:
         """ Printing the elapsed time. """
         print(f'\n{self.yellow}Finished successfully:{self.endc}',
               time.strftime(f'{self.cyan}%H:%M:%S{self.endc}',
                             time.gmtime(elapsed_time)))
 
-    def read_sbo_build_tag(self, sbo: str, location: str) -> str:
+    def read_slackbuild_build_tag(self, sbo: str, location: str, repository: str) -> str:
         """ Returns build tag from .SlackBuild file. """
-        build: str = ''
-
-        sbo_script = Path(self.repos.sbo_repo_path, location, sbo, f'{sbo}.SlackBuild')
+        build: str = str()
+        sbo_script = Path(self.repos.repositories[repository]['path'], location, sbo, f'{sbo}.SlackBuild')
 
         if sbo_script.is_file():
-            lines = self.read_file(sbo_script)
+            lines = self.read_text_file(sbo_script)
 
             for line in lines:
                 if line.startswith('BUILD=$'):
                     build = ''.join(re.findall(r'\d+', line))
-
         return build
 
     @staticmethod
-    def is_option(flag: list, flags: list) -> bool:
-        """ Checking for flags. """
-        for f in flag:
-            if f in flags:
+    def is_option(options: list, flags: list) -> bool:
+        """ Checking if the option is applied. """
+        for option in options:
+            if option in flags:
                 return True
-        return False
 
     def read_packages_from_file(self, file: Path) -> Generator:
         """ Reads packages from file and split these to list. """
         try:
-
             with open(file, 'r', encoding='utf-8') as pkgs:
                 packages: list = pkgs.read().splitlines()
 
             for package in packages:
                 if package and not package.startswith('#'):
                     if '#' in package:
                         package = package.split('#')[0].strip()
-
                     yield package
-
         except FileNotFoundError:
-            logger = logging.getLogger(LoggingConfig.date)
+            logger = logging.getLogger(LoggingConfig.date_time)
             logger.exception(f'{self.__class__.__name__}: '
                              f'{self.__class__.read_packages_from_file.__name__}')
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
-    def read_file(self, file: Path) -> list:
+    def read_text_file(self, file: Path) -> list:
         """ Reads the text file. """
         try:
-            with open(file, 'r', encoding='utf-8', errors='replace') as f:
-                return f.readlines()
+            with open(file, 'r', encoding='utf-8', errors='replace') as text_file:
+                return text_file.readlines()
         except FileNotFoundError:
-            logger = logging.getLogger(LoggingConfig.date)
+            logger = logging.getLogger(LoggingConfig.date_time)
             logger.exception(f'{self.__class__.__name__}: '
-                             f'{self.__class__.read_file.__name__}')
+                             f'{self.__class__.read_text_file.__name__}')
             self.errors.raise_error_message(f"No such file or directory: '{file}'", exit_status=20)
 
     def process(self, command: str, stderr=None, stdout=None) -> None:
         """ Handle the processes. """
         try:
             subprocess.call(command, shell=True, stderr=stderr, stdout=stdout)
         except subprocess.CalledProcessError as error:
-            logger = logging.getLogger(LoggingConfig.date)
+            logger = logging.getLogger(LoggingConfig.date_time)
             logger.exception(f'{self.__class__.__name__}'
                              f'{self.__class__.process.__name__}')
             self.errors.raise_error_message(str(error), exit_status=20)
         except KeyboardInterrupt:
             raise SystemExit(1)
 
     def get_file_size(self, file: Path) -> str:
         """ Get the local file size and converted to units. """
         size: int = file.stat().st_size
         return self.convert_file_sizes(size)
 
     @staticmethod
     def convert_file_sizes(size: int) -> str:
         """ Convert file sizes. """
-        units: list = ['KB', 'MB', 'GB']
-
+        units: tuple = ('KB', 'MB', 'GB')
         for unit in units:
             if size < 1000:
                 return f'{size:.0f} {unit}'
             size /= 1000
 
     @staticmethod
     def apply_package_pattern(data: dict, packages: list) -> list:
-        """ Apply the pattern. """
+        """ If the '*' applied returns all the package names. """
         for pkg in packages:
-
             if pkg == '*':
                 packages.remove(pkg)
-                packages += list(data.keys())
-
+                packages.extend(list(data.keys()))
         return packages
 
     def blacklist_pattern(self, name: str) -> bool:
         """ This module provides support for Unix shell-style wildcards. """
-        if [black for black in self.black.packages() if fnmatch.fnmatch(name, black)]:
+        blacklist: list[str] = ['%README%']
+        blacklist.extend(self.black.packages())
+        if [black for black in blacklist if fnmatch.fnmatch(name, black)]:
             return True
 
-    def repository_name(self, data: dict) -> str:
-        """ Get the binary repository name from the repository data. """
-        try:
-            # Binary repository name
-            repo: list = list(data.values())[0][11]
-        except (IndexError, AttributeError):
-            # Slackbuilds repository name 'sbo | ponce'
-            repo: str = self.repos.sbo_enabled_repo_name
+    def is_binary_repo(self, repo: str) -> bool:
+        """ Checks if the repository is binary. """
+        if repo in tuple(self.repos.repositories.keys())[2:]:
+            return True
 
-        return repo
+    @staticmethod
+    def change_owner_privileges(folder: Path):
+        os.chown(folder, 0, 0)
+        for file in os.listdir(folder):
+            os.chown(Path(folder, file), 0, 0)
```

### Comparing `slpkg-4.8.2/slpkg/dependees.py` & `slpkg-4.8.3/slpkg/dependees.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,94 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 from typing import Generator
 from slpkg.configs import Configs
-from slpkg.views.ascii import Ascii
 from slpkg.utilities import Utilities
-from slpkg.repositories import Repositories
+from slpkg.views.asciibox import AsciiBox
 
 
 class Dependees(Configs):
-    """ Show which packages depend. """
+    """ Prints the packages that depend on. """
 
-    def __init__(self, data: dict, packages: list, flags: list):
-        __slots__ = 'data', 'packages', 'flags'
+    def __init__(self, data: dict, packages: list, flags: list, repository: str):
         super(Configs, self).__init__()
         self.data: dict = data
         self.packages: list = packages
         self.flags: list = flags
 
-        self.ascii = Ascii()
-        self.repos = Repositories()
+        self.ascii = AsciiBox()
         self.utils = Utilities()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.var: str = self.ascii.vertical_and_right
+        self.package_version: str = str()
+
+        self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_full_reverse: bool = self.utils.is_option(
             ['-E', '--full-reverse'], flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ['-p', '--pkg-version'], flags)
 
-        self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], flags)
-
     def find(self) -> None:
-        """ Collecting the dependees. """
-        print(f"The list below shows the "
-              f"packages that dependees on '{', '.join([p for p in self.packages])}':\n")
-
-        self.packages: list = self.utils.apply_package_pattern(self.data, self.packages)
-
-        for pkg in self.packages:
-            dependees: dict = dict(self.find_requires(pkg))
-
-            package: str = f'{self.byellow}{pkg}{self.endc}'
-
-            if self.option_for_pkg_version:
-                if self.option_for_binaries:
-                    version: str = self.data[pkg][0]
-                else:
-                    version: str = self.data[pkg][2]
-
-                package: str = f'{self.byellow}{pkg} {version}{self.endc}'
-
-            print(package)
+        self.view_the_title()
 
-            print(f' {self.llc}{self.hl}', end='')
+        for package in self.packages:
+            dependees: dict = dict(self.find_requires(package))
+            self.view_the_main_package(package)
+            self.view_no_dependees(dependees)
+            self.view_dependees(dependees)
+            self.view_summary_of_dependees(dependees, package)
 
-            if not dependees:
-                print(f'{self.cyan} No dependees{self.endc}')
+    def set_the_package_version(self, package: str):
+        self.package_version: str = self.data[package]['version']
 
-            sp: str = ' ' * 4
-            for i, (name, requires) in enumerate(dependees.items(), start=1):
-                dependency: str = f'{self.cyan}{name}{self.endc}'
-
-                if self.option_for_pkg_version:
-
-                    if self.option_for_binaries:
-                        version: str = self.data[name][0]
-                    else:
-                        version: str = self.data[name][2]
-
-                    dependency: str = (f'{self.cyan}{name}{self.endc} {self.yellow}'
-                                       f'{version}{self.endc}')
-
-                if i == 1:
-                    print(f' {dependency}')
-                else:
-                    print(f'{sp}{dependency}')
-
-                if self.option_for_full_reverse:
-                    if i == len(dependees):
-                        print(' ' * 4 + f' {self.llc}{self.hl} {self.violet}{requires}{self.endc}')
-                    else:
-                        print(' ' * 4 + f' {self.var}{self.hl} {self.violet}{requires}{self.endc}')
+    def find_requires(self, package: str) -> Generator:
+        """ Find requires that package dependees. """
+        for name, data in self.data.items():
+            if package in data['requires'].split():
+                yield name, data['requires']
 
-            print(f'\n{self.grey}{len(dependees)} dependees for {pkg}{self.endc}\n')
+    def view_the_title(self) -> None:
+        print(f"The list below shows the "
+              f"packages that dependees on '{', '.join([pkg for pkg in self.packages])}':\n")
+        self.packages: tuple = tuple(self.utils.apply_package_pattern(self.data, self.packages))
 
-    def find_requires(self, pkg: str) -> Generator:
-        """ Find requires that package dependees. """
-        if self.option_for_binaries:
+    def view_no_dependees(self, dependees: dict) -> None:
+        if not dependees:
+            print(f"{'':>1}{self.cyan}No dependees{self.endc}")
+
+    def view_the_main_package(self, package: str) -> None:
+        print(f'{self.byellow}{package}{self.endc}')
+        print(f"{'':>1}{self.llc}{self.hl}", end='')
+
+    @staticmethod
+    def view_dependency_line(n: int, dependency: str) -> None:
+        str_dependency: str = f"{'':>4}{dependency}"
+        if n == 1:
+            str_dependency: str = f"{'':>1}{dependency}"
+        print(str_dependency)
+
+    def view_dependees(self, dependees: dict) -> None:
+        for n, (name, requires) in enumerate(dependees.items(), start=1):
+            dependency: str = f'{self.cyan}{name}{self.endc}'
+            if self.option_for_pkg_version:
+                self.set_the_package_version(name)
+                dependency: str = (f'{self.cyan}{name}{self.endc} {self.yellow}'
+                                   f'{self.package_version}{self.endc}')
+
+            self.view_dependency_line(n, dependency)
+
+            if self.option_for_full_reverse:
+                self.view_full_reverse(n, dependees, requires)
+
+    def view_full_reverse(self, n: int, dependees: dict, requires: str) -> None:
+        str_requires: str = f"{'':>5}{self.var}{self.hl} {self.violet}{requires}{self.endc}"
+        if n == len(dependees):
+            str_requires: str = f"{'':>5}{self.llc}{self.hl} {self.violet}{requires}{self.endc}"
+        print(str_requires)
 
-            for name, data in self.data.items():
-                if pkg in data[6].split():
-                    yield name, data[6]
-
-        else:
-            for name, data in self.data.items():
-                if pkg in data[7].split():
-                    yield name, data[7]
+    def view_summary_of_dependees(self, dependees: dict, package: str) -> None:
+        print(f'\n{self.grey}{len(dependees)} dependees for {package}{self.endc}\n')
```

### Comparing `slpkg-4.8.2/slpkg/toml_error_message.py` & `slpkg-4.8.3/slpkg/toml_error_message.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/slpkg/check_updates.py` & `slpkg-4.8.3/slpkg/check_updates.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,130 +13,140 @@
 from slpkg.repositories import Repositories
 from slpkg.logging_config import LoggingConfig
 
 
 class CheckUpdates(Configs):
     """ Check for changes in the ChangeLog file. """
 
-    def __init__(self, flags: list, repo: str):
-        __slots__ = 'flags', 'repo'
+    def __init__(self, flags: list, repository: str):
         super(Configs, self).__init__()
         self.flags: list = flags
-        self.repo: str = repo
+        self.repository: str = repository
 
         self.utils = Utilities()
         self.progress = ProgressBar()
         self.repos = Repositories()
 
         self.compare: dict = {}
+        self.http = PoolManager()
+        self.proxy_default_headers = make_headers(
+            proxy_basic_auth=f'{self.proxy_username}:{self.proxy_password}')
 
-        self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], flags)
+        self.is_binary: bool = self.utils.is_binary_repo(repository)
+
+        self.option_for_repository: bool = self.utils.is_option(
+            ['-o', '--repository='], flags)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
-    def check(self) -> dict:
-        if self.option_for_binaries:
+    def check_the_repositories(self) -> dict:
+        if self.option_for_repository:
+            self.check_updates_for_repository()
+        else:
+            self.check_updates_for_repositories()
 
-            for repo in list(self.repos.repositories.keys())[2:]:
+        return self.compare
 
-                if self.repos.repositories[repo][0] and repo == self.repo:
-                    self.binary_repository(repo)
-                    break
+    def check_updates_for_repository(self):
+        sbo_repository: dict = {
+            self.repos.sbo_repo_name: self.sbo_repository,
+            self.repos.ponce_repo_name: self.ponce_repository
+        }
 
-                if self.repos.repositories[repo][0] and self.repo == '*':
-                    self.binary_repository(repo)
+        if self.is_binary:
+            self.binary_repository(self.repository)
         else:
+            sbo_repository[self.repository]()
 
-            if self.repos.ponce_repo:
-                self.ponce_repository()
-            else:
-                self.sbo_repository()
-
-        return self.compare
-
-    def binary_repository(self, repo) -> None:
-        local_chg_txt: Path = Path(self.repos.repositories[repo][1], self.repos.repositories[repo][5])
-        repo_chg_txt: str = f'{self.repos.repositories[repo][2][0]}{self.repos.repositories[repo][5]}'
-        self.compare[repo] = self.compare_dates(local_chg_txt, repo_chg_txt)
+    def check_updates_for_repositories(self):
+        if self.repos.sbo_repo:
+            self.sbo_repository()
+
+        if self.repos.ponce_repo:
+            self.ponce_repository()
+
+        for repo in list(self.repos.repositories.keys())[2:]:
+            if self.repos.repositories[repo]['enable']:
+                self.binary_repository(repo)
+
+    def binary_repository(self, repo: str) -> None:
+        local_chg_txt: Path = Path(self.repos.repositories[repo]['path'],
+                                   self.repos.repositories[repo]['changelog_txt'])
+        repo_chg_txt: str = (f"{self.repos.repositories[repo]['mirror'][0]}"
+                             f"{self.repos.repositories[repo]['changelog_txt']}")
+        self.compare[repo] = self.compare_the_changelogs(local_chg_txt, repo_chg_txt)
 
     def sbo_repository(self) -> None:
         local_chg_txt: Path = Path(self.repos.sbo_repo_path, self.repos.sbo_repo_changelog)
         repo_chg_txt: str = f'{self.repos.sbo_repo_mirror[0]}{self.repos.sbo_repo_changelog}'
-        self.compare[self.repos.sbo_repo_name] = self.compare_dates(local_chg_txt, repo_chg_txt)
+        self.compare[self.repos.sbo_repo_name] = self.compare_the_changelogs(local_chg_txt, repo_chg_txt)
 
     def ponce_repository(self) -> None:
         local_chg_txt: Path = Path(self.repos.ponce_repo_path, self.repos.ponce_repo_changelog)
         repo_chg_txt: str = f'{self.repos.ponce_repo_mirror[0]}{self.repos.ponce_repo_changelog}'
-        self.compare[self.repos.ponce_repo_name] = self.compare_dates(local_chg_txt, repo_chg_txt)
+        self.compare[self.repos.ponce_repo_name] = self.compare_the_changelogs(local_chg_txt, repo_chg_txt)
 
-    def compare_dates(self, local_chg_txt: Path, repo_chg_txt: str) -> bool:
+    def compare_the_changelogs(self, local_chg_txt: Path, repo_chg_txt: str) -> bool:
         local_size: int = 0
 
-        if repo_chg_txt.startswith('file'):
-            return False
+        if self.proxy_address.startswith('http'):
+            self.set_http_proxy_server()
 
-        try:
-            http = PoolManager()
-            proxy_default_headers = make_headers(proxy_basic_auth=f'{self.proxy_username}:{self.proxy_password}')
-
-            if self.proxy_address.startswith('http'):
-                http = ProxyManager(f'{self.proxy_address}', headers=proxy_default_headers)
-
-            elif self.proxy_address.startswith('socks'):
-                # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
-                try:  # Try to import PySocks if it's installed.
-                    from urllib3.contrib.socks import SOCKSProxyManager
-                except (ModuleNotFoundError, ImportError):
-                    logger = logging.getLogger(LoggingConfig.date)
-                    logger.exception(f'{self.__class__.__name__}: '
-                                     f'{self.__class__.compare_dates.__name__}')
-                    raise SystemExit()
-
-                http = SOCKSProxyManager(f'{self.proxy_address}', headers=proxy_default_headers)
-
-            repo = http.request('GET', repo_chg_txt)
-        except KeyboardInterrupt:
-            raise SystemExit(1)
+        if self.proxy_address.startswith('socks'):
+            self.set_socks_proxy_server()
 
+        repo = self.http.request('GET', repo_chg_txt)
         if local_chg_txt.is_file():
             local_size: int = int(os.stat(local_chg_txt).st_size)
 
         repo_size: int = int(repo.headers['Content-Length'])
 
-        logger = logging.getLogger(LoggingConfig.date)
+        logger = logging.getLogger(LoggingConfig.date_time)
         logger.info(f'{self.__class__.__name__}: '
-                    f'{self.__class__.compare_dates.__name__}: '
+                    f'{self.__class__.compare_the_changelogs.__name__}: '
                     f'{local_chg_txt=}, {local_size=}, '
                     f'{repo_chg_txt=}, {repo_size=}, '
                     f'{local_size != repo_size}')
 
         return local_size != repo_size
 
-    def view_message(self) -> None:
-        self.check()
+    def set_http_proxy_server(self):
+        self.http = ProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
+
+    def set_socks_proxy_server(self):
+        try:  # Try to import PySocks if it's installed.
+            from urllib3.contrib.socks import SOCKSProxyManager
+        except (ModuleNotFoundError, ImportError) as error:
+            print(error)
+        # https://urllib3.readthedocs.io/en/stable/advanced-usage.html#socks-proxies
+        self.http = SOCKSProxyManager(f'{self.proxy_address}', headers=self.proxy_default_headers)
+
+    def check_for_updates(self) -> None:
+        self.check_the_repositories()
+        self.view_messages()
 
+    def view_messages(self) -> None:
         print()
         for repo, comp in self.compare.items():
             if comp:
                 print(f"\n{self.endc}There are new updates available for the "
                       f"'{self.bgreen}{repo}{self.endc}' repository!")
 
         if True not in self.compare.values():
             print(f'\n{self.endc}{self.yellow}No updated packages since the last check.{self.endc}')
 
     def updates(self) -> None:
         message: str = 'Checking for news, please wait...'
 
         # Starting multiprocessing
-        p1 = Process(target=self.view_message)
-        p2 = Process(target=self.progress.bar, args=(message, ''))
+        p1 = Process(target=self.check_for_updates)
+        p2 = Process(target=self.progress.progress_bar, args=(message, ''))
 
         p1.start()
         p2.start()
 
         # Wait until process 1 finish
         p1.join()
```

### Comparing `slpkg-4.8.2/slpkg/remove_packages.py` & `slpkg-4.8.3/slpkg/remove_packages.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,160 +1,152 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
+import os
 import time
-import subprocess
-from multiprocessing import Process
 
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
+from slpkg.dialog_box import DialogBox
 from slpkg.views.views import ViewMessage
-from slpkg.progress_bar import ProgressBar
+from slpkg.multi_process import MultiProcess
 from slpkg.models.models import LogsDependencies
 from slpkg.models.models import session as Session
 
 
 class RemovePackages(Configs):
-    """ Removes installed packages. """
+    """ Removes installed packages with dependencies if they installed with
+        slpkg install command.
+    """
 
     def __init__(self, packages: list, flags: list):
-        __slots__ = 'packages', 'flags'
         super(Configs, self).__init__()
         self.packages: list = packages
         self.flags: list = flags
 
         self.session = Session
+        self.dialogbox = DialogBox()
         self.utils = Utilities()
-        self.progress = ProgressBar()
+        self.multi_proc = MultiProcess(flags)
         self.view = ViewMessage(flags)
 
-        self.process_message: str = ''
+        self.logs_dependencies: dict = {}
         self.installed_packages: list = []
+        self.installed_dependencies: list = []
         self.dependencies: list = []
-        self.stderr = None
-        self.stdout = None
 
-        self.option_resolve_off: bool = self.utils.is_option(
-            ['-o', '--resolve-off'], flags)
-
-        self.option_for_no_silent: bool = self.utils.is_option(
-            ['-n', '--no-silent'], flags)
+        self.option_for_resolve_off: bool = self.utils.is_option(
+            ['-O', '--resolve-off'], flags)
 
         self.option_for_yes: bool = self.utils.is_option(
             ['-y', '--yes'], flags)
 
     def remove(self) -> None:
-        """ Removes package with dependencies. """
-        self.installed_packages, self.dependencies = self.view.remove_packages(self.packages)
+        self.query_logs_dependencies()
+        self.save_dependencies_for_remove()
+        self.remove_doubles_dependencies()
+        self.remove_doubles_installed_dependencies()
+        self.add_dependencies_to_remove()
+        self.choose_dependencies_for_remove()
+        self.save_packages_for_remove()
 
+        self.view.remove_packages(self.packages, self.dependencies)
         self.view.question()
 
         start: float = time.time()
         self.remove_packages()
-
-        if self.dependencies and not self.option_resolve_off:
-            self.delete_deps_logs()
-
-        self.delete_main_logs()
-
         elapsed_time: float = time.time() - start
-
         self.utils.finished_time(elapsed_time)
 
+    def save_dependencies_for_remove(self) -> None:
+        if not self.option_for_resolve_off:
+            for package in self.packages:
+                if self.logs_dependencies.get(package):
+                    requires: tuple = self.logs_dependencies[package]
+
+                    for require in requires:
+                        installed: str = self.utils.is_package_installed(require)
+                        if installed and require not in self.packages:
+                            self.dependencies.append(require)
+                            self.installed_dependencies.append(installed)
+
+    def remove_doubles_dependencies(self) -> None:
+        self.dependencies: list = list(set(self.dependencies))
+
+    def remove_doubles_installed_dependencies(self):
+        self.installed_dependencies: list = list(set(self.installed_dependencies))
+
+    def add_dependencies_to_remove(self) -> None:
+        self.installed_packages.extend(self.installed_dependencies)
+
+    def save_packages_for_remove(self) -> None:
+        for package in self.packages:
+            installed: str = self.utils.is_package_installed(package)
+            if installed:
+                self.installed_packages.append(installed)
+
     def remove_packages(self) -> None:
-        """ Run Slackware command to remove the packages. """
         for package in self.installed_packages:
-            name: str = self.utils.split_binary_pkg(package)[0]
-            self.process_message: str = f"package '{name}' to remove"
+            command: str = f'{self.removepkg} {package}'
+            name: str = self.utils.split_package(package)['name']
+            process_message: str = f"package '{name}' to remove"
+            progress_message: str = f'{self.bold}{self.red}Remove{self.endc}'
+
+            dependencies: list = self.is_dependency(name)
+            if dependencies:
+                self.view_warning_message(dependencies, name)
+                if not self.question_to_remove():
+                    continue
 
-            if self.check_in_logs_for_dependencies_to_remove(name):
-                command: str = f'{self.removepkg} {package}'
-                self.multi_process(command, package)
+            self.multi_proc.process(command, package, process_message, progress_message)
+            self.delete_package_from_logs(name)
 
-    def check_in_logs_for_dependencies_to_remove(self, name: str) -> bool:
+    def is_dependency(self, name: str) -> list:
         dependencies: list = []
-        logs: dict = self.query_dependencies()
-
-        for package, requires in logs.items():
-            if name in requires:
+        for package, requires in self.logs_dependencies.items():
+            if name in requires and package not in self.packages:
                 dependencies.append(package)
 
-        if dependencies and not self.option_for_yes and self.ask_question:
-            print(f"\n{self.bold}{self.violet}WARNING!{self.endc}: The package '{self.red}{name}{self.endc}' "
-                  f"is a dependency for the packages:")
-
-            for dep in dependencies:
-                print(f"{self.cyan:>16}-> {dep}{self.endc}")
-
-            try:
-                answer: str = input('\nDo you want to remove? [y/N] ')
-            except KeyboardInterrupt:
-                raise SystemExit()
+        if dependencies:
+            return dependencies
 
-            if answer not in ['Y', 'y']:
-                return False
+    def question_to_remove(self) -> bool:
+        if not self.option_for_yes and self.ask_question:
+            answer: str = input('\nDo you want to remove? [y/N] ')
+            if answer in ['Y', 'y']:
+                return True
             print()
 
-        return True
+    def view_warning_message(self, dependencies: list, name: str) -> None:
+        print(f"\n{self.bold}{self.violet}WARNING!{self.endc}: The package '{self.red}{name}{self.endc}' "
+              f"is a dependency for the packages:")
+        for dependency in dependencies:
+            print(f"{self.cyan:>16}-> {dependency}{self.endc}")
 
-    def query_dependencies(self) -> dict:
-        """ Returns a dictionary with the package name and the dependencies
-            before they are saved with the command slpkg install. """
-        logs_deps: dict = {}
+    def query_logs_dependencies(self) -> None:
         package_requires: tuple = self.session.query(
             LogsDependencies.name, LogsDependencies.requires).all()
-
         for package in package_requires:
-            if package[0] not in self.packages:
-                logs_deps[package[0]] = package[1].split()
-
-        return logs_deps
-
-    def delete_main_logs(self) -> None:
-        """ Deletes main packages from logs. """
-        for pkg in self.packages:
-            self.session.query(LogsDependencies).filter(
-                LogsDependencies.name == pkg).delete()
-        self.session.commit()
+            self.logs_dependencies[package[0]] = package[1].split()
 
-    def delete_deps_logs(self) -> None:
-        """ Deletes depends packages from logs. """
-        for pkg in self.dependencies:
+    def delete_package_from_logs(self, package) -> None:
+        if not self.option_for_resolve_off:
             self.session.query(LogsDependencies).filter(
-                LogsDependencies.name == pkg).delete()
-        self.session.commit()
-
-    def multi_process(self, command: str, package: str) -> None:
-        """ Starting multiprocessing remove process. """
-        if self.silent_mode and not self.option_for_no_silent:
-
-            done: str = f' {self.byellow} Done{self.endc}'
-            message: str = f'{self.bold}{self.red}Remove{self.endc}'
-            self.stderr = subprocess.DEVNULL
-            self.stdout = subprocess.DEVNULL
-
-            # Starting multiprocessing
-            p1 = Process(target=self.utils.process, args=(command, self.stderr, self.stdout))
-            p2 = Process(target=self.progress.bar, args=(f'{message}:', package))
-
-            p1.start()
-            p2.start()
-
-            # Wait until process 1 finish
-            p1.join()
-
-            # Terminate process 2 if process 1 finished
-            if not p1.is_alive():
-
-                if p1.exitcode != 0:
-                    done: str = f'{self.bred}Failed: {self.endc}{self.process_message}'
-
-                print(f'{self.endc}{done}', end='')
-                p2.terminate()
-
-            # Wait until process 2 finish
-            p2.join()
+                LogsDependencies.name == package).delete()
+            self.session.commit()
 
-            # Restore the terminal cursor
-            print('\x1b[?25h', self.endc)
-        else:
-            self.utils.process(command, self.stderr, self.stdout)
+    def choose_dependencies_for_remove(self) -> None:
+        height: int = 10
+        width: int = 70
+        list_height: int = 0
+        choices: list = []
+        title: str = " Choose dependencies you want to remove "
+
+        for package in self.dependencies:
+            installed_package: str = self.utils.is_package_installed(package)
+            installed_version: str = self.utils.split_package(installed_package)['version']
+            choices.extend([(package, installed_version, True, f'Package: {installed_package}')])
+
+        text: str = f'There are {len(choices)} dependencies:'
+        code, self.dependencies = self.dialogbox.checklist(text, self.dependencies, title, height,
+                                                           width, list_height, choices)
+        os.system('clear')
```

### Comparing `slpkg-4.8.2/slpkg/blacklist.py` & `slpkg-4.8.3/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.2/slpkg/download_only.py` & `slpkg-4.8.3/slpkg/download_only.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,68 +9,82 @@
 from slpkg.utilities import Utilities
 from slpkg.downloader import Downloader
 from slpkg.views.views import ViewMessage
 from slpkg.repositories import Repositories
 from slpkg.models.models import session as Session
 
 
-class Download(Configs):
-    """ Download the slackbuilds with the sources only. """
+class DownloadOnly(Configs):
+    """ Download only the sources and the slackbuilds or the packages
+        for binary repositories.
+    """
 
-    def __init__(self, directory: Path, flags: list):
-        __slots__ = 'directory', 'flags'
+    def __init__(self, directory: Path, flags: list, data: dict, repository: str):
         super(Configs, self).__init__()
-        self.flags: list = flags
         self.directory: Path = directory
+        self.flags: list = flags
+        self.data: dict = data
+        self.repository: str = repository
 
+        self.view = ViewMessage(flags, repository, data)
         self.repos = Repositories()
         self.utils = Utilities()
         self.session = Session
+        self.urls: list = []
+        self.download_path: Path = Path()
 
+        self.sbo_repo: dict = {
+            self.repos.sbo_repo_name: self.repos.sbo_repo_path,
+            self.repos.ponce_repo_name: self.repos.ponce_repo_path
+        }
+
+        self.is_binary: bool = self.utils.is_binary_repo(repository)
         self.option_for_directory: bool = self.utils.is_option(
             ['-z', '--directory='], flags)
 
-        self.option_for_binaries: bool = self.utils.is_option(
-            ['-B', '--bin-repo='], flags)
-
-    def packages(self, data: dict, packages: list) -> None:
-        """ Download the package only. """
-        packages: list = self.utils.apply_package_pattern(data, packages)
-
-        view = ViewMessage(self.flags, data)
-        view.download_packages(packages, self.directory)
-        view.question()
-
-        download_path: Path = self.download_only_path
-        if self.option_for_directory:
-            download_path: Path = self.directory
-
+    def packages(self, packages: list) -> None:
+        packages: list = self.utils.apply_package_pattern(self.data, packages)
+        self.view.download_packages(packages, self.directory)
+        self.view.question()
+        self.set_download_path()
         start: float = time.time()
-        urls: list = []
-        for pkg in packages:
 
-            if self.option_for_binaries:
-                package: str = data[pkg][1]
-                mirror: str = data[pkg][2]
-                location: str = data[pkg][3]
-                urls.append(f'{mirror}{location}/{package}')
+        for pkg in packages:
+            if self.is_binary:
+                self.save_binary_sources(pkg)
             else:
-                location: str = data[pkg][0]
-                if self.os_arch == 'x86_64' and data[pkg][4]:
-                    sources = data[pkg][4].split()
-                else:
-                    sources = data[pkg][3].split()
-
-                urls += sources
-
-                if self.repos.ponce_repo:
-                    ponce_repo_path_package = Path(self.repos.ponce_repo_path, location, pkg)
-                    shutil.copytree(ponce_repo_path_package, Path(download_path, pkg))
-                else:
-                    file: str = f'{pkg}{self.repos.sbo_repo_tar_suffix}'
-                    urls += [f'{self.repos.sbo_repo_mirror[0]}{location}/{file}']
+                self.save_slackbuild_sources(pkg)
+                self.copy_slackbuild_scripts(pkg)
 
-        down = Downloader(download_path, urls, self.flags)
-        down.download()
+        self.download_the_sources()
 
         elapsed_time: float = time.time() - start
         self.utils.finished_time(elapsed_time)
+
+    def set_download_path(self) -> None:
+        self.download_path: Path = self.download_only_path
+        if self.option_for_directory:
+            self.download_path: Path = self.directory
+
+    def save_binary_sources(self, name: str) -> None:
+        package: str = self.data[name]['package']
+        mirror: str = self.data[name]['mirror']
+        location: str = self.data[name]['location']
+        self.urls.append(f'{mirror}{location}/{package}')
+
+    def save_slackbuild_sources(self, name: str) -> None:
+        if self.os_arch == 'x86_64' and self.data[name]['download64']:
+            sources: list = self.data[name]['download64'].split()
+        else:
+            sources: list = self.data[name]['download'].split()
+        self.urls.extend(sources)
+
+    def copy_slackbuild_scripts(self, name: str) -> None:
+        repo_path_package: Path = Path(self.sbo_repo[self.repository], self.data[name]['location'], name)
+        if not Path(self.download_path, name).is_dir():
+            shutil.copytree(repo_path_package, Path(self.download_path, name))
+        print(f"{self.byellow}Copying{self.endc}: {repo_path_package} -> {Path(self.download_path, name)}")
+
+    def download_the_sources(self) -> None:
+        print('\nDownloading the sources:')
+        down = Downloader(self.download_path, self.urls, self.flags)
+        down.download()
```

### Comparing `slpkg-4.8.2/slpkg/main.py` & `slpkg-4.8.3/slpkg/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,146 +14,149 @@
 from slpkg.dependees import Dependees
 from slpkg.utilities import Utilities
 from slpkg.cleanings import Cleanings
 from slpkg.search import SearchPackage
 from slpkg.views.cli_menu import Usage
 from slpkg.dialog_box import DialogBox
 from slpkg.views.version import Version
-from slpkg.download_only import Download
 from slpkg.sbos.queries import SBoQueries
 from slpkg.views.help_commands import Help
 from slpkg.repositories import Repositories
 from slpkg.binaries.install import Packages
 from slpkg.dialog_configs import FormConfigs
 from slpkg.check_updates import CheckUpdates
+from slpkg.download_only import DownloadOnly
 from slpkg.sbos.slackbuild import Slackbuilds
 from slpkg.binaries.queries import BinQueries
 from slpkg.logging_config import LoggingConfig
 from slpkg.find_installed import FindInstalled
 from slpkg.views.view_package import ViewPackage
 from slpkg.remove_packages import RemovePackages
 from slpkg.update_repository import UpdateRepository
 
 
 class Argparse(Configs):
 
     def __init__(self, args: list):
-        __slots__ = 'args'
         super(Configs).__init__()
         self.args: list = args
         self.flags: list = []
-        self.binary_repo: str = ''
-        self.directory = self.tmp_slpkg
+        self.directory: Path = self.tmp_slpkg
 
         self.dialogbox = DialogBox()
         self.utils = Utilities()
         self.usage = Usage()
         self.form_configs = FormConfigs()
         self.repos = Repositories()
 
-        self.binary_repo: str = ''
+        self.repository: str = self.repos.default_repository
 
         if len(args) == 0 or '' in args:
             self.usage.help_short(1)
 
         self.data: dict = {}
         self.flag_yes: str = '--yes'
         self.flag_short_yes: str = '-y'
         self.flag_jobs: str = '--jobs'
         self.flag_short_jobs: str = '-j'
         self.flag_resolve_off: str = '--resolve-off'
-        self.flag_short_resolve_off: str = '-o'
+        self.flag_short_resolve_off: str = '-O'
         self.flag_reinstall: str = '--reinstall'
         self.flag_short_reinstall: str = '-r'
         self.flag_skip_installed: str = '--skip-installed'
         self.flag_short_skip_installed: str = '-k'
+        self.flag_install_data: str = '--install-data'
+        self.flag_short_install_data: str = '-a'
         self.flag_full_reverse: str = '--full-reverse'
         self.flag_short_full_reverse: str = '-E'
         self.flag_search: str = '--search'
         self.flag_short_search: str = '-S'
         self.flag_no_silent: str = '--no-silent'
         self.flag_short_no_silent: str = '-n'
         self.flag_pkg_version: str = '--pkg-version'
         self.flag_short_pkg_version: str = '-p'
-        self.flag_generate: str = '--generate-only'
-        self.flag_short_generate: str = '-G'
         self.flag_parallel: str = '--parallel'
         self.flag_short_parallel: str = '-P'
-        self.flag_bin_repository: str = '--bin-repo='
-        self.flag_short_bin_repository: str = '-B'
+        self.flag_repository: str = '--repository='
+        self.flag_short_repository: str = '-o'
         self.flag_directory: str = '--directory='
         self.flag_short_directory: str = '-z'
 
-        self.flag_searches: list = [self.flag_short_search, self.flag_search]
-        self.flag_binaries: list = [self.flag_short_bin_repository, self.flag_bin_repository]
+        self.flag_searches: list = [
+            self.flag_short_search,
+            self.flag_search
+        ]
 
         self.options: list = [
             self.flag_yes,
             self.flag_short_yes,
             self.flag_jobs,
             self.flag_short_jobs,
             self.flag_resolve_off,
             self.flag_short_resolve_off,
             self.flag_reinstall,
             self.flag_short_reinstall,
             self.flag_skip_installed,
             self.flag_short_skip_installed,
+            self.flag_install_data,
+            self.flag_short_install_data,
             self.flag_full_reverse,
             self.flag_short_full_reverse,
             self.flag_search,
             self.flag_short_search,
             self.flag_no_silent,
             self.flag_short_no_silent,
             self.flag_pkg_version,
             self.flag_short_pkg_version,
-            self.flag_generate,
-            self.flag_short_generate,
             self.flag_parallel,
             self.flag_short_parallel,
-            self.flag_bin_repository,
-            self.flag_short_bin_repository,
+            self.flag_repository,
+            self.flag_short_repository,
             self.flag_directory,
             self.flag_short_directory,
         ]
 
         self.commands: dict = {
             '--help': [],
             '--version': [],
             'help': [],
             'update': [
                 self.flag_yes,
                 self.flag_short_yes,
-                self.flag_generate,
-                self.flag_short_generate,
-                self.flag_bin_repository,
-                self.flag_short_bin_repository,
+                self.flag_install_data,
+                self.flag_short_install_data,
+                self.flag_repository,
+                self.flag_short_repository,
                 self.flag_parallel,
                 self.flag_short_parallel
             ],
             'upgrade': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_jobs,
                 self.flag_short_jobs,
                 self.flag_resolve_off,
                 self.flag_short_resolve_off,
                 self.flag_reinstall,
                 self.flag_short_reinstall,
                 self.flag_no_silent,
                 self.flag_short_no_silent,
-                self.flag_bin_repository,
-                self.flag_short_bin_repository,
+                self.flag_repository,
+                self.flag_short_repository,
                 self.flag_parallel,
                 self.flag_short_parallel
             ],
             'check-updates': [
-                self.flag_bin_repository,
-                self.flag_short_bin_repository
+                self.flag_repository,
+                self.flag_short_repository
+            ],
+            'repo-info': [
+                self.flag_repository,
+                self.flag_short_repository
             ],
-            'repo-info': [],
             'configs': [],
             'clean-logs': [
                 self.flag_yes,
                 self.flag_short_yes
             ],
             'clean-data': [
                 self.flag_yes,
@@ -167,14 +170,16 @@
                 self.flag_short_jobs,
                 self.flag_resolve_off,
                 self.flag_short_resolve_off,
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_no_silent,
                 self.flag_short_no_silent,
+                self.flag_repository,
+                self.flag_short_repository,
                 self.flag_parallel,
                 self.flag_short_parallel
             ],
             'install': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_jobs,
@@ -185,28 +190,28 @@
                 self.flag_short_reinstall,
                 self.flag_skip_installed,
                 self.flag_short_skip_installed,
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_no_silent,
                 self.flag_short_no_silent,
-                self.flag_bin_repository,
-                self.flag_short_bin_repository,
+                self.flag_repository,
+                self.flag_short_repository,
                 self.flag_parallel,
                 self.flag_short_parallel
             ],
             'download': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_directory,
                 self.flag_short_directory,
-                self.flag_bin_repository,
-                self.flag_short_bin_repository,
+                self.flag_repository,
+                self.flag_short_repository,
                 self.flag_parallel,
                 self.flag_short_parallel
             ],
             'remove': [
                 self.flag_yes,
                 self.flag_short_yes,
                 self.flag_resolve_off,
@@ -219,42 +224,42 @@
             'find': [
                 self.flag_search,
                 self.flag_short_search,
             ],
             'view': [
                 self.flag_search,
                 self.flag_short_search,
-                self.flag_bin_repository,
-                self.flag_short_bin_repository,
+                self.flag_repository,
+                self.flag_short_repository,
                 self.flag_pkg_version,
                 self.flag_short_pkg_version
             ],
             'search': [
                 self.flag_search,
                 self.flag_short_search,
-                self.flag_bin_repository,
-                self.flag_short_bin_repository
+                self.flag_repository,
+                self.flag_short_repository
             ],
             'dependees': [
                 self.flag_full_reverse,
                 self.flag_short_full_reverse,
                 self.flag_search,
                 self.flag_short_search,
-                self.flag_bin_repository,
-                self.flag_short_bin_repository,
+                self.flag_repository,
+                self.flag_short_repository,
                 self.flag_pkg_version,
                 self.flag_short_pkg_version
             ],
             'tracking': [
                 self.flag_search,
                 self.flag_short_search,
                 self.flag_pkg_version,
                 self.flag_short_pkg_version,
-                self.flag_bin_repository,
-                self.flag_short_bin_repository
+                self.flag_repository,
+                self.flag_short_repository
             ]
         }
 
         self.commands['-h'] = self.commands['--help']
         self.commands['-v'] = self.commands['--version']
         self.commands['-u'] = self.commands['update']
         self.commands['-U'] = self.commands['upgrade']
@@ -274,52 +279,50 @@
         self.commands['-e'] = self.commands['dependees']
         self.commands['-t'] = self.commands['tracking']
 
         self.split_options()
         self.split_options_from_args()
         self.move_options()
         self.invalid_options()
-        self.check_for_bin_repositories()
+        self.check_for_repositories()
 
-        if self.utils.is_option(self.flag_binaries, self.flags):
-            self.data: dict = BinQueries(self.binary_repo).repository_data()
-        else:
-            self.data: dict = SBoQueries().repository_data()
+        self.is_binary: bool = self.utils.is_binary_repo(self.repository)
 
-        self.check = Check(self.flags, self.data)
+        if self.repository != '*':
+            if self.is_binary:
+                self.data: dict = BinQueries(self.repository).repository_data()
+            else:
+                self.data: dict = SBoQueries(self.repository).repository_data()
+
+        self.check = Check(self.repository, self.data)
 
         logging.basicConfig(filename=LoggingConfig.log_file,
                             filemode=LoggingConfig.filemode,
                             encoding=LoggingConfig.encoding,
                             level=LoggingConfig.level)
 
-        logger = logging.getLogger(LoggingConfig.date)
+        logger = logging.getLogger(LoggingConfig.date_time)
         logger.info(f'{self.__class__.__name__}: '
                     f'{self.__class__.__init__.__name__}: '
-                    f'{args=}, {self.flags=}, {self.binary_repo=}')
+                    f'{args=}, {self.flags=}, {self.repository=}')
 
-    def check_for_bin_repositories(self) -> None:
+    def check_for_repositories(self) -> None:
         """ Checks combination for binaries use repositories only and if repository exists. """
-        if self.utils.is_option(self.flag_binaries, self.flags):
-
-            except_options: list = [
-                '-s', 'search',
-                '-u', 'update',
-                '-c', 'check-updates',
-            ]
-
-            if (self.binary_repo in list(self.repos.repositories.keys())[2:]
-                    and not self.repos.repositories[self.binary_repo][0]):
-                self.usage.help_minimal(f"{self.prog_name}: repository '{self.binary_repo}' is disabled")
+        except_options: list = [
+            '-s', 'search',
+        ]
+        if self.repository == '*' and not self.utils.is_option(except_options, self.args):
+            self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
-            elif self.binary_repo == '*' and not self.utils.is_option(except_options, self.args):
-                self.usage.help_minimal(f"{self.prog_name}: invalid binary repository '{self.binary_repo}'")
+        elif self.repository not in list(self.repos.repositories.keys()) and self.repository != '*':
+            self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
 
-            elif self.binary_repo not in list(self.repos.repositories.keys())[2:] and self.binary_repo != '*':
-                self.usage.help_minimal(f"{self.prog_name}: invalid binary repository '{self.binary_repo}'")
+        if self.repository != '*':
+            if not self.repos.repositories[self.repository]['enable']:
+                self.usage.help_minimal(f"{self.prog_name}: repository '{self.repository}' is disabled")
 
     def invalid_options(self) -> None:
         """ Checks for invalid options. """
         invalid, commands, repeat = [], [], []
 
         for arg in self.args:
             if arg[0] == '-' and arg in self.commands.keys():
@@ -343,17 +346,14 @@
         # Fixed for correct options by command.
         try:
             options: list = self.commands[self.args[0]]
             for opt in self.flags:
                 if opt not in options:
                     invalid.append(opt)
         except (KeyError, IndexError):
-            logger = logging.getLogger(LoggingConfig.date)
-            logger.exception(f'{self.__class__.__name__}: '
-                             f'{self.__class__.invalid_options.__name__}')
             self.usage.help_short(1)
 
         # Prints error for invalid options.
         if invalid:
             self.usage.help_minimal(f"{self.prog_name}: invalid options '{','.join(invalid)}'")
 
     def split_options(self) -> None:
@@ -374,51 +374,43 @@
                         continue
 
                     self.args.append(opt)
 
     def split_options_from_args(self) -> None:
         """ Split options from arguments.
 
-            slpkg -f package --file-pattern='*'
+            slpkg -d package --directory=/path/to/download
 
-            Splits the option ['--file-pattern'] and ['*']
+            Splits the option ['--directory'] and ['/path/to/download/']
         """
         for arg in self.args:
+
             if arg.startswith(self.flag_directory):
                 self.directory: str = arg.split('=')[1]
-                self.args[self.args.index(arg)] = self.flag_directory
+                self.args.remove(arg)
+                self.args.append(self.flag_directory)
 
-            if arg.startswith(self.flag_short_directory) and len(self.args) > 3:
-                try:
+            try:
+                if arg.startswith(self.flag_short_directory):
                     self.directory: str = self.args[self.args.index(arg) + 1]
-                except IndexError:
-                    logger = logging.getLogger(LoggingConfig.date)
-                    logger.exception(f'{self.__class__.__name__}: '
-                                     f'{self.__class__.split_options_from_args.__name__}')
-                    self.directory: Path = self.tmp_slpkg
-                else:
                     self.args.remove(self.directory)
+            except IndexError:
+                self.directory: Path = self.tmp_slpkg
 
-            if arg.startswith(self.flag_bin_repository):
-                self.binary_repo: str = arg.split('=')[1]
-                self.args[self.args.index(arg)] = self.flag_bin_repository
-
-            if arg.startswith(self.flag_short_bin_repository) and len(self.args) > 2:
-                try:
-                    self.binary_repo: str = self.args[self.args.index(arg) + 1]
-                except IndexError:
-                    logger = logging.getLogger(LoggingConfig.date)
-                    logger.exception(f'{self.__class__.__name__}: '
-                                     f'{self.__class__.split_options_from_args.__name__}')
-                    self.binary_repo = ''
-                else:
-                    self.args.remove(self.binary_repo)
+            if arg.startswith(self.flag_repository):
+                self.repository: str = arg.split('=')[1]
+                self.args.remove(arg)
+                self.args.append(self.flag_repository)
 
-        if self.binary_repo in self.options:
-            self.binary_repo: str = ''
+            try:
+                if arg.startswith(self.flag_short_repository):
+                    self.repository: str = self.args[self.args.index(arg) + 1]
+                    self.args.remove(self.repository)
+            except IndexError:
+                self.repository: str = str()
 
     def move_options(self) -> None:
         """ Move options to the flags and removes from the arguments. """
         new_args: list = []
 
         for arg in self.args:
             if arg in self.options:
@@ -448,73 +440,65 @@
 
         repo_packages: list = list(self.data.keys())
 
         if method in ['remove', 'find']:
             installed: list = list(self.utils.installed_packages.values())
 
             for package in installed:
-                split_package: list = self.utils.split_binary_pkg(package)
+                package_name: str = self.utils.split_package(package)['name']
+                package_version: str = self.utils.split_package(package)['version']
 
                 for pkg in packages:
-
                     if pkg in package or pkg == '*':
-                        choices += [(split_package[0], split_package[1], False, f'Package: {package}')]
+                        choices.extend([(package_name, package_version, False, f'Package: {package}')])
 
         elif method == 'upgrade':
             for pkg in packages:
                 for package in repo_packages:
 
                     if pkg == package:
-
                         inst_pkg: str = self.utils.is_package_installed(package)
-                        split_inst_pkg: list = self.utils.split_binary_pkg(inst_pkg)
-
-                        if self.utils.is_option(self.flag_binaries, self.flags):
-                            repo_ver: str = self.data[package][0]
-                            bin_pkg: str = self.data[package][1]
-                            repo_build_tag: str = self.utils.split_binary_pkg(bin_pkg[:-4])[3]
+                        inst_package_version: str = self.utils.split_package(inst_pkg)['version']
+                        inst_package_build: str = self.utils.split_package(inst_pkg)['build']
+                        repo_ver: str = self.data[package]['version']
+
+                        if self.is_binary:
+                            bin_pkg: str = self.data[package]['package']
+                            repo_build_tag: str = self.utils.split_package(bin_pkg[:-4])['build']
                         else:
-                            repo_ver: str = self.data[package][2]
-                            repo_location: str = self.data[package][0]
-                            repo_build_tag: str = self.utils.read_sbo_build_tag(package, repo_location)
-
-                        choices += [(package, f'{split_inst_pkg[1]} -> {repo_ver}', True,
-                                     f'Installed: {package}-{split_inst_pkg[1]} Build: {split_inst_pkg[3]} -> '
-                                     f'Available: {repo_ver} Build: {repo_build_tag}')]
+                            repo_location: str = self.data[package]['location']
+                            repo_build_tag: str = self.utils.read_slackbuild_build_tag(
+                                package, repo_location, self.repository
+                            )
+
+                        choices.extend([(package, f'{inst_package_version} -> {repo_ver}', True,
+                                         f'Installed: {package}-{inst_package_version} Build: {inst_package_build} -> '
+                                        f'Available: {repo_ver} Build: {repo_build_tag}')])
         else:
             for pkg in packages:
                 for package in repo_packages:
 
                     if pkg in package or pkg == '*':
-                        if self.utils.is_option(self.flag_binaries, self.flags):
-                            repo_ver: str = self.data[package][0]
-                            repo: str = self.binary_repo
-                        else:
-                            repo_ver: str = self.data[package][2]
-                            repo: str = self.repos.sbo_enabled_repo_name
-
-                        choices += [(package, repo_ver, False, f'Package: {package}-{repo_ver} '
-                                                               f'> {repo}')]
+                        version: str = self.data[package]['version']
+                        choices.extend([(package, version, False, f'Package: {package}-{version} '
+                                       f'> {self.repository}')])
 
         if not choices:
             return packages
 
         text: str = f'There are {len(choices)} packages:'
-        code, tags = self.dialogbox.checklist(text, packages, title, height,
-                                              width, list_height, choices)
-        if code == 'cancel':
+        code, packages = self.dialogbox.checklist(text, packages, title, height,
+                                                  width, list_height, choices)
+        if code == 'cancel' or not packages:
             os.system('clear')
             raise SystemExit()
 
-        if not tags or not code:
-            return packages
-
         os.system('clear')
 
-        return list(set(tags))
+        return packages
 
     def help(self) -> None:
         if len(self.args) == 1:
             self.usage.help(0)
         self.usage.help_short(1)
 
     def version(self) -> None:
@@ -522,67 +506,71 @@
             version = Version()
             version.view()
             raise SystemExit()
         self.usage.help_short(1)
 
     def update(self) -> None:
         if len(self.args) == 1:
-            update = UpdateRepository(self.flags, self.binary_repo)
+            update = UpdateRepository(self.flags, self.repository)
             update.repositories()
             raise SystemExit()
         self.usage.help_short(1)
 
     def upgrade(self) -> None:
-        command = Argparse.upgrade.__name__
+        command: str = Argparse.upgrade.__name__
 
         if len(self.args) == 1:
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
 
-            upgrade = Upgrade(self.flags, self.data)
+            upgrade = Upgrade(self.repository, self.data)
             packages: list = list(upgrade.packages())
 
             packages: list = self.choose_packages(packages, command)
 
             if not packages:
                 print('\nEverything is up-to-date!\n')
                 raise SystemExit()
 
-            if self.utils.is_option(self.flag_binaries, self.flags):
-                install = Packages(self.data, packages, self.flags, mode=command)
-                install.execute()
+            if self.is_binary:
+                install = Packages(
+                    self.repository, self.data, packages, self.flags, mode=command
+                )
             else:
-                install = Slackbuilds(self.data, packages, self.flags, mode=command)
-                install.execute()
+                install = Slackbuilds(
+                    self.repository, self.data, packages, self.flags, mode=command
+                )
+
+            install.execute()
             raise SystemExit()
         self.usage.help_short(1)
 
     def check_updates(self) -> None:
         if len(self.args) == 1:
-            check = CheckUpdates(self.flags, self.binary_repo)
+            check = CheckUpdates(self.flags, self.repository)
             check.updates()
             raise SystemExit()
         self.usage.help_short(1)
 
     def repo_info(self) -> None:
         if len(self.args) == 1:
-            repo = RepoInfo()
+            repo = RepoInfo(self.flags, self.repository)
             repo.info()
             raise SystemExit()
         self.usage.help_short(1)
 
     def edit_configs(self) -> None:
         if len(self.args) == 1:
             self.form_configs.edit()
             raise SystemExit()
         self.usage.help_short(1)
 
     def clean_logs(self) -> None:
         if len(self.args) == 1:
             clean = Cleanings(self.flags)
-            clean.logs_deps()
+            clean.logs_dependencies()
             raise SystemExit()
         self.usage.help_short(1)
 
     def clean_tmp(self) -> None:
         if len(self.args) == 1:
             clean = Cleanings(self.flags)
             clean.tmp()
@@ -593,204 +581,201 @@
         if len(self.args) == 1:
             clean = Cleanings(self.flags)
             clean.db_tables()
             raise SystemExit()
         self.usage.help_short(1)
 
     def build(self) -> None:
-        command = Argparse.build.__name__
+        command: str = Argparse.build.__name__
 
         if len(self.args) >= 2:
-
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages)
             self.check.is_package_unsupported(packages)
 
-            build = Slackbuilds(self.data, packages, self.flags, mode=command)
-            build.execute()
+            if self.repository in list(self.repos.repositories.keys())[:2]:
+                build = Slackbuilds(
+                    self.repository, self.data, packages, self.flags, mode=command
+                )
+                build.execute()
+            else:
+                self.usage.help_minimal(f"{self.prog_name}: invalid repository '{self.repository}'")
+
             raise SystemExit()
         self.usage.help_short(1)
 
     def install(self) -> None:
-        command = Argparse.install.__name__
+        command: str = Argparse.install.__name__
 
         if len(self.args) >= 2:
-
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            if self.utils.is_option(self.flag_binaries, self.flags):
-                self.check.exists_in_the_database(packages)
+            if self.is_binary:
+                self.check.package_exists_in_the_database(packages)
 
-                install = Packages(self.data, packages, self.flags, mode=command)
+                install = Packages(self.repository, self.data, packages, self.flags, mode=command)
                 install.execute()
             else:
-                self.check.exists_in_the_database(packages)
+                self.check.package_exists_in_the_database(packages)
                 self.check.is_package_unsupported(packages)
 
-                install = Slackbuilds(self.data, packages, self.flags, mode=command)
+                install = Slackbuilds(self.repository, self.data, packages, self.flags, mode=command)
                 install.execute()
             raise SystemExit()
         self.usage.help_short(1)
 
     def download(self) -> None:
-        command = Argparse.download.__name__
+        command: str = Argparse.download.__name__
 
         if len(self.args) >= 2:
-
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages)
-            download = Download(self.directory, self.flags)
-            download.packages(self.data, packages)
+            self.check.package_exists_in_the_database(packages)
+            down_only = DownloadOnly(self.directory, self.flags, self.data, self.repository)
+            down_only.packages(packages)
             raise SystemExit()
         self.usage.help_short(1)
 
     def remove(self) -> None:
-        command = Argparse.remove.__name__
+        command: str = Argparse.remove.__name__
 
         if len(self.args) >= 2:
-
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.is_installed(packages)
+            self.check.is_package_installed(packages)
 
             remove = RemovePackages(packages, self.flags)
             remove.remove()
             raise SystemExit()
         self.usage.help_short(1)
 
     def find(self) -> None:
-        command = Argparse.find.__name__
+        command: str = Argparse.find.__name__
 
         if len(self.args) >= 2:
-
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            find = FindInstalled()
-            find.find(packages)
+            find = FindInstalled(packages)
+            find.find()
             raise SystemExit()
         self.usage.help_short(1)
 
     def view(self) -> None:
-        command = Argparse.view.__name__
+        command: str = Argparse.view.__name__
 
         if len(self.args) >= 2:
-
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages)
 
-            view = ViewPackage(self.flags)
+            view = ViewPackage(self.flags, self.repository)
 
-            if self.utils.is_option(self.flag_binaries, self.flags):
-                view.package(self.data, packages, self.binary_repo)
+            if self.is_binary:
+                view.package(self.data, packages)
             else:
                 view.slackbuild(self.data, packages)
             raise SystemExit()
         self.usage.help_short(1)
 
     def search(self) -> None:
-        command = Argparse.search.__name__
+        command: str = Argparse.search.__name__
 
         if len(self.args) >= 2:
-
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            search = SearchPackage(self.flags)
-            search.package(self.data, packages, self.binary_repo)
+            pkgs = SearchPackage(self.data, packages, self.repository)
+            pkgs.search()
             raise SystemExit()
         self.usage.help_short(1)
 
     def dependees(self) -> None:
-        command = Argparse.dependees.__name__
+        command: str = Argparse.dependees.__name__
 
         if len(self.args) >= 2:
-
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages)
 
-            dependees = Dependees(self.data, packages, self.flags)
+            dependees = Dependees(self.data, packages, self.flags, self.repository)
             dependees.find()
             raise SystemExit()
         self.usage.help_short(1)
 
     def tracking(self) -> None:
-        command = Argparse.tracking.__name__
+        command: str = Argparse.tracking.__name__
 
         if len(self.args) >= 2:
-
-            self.check.is_empty_database(self.binary_repo)
+            self.check.is_database_empty()
             packages: list = self.is_file_list_packages()
 
             if self.utils.is_option(self.flag_searches, self.flags):
                 packages: list = self.choose_packages(packages, command)
 
-            self.check.exists_in_the_database(packages)
+            self.check.package_exists_in_the_database(packages)
 
-            tracking = Tracking(self.flags)
-            tracking.packages(self.data, packages)
+            tracking = Tracking(self.data, packages, self.flags, self.repository)
+            tracking.package()
             raise SystemExit()
         self.usage.help_short(1)
 
     def help_for_commands(self) -> None:
         """ Extra help information for commands. """
         if len(self.args) == 2:
             try:
-                flags = self.commands[self.args[1]]
+                flags: list = self.commands[self.args[1]]
                 Help(self.args[1], flags).view()
             except KeyError:
-                logger = logging.getLogger(LoggingConfig.date)
+                logger = logging.getLogger(LoggingConfig.date_time)
                 logger.exception(f'{self.__class__.__name__}: '
                                  f'{self.__class__.help_for_commands.__name__}')
                 self.usage.help_minimal(f"{self.prog_name}: invalid argument '{''.join(self.args[1])}'")
         else:
             self.usage.help_short(1)
 
 
 def main() -> None:
     args: list = sys.argv
     args.pop(0)
 
     usage = Usage()
     argparse = Argparse(args)
 
-    arguments: dict = {
+    arguments: dict[str] = {
         '-h': argparse.help,
         '--help': argparse.help,
         '-v': argparse.version,
         '--version': argparse.version,
         'help': argparse.help_for_commands,
         'update': argparse.update,
         '-u': argparse.update,
@@ -827,14 +812,16 @@
         'tracking': argparse.tracking,
         '-t': argparse.tracking
     }
 
     try:
         arguments[args[0]]()
     except (KeyError, IndexError):
-        logger = logging.getLogger(LoggingConfig.date)
-        logger.exception(f'{main.__name__}')
+        logger = logging.getLogger(LoggingConfig.date_time)
+        logger.exception(main.__name__)
         usage.help_short(1)
+    except KeyboardInterrupt:
+        raise SystemExit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `slpkg-4.8.2/slpkg/find_installed.py` & `slpkg-4.8.3/slpkg/find_installed.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,33 +4,39 @@
 from slpkg.configs import Configs
 from slpkg.utilities import Utilities
 
 
 class FindInstalled(Configs):
     """ Find installed packages. """
 
-    def __init__(self):
+    def __init__(self, packages: list):
         super(Configs, self).__init__()
+        self.packages: list = packages
 
         self.utils = Utilities()
         self.matching: list = []
 
-    def find(self, packages: list) -> None:
-        """ Find the packages. """
-        print(f'The list below shows the installed packages '
-              f'that contains \'{", ".join([p for p in packages])}\' files:\n')
-
-        for pkg in packages:
+    def find(self) -> None:
+        self.view_title()
+        for pkg in self.packages:
             for package in self.utils.installed_packages.values():
                 if pkg in package or pkg == '*':
                     self.matching.append(package)
-
         self.matched()
 
+    def view_title(self):
+        print(f'The list below shows the installed packages '
+              f'that contains \'{", ".join([p for p in self.packages])}\' files:\n')
+
     def matched(self) -> None:
-        """ Print the matched packages. """
         if self.matching:
-            for package in self.matching:
-                print(f'{self.cyan}{package}{self.endc}')
-            print(f'\n{self.grey}Total found {len(self.matching)} packages.{self.endc}')
+            self.view_matched_packages()
         else:
             print('\nDoes not match any package.\n')
+
+    def view_matched_packages(self):
+        for package in self.matching:
+            print(f'{self.cyan}{package}{self.endc}')
+        self.view_summary()
+
+    def view_summary(self):
+        print(f'\n{self.grey}Total found {len(self.matching)} packages.{self.endc}')
```

### Comparing `slpkg-4.8.2/setup.cfg` & `slpkg-4.8.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = slpkg
-version = 4.8.2
+version = 4.8.3
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = d.zlatanidis@gmail.com
 description = Package manager utility for Slackware Linux.
 long_description = file:README.rst
 url = https://dslackw.gitlab.io/slpkg/
 project_urls =
```

### Comparing `slpkg-4.8.2/slpkg.egg-info/SOURCES.txt` & `slpkg-4.8.3/slpkg.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 slpkg/downloader.py
 slpkg/error_messages.py
 slpkg/find_installed.py
 slpkg/install_data.py
 slpkg/logging_config.py
 slpkg/logging_deps.py
 slpkg/main.py
+slpkg/multi_process.py
 slpkg/new_configs.py
 slpkg/progress_bar.py
 slpkg/remove_packages.py
 slpkg/repo_info.py
 slpkg/repositories.py
 slpkg/search.py
 slpkg/toml_error_message.py
@@ -42,15 +43,16 @@
 slpkg/binaries/queries.py
 slpkg/binaries/required.py
 slpkg/models/__init__.py
 slpkg/models/models.py
 slpkg/sbos/__init__.py
 slpkg/sbos/dependencies.py
 slpkg/sbos/queries.py
+slpkg/sbos/sbo_generate.py
 slpkg/sbos/slackbuild.py
 slpkg/views/__init__.py
-slpkg/views/ascii.py
+slpkg/views/asciibox.py
 slpkg/views/cli_menu.py
 slpkg/views/help_commands.py
 slpkg/views/version.py
 slpkg/views/view_package.py
 slpkg/views/views.py
```

### Comparing `slpkg-4.8.2/slpkg.egg-info/PKG-INFO` & `slpkg-4.8.3/slpkg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slpkg
-Version: 4.8.2
+Version: 4.8.3
 Summary: Package manager utility for Slackware Linux.
 Home-page: https://dslackw.gitlab.io/slpkg/
 Author: Dimitris Zlatanidis
 Author-email: d.zlatanidis@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://dslackw.gitlab.io/slpkg/
 Project-URL: Documentation, https://dslackw.gitlab.io/slpkg/
```

### Comparing `slpkg-4.8.2/README.md` & `slpkg-4.8.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 ```
 $ slpkg repo-info
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_repo_info.png" width="900">
 
 ```
-$ slpkg install audacity --bin-repo=alien
+$ slpkg install audacity --repository=alien
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install.png" width="900">
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_install_done.png" width="900">
 
 ```
 $ slpkg remove audacity
 ```
@@ -56,16 +56,16 @@
 $ slpkg tracking --pkg-version Flask awscli pychess
 ```
 <img src="https://gitlab.com/dslackw/images/raw/master/slpkg/slpkg_tracking.png" width="900">
 
 ### Installation
 
 ```
-$ tar xvf slpkg-4.8.2.tar.gz
-$ cd slpkg-4.8.2
+$ tar xvf slpkg-4.8.3.tar.gz
+$ cd slpkg-4.8.3
 $ ./install.sh
 ```
 
 ### Requirements
 
 ```
 SQLAlchemy >= 1.4.46
@@ -82,15 +82,15 @@
 
 The majority of trials have been made in Slackware x86_64 'stable' environment.
 
 
 ### Command Line Tool Usage
 
 ```
-slpkg - version 4.8.2
+slpkg - version 4.8.3
 
 USAGE:
   slpkg [COMMAND] [OPTIONS] [FILELIST|PACKAGES...]
 
 DESCRIPTION:
   Package manager utility for Slackware.
 
@@ -112,25 +112,25 @@
   -s, search [packages...]      Search packages from the repository.
   -e, dependees [packages...]   Show which packages depend on.
   -t, tracking [packages...]    Tracking the packages dependencies.
 
 OPTIONS:
   -y, --yes                     Answer Yes to all questions.
   -j, --jobs                    Set it for multicore systems.
-  -o, --resolve-off             Turns off dependency resolving.
+  -O, --resolve-off             Turns off dependency resolving.
   -r, --reinstall               Upgrade packages of the same version.
   -k, --skip-installed          Skip installed packages.
+  -a, --install-data            Install data into the database only.
   -E, --full-reverse            Full reverse dependency.
   -S, --search                  Search packages from the repository.
   -n, --no-silent               Disable silent mode.
   -p, --pkg-version             Print the repository package version.
-  -G, --generate-only           Generates only the SLACKBUILDS.TXT file.
   -P, --parallel                Download files in parallel.
-  -B, --bin-repo=[REPO]         Set a binary repository.
-  -z, --directory=[PATH]        Download files to a specific path.
+  -o, --repository=NAME         Change repository you want to work.
+  -z, --directory=PATH          Download files to a specific path.
 
   -h, --help                    Show this message and exit.
   -v, --version                 Print version and exit.
 ```
 
 
 ### How to start
@@ -141,49 +141,44 @@
 The second step is to update the package lists and install the data to the database, just run:
 
 
 ```
     $ slpkg update
 ```
 
-or for binary repositories:
-
-```
-    $ slpkg update --bin-repo='*'
-```
 Now you are ready to start!
 
-To install a package from the [SlackBuilds.org](https://slackbuilds.org) or [Ponce](https://cgit.ponce.cc/slackbuilds) repository, run:
+To install a package, run:
 
 ```
     $ slpkg install <package_name>
 ```
 
-or from a binary repository:
+or change the repository:
 
 ```
-    $ slpkg install <package_name> --bin-repo=<repo_name>
+    $ slpkg install <package_name> --repository=<repo_name>
 ```
 
 You can install a whole repository with the command:
 
 ```
-    $ slpkg install '*' --bin-repo=<repository_name> --resolve-off
+    $ slpkg install '*' --repository=<repository_name>
 ```
 
 To remove a package with the dependencies:
 
 ```
     $ slpkg remove <package_name>
 ```
 
-If you want to search a package from all binaries repositories, run:
+If you want to search a package from all repositories, run:
 
 ```
-    $ slpkg search <package_name> --bin-repo='*'
+    $ slpkg search <package_name> --repository='*'
 ```
 
 Edit the configuration `/etc/slpkg/slpkg.toml` file:
 
 ```
     $ slpkg configs
 ```
```

### Comparing `slpkg-4.8.2/tools/gen_sbo_txt.sh` & `slpkg-4.8.3/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*

