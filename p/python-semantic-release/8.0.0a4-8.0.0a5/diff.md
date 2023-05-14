# Comparing `tmp/python-semantic-release-8.0.0a4.tar.gz` & `tmp/python-semantic-release-8.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.0a4.tar", last modified: Mon Feb 27 22:12:29 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.0a5.tar", last modified: Mon Apr 17 20:00:17 2023, max compression
```

## Comparing `python-semantic-release-8.0.0a4.tar` & `python-semantic-release-8.0.0a5.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.800116 python-semantic-release-8.0.0a4/
--rw-r--r--   0 root         (0) root         (0)      230 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2747 2023-02-27 22:12:29.800116 python-semantic-release-8.0.0a4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1858 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/README.rst
--rw-r--r--   0 root         (0) root         (0)     5302 2023-02-27 22:12:12.000000 python-semantic-release-8.0.0a4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.788116 python-semantic-release-8.0.0a4/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2747 2023-02-27 22:12:29.000000 python-semantic-release-8.0.0a4/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4024 2023-02-27 22:12:29.000000 python-semantic-release-8.0.0a4/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 22:12:29.000000 python-semantic-release-8.0.0a4/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-02-27 22:12:29.000000 python-semantic-release-8.0.0a4/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      498 2023-02-27 22:12:29.000000 python-semantic-release-8.0.0a4/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-27 22:12:29.000000 python-semantic-release-8.0.0a4/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.792116 python-semantic-release-8.0.0a4/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-02-27 22:12:12.000000 python-semantic-release-8.0.0a4/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.792116 python-semantic-release-8.0.0a4/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4300 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/changelog/template.py
--rw-r--r--   0 root         (0) root         (0)     4106 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/ci_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.792116 python-semantic-release-8.0.0a4/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      427 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.792116 python-semantic-release-8.0.0a4/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)      129 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3472 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     5233 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    14454 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)    16793 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2913 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.792116 python-semantic-release-8.0.0a4/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      589 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.788116 python-semantic-release-8.0.0a4/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.792116 python-semantic-release-8.0.0a4/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1143 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      507 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      815 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.792116 python-semantic-release-8.0.0a4/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     9035 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10675 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     6016 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.792116 python-semantic-release-8.0.0a4/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14127 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14060 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-27 22:12:29.800116 python-semantic-release-8.0.0a4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.788116 python-semantic-release-8.0.0a4/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    44485 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/scenario/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/cli/conftest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/cli/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)      504 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/cli/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/cli/test_main.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/cli/test_publish.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/cli/test_version.py
--rw-r--r--   0 root         (0) root         (0)    41833 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12291 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5089 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    24086 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    25566 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    10376 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 22:12:29.796116 python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7319 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3502 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-02-27 22:11:26.000000 python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.356697 python-semantic-release-8.0.0a5/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-04-17 20:00:17.356697 python-semantic-release-8.0.0a5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/README.rst
+-rw-r--r--   0 root         (0) root         (0)     5340 2023-04-17 19:59:59.000000 python-semantic-release-8.0.0a5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4022 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      520 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 19:59:59.000000 python-semantic-release-8.0.0a5/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    16552 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    17524 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)      846 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      615 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.344697 python-semantic-release-8.0.0a5/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      507 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5813 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     9035 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10675 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     6016 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14060 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 20:00:17.356697 python-semantic-release-8.0.0a5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.344697 python-semantic-release-8.0.0a5/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)    23514 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    45283 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5089 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    24084 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    25564 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    10376 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.356697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7319 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.0a4/LICENSE` & `python-semantic-release-8.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/PKG-INFO` & `python-semantic-release-8.0.0a5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0a4
+Version: 8.0.0a5
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mypy
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Python Semantic Release
 ***********************
```

### Comparing `python-semantic-release-8.0.0a4/README.rst` & `python-semantic-release-8.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/pyproject.toml` & `python-semantic-release-8.0.0a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.0-alpha.4"
+version = "8.0.0-alpha.5"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
 ]
 readme = "README.rst"
 authors = [{ name = "Rolf Erik Lekang", email = "me@rolflekang.com" }]
 dependencies = [
   "click>=7,<9",
   "gitpython>=3.0.8,<4",
   "twine>=4,<5",
   "requests>=2.25,<3",
-  "wheel",
   "jinja2>=3.1.2,<4",
   "python-gitlab>=2,<4",
   "tomlkit~=0.10",
   "dotty-dict>=1.3.0,<2",
   "dataclasses==0.8; python_version < '3.7.0'",
   "importlib-resources==5.7",
   "pydantic>=1.10.2,<2",
@@ -40,30 +38,35 @@
 semantic-release = "semantic_release.cli:main"
 
 [project.urls]
 "Project Url" = "http://github.com/python-semantic-release/python-semantic-release"
 Homepage = "https://python-semantic-release.readthedocs.io"
 
 [project.optional-dependencies]
+docs = [
+  "Sphinx==5.2.3",
+  "sphinxcontrib-apidoc==0.3.0",
+  "sphinx-autobuild==2021.3.14",
+]
 test = [
   "coverage[toml]>=6,<7",
   "pytest>=7,<8",
   "pytest-xdist>=2,<3",
   "pytest-mock>=3,<4",
   "pytest-lazy-fixture~=0.6.3",
   "pytest-cov>=4,<5",
   "responses==0.21.0",
   "requests-mock>=1.10.0,<2",
 ]
-docs = ["Sphinx==5.2.3", "sphinxcontrib-apidoc==0.3.0"]
 dev = ["tox", "isort", "black"]
 mypy = ["mypy", "types-requests"]
 
 [tool.pytest.ini_options]
 addopts = [
+  "-nauto",
   "-ra",
   "--cache-clear",
   "--cov=semantic_release",
   "--cov-report",
   "html:coverage-html",
   "--cov-report",
   "term",
@@ -71,15 +74,15 @@
 python_files = ["tests/test_*.py", "tests/**/test_*.py"]
 
 [tool.coverage.run]
 omit = ["*/tests/*"]
 
 [tool.isort]
 profile = "black"
-skip = [".tox", "venv"]
+skip = [".tox", "venv", ".venv"]
 combine_as_imports = true
 group_by_package = true
 default_section = "THIRDPARTY"
 known_first_party = ["semantic_release"]
 known_tests = ["tests"]
 multi_line_output = 3
 include_trailing_comma = true
@@ -96,23 +99,24 @@
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
     mypy,
-    py{37,38,39,310},
+    py{37,38,39,310,311},
     coverage
 skipsdist = True
 
 [testenv]
 passenv = CI
 setenv =
     PYTHONPATH = {toxinidir}
     TESTING = True
+    PYTHONHASHSEED = 123456
 deps = .[test]
 commands =
     coverage run -p --source=semantic_release -m pytest -v {posargs:tests}
 
 [testenv:mypy]
 deps = .[mypy]
 commands =
```

### Comparing `python-semantic-release-8.0.0a4/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.0a5/python_semantic_release.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0a4
+Version: 8.0.0a5
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 Provides-Extra: docs
+Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: mypy
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Python Semantic Release
 ***********************
```

### Comparing `python-semantic-release-8.0.0a4/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.0a5/python_semantic_release.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 python_semantic_release.egg-info/SOURCES.txt
 python_semantic_release.egg-info/dependency_links.txt
 python_semantic_release.egg-info/entry_points.txt
 python_semantic_release.egg-info/requires.txt
 python_semantic_release.egg-info/top_level.txt
 semantic_release/__init__.py
 semantic_release/__main__.py
-semantic_release/ci_checks.py
 semantic_release/const.py
 semantic_release/enums.py
 semantic_release/errors.py
 semantic_release/helpers.py
 semantic_release/changelog/__init__.py
 semantic_release/changelog/context.py
 semantic_release/changelog/release_history.py
 semantic_release/changelog/template.py
 semantic_release/cli/__init__.py
+semantic_release/cli/common.py
 semantic_release/cli/config.py
 semantic_release/cli/const.py
 semantic_release/cli/masking_filter.py
 semantic_release/cli/util.py
 semantic_release/cli/commands/__init__.py
 semantic_release/cli/commands/changelog.py
 semantic_release/cli/commands/generate_config.py
@@ -50,30 +50,30 @@
 semantic_release/hvcs/token_auth.py
 semantic_release/hvcs/util.py
 semantic_release/version/__init__.py
 semantic_release/version/algorithm.py
 semantic_release/version/declaration.py
 semantic_release/version/translator.py
 semantic_release/version/version.py
+tests/command_line/__init__.py
+tests/command_line/conftest.py
+tests/command_line/test_changelog.py
+tests/command_line/test_generate_config.py
+tests/command_line/test_help.py
+tests/command_line/test_main.py
+tests/command_line/test_version.py
 tests/fixtures/__init__.py
 tests/fixtures/commit_parsers.py
 tests/fixtures/example_project.py
 tests/fixtures/git_repo.py
 tests/fixtures/scipy.py
 tests/scenario/__init__.py
 tests/scenario/test_next_version.py
 tests/scenario/test_release_history.py
 tests/scenario/test_template_render.py
-tests/scenario/cli/__init__.py
-tests/scenario/cli/conftest.py
-tests/scenario/cli/test_changelog.py
-tests/scenario/cli/test_generate_config.py
-tests/scenario/cli/test_main.py
-tests/scenario/cli/test_publish.py
-tests/scenario/cli/test_version.py
 tests/unit/__init__.py
 tests/unit/semantic_release/__init__.py
 tests/unit/semantic_release/changelog/__init__.py
 tests/unit/semantic_release/changelog/test_changelog_context.py
 tests/unit/semantic_release/changelog/test_default_changelog.py
 tests/unit/semantic_release/changelog/test_release_notes.py
 tests/unit/semantic_release/changelog/test_template.py
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/__init__.py` & `python-semantic-release-8.0.0a5/semantic_release/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.0-alpha.4"
+__version__ = "8.0.0-alpha.5"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/changelog/context.py` & `python-semantic-release-8.0.0a5/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.0a5/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/changelog/template.py` & `python-semantic-release-8.0.0a5/semantic_release/changelog/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,39 +69,38 @@
     )
 
 
 # pylint: disable=redefined-outer-name
 def recursive_render(
     template_dir: str, environment: Environment, _root_dir: str = "."
 ) -> list[str]:
+    rendered_paths: list[str] = []
     for root, file in (
         (root, file)
         for root, _, files in os.walk(template_dir)
         for file in files
         if not any(elem.startswith(".") for elem in root.split(os.sep))
         and not file.startswith(".")
     ):
-        rendered_paths = []
         src_path = Path(root)
         output_path = (_root_dir / src_path.relative_to(template_dir)).resolve()
         log.info("Rendering templates from %s to %s", src_path, output_path)
         os.makedirs(str(output_path), exist_ok=True)
         if file.endswith(".j2"):
             # We know the file ends with .j2 by the filter in the for-loop
             output_filename = file[:-3]
             # Strip off the template directory from the front of the root path -
             # that's the output location relative to the repo root
-            output_file_path = str((src_path / file).relative_to(template_dir))
+            src_file_path = str((src_path / file).relative_to(template_dir))
+            output_file_path = str((output_path / output_filename).resolve())
 
-            log.debug("rendering %s to %s", file, output_file_path)
-            stream = environment.get_template(output_file_path).stream()
+            log.debug("rendering %s to %s", src_file_path, output_file_path)
+            stream = environment.get_template(src_file_path).stream()
 
-            with open(
-                str((output_path / output_filename).resolve()), "wb+"
-            ) as output_file:
+            with open(output_file_path, "wb+") as output_file:
                 stream.dump(output_file, encoding="utf-8")
 
             rendered_paths.append(output_file_path)
         else:
             src_file = str((src_path / file).resolve())
             target_file = str((output_path / file).resolve())
             log.debug(
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.0a5/semantic_release/cli/commands/changelog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from __future__ import annotations
 
 import logging
 import os
 
 import click
 
-# NOTE: use backport with newer API than stdlib
-from importlib_resources import files
-
 from semantic_release.changelog import ReleaseHistory, recursive_render
 from semantic_release.changelog.context import make_changelog_context
+from semantic_release.cli.common import (
+    render_default_changelog_file,
+    render_release_notes,
+)
 from semantic_release.cli.util import noop_report
 
 log = logging.getLogger(__name__)
 
 
-@click.command(short_help="Generate a changelog")
+@click.command(
+    short_help="Generate a changelog",
+    context_settings={
+        "help_option_names": ["-h", "--help"],
+    },
+)
 @click.option(
     "--post-to-release-tag",
     "release_tag",
     default=None,
     help="Post the generated changelog to the remote VCS's release for this tag",
 )
 @click.pass_context
@@ -46,27 +52,23 @@
     changelog_context = make_changelog_context(
         hvcs_client=hvcs_client, release_history=rh
     )
     changelog_context.bind_to_environment(env)
 
     if not os.path.exists(template_dir):
         log.info("Path %r not found, using default changelog template", template_dir)
-        changelog_text = (
-            files("semantic_release")
-            .joinpath("data/templates/CHANGELOG.md.j2")
-            .read_text(encoding="utf-8")
-        )
-        tmpl = env.from_string(changelog_text).stream()
         if runtime.global_cli_options.noop:
             noop_report(
                 f"would have written your changelog to {changelog_file.relative_to(repo.working_dir)}"
             )
             ctx.exit(0)
+
+        changelog_text = render_default_changelog_file(env)
         with open(str(changelog_file), "w+", encoding="utf-8") as f:
-            tmpl.dump(f)
+            f.write(changelog_text)
     else:
         if runtime.global_cli_options.noop:
             noop_report(
                 f"would have recursively rendered the template directory "
                 f"{template_dir!r} relative to {repo.working_dir!r}"
             )
             ctx.exit(0)
@@ -77,21 +79,16 @@
     elif release_tag:
         v = translator.from_tag(release_tag)
         try:
             release = rh.released[v]
         except KeyError:
             ctx.fail(f"tag {release_tag} not in release history")
 
-        release_template = (
-            files("semantic_release")
-            .joinpath("data/templates/release_notes.md.j2")
-            .read_text(encoding="utf-8")
-        )
-        release_notes = env.from_string(release_template).render(
-            version=v, release=release
+        release_notes = render_release_notes(
+            template_environment=env, version=v, release=release
         )
         version = translator.from_tag(release_tag)
         try:
             hvcs_client.create_or_update_release(
                 release_tag, release_notes, prerelease=version.is_prerelease
             )
         except Exception as e:
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.0a5/semantic_release/cli/commands/generate_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 
 import click
 import tomlkit
 
 from semantic_release.cli.config import RawConfig
 
 
-@click.command(short_help="Generate semantic-release's default configuration")
+@click.command(
+    short_help="Generate semantic-release's default configuration",
+    context_settings={
+        "help_option_names": ["-h", "--help"],
+    },
+)
 @click.option(
     "-f",
     "--format",
     "fmt",
     type=click.Choice(["toml", "json"], case_sensitive=False),
     default="toml",
     help="format for the config to be generated",
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.0a5/semantic_release/cli/commands/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,34 @@
 from __future__ import annotations
 
 import json
 import logging
 from pathlib import Path
-from typing import Any
 
 import click
-import tomlkit
 from git import InvalidGitRepositoryError
 from git.repo.base import Repo
 from rich.console import Console
 from rich.logging import RichHandler
 
 import semantic_release
 from semantic_release.cli.commands.generate_config import generate_config
 from semantic_release.cli.config import (
     GlobalCommandLineOptions,
     RawConfig,
     RuntimeContext,
+    read_toml,
 )
 from semantic_release.cli.const import DEFAULT_CONFIG_FILE
 from semantic_release.cli.util import rprint
-from semantic_release.errors import InvalidConfiguration
+from semantic_release.errors import InvalidConfiguration, NotAReleaseBranch
 
 FORMAT = "[%(name)s] %(module)s:%(funcName)s: %(message)s"
 
 
-def _read_toml(path: str) -> dict[str, Any]:
-    raw_text = (Path() / path).resolve().read_text(encoding="utf-8")
-    try:
-        toml_text = tomlkit.loads(raw_text)
-    except tomlkit.exceptions.TOMLKitError as exc:
-        raise InvalidConfiguration(f"File {path!r} contains invalid TOML") from exc
-
-    # Look for [tool.semantic_release]
-    cfg_text = toml_text.get("tool", {}).get("semantic_release")
-    if cfg_text is not None:
-        return cfg_text
-    # Look for [semantic_release]
-    cfg_text = toml_text.get("semantic_release")
-    if cfg_text is not None:
-        return cfg_text
-
-    raise InvalidConfiguration(
-        f"Missing keys 'tool.semantic_release' or 'semantic_release' in {path}"
-    )
-
-
 @click.group(
     context_settings={
         "help_option_names": ["-h", "--help"],
     },
 )
 @click.version_option(
     version=semantic_release.__version__,
@@ -104,15 +82,15 @@
     logging.basicConfig(
         level=log_level,
         format=FORMAT,
         datefmt="[%X]",
         handlers=[
             RichHandler(
                 console=console, rich_tracebacks=True, tracebacks_suppress=[click]
-            )
+            ),
         ],
     )
 
     log = logging.getLogger(__name__)
 
     if ctx.invoked_subcommand == generate_config.name:
         # generate-config doesn't require any of the usual setup,
@@ -133,31 +111,34 @@
         )
     cli_options = GlobalCommandLineOptions(
         noop=noop, verbosity=verbosity, config_file=config_file
     )
 
     try:
         if config_file and config_file.endswith(".toml"):
-            rprint(f"Loading TOML configuration from {config_file}")
-            config_text = _read_toml(config_file)
+            log.info(f"Loading TOML configuration from {config_file}")
+            config_text = read_toml(config_file)
         elif config_file and config_file.endswith(".json"):
-            rprint(f"Loading JSON configuration from {config_file}")
+            log.info(f"Loading JSON configuration from {config_file}")
             raw_text = (Path() / config_file).resolve().read_text(encoding="utf-8")
             config_text = json.loads(raw_text)["semantic_release"]
         elif config_file:
             *_, suffix = config_file.split(".")
             ctx.fail(f"{suffix!r} is not a supported configuration format")
     except (FileNotFoundError, InvalidConfiguration) as exc:
         ctx.fail(str(exc))
 
     raw_config = RawConfig.parse_obj(config_text)
     try:
         runtime = RuntimeContext.from_raw_config(
             raw_config, repo=repo, global_cli_options=cli_options
         )
+    except NotAReleaseBranch as exc:
+        rprint(f"[bold red]{str(exc)}")
+        ctx.exit(2)
     except InvalidConfiguration as exc:
         ctx.fail(str(exc))
     ctx.obj = runtime
 
     # This allows us to mask secrets in the logging
     # by applying it to all the configured handlers
     for handler in logging.getLogger().handlers:
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/cli/commands/publish.py` & `python-semantic-release-8.0.0a5/semantic_release/cli/commands/publish.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 
 from semantic_release.cli.util import noop_report
 from semantic_release.version import tags_and_versions
 
 log = logging.getLogger(__name__)
 
 
-@click.command(short_help="Build and publish a distribution")
+@click.command(
+    short_help="Build and publish a distribution",
+    context_settings={
+        "help_option_names": ["-h", "--help"],
+    },
+)
 @click.option(
     "--upload-to-repository/--no-upload-to-repository",
     "upload_to_repository",
     default=True,
     help="Whether or not to upload any built artefacts to the configured artefact repository",
 )
 @click.option(
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.0a5/semantic_release/cli/commands/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 from __future__ import annotations
 
 import logging
 import os
+from contextlib import nullcontext
 from datetime import datetime
+from typing import TYPE_CHECKING, ContextManager
 
 import click
 
-# NOTE: use backport with newer API than stdlib
-from importlib_resources import files
-
 from semantic_release.changelog import ReleaseHistory, environment, recursive_render
 from semantic_release.changelog.context import make_changelog_context
-from semantic_release.cli.util import indented, noop_report
+from semantic_release.cli.common import (
+    render_default_changelog_file,
+    render_release_notes,
+)
+from semantic_release.cli.util import indented, noop_report, rprint
+from semantic_release.const import DEFAULT_VERSION
 from semantic_release.enums import LevelBump
-from semantic_release.version import next_version, tags_and_versions
+from semantic_release.version import (
+    Version,
+    VersionTranslator,
+    next_version,
+    tags_and_versions,
+)
 
 log = logging.getLogger(__name__)
 
+if TYPE_CHECKING:
+    from git import Repo
+
+    from semantic_release.version.declaration import VersionDeclarationABC
+
 
 def is_forced_prerelease(
     force_prerelease: bool, force_level: str | None, prerelease: bool
 ) -> bool:
     """
     Determine if this release is forced to have prerelease on/off.
     If ``force_prerelease`` is set then yes.
@@ -28,15 +42,59 @@
     it's False.
     Otherwise (``force_level is None``) use the value of ``prerelease``
     """
     log.debug(", ".join(f"{k} = {v}" for k, v in locals().items()))
     return force_prerelease or ((force_level is None) and prerelease)
 
 
-@click.command(short_help="Detect and apply a new version")
+def version_from_forced_level(
+    repo: Repo, level_bump: LevelBump, translator: VersionTranslator
+) -> Version:
+    ts_and_vs = tags_and_versions(repo.tags, translator)
+
+    # If we have no tags, return the default version
+    if not ts_and_vs:
+        return Version.parse(DEFAULT_VERSION).bump(level_bump)
+
+    _, latest_version = ts_and_vs[0]
+    return latest_version.bump(level_bump)
+
+
+def apply_version_to_source_files(
+    repo: Repo,
+    version_declarations: list[VersionDeclarationABC],
+    version: Version,
+    noop: bool = False,
+) -> list[str]:
+    working_dir = os.getcwd() if repo.working_dir is None else repo.working_dir
+
+    paths = [
+        str(declaration.path.resolve().relative_to(working_dir))
+        for declaration in version_declarations
+    ]
+    if noop:
+        noop_report(
+            "would have updated versions in the following paths:"
+            + "".join(f"\n    {path}" for path in paths)
+        )
+    else:
+        log.debug("writing version %s to source paths %s", version, paths)
+        for declaration in version_declarations:
+            new_content = declaration.replace(new_version=version)
+            declaration.path.write_text(new_content)
+
+    return paths
+
+
+@click.command(
+    short_help="Detect and apply a new version",
+    context_settings={
+        "help_option_names": ["-h", "--help"],
+    },
+)
 @click.option(
     "--print", "print_only", is_flag=True, help="Print the next version and exit"
 )
 @click.option(
     "--prerelease",
     "force_prerelease",
     is_flag=True,
@@ -166,70 +224,69 @@
         )
 
     if force_level:
         level_bump = LevelBump.from_string(force_level)
         log.warning(
             "Forcing a %s level bump due to '--force' command-line option", force_level
         )
-        ts_and_vs = tags_and_versions(repo.tags, translator)
-        _, latest_version = ts_and_vs[0]
-        v = latest_version.bump(level_bump)
+
+        new_version = version_from_forced_level(
+            repo=repo, level_bump=level_bump, translator=translator
+        )
 
         # We only turn the forced version into a prerelease if the user has specified
         # that that is what they want on the command-line; otherwise we assume they are
         # forcing a full release
-        if prerelease:
-            v = v.to_prerelease()
-        else:
-            v = v.finalize_version()
+        new_version = (
+            new_version.to_prerelease(token=translator.prerelease_token)
+            if prerelease
+            else new_version.finalize_version()
+        )
 
     else:
-        v = next_version(
+        new_version = next_version(
             repo=repo,
             translator=translator,
             commit_parser=parser,
             prerelease=prerelease,
             major_on_zero=major_on_zero,
         )
 
     if build_metadata:
-        v.build_metadata = build_metadata
+        new_version.build_metadata = build_metadata
+
+    # If the new version has already been released, we fail and abort
+    if new_version in {v for _, v in tags_and_versions(repo.tags, translator)}:
+        ctx.fail(
+            f"No release will be made, {str(new_version)} has already been released!"
+        )
 
-    # Perhaps this behaviour should change if no release should be made?
-    # Or perhaps a graceful exit if the tag already exists
-    click.echo(str(v))
     if print_only:
+        click.echo(str(new_version))
         ctx.exit(0)
 
-    working_dir = os.getcwd() if repo.working_dir is None else repo.working_dir
-
-    paths = [
-        str(declaration.path.resolve().relative_to(working_dir))
-        for declaration in runtime.version_declarations
-    ]
-    log.debug("versions declared in: %s", ", ".join(paths))
-    if opts.noop:
-        noop_report(
-            "would have updated versions in the following paths:"
-            + "".join(f"\n    {path}" for path in paths)
-        )
-    else:
-        for declaration in runtime.version_declarations:
-            new_content = declaration.replace(new_version=v)
-            declaration.path.write_text(new_content)
+    rprint(
+        f"[bold green]The next version is: [white]{str(new_version)}[/white]! :rocket:"
+    )
 
-    all_paths_to_add = paths + (assets if assets else [])
-    # _head_is_new_release_commit = False
+    files_with_new_version_written = apply_version_to_source_files(
+        repo=repo,
+        version_declarations=runtime.version_declarations,
+        version=new_version,
+        noop=opts.noop,
+    )
+    all_paths_to_add = files_with_new_version_written + (assets or [])
 
+    # Commit changes
     if commit_changes and opts.noop:
         # Indents the newlines so that terminal formatting is happy - note the
         # git commit line of the output is 24 spaces indented too
         # Only this message needs such special handling because of the newlines
         # that might be in a commit message between the subject and body
-        indented_commit_message = commit_message.format(version=v).replace(
+        indented_commit_message = commit_message.format(version=new_version).replace(
             "\n\n", "\n\n" + " " * 24
         )
         noop_report(
             indented(
                 f"""
                 would have run:
                     git add {" ".join(all_paths_to_add)}
@@ -245,55 +302,55 @@
         repo=repo,
         translator=translator,
         commit_parser=parser,
         exclude_commit_patterns=changelog_excluded_commit_patterns,
     )
 
     commit_date = datetime.now()
-    rh = rh.release(
-        v, tagger=commit_author, committer=commit_author, tagged_date=commit_date
-    )
+    try:
+        rh = rh.release(
+            new_version,
+            tagger=commit_author,
+            committer=commit_author,
+            tagged_date=commit_date,
+        )
+    except ValueError as ve:
+        ctx.fail(str(ve))
 
     changelog_context = make_changelog_context(
         hvcs_client=hvcs_client, release_history=rh
     )
     changelog_context.bind_to_environment(env)
 
+    updated_paths: list[str] = []
     if update_changelog:
-        updated_paths: list[str] = []
-
         if not os.path.exists(template_dir):
             log.info(
                 "Path %r not found, using default changelog template", template_dir
             )
-            changelog_text = (
-                files("semantic_release")
-                .joinpath("data/templates/CHANGELOG.md.j2")
-                .read_text(encoding="utf-8")
-            )
-            tmpl = env.from_string(changelog_text).stream()
             if opts.noop:
                 noop_report(
                     f"would have written your changelog to {changelog_file.relative_to(repo.working_dir)}"
                 )
             else:
+                changelog_text = render_default_changelog_file(env)
                 with open(str(changelog_file), "w+", encoding="utf-8") as f:
-                    tmpl.dump(f)
+                    f.write(changelog_text)
 
-            updated_paths.append(str(changelog_file.relative_to(repo.working_dir)))
+            updated_paths = [str(changelog_file.relative_to(repo.working_dir))]
         else:
             if opts.noop:
                 noop_report(
                     f"would have recursively rendered the template directory "
                     f"{template_dir!r} relative to {repo.working_dir!r}. "
                     "Paths which would be modified by this operation cannot be "
                     "determined in no-op mode."
                 )
             else:
-                updated_paths += recursive_render(
+                updated_paths = recursive_render(
                     template_dir, environment=env, _root_dir=repo.working_dir
                 )
 
         if commit_changes and opts.noop:
             noop_report(
                 indented(
                     f"""
@@ -302,64 +359,84 @@
                     """
                 )
             )
         elif commit_changes:
             # Anything changed here should be staged.
             repo.git.add(updated_paths)
 
-    # If there are any modifications to the source code of the repository, we make
-    # a release commit to commit the CHANGELOG and other files changed by rendering
-    # to the repo, which will be the new HEAD commit
+    def custom_git_environment() -> ContextManager[None]:
+        """
+        git.custom_environment is a context manager but
+        is not reentrant, so once we have "used" it
+        we need to throw it away and re-create it in
+        order to use it again
+        """
+        return (
+            nullcontext()
+            if not commit_author
+            else repo.git.custom_environment(
+                GIT_AUTHOR_NAME=commit_author.name,
+                GIT_AUTHOR_EMAIL=commit_author.email,
+                GIT_COMMITTER_NAME=commit_author.name,
+                GIT_COMMITTER_EMAIL=commit_author.email,
+            )
+        )
 
     # If we haven't modified any source code then we skip trying to make a commit
     # and any tag that we apply will be to the HEAD commit (made outside of
     # running PSR
     if not repo.index.diff("HEAD"):
         log.info("No local changes to add to any commit, skipping")
 
     elif commit_changes and opts.noop:
-        command = "git commit -m '{commit_message.format(version=v)}'"
-        command += (
-            f" --author '{commit_author.name} <{commit_author.email}>'"
+        command = (
+            f"""\
+            GIT_AUTHOR_NAME={commit_author.name} \\
+                GIT_AUTHOR_EMAIL={commit_author.email} \\
+                GIT_COMMITTER_NAME={commit_author.name} \\
+                GIT_COMMITTER_EMAIL={commit_author.email} \\
+                """
             if commit_author
             else ""
         )
+        command += "git commit -m '{commit_message.format(version=v)}'"
 
         noop_report(
             indented(
                 f"""
                 would have run:
                     {command}
                 """
             )
         )
 
     elif commit_changes:
-        repo.git.commit(
-            m=commit_message.format(version=v),
-            author=f"{commit_author.name} <{commit_author.email}>",
-            date=int(commit_date.timestamp()),
-        )
+        with custom_git_environment():
+            repo.git.commit(
+                m=commit_message.format(version=new_version),
+                date=int(commit_date.timestamp()),
+            )
 
     # Run the tagging after potentially creating a new HEAD commit.
     # This way if no source code is modified, i.e. all metadata updates
     # are disabled, and the changelog generation is disabled or it's not
     # modified, then the HEAD commit will be tagged as a release commit
     # despite not being made by PSR
     if commit_changes and opts.noop:
         noop_report(
             indented(
                 f"""
                 would have run:
-                    git tag -a {v.as_tag()} -m "{v.as_tag()}"
+                    git tag -a {new_version.as_tag()} -m "{new_version.as_tag()}"
                 """
             )
         )
     elif commit_changes:
-        repo.git.tag("-a", v.as_tag(), m=v.as_tag())
+        with custom_git_environment():
+            repo.git.tag("-a", new_version.as_tag(), m=new_version.as_tag())
 
     if push_changes:
         remote_url = runtime.hvcs_client.remote_url(
             use_token=not runtime.ignore_token_for_push
         )
         active_branch = repo.active_branch.name
         if opts.noop:
@@ -374,34 +451,33 @@
             )
         else:
             # Wrap in GitCommandError handling - remove token
             repo.git.push(remote_url, active_branch)
             repo.git.push("--tags", remote_url, active_branch)
 
     if make_vcs_release and opts.noop:
-        noop_report(f"would have created a release for the tag {v.as_tag()!r}")
+        noop_report(
+            f"would have created a release for the tag {new_version.as_tag()!r}"
+        )
         noop_report(f"would have uploaded the following assets: {runtime.assets}")
     elif make_vcs_release:
-        release = rh.released[v]
-        release_template = (
-            files("semantic_release")
-            .joinpath("data/templates/release_notes.md.j2")
-            .read_text(encoding="utf-8")
-        )
+        release = rh.released[new_version]
         # Use a new, non-configurable environment for release notes - not user-configurable at the moment
         release_note_environment = environment(template_dir=runtime.template_dir)
         changelog_context.bind_to_environment(release_note_environment)
-        release_notes = release_note_environment.from_string(release_template).render(
-            version=v, release=release
+        release_notes = render_release_notes(
+            template_environment=release_note_environment,
+            version=new_version,
+            release=release,
         )
         try:
             release_id = hvcs_client.create_or_update_release(
-                tag=v.as_tag(),
+                tag=new_version.as_tag(),
                 release_notes=release_notes,
-                prerelease=v.is_prerelease,
+                prerelease=new_version.is_prerelease,
             )
         except Exception as e:
             log.error("%s", str(e), exc_info=True)
             ctx.fail(str(e))
         if not release_id:
             log.warning("release_id not identified, cannot upload assets")
         else:
@@ -409,8 +485,8 @@
                 log.info("Uploading asset %s", asset)
                 try:
                     hvcs_client.upload_asset(release_id, asset)
                 except Exception as e:
                     log.error("%s", str(e), exc_info=True)
                     ctx.fail(str(e))
 
-    return str(v)
+    return str(new_version)
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/cli/config.py` & `python-semantic-release-8.0.0a5/semantic_release/cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import platform
 import re
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, Optional, Tuple, Union
 
+import tomlkit
 import twine.utils
 from git import Actor
 from git.repo.base import Repo
 from jinja2 import Environment
 from pydantic import BaseModel
 from twine.exceptions import TwineException
 from twine.settings import Settings as TwineSettings
@@ -40,14 +41,35 @@
     TomlVersionDeclaration,
     VersionDeclarationABC,
 )
 
 log = logging.getLogger(__name__)
 
 
+def read_toml(path: str) -> dict[str, Any]:
+    raw_text = (Path() / path).resolve().read_text(encoding="utf-8")
+    try:
+        toml_text = tomlkit.loads(raw_text)
+    except tomlkit.exceptions.TOMLKitError as exc:
+        raise InvalidConfiguration(f"File {path!r} contains invalid TOML") from exc
+
+    # Look for [tool.semantic_release]
+    cfg_text = toml_text.get("tool", {}).get("semantic_release")
+    if cfg_text is not None:
+        return cfg_text
+    # Look for [semantic_release]
+    cfg_text = toml_text.get("semantic_release")
+    if cfg_text is not None:
+        return cfg_text
+
+    raise InvalidConfiguration(
+        f"Missing keys 'tool.semantic_release' or 'semantic_release' in {path}"
+    )
+
+
 class HvcsClient(str, Enum):
     GITHUB = "github"
     GITLAB = "gitlab"
     GITEA = "gitea"
 
 
 class EnvConfigVar(BaseModel):
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.0a5/semantic_release/cli/masking_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from __future__ import annotations
 
 import logging
 import re
 from collections import defaultdict
 from typing import Iterable
 
-# else:
-# from typing import Pattern
-
 log = logging.getLogger(__name__)
 
 
 # https://relaxdiego.com/2014/07/logging-in-python.html
 # Updated/adapted for Python3
 class MaskingFilter(logging.Filter):
     REPLACE_STR = "*" * 4
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/cli/util.py` & `python-semantic-release-8.0.0a5/semantic_release/cli/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Utilities for command-line functionality
+"""
 import sys
 from textwrap import dedent, indent
 
 import rich
 
 
 def rprint(msg: str) -> None:
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.0a5/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.0a5/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.0a5/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.0a5/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.0a5/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.0a5/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/commit_parser/token.py` & `python-semantic-release-8.0.0a5/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.0a5/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/const.py` & `python-semantic-release-8.0.0a5/semantic_release/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,7 +12,8 @@
     (?:\+(?P<buildmetadata>[0-9a-zA-Z-]+(?:\.[0-9a-zA-Z-]+)*))?
     """,
     flags=re.VERBOSE,
 )
 
 COMMIT_MESSAGE = "{version}\n\nAutomatically generated by python-semantic-release"
 DEFAULT_COMMIT_AUTHOR = "semantic-release <semantic-release>"
+DEFAULT_VERSION = "0.0.0"
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-8.0.0a5/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/enums.py` & `python-semantic-release-8.0.0a5/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/errors.py` & `python-semantic-release-8.0.0a5/semantic_release/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,13 +24,7 @@
 
 
 class CommitParseError(SemanticReleaseBaseError):
     """
     Raised when a commit cannot be parsed by a commit parser. Custom commit parsers
     should also raise this Exception
     """
-
-
-class CiVerificationError(SemanticReleaseBaseError):
-    """
-    Raised when consistency cannot be ensured within a CI environment
-    """
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/helpers.py` & `python-semantic-release-8.0.0a5/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.0a5/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.0a5/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.0a5/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/hvcs/gitlab.py` & `python-semantic-release-8.0.0a5/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.0a5/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.0a5/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.0a5/semantic_release/version/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from semantic_release.commit_parser import (
     CommitParser,
     ParsedCommit,
     ParseResult,
     ParserOptions,
 )
+from semantic_release.const import DEFAULT_VERSION
 from semantic_release.enums import LevelBump
 from semantic_release.version.translator import VersionTranslator
 from semantic_release.version.version import Version
 
 log = logging.getLogger(__name__)
 
 
@@ -225,18 +226,18 @@
         (t, v) for t, v in all_git_tags_as_versions if not v.is_prerelease
     ]
     log.info(
         "Found %s full releases (excluding prereleases)",
         len(all_full_release_tags_and_versions),
     )
 
-    # Default initial version of 0.0.0
+    # Default initial version
     latest_full_release_tag, latest_full_release_version = next(
         iter(all_full_release_tags_and_versions),
-        (None, translator.from_string("0.0.0")),
+        (None, translator.from_string(DEFAULT_VERSION)),
     )
     if latest_full_release_tag is None:
         # Workaround - we can safely scan the extra commits on this
         # branch if it's never been released, but we have no other
         # guarantees that other branches exist
         log.info(
             "No full releases have been made yet, the default version to use is %s",
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/version/declaration.py` & `python-semantic-release-8.0.0a5/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/semantic_release/version/translator.py` & `python-semantic-release-8.0.0a5/semantic_release/version/translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,20 +68,15 @@
         """
         tag_match = self.from_tag_re.match(tag)
         if not tag_match:
             raise ValueError(
                 f"Tag {tag!r} doesn't match tag format {self.tag_format!r}"
             )
         raw_version_str = tag_match.group("version")
-        m = self._VERSION_REGEX.fullmatch(raw_version_str)
-        if not m:
-            raise ValueError(
-                f"Tag {tag!r} doesn't match tag format {self.tag_format!r}"
-            )
-        return self.from_string(m.string)
+        return self.from_string(raw_version_str)
 
     def str_to_tag(self, version_str: str) -> str:
         """
         Formats a version string into a tag name
         """
         return self.tag_format.format(version=version_str)
```

### Comparing `python-semantic-release-8.0.0a4/semantic_release/version/version.py` & `python-semantic-release-8.0.0a5/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.0a5/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/fixtures/example_project.py` & `python-semantic-release-8.0.0a5/tests/fixtures/example_project.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import os
+from contextlib import contextmanager
+from pathlib import Path
 from textwrap import dedent
+from typing import Generator
 
 import pytest
 
 from tests.const import (
     EXAMPLE_CHANGELOG_MD_CONTENT,
     EXAMPLE_PROJECT_NAME,
     EXAMPLE_PROJECT_VERSION,
     EXAMPLE_PYPROJECT_TOML_CONTENT,
     EXAMPLE_SETUP_CFG_CONTENT,
     EXAMPLE_SETUP_PY_CONTENT,
 )
 
 
-@pytest.fixture
-def temp_cwd(tmp_path):
+@contextmanager
+def cd(path: Path) -> Generator[Path, None, None]:
     cwd = os.getcwd()
-    os.chdir(str(tmp_path.resolve()))
-    yield tmp_path
+    os.chdir(str(path.resolve()))
+    yield path
     os.chdir(cwd)
 
 
 @pytest.fixture
-@pytest.mark.usefixtures("temp_cwd")
 def example_project(tmp_path):
-    src_dir = tmp_path / "src"
-    src_dir.mkdir()
-    example_dir = src_dir / EXAMPLE_PROJECT_NAME
-    example_dir.mkdir()
-    init_py = example_dir / "__init__.py"
-    init_py.write_text(
-        dedent(
-            f'''
-            """
-            An example package with a very informative docstring
-            """
-            from __future__ import annotations
-
-
-            __version__ = "{EXAMPLE_PROJECT_VERSION}"
-
-            def hello_world() -> None:
-                print("Hello World")
-            '''
+    with cd(tmp_path):
+        src_dir = tmp_path / "src"
+        src_dir.mkdir()
+        example_dir = src_dir / EXAMPLE_PROJECT_NAME
+        example_dir.mkdir()
+        init_py = example_dir / "__init__.py"
+        init_py.write_text(
+            dedent(
+                f'''
+                """
+                An example package with a very informative docstring
+                """
+                __version__ = "{EXAMPLE_PROJECT_VERSION}"
+
+
+                def hello_world() -> None:
+                    print("Hello World")
+                '''
+            )
         )
-    )
-    pyproject_toml = tmp_path / "pyproject.toml"
-    pyproject_toml.write_text(EXAMPLE_PYPROJECT_TOML_CONTENT)
-    setup_cfg = tmp_path / "setup.cfg"
-    setup_cfg.write_text(EXAMPLE_SETUP_CFG_CONTENT)
-    setup_py = tmp_path / "setup.py"
-    setup_py.write_text(EXAMPLE_SETUP_PY_CONTENT)
-    template_dir = tmp_path / "templates"
-    template_dir.mkdir()
-    changelog_md = tmp_path / "CHANGELOG.md"
-    changelog_md.write_text(EXAMPLE_CHANGELOG_MD_CONTENT)
-    yield tmp_path
+        pyproject_toml = tmp_path / "pyproject.toml"
+        pyproject_toml.write_text(EXAMPLE_PYPROJECT_TOML_CONTENT)
+        setup_cfg = tmp_path / "setup.cfg"
+        setup_cfg.write_text(EXAMPLE_SETUP_CFG_CONTENT)
+        setup_py = tmp_path / "setup.py"
+        setup_py.write_text(EXAMPLE_SETUP_PY_CONTENT)
+        template_dir = tmp_path / "templates"
+        template_dir.mkdir()
+        changelog_md = tmp_path / "CHANGELOG.md"
+        changelog_md.write_text(EXAMPLE_CHANGELOG_MD_CONTENT)
+        yield tmp_path
 
 
 @pytest.fixture
 def example_pyproject_toml(example_project):
     yield example_project / "pyproject.toml"
```

### Comparing `python-semantic-release-8.0.0a4/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.0a5/tests/fixtures/git_repo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 from git import Actor, Repo
 from pytest_lazyfixture import lazy_fixture
 
 from tests.const import COMMIT_MESSAGE, EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER
-from tests.helper import add_text_to_file, shortuid
+from tests.util import add_text_to_file, shortuid
 
 
 @pytest.fixture
 def commit_author():
     yield Actor(name="semantic release testing", email="not_a_real@email.com")
 
 
@@ -386,25 +386,26 @@
     git_repo.git.commit(m="feat: add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.2.0"))
     git_repo.git.tag("v0.2.0", m="v0.2.0")
 
     assert git_repo.commit("v0.2.0").hexsha == git_repo.head.commit.hexsha
 
-    git_repo.create_head("feature")
-    git_repo.heads.feature.checkout()
+    git_repo.create_head("beta_testing")
+    git_repo.heads.beta_testing.checkout()
 
     # Do a prerelease on the branch
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="feat: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.3.0-rc.1"))
-    git_repo.git.tag("v0.3.0-rc.1", m="v0.3.0-rc.1")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.3.0-beta.1"))
+    git_repo.git.tag("v0.3.0-beta.1", m="v0.3.0-beta.1")
 
-    assert git_repo.commit("v0.3.0-rc.1").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.commit("v0.3.0-beta.1").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "beta_testing"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_main_and_feature_branches_emoji_commits(git_repo_factory, file_in_repo):
     git_repo = git_repo_factory()
@@ -435,25 +436,26 @@
     git_repo.git.commit(m=":sparkles: add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.2.0"))
     git_repo.git.tag("v0.2.0", m="v0.2.0")
 
     assert git_repo.commit("v0.2.0").hexsha == git_repo.head.commit.hexsha
 
-    git_repo.create_head("feature")
-    git_repo.heads.feature.checkout()
+    git_repo.create_head("beta_testing")
+    git_repo.heads.beta_testing.checkout()
 
     # Do a prerelease on the branch
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":sparkles: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.3.0-rc.1"))
-    git_repo.git.tag("v0.3.0-rc.1", m="v0.3.0-rc.1")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.3.0-beta.1"))
+    git_repo.git.tag("v0.3.0-beta.1", m="v0.3.0-beta.1")
 
-    assert git_repo.commit("v0.3.0-rc.1").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.commit("v0.3.0-beta.1").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "beta_testing"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_main_and_feature_branches_scipy_commits(git_repo_factory, file_in_repo):
     git_repo = git_repo_factory()
@@ -484,25 +486,26 @@
     git_repo.git.commit(m="ENH: add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.2.0"))
     git_repo.git.tag("v0.2.0", m="v0.2.0")
 
     assert git_repo.commit("v0.2.0").hexsha == git_repo.head.commit.hexsha
 
-    git_repo.create_head("feature")
-    git_repo.heads.feature.checkout()
+    git_repo.create_head("beta_testing")
+    git_repo.heads.beta_testing.checkout()
 
     # Do a prerelease on the branch
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="ENH: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.3.0-rc.1"))
-    git_repo.git.tag("v0.3.0-rc.1", m="v0.3.0-rc.1")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.3.0-beta.1"))
+    git_repo.git.tag("v0.3.0-beta.1", m="v0.3.0-beta.1")
 
-    assert git_repo.commit("v0.3.0-rc.1").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.commit("v0.3.0-beta.1").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "beta_testing"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_main_and_feature_branches_tag_commits(git_repo_factory, file_in_repo):
     git_repo = git_repo_factory()
@@ -533,25 +536,26 @@
     git_repo.git.commit(m=":sparkles: add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.2.0"))
     git_repo.git.tag("v0.2.0", m="v0.2.0")
 
     assert git_repo.commit("v0.2.0").hexsha == git_repo.head.commit.hexsha
 
-    git_repo.create_head("feature")
-    git_repo.heads.feature.checkout()
+    git_repo.create_head("beta_testing")
+    git_repo.heads.beta_testing.checkout()
 
     # Do a prerelease on the branch
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":sparkles: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.3.0-rc.1"))
-    git_repo.git.tag("v0.3.0-rc.1", m="v0.3.0-rc.1")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="0.3.0-beta.1"))
+    git_repo.git.tag("v0.3.0-beta.1", m="v0.3.0-beta.1")
 
-    assert git_repo.commit("v0.3.0-rc.1").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.commit("v0.3.0-beta.1").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "beta_testing"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_git_flow_angular_commits(git_repo_factory, file_in_repo):
     git_repo = git_repo_factory()
@@ -606,26 +610,27 @@
     git_repo.create_head("feature")
     git_repo.heads.feature.checkout()
 
     # Do a prerelease on the branch
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="feat: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-rc.1"))
-    git_repo.git.tag("v1.2.0-rc.1", m="v1.2.0-rc.1")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-alpha.1"))
+    git_repo.git.tag("v1.2.0-alpha.1", m="v1.2.0-alpha.1")
 
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="feat: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="fix: (feature) add some missing text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-rc.2"))
-    git_repo.git.tag("v1.2.0-rc.2", m="v1.2.0-rc.2")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-alpha.2"))
+    git_repo.git.tag("v1.2.0-alpha.2", m="v1.2.0-alpha.2")
 
-    assert git_repo.commit("v1.2.0-rc.2").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.commit("v1.2.0-alpha.2").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_git_flow_emoji_commits(git_repo_factory, file_in_repo):
     git_repo = git_repo_factory()
@@ -680,26 +685,27 @@
     git_repo.create_head("feature")
     git_repo.heads.feature.checkout()
 
     # Do a prerelease on the branch
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":sparkles: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-rc.1"))
-    git_repo.git.tag("v1.2.0-rc.1", m="v1.2.0-rc.1")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-alpha.1"))
+    git_repo.git.tag("v1.2.0-alpha.1", m="v1.2.0-alpha.1")
 
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":sparkles: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":bug: (feature) add some missing text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-rc.2"))
-    git_repo.git.tag("v1.2.0-rc.2", m="v1.2.0-rc.2")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-alpha.2"))
+    git_repo.git.tag("v1.2.0-alpha.2", m="v1.2.0-alpha.2")
 
-    assert git_repo.commit("v1.2.0-rc.2").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.commit("v1.2.0-alpha.2").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_git_flow_scipy_commits(git_repo_factory, file_in_repo):
     git_repo = git_repo_factory()
@@ -754,26 +760,27 @@
     git_repo.create_head("feature")
     git_repo.heads.feature.checkout()
 
     # Do a prerelease on the branch
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="ENH: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-rc.1"))
-    git_repo.git.tag("v1.2.0-rc.1", m="v1.2.0-rc.1")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-alpha.1"))
+    git_repo.git.tag("v1.2.0-alpha.1", m="v1.2.0-alpha.1")
 
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="ENH: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="MAINT: (feature) add some missing text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-rc.2"))
-    git_repo.git.tag("v1.2.0-rc.2", m="v1.2.0-rc.2")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-alpha.2"))
+    git_repo.git.tag("v1.2.0-alpha.2", m="v1.2.0-alpha.2")
 
-    assert git_repo.commit("v1.2.0-rc.2").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.commit("v1.2.0-alpha.2").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_git_flow_tag_commits(git_repo_factory, file_in_repo):
     git_repo = git_repo_factory()
@@ -830,26 +837,27 @@
     git_repo.create_head("feature")
     git_repo.heads.feature.checkout()
 
     # Do a prerelease on the branch
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":sparkles: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-rc.1"))
-    git_repo.git.tag("v1.2.0-rc.1", m="v1.2.0-rc.1")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-alpha.1"))
+    git_repo.git.tag("v1.2.0-alpha.1", m="v1.2.0-alpha.1")
 
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":sparkles: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":nut_and_bolt: (feature) add some missing text")
     add_text_to_file(git_repo, file_in_repo)
-    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-rc.2"))
-    git_repo.git.tag("v1.2.0-rc.2", m="v1.2.0-rc.2")
+    git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.2.0-alpha.2"))
+    git_repo.git.tag("v1.2.0-alpha.2", m="v1.2.0-alpha.2")
 
-    assert git_repo.commit("v1.2.0-rc.2").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.commit("v1.2.0-alpha.2").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_git_flow_and_release_channels_angular_commits(
     git_repo_factory, file_in_repo
@@ -924,14 +932,15 @@
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="fix: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-alpha.3"))
     git_repo.git.tag("v1.1.0-alpha.3", m="v1.1.0-alpha.3")
 
     assert git_repo.commit("v1.1.0-alpha.3").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_git_flow_and_release_channels_emoji_commits(
     git_repo_factory, file_in_repo
@@ -1006,14 +1015,15 @@
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":bug: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-alpha.3"))
     git_repo.git.tag("v1.1.0-alpha.3", m="v1.1.0-alpha.3")
 
     assert git_repo.commit("v1.1.0-alpha.3").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_git_flow_and_release_channels_scipy_commits(
     git_repo_factory, file_in_repo
@@ -1088,14 +1098,15 @@
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m="MAINT: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-alpha.3"))
     git_repo.git.tag("v1.1.0-alpha.3", m="v1.1.0-alpha.3")
 
     assert git_repo.commit("v1.1.0-alpha.3").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
 
 
 @pytest.fixture
 def repo_with_git_flow_and_release_channels_tag_commits(git_repo_factory, file_in_repo):
     git_repo = git_repo_factory()
@@ -1170,9 +1181,10 @@
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=":nut_and_bolt: (feature) add some more text")
     add_text_to_file(git_repo, file_in_repo)
     git_repo.git.commit(m=COMMIT_MESSAGE.format(version="1.1.0-alpha.3"))
     git_repo.git.tag("v1.1.0-alpha.3", m="v1.1.0-alpha.3")
 
     assert git_repo.commit("v1.1.0-alpha.3").hexsha == git_repo.head.commit.hexsha
+    assert git_repo.active_branch.name == "feature"
     yield git_repo
     git_repo.close()
```

### Comparing `python-semantic-release-8.0.0a4/tests/fixtures/scipy.py` & `python-semantic-release-8.0.0a5/tests/fixtures/scipy.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     ScipyCommitParser,
     ScipyParserOptions,
     tag_to_section,
 )
 from semantic_release.enums import LevelBump
 
 from tests.const import SCIPY_FORMATTED_COMMIT_BODY_PARTS
+from tests.util import xdist_sort_hack
 
 
 @pytest.fixture
 def default_scipy_parser_options():
     yield ScipyCommitParser.parser_options()
 
 
@@ -25,29 +26,31 @@
 
 @pytest.fixture(params=tag_to_section.keys())
 def scipy_tag(request):
     return request.param
 
 
 @pytest.fixture(
-    params=[
-        "scipy.stats.qmc: centered-discrepancy optimization of a Latin hypercube",
-        "inverse missing in idstn, idctn (#14479)",
-        "Merge pull request #14447 from AnirudhDagar/rename_ndimage_modules",
-        "Add tests for args kwarg in quad_vec",
-        "badge with version of the doc in the navbar (#14132)",
-        "Bump scipy from 1.7.0 to 1.7.1 (#28)",
-        "avoid nan if angle=0 in RotvecRotation",
-    ]
+    params=xdist_sort_hack(
+        [
+            "scipy.stats.qmc: centered-discrepancy optimization of a Latin hypercube",
+            "inverse missing in idstn, idctn (#14479)",
+            "Merge pull request #14447 from AnirudhDagar/rename_ndimage_modules",
+            "Add tests for args kwarg in quad_vec",
+            "badge with version of the doc in the navbar (#14132)",
+            "Bump scipy from 1.7.0 to 1.7.1 (#28)",
+            "avoid nan if angle=0 in RotvecRotation",
+        ]
+    )
 )
 def subject(request):
     return request.param
 
 
-@pytest.fixture(params=SCIPY_FORMATTED_COMMIT_BODY_PARTS)
+@pytest.fixture(params=xdist_sort_hack(SCIPY_FORMATTED_COMMIT_BODY_PARTS))
 def body_parts(request):
     return request.param
 
 
 @pytest.fixture()
 def expected_response_scipy(
     default_scipy_parser_options, scipy_tag, subject, body_parts
@@ -66,29 +69,37 @@
 
 @pytest.fixture
 def valid_scipy_commit(scipy_tag, subject, body_parts):
     return _make_scipy_commit(scipy_tag, subject, body_parts)
 
 
 @pytest.fixture(
-    params=[
-        k for k, v in ScipyParserOptions().tag_to_level.items() if v is LevelBump.PATCH
-    ]
+    params=xdist_sort_hack(
+        [
+            k
+            for k, v in ScipyParserOptions().tag_to_level.items()
+            if v is LevelBump.PATCH
+        ]
+    )
 )
 def scipy_commits_patch(request, subject):
     yield [
         _make_scipy_commit(request.param, subject, body_parts)
         for body_parts in SCIPY_FORMATTED_COMMIT_BODY_PARTS
     ]
 
 
 @pytest.fixture(
-    params=[
-        k for k, v in ScipyParserOptions().tag_to_level.items() if v is LevelBump.MINOR
-    ]
+    params=xdist_sort_hack(
+        [
+            k
+            for k, v in ScipyParserOptions().tag_to_level.items()
+            if v is LevelBump.MINOR
+        ]
+    )
 )
 def scipy_commits_minor(request, subject, default_scipy_parser_options):
     patch_tags = [
         k
         for k, v in default_scipy_parser_options.tag_to_level.items()
         if v is LevelBump.PATCH
     ]
@@ -104,17 +115,21 @@
         chain.from_iterable(
             zip_longest(minor_commits, patch_commits, fillvalue="uninteresting")
         )
     )
 
 
 @pytest.fixture(
-    params=[
-        k for k, v in ScipyParserOptions().tag_to_level.items() if v is LevelBump.MAJOR
-    ]
+    params=xdist_sort_hack(
+        [
+            k
+            for k, v in ScipyParserOptions().tag_to_level.items()
+            if v is LevelBump.MAJOR
+        ]
+    )
 )
 def scipy_commits_major(request, subject, default_scipy_parser_options):
     patch_tags = [
         k
         for k, v in default_scipy_parser_options.tag_to_level.items()
         if v is LevelBump.PATCH
     ]
```

### Comparing `python-semantic-release-8.0.0a4/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.0a5/tests/scenario/test_next_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     EMOJI_COMMITS_MAJOR,
     EMOJI_COMMITS_MINOR,
     EMOJI_COMMITS_PATCH,
     TAG_COMMITS_MAJOR,
     TAG_COMMITS_MINOR,
     TAG_COMMITS_PATCH,
 )
-from tests.helper import add_text_to_file
+from tests.util import add_text_to_file, xdist_sort_hack
 
 # TODO: it'd be nice to not hard-code the versions into
 # this testing
 
 
 # NOTE: There is a bit of a corner-case where if we are not doing a
 # prerelease, we will get a full version based on already-released commits.
@@ -32,68 +32,73 @@
 # which previously triggered a prerelease on a branch will subsequently trigger a full
 # release when merged to a full release branch where prerelease=False.
 # For this reason a couple of these test cases predict a new version even when the
 # commits being added here don't induce a version bump.
 @pytest.mark.parametrize(
     "repo, commit_parser, translator, commit_messages,"
     "prerelease, expected_new_version",
-    [
-        (
-            lazy_fixture(repo_fixture_name),
-            lazy_fixture(parser_fixture_name),
-            translator,
-            commit_messages,
-            prerelease,
-            expected_new_version,
-        )
-        for (repo_fixture_name, parser_fixture_name, translator), values in {
-            # Latest version for repo_with_git_flow is currently 1.2.0-rc.2
-            # The last full release version was 1.1.1, so it's had a minor prerelease
+    xdist_sort_hack(
+        [
             (
-                "repo_with_git_flow_angular_commits",
-                "default_angular_parser",
-                VersionTranslator(),
-            ): [
-                *((commits, True, "1.2.0-rc.2") for commits in ([], ["uninteresting"])),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *((commits, False, "1.2.0") for commits in ([], ["uninteresting"])),
-                (ANGULAR_COMMITS_PATCH, False, "1.2.0"),
-                (ANGULAR_COMMITS_PATCH, True, "1.2.0-rc.3"),
-                (ANGULAR_COMMITS_MINOR, False, "1.2.0"),
-                (ANGULAR_COMMITS_MINOR, True, "1.2.0-rc.3"),
-                (ANGULAR_COMMITS_MAJOR, False, "2.0.0"),
-                (ANGULAR_COMMITS_MAJOR, True, "2.0.0-rc.1"),
-            ],
-            # Latest version for repo_with_git_flow_and_release_channels is currently 1.1.0-alpha.3
-            # The last full release version was 1.0.0, so it's had a minor prerelease
-            (
-                "repo_with_git_flow_and_release_channels_angular_commits",
-                "default_angular_parser",
-                VersionTranslator(prerelease_token="alpha"),
-            ): [
-                *(
-                    (commits, True, "1.1.0-alpha.3")
-                    for commits in ([], ["uninteresting"])
-                ),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *((commits, False, "1.1.0") for commits in ([], ["uninteresting"])),
-                (ANGULAR_COMMITS_PATCH, False, "1.1.0"),
-                (ANGULAR_COMMITS_PATCH, True, "1.1.0-alpha.4"),
-                (ANGULAR_COMMITS_MINOR, False, "1.1.0"),
-                (ANGULAR_COMMITS_MINOR, True, "1.1.0-alpha.4"),
-                (ANGULAR_COMMITS_MAJOR, False, "2.0.0"),
-                (ANGULAR_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
-            ],
-        }.items()
-        for (commit_messages, prerelease, expected_new_version) in values
-    ],
+                lazy_fixture(repo_fixture_name),
+                lazy_fixture(parser_fixture_name),
+                translator,
+                commit_messages,
+                prerelease,
+                expected_new_version,
+            )
+            for (repo_fixture_name, parser_fixture_name, translator), values in {
+                # Latest version for repo_with_git_flow is currently 1.2.0-rc.2
+                # The last full release version was 1.1.1, so it's had a minor prerelease
+                (
+                    "repo_with_git_flow_angular_commits",
+                    "default_angular_parser",
+                    VersionTranslator(prerelease_token="alpha"),
+                ): [
+                    *(
+                        (commits, True, "1.2.0-alpha.2")
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *((commits, False, "1.2.0") for commits in ([], ["uninteresting"])),
+                    (ANGULAR_COMMITS_PATCH, False, "1.2.0"),
+                    (ANGULAR_COMMITS_PATCH, True, "1.2.0-alpha.3"),
+                    (ANGULAR_COMMITS_MINOR, False, "1.2.0"),
+                    (ANGULAR_COMMITS_MINOR, True, "1.2.0-alpha.3"),
+                    (ANGULAR_COMMITS_MAJOR, False, "2.0.0"),
+                    (ANGULAR_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
+                ],
+                # Latest version for repo_with_git_flow_and_release_channels is currently 1.1.0-alpha.3
+                # The last full release version was 1.0.0, so it's had a minor prerelease
+                (
+                    "repo_with_git_flow_and_release_channels_angular_commits",
+                    "default_angular_parser",
+                    VersionTranslator(prerelease_token="alpha"),
+                ): [
+                    *(
+                        (commits, True, "1.1.0-alpha.3")
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *((commits, False, "1.1.0") for commits in ([], ["uninteresting"])),
+                    (ANGULAR_COMMITS_PATCH, False, "1.1.0"),
+                    (ANGULAR_COMMITS_PATCH, True, "1.1.0-alpha.4"),
+                    (ANGULAR_COMMITS_MINOR, False, "1.1.0"),
+                    (ANGULAR_COMMITS_MINOR, True, "1.1.0-alpha.4"),
+                    (ANGULAR_COMMITS_MAJOR, False, "2.0.0"),
+                    (ANGULAR_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
+                ],
+            }.items()
+            for (commit_messages, prerelease, expected_new_version) in values
+        ]
+    ),
 )
-@pytest.mark.parametrize("major_on_zero", (True, False))
+@pytest.mark.parametrize("major_on_zero", [True, False])
 def test_algorithm_no_zero_dot_versions_angular(
     repo,
     file_in_repo,
     commit_parser,
     translator,
     commit_messages,
     prerelease,
@@ -112,68 +117,73 @@
         expected_new_version, prerelease_token=translator.prerelease_token
     )
 
 
 @pytest.mark.parametrize(
     "repo, commit_parser, translator, commit_messages,"
     "prerelease, expected_new_version",
-    [
-        (
-            lazy_fixture(repo_fixture_name),
-            lazy_fixture(parser_fixture_name),
-            translator,
-            commit_messages,
-            prerelease,
-            expected_new_version,
-        )
-        for (repo_fixture_name, parser_fixture_name, translator), values in {
-            # Latest version for repo_with_git_flow is currently 1.2.0-rc.2
-            # The last full release version was 1.1.1, so it's had a minor prerelease
-            (
-                "repo_with_git_flow_emoji_commits",
-                "default_emoji_parser",
-                VersionTranslator(),
-            ): [
-                *((commits, True, "1.2.0-rc.2") for commits in ([], ["uninteresting"])),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *((commits, False, "1.2.0") for commits in ([], ["uninteresting"])),
-                (EMOJI_COMMITS_PATCH, False, "1.2.0"),
-                (EMOJI_COMMITS_PATCH, True, "1.2.0-rc.3"),
-                (EMOJI_COMMITS_MINOR, False, "1.2.0"),
-                (EMOJI_COMMITS_MINOR, True, "1.2.0-rc.3"),
-                (EMOJI_COMMITS_MAJOR, False, "2.0.0"),
-                (EMOJI_COMMITS_MAJOR, True, "2.0.0-rc.1"),
-            ],
-            # Latest version for repo_with_git_flow_and_release_channels is currently 1.1.0-alpha.3
-            # The last full release version was 1.0.0, so it's had a minor prerelease
+    xdist_sort_hack(
+        [
             (
-                "repo_with_git_flow_and_release_channels_emoji_commits",
-                "default_emoji_parser",
-                VersionTranslator(prerelease_token="alpha"),
-            ): [
-                *(
-                    (commits, True, "1.1.0-alpha.3")
-                    for commits in ([], ["uninteresting"])
-                ),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *((commits, False, "1.1.0") for commits in ([], ["uninteresting"])),
-                (EMOJI_COMMITS_PATCH, False, "1.1.0"),
-                (EMOJI_COMMITS_PATCH, True, "1.1.0-alpha.4"),
-                (EMOJI_COMMITS_MINOR, False, "1.1.0"),
-                (EMOJI_COMMITS_MINOR, True, "1.1.0-alpha.4"),
-                (EMOJI_COMMITS_MAJOR, False, "2.0.0"),
-                (EMOJI_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
-            ],
-        }.items()
-        for (commit_messages, prerelease, expected_new_version) in values
-    ],
+                lazy_fixture(repo_fixture_name),
+                lazy_fixture(parser_fixture_name),
+                translator,
+                commit_messages,
+                prerelease,
+                expected_new_version,
+            )
+            for (repo_fixture_name, parser_fixture_name, translator), values in {
+                # Latest version for repo_with_git_flow is currently 1.2.0-alpha.2
+                # The last full release version was 1.1.1, so it's had a minor prerelease
+                (
+                    "repo_with_git_flow_emoji_commits",
+                    "default_emoji_parser",
+                    VersionTranslator(prerelease_token="alpha"),
+                ): [
+                    *(
+                        (commits, True, "1.2.0-alpha.2")
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *((commits, False, "1.2.0") for commits in ([], ["uninteresting"])),
+                    (EMOJI_COMMITS_PATCH, False, "1.2.0"),
+                    (EMOJI_COMMITS_PATCH, True, "1.2.0-alpha.3"),
+                    (EMOJI_COMMITS_MINOR, False, "1.2.0"),
+                    (EMOJI_COMMITS_MINOR, True, "1.2.0-alpha.3"),
+                    (EMOJI_COMMITS_MAJOR, False, "2.0.0"),
+                    (EMOJI_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
+                ],
+                # Latest version for repo_with_git_flow_and_release_channels is currently 1.1.0-alpha.3
+                # The last full release version was 1.0.0, so it's had a minor prerelease
+                (
+                    "repo_with_git_flow_and_release_channels_emoji_commits",
+                    "default_emoji_parser",
+                    VersionTranslator(prerelease_token="alpha"),
+                ): [
+                    *(
+                        (commits, True, "1.1.0-alpha.3")
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *((commits, False, "1.1.0") for commits in ([], ["uninteresting"])),
+                    (EMOJI_COMMITS_PATCH, False, "1.1.0"),
+                    (EMOJI_COMMITS_PATCH, True, "1.1.0-alpha.4"),
+                    (EMOJI_COMMITS_MINOR, False, "1.1.0"),
+                    (EMOJI_COMMITS_MINOR, True, "1.1.0-alpha.4"),
+                    (EMOJI_COMMITS_MAJOR, False, "2.0.0"),
+                    (EMOJI_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
+                ],
+            }.items()
+            for (commit_messages, prerelease, expected_new_version) in values
+        ]
+    ),
 )
-@pytest.mark.parametrize("major_on_zero", (True, False))
+@pytest.mark.parametrize("major_on_zero", [True, False])
 def test_algorithm_no_zero_dot_versions_emoji(
     repo,
     file_in_repo,
     commit_parser,
     translator,
     commit_messages,
     prerelease,
@@ -192,68 +202,73 @@
         expected_new_version, prerelease_token=translator.prerelease_token
     )
 
 
 @pytest.mark.parametrize(
     "repo, commit_parser, translator, commit_messages,"
     "prerelease, expected_new_version",
-    [
-        (
-            lazy_fixture(repo_fixture_name),
-            lazy_fixture(parser_fixture_name),
-            translator,
-            commit_messages,
-            prerelease,
-            expected_new_version,
-        )
-        for (repo_fixture_name, parser_fixture_name, translator), values in {
-            # Latest version for repo_with_git_flow is currently 1.2.0-rc.2
-            # The last full release version was 1.1.1, so it's had a minor prerelease
+    xdist_sort_hack(
+        [
             (
-                "repo_with_git_flow_scipy_commits",
-                "default_scipy_parser",
-                VersionTranslator(),
-            ): [
-                *((commits, True, "1.2.0-rc.2") for commits in ([], ["uninteresting"])),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *((commits, False, "1.2.0") for commits in ([], ["uninteresting"])),
-                (lazy_fixture("scipy_commits_patch"), False, "1.2.0"),
-                (lazy_fixture("scipy_commits_patch"), True, "1.2.0-rc.3"),
-                (lazy_fixture("scipy_commits_minor"), False, "1.2.0"),
-                (lazy_fixture("scipy_commits_minor"), True, "1.2.0-rc.3"),
-                (lazy_fixture("scipy_commits_major"), False, "2.0.0"),
-                (lazy_fixture("scipy_commits_major"), True, "2.0.0-rc.1"),
-            ],
-            # Latest version for repo_with_git_flow_and_release_channels is currently 1.1.0-alpha.3
-            # The last full release version was 1.0.0, so it's had a minor prerelease
-            (
-                "repo_with_git_flow_and_release_channels_scipy_commits",
-                "default_scipy_parser",
-                VersionTranslator(prerelease_token="alpha"),
-            ): [
-                *(
-                    (commits, True, "1.1.0-alpha.3")
-                    for commits in ([], ["uninteresting"])
-                ),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *((commits, False, "1.1.0") for commits in ([], ["uninteresting"])),
-                (lazy_fixture("scipy_commits_patch"), False, "1.1.0"),
-                (lazy_fixture("scipy_commits_patch"), True, "1.1.0-alpha.4"),
-                (lazy_fixture("scipy_commits_minor"), False, "1.1.0"),
-                (lazy_fixture("scipy_commits_minor"), True, "1.1.0-alpha.4"),
-                (lazy_fixture("scipy_commits_major"), False, "2.0.0"),
-                (lazy_fixture("scipy_commits_major"), True, "2.0.0-alpha.1"),
-            ],
-        }.items()
-        for (commit_messages, prerelease, expected_new_version) in values
-    ],
+                lazy_fixture(repo_fixture_name),
+                lazy_fixture(parser_fixture_name),
+                translator,
+                commit_messages,
+                prerelease,
+                expected_new_version,
+            )
+            for (repo_fixture_name, parser_fixture_name, translator), values in {
+                # Latest version for repo_with_git_flow is currently 1.2.0-alpha.2
+                # The last full release version was 1.1.1, so it's had a minor prerelease
+                (
+                    "repo_with_git_flow_scipy_commits",
+                    "default_scipy_parser",
+                    VersionTranslator(prerelease_token="alpha"),
+                ): [
+                    *(
+                        (commits, True, "1.2.0-alpha.2")
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *((commits, False, "1.2.0") for commits in ([], ["uninteresting"])),
+                    (lazy_fixture("scipy_commits_patch"), False, "1.2.0"),
+                    (lazy_fixture("scipy_commits_patch"), True, "1.2.0-alpha.3"),
+                    (lazy_fixture("scipy_commits_minor"), False, "1.2.0"),
+                    (lazy_fixture("scipy_commits_minor"), True, "1.2.0-alpha.3"),
+                    (lazy_fixture("scipy_commits_major"), False, "2.0.0"),
+                    (lazy_fixture("scipy_commits_major"), True, "2.0.0-alpha.1"),
+                ],
+                # Latest version for repo_with_git_flow_and_release_channels is currently 1.1.0-alpha.3
+                # The last full release version was 1.0.0, so it's had a minor prerelease
+                (
+                    "repo_with_git_flow_and_release_channels_scipy_commits",
+                    "default_scipy_parser",
+                    VersionTranslator(prerelease_token="alpha"),
+                ): [
+                    *(
+                        (commits, True, "1.1.0-alpha.3")
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *((commits, False, "1.1.0") for commits in ([], ["uninteresting"])),
+                    (lazy_fixture("scipy_commits_patch"), False, "1.1.0"),
+                    (lazy_fixture("scipy_commits_patch"), True, "1.1.0-alpha.4"),
+                    (lazy_fixture("scipy_commits_minor"), False, "1.1.0"),
+                    (lazy_fixture("scipy_commits_minor"), True, "1.1.0-alpha.4"),
+                    (lazy_fixture("scipy_commits_major"), False, "2.0.0"),
+                    (lazy_fixture("scipy_commits_major"), True, "2.0.0-alpha.1"),
+                ],
+            }.items()
+            for (commit_messages, prerelease, expected_new_version) in values
+        ]
+    ),
 )
-@pytest.mark.parametrize("major_on_zero", (True, False))
+@pytest.mark.parametrize("major_on_zero", [True, False])
 def test_algorithm_no_zero_dot_versions_scipy(
     repo,
     file_in_repo,
     commit_parser,
     translator,
     commit_messages,
     prerelease,
@@ -272,68 +287,73 @@
         expected_new_version, prerelease_token=translator.prerelease_token
     )
 
 
 @pytest.mark.parametrize(
     "repo, commit_parser, translator, commit_messages,"
     "prerelease, expected_new_version",
-    [
-        (
-            lazy_fixture(repo_fixture_name),
-            lazy_fixture(parser_fixture_name),
-            translator,
-            commit_messages,
-            prerelease,
-            expected_new_version,
-        )
-        for (repo_fixture_name, parser_fixture_name, translator), values in {
-            # Latest version for repo_with_git_flow is currently 1.2.0-rc.2
-            # The last full release version was 1.1.1, so it's had a minor prerelease
-            (
-                "repo_with_git_flow_tag_commits",
-                "default_tag_parser",
-                VersionTranslator(),
-            ): [
-                *((commits, True, "1.2.0-rc.2") for commits in ([], ["uninteresting"])),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *((commits, False, "1.2.0") for commits in ([], ["uninteresting"])),
-                (TAG_COMMITS_PATCH, False, "1.2.0"),
-                (TAG_COMMITS_PATCH, True, "1.2.0-rc.3"),
-                (TAG_COMMITS_MINOR, False, "1.2.0"),
-                (TAG_COMMITS_MINOR, True, "1.2.0-rc.3"),
-                (TAG_COMMITS_MAJOR, False, "2.0.0"),
-                (TAG_COMMITS_MAJOR, True, "2.0.0-rc.1"),
-            ],
-            # Latest version for repo_with_git_flow_and_release_channels is currently 1.1.0-alpha.3
-            # The last full release version was 1.0.0, so it's had a minor prerelease
+    xdist_sort_hack(
+        [
             (
-                "repo_with_git_flow_and_release_channels_tag_commits",
-                "default_tag_parser",
-                VersionTranslator(prerelease_token="alpha"),
-            ): [
-                *(
-                    (commits, True, "1.1.0-alpha.3")
-                    for commits in ([], ["uninteresting"])
-                ),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *((commits, False, "1.1.0") for commits in ([], ["uninteresting"])),
-                (TAG_COMMITS_PATCH, False, "1.1.0"),
-                (TAG_COMMITS_PATCH, True, "1.1.0-alpha.4"),
-                (TAG_COMMITS_MINOR, False, "1.1.0"),
-                (TAG_COMMITS_MINOR, True, "1.1.0-alpha.4"),
-                (TAG_COMMITS_MAJOR, False, "2.0.0"),
-                (TAG_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
-            ],
-        }.items()
-        for (commit_messages, prerelease, expected_new_version) in values
-    ],
+                lazy_fixture(repo_fixture_name),
+                lazy_fixture(parser_fixture_name),
+                translator,
+                commit_messages,
+                prerelease,
+                expected_new_version,
+            )
+            for (repo_fixture_name, parser_fixture_name, translator), values in {
+                # Latest version for repo_with_git_flow is currently 1.2.0-rc.2
+                # The last full release version was 1.1.1, so it's had a minor prerelease
+                (
+                    "repo_with_git_flow_tag_commits",
+                    "default_tag_parser",
+                    VersionTranslator(prerelease_token="alpha"),
+                ): [
+                    *(
+                        (commits, True, "1.2.0-alpha.2")
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *((commits, False, "1.2.0") for commits in ([], ["uninteresting"])),
+                    (TAG_COMMITS_PATCH, False, "1.2.0"),
+                    (TAG_COMMITS_PATCH, True, "1.2.0-alpha.3"),
+                    (TAG_COMMITS_MINOR, False, "1.2.0"),
+                    (TAG_COMMITS_MINOR, True, "1.2.0-alpha.3"),
+                    (TAG_COMMITS_MAJOR, False, "2.0.0"),
+                    (TAG_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
+                ],
+                # Latest version for repo_with_git_flow_and_release_channels is currently 1.1.0-alpha.3
+                # The last full release version was 1.0.0, so it's had a minor prerelease
+                (
+                    "repo_with_git_flow_and_release_channels_tag_commits",
+                    "default_tag_parser",
+                    VersionTranslator(prerelease_token="alpha"),
+                ): [
+                    *(
+                        (commits, True, "1.1.0-alpha.3")
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *((commits, False, "1.1.0") for commits in ([], ["uninteresting"])),
+                    (TAG_COMMITS_PATCH, False, "1.1.0"),
+                    (TAG_COMMITS_PATCH, True, "1.1.0-alpha.4"),
+                    (TAG_COMMITS_MINOR, False, "1.1.0"),
+                    (TAG_COMMITS_MINOR, True, "1.1.0-alpha.4"),
+                    (TAG_COMMITS_MAJOR, False, "2.0.0"),
+                    (TAG_COMMITS_MAJOR, True, "2.0.0-alpha.1"),
+                ],
+            }.items()
+            for (commit_messages, prerelease, expected_new_version) in values
+        ]
+    ),
 )
-@pytest.mark.parametrize("major_on_zero", (True, False))
+@pytest.mark.parametrize("major_on_zero", [True, False])
 def test_algorithm_no_zero_dot_versions_tag(
     repo,
     file_in_repo,
     commit_parser,
     translator,
     commit_messages,
     prerelease,
@@ -357,148 +377,155 @@
 # 0.x.y versions
 #####
 
 
 @pytest.mark.parametrize(
     "repo, commit_parser, translator, commit_messages,"
     "prerelease, major_on_zero, expected_new_version",
-    [
-        (
-            lazy_fixture(repo_fixture_name),
-            lazy_fixture(parser_fixture_name),
-            translator,
-            commit_messages,
-            prerelease,
-            major_on_zero,
-            expected_new_version,
-        )
-        for (repo_fixture_name, parser_fixture_name, translator), values in {
-            # Latest version for repo_with_no_tags is currently 0.0.0 (default)
-            # It's biggest change type is minor, so the next version should be 0.1.0
+    xdist_sort_hack(
+        [
             (
-                "repo_with_no_tags_angular_commits",
-                "default_angular_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, False, major_on_zero, "0.1.0")
-                    for major_on_zero in (True, False)
-                    for commits in (
-                        [],
-                        ["uninteresting"],
-                        ANGULAR_COMMITS_PATCH,
-                        ANGULAR_COMMITS_MINOR,
-                    )
-                ),
-                (ANGULAR_COMMITS_MAJOR, False, False, "0.1.0"),
-                (ANGULAR_COMMITS_MAJOR, False, True, "1.0.0"),
-            ],
-            # Latest version for repo_with_single_branch is currently 0.1.1
-            # Note repo_with_single_branch isn't modelled with prereleases
-            (
-                "repo_with_single_branch_angular_commits",
-                "default_angular_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, False, major_on_zero, "0.1.1")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (ANGULAR_COMMITS_PATCH, False, major_on_zero, "0.1.2")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (ANGULAR_COMMITS_MINOR, False, major_on_zero, "0.2.0")
-                    for major_on_zero in (True, False)
-                ),
-                (ANGULAR_COMMITS_MAJOR, False, False, "0.2.0"),
-                (ANGULAR_COMMITS_MAJOR, False, True, "1.0.0"),
-            ],
-            # Latest version for repo_with_single_branch_and_prereleases is currently 0.2.0
-            (
-                "repo_with_single_branch_and_prereleases_angular_commits",
-                "default_angular_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, prerelease, major_on_zero, "0.2.0")
-                    for prerelease in (True, False)
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (ANGULAR_COMMITS_PATCH, False, major_on_zero, "0.2.1")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (ANGULAR_COMMITS_PATCH, True, major_on_zero, "0.2.1-rc.1")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (ANGULAR_COMMITS_MINOR, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (ANGULAR_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.1")
-                    for major_on_zero in (True, False)
-                ),
-                (ANGULAR_COMMITS_MAJOR, False, True, "1.0.0"),
-                (ANGULAR_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
-                (ANGULAR_COMMITS_MAJOR, False, False, "0.3.0"),
-                (ANGULAR_COMMITS_MAJOR, True, False, "0.3.0-rc.1"),
-            ],
-            # Latest version for repo_with_main_and_feature_branches is currently 0.3.0-rc.1.
-            # The last full release version was 0.2.0, so it's had a minor prerelease
-            (
-                "repo_with_main_and_feature_branches_angular_commits",
-                "default_angular_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, True, major_on_zero, "0.3.0-rc.1")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *(
-                    (commits, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (ANGULAR_COMMITS_PATCH, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (ANGULAR_COMMITS_PATCH, True, major_on_zero, "0.3.0-rc.2")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (ANGULAR_COMMITS_MINOR, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (ANGULAR_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.2")
-                    for major_on_zero in (True, False)
-                ),
-                (ANGULAR_COMMITS_MAJOR, False, True, "1.0.0"),
-                (ANGULAR_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
-                (ANGULAR_COMMITS_MAJOR, False, False, "0.3.0"),
-                # Note - since breaking changes are absorbed into the minor digit
-                # with major_on_zero = False, and that's already been incremented
-                # since the last full release, the breaking change here will only
-                # trigger a prerelease revision
-                (ANGULAR_COMMITS_MAJOR, True, False, "0.3.0-rc.2"),
-            ],
-        }.items()
-        for (commit_messages, prerelease, major_on_zero, expected_new_version) in values
-    ],
+                lazy_fixture(repo_fixture_name),
+                lazy_fixture(parser_fixture_name),
+                translator,
+                commit_messages,
+                prerelease,
+                major_on_zero,
+                expected_new_version,
+            )
+            for (repo_fixture_name, parser_fixture_name, translator), values in {
+                # Latest version for repo_with_no_tags is currently 0.0.0 (default)
+                # It's biggest change type is minor, so the next version should be 0.1.0
+                (
+                    "repo_with_no_tags_angular_commits",
+                    "default_angular_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, False, major_on_zero, "0.1.0")
+                        for major_on_zero in (True, False)
+                        for commits in (
+                            [],
+                            ["uninteresting"],
+                            ANGULAR_COMMITS_PATCH,
+                            ANGULAR_COMMITS_MINOR,
+                        )
+                    ),
+                    (ANGULAR_COMMITS_MAJOR, False, False, "0.1.0"),
+                    (ANGULAR_COMMITS_MAJOR, False, True, "1.0.0"),
+                ],
+                # Latest version for repo_with_single_branch is currently 0.1.1
+                # Note repo_with_single_branch isn't modelled with prereleases
+                (
+                    "repo_with_single_branch_angular_commits",
+                    "default_angular_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, False, major_on_zero, "0.1.1")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_PATCH, False, major_on_zero, "0.1.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_MINOR, False, major_on_zero, "0.2.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    (ANGULAR_COMMITS_MAJOR, False, False, "0.2.0"),
+                    (ANGULAR_COMMITS_MAJOR, False, True, "1.0.0"),
+                ],
+                # Latest version for repo_with_single_branch_and_prereleases is currently 0.2.0
+                (
+                    "repo_with_single_branch_and_prereleases_angular_commits",
+                    "default_angular_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, prerelease, major_on_zero, "0.2.0")
+                        for prerelease in (True, False)
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_PATCH, False, major_on_zero, "0.2.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_PATCH, True, major_on_zero, "0.2.1-rc.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_MINOR, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    (ANGULAR_COMMITS_MAJOR, False, True, "1.0.0"),
+                    (ANGULAR_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
+                    (ANGULAR_COMMITS_MAJOR, False, False, "0.3.0"),
+                    (ANGULAR_COMMITS_MAJOR, True, False, "0.3.0-rc.1"),
+                ],
+                # Latest version for repo_with_main_and_feature_branches is currently 0.3.0-rc.1.
+                # The last full release version was 0.2.0, so it's had a minor prerelease
+                (
+                    "repo_with_main_and_feature_branches_angular_commits",
+                    "default_angular_parser",
+                    VersionTranslator(prerelease_token="beta"),
+                ): [
+                    *(
+                        (commits, True, major_on_zero, "0.3.0-beta.1")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *(
+                        (commits, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_PATCH, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_PATCH, True, major_on_zero, "0.3.0-beta.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_MINOR, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (ANGULAR_COMMITS_MINOR, True, major_on_zero, "0.3.0-beta.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    (ANGULAR_COMMITS_MAJOR, False, True, "1.0.0"),
+                    (ANGULAR_COMMITS_MAJOR, True, True, "1.0.0-beta.1"),
+                    (ANGULAR_COMMITS_MAJOR, False, False, "0.3.0"),
+                    # Note - since breaking changes are absorbed into the minor digit
+                    # with major_on_zero = False, and that's already been incremented
+                    # since the last full release, the breaking change here will only
+                    # trigger a prerelease revision
+                    (ANGULAR_COMMITS_MAJOR, True, False, "0.3.0-beta.2"),
+                ],
+            }.items()
+            for (
+                commit_messages,
+                prerelease,
+                major_on_zero,
+                expected_new_version,
+            ) in values
+        ]
+    ),
 )
 def test_algorithm_with_zero_dot_versions_angular(
     repo,
     file_in_repo,
     commit_parser,
     translator,
     commit_messages,
@@ -518,148 +545,155 @@
         expected_new_version, prerelease_token=translator.prerelease_token
     )
 
 
 @pytest.mark.parametrize(
     "repo, commit_parser, translator, commit_messages,"
     "prerelease, major_on_zero, expected_new_version",
-    [
-        (
-            lazy_fixture(repo_fixture_name),
-            lazy_fixture(parser_fixture_name),
-            translator,
-            commit_messages,
-            prerelease,
-            major_on_zero,
-            expected_new_version,
-        )
-        for (repo_fixture_name, parser_fixture_name, translator), values in {
-            # Latest version for repo_with_no_tags is currently 0.0.0 (default)
-            # It's biggest change type is minor, so the next version should be 0.1.0
-            (
-                "repo_with_no_tags_emoji_commits",
-                "default_emoji_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, False, major_on_zero, "0.1.0")
-                    for major_on_zero in (True, False)
-                    for commits in (
-                        [],
-                        ["uninteresting"],
-                        EMOJI_COMMITS_PATCH,
-                        EMOJI_COMMITS_MINOR,
-                    )
-                ),
-                (EMOJI_COMMITS_MAJOR, False, False, "0.1.0"),
-                (EMOJI_COMMITS_MAJOR, False, True, "1.0.0"),
-            ],
-            # Latest version for repo_with_single_branch is currently 0.1.1
-            # Note repo_with_single_branch isn't modelled with prereleases
+    xdist_sort_hack(
+        [
             (
-                "repo_with_single_branch_emoji_commits",
-                "default_emoji_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, False, major_on_zero, "0.1.1")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (EMOJI_COMMITS_PATCH, False, major_on_zero, "0.1.2")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (EMOJI_COMMITS_MINOR, False, major_on_zero, "0.2.0")
-                    for major_on_zero in (True, False)
-                ),
-                (EMOJI_COMMITS_MAJOR, False, False, "0.2.0"),
-                (EMOJI_COMMITS_MAJOR, False, True, "1.0.0"),
-            ],
-            # Latest version for repo_with_single_branch_and_prereleases is currently 0.2.0
-            (
-                "repo_with_single_branch_and_prereleases_emoji_commits",
-                "default_emoji_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, prerelease, major_on_zero, "0.2.0")
-                    for prerelease in (True, False)
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (EMOJI_COMMITS_PATCH, False, major_on_zero, "0.2.1")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (EMOJI_COMMITS_PATCH, True, major_on_zero, "0.2.1-rc.1")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (EMOJI_COMMITS_MINOR, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (EMOJI_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.1")
-                    for major_on_zero in (True, False)
-                ),
-                (EMOJI_COMMITS_MAJOR, False, True, "1.0.0"),
-                (EMOJI_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
-                (EMOJI_COMMITS_MAJOR, False, False, "0.3.0"),
-                (EMOJI_COMMITS_MAJOR, True, False, "0.3.0-rc.1"),
-            ],
-            # Latest version for repo_with_main_and_feature_branches is currently 0.3.0-rc.1.
-            # The last full release version was 0.2.0, so it's had a minor prerelease
-            (
-                "repo_with_main_and_feature_branches_emoji_commits",
-                "default_emoji_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, True, major_on_zero, "0.3.0-rc.1")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *(
-                    (commits, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (EMOJI_COMMITS_PATCH, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (EMOJI_COMMITS_PATCH, True, major_on_zero, "0.3.0-rc.2")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (EMOJI_COMMITS_MINOR, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (EMOJI_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.2")
-                    for major_on_zero in (True, False)
-                ),
-                (EMOJI_COMMITS_MAJOR, False, True, "1.0.0"),
-                (EMOJI_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
-                (EMOJI_COMMITS_MAJOR, False, False, "0.3.0"),
-                # Note - since breaking changes are absorbed into the minor digit
-                # with major_on_zero = False, and that's already been incremented
-                # since the last full release, the breaking change here will only
-                # trigger a prerelease revision
-                (EMOJI_COMMITS_MAJOR, True, False, "0.3.0-rc.2"),
-            ],
-        }.items()
-        for (commit_messages, prerelease, major_on_zero, expected_new_version) in values
-    ],
+                lazy_fixture(repo_fixture_name),
+                lazy_fixture(parser_fixture_name),
+                translator,
+                commit_messages,
+                prerelease,
+                major_on_zero,
+                expected_new_version,
+            )
+            for (repo_fixture_name, parser_fixture_name, translator), values in {
+                # Latest version for repo_with_no_tags is currently 0.0.0 (default)
+                # It's biggest change type is minor, so the next version should be 0.1.0
+                (
+                    "repo_with_no_tags_emoji_commits",
+                    "default_emoji_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, False, major_on_zero, "0.1.0")
+                        for major_on_zero in (True, False)
+                        for commits in (
+                            [],
+                            ["uninteresting"],
+                            EMOJI_COMMITS_PATCH,
+                            EMOJI_COMMITS_MINOR,
+                        )
+                    ),
+                    (EMOJI_COMMITS_MAJOR, False, False, "0.1.0"),
+                    (EMOJI_COMMITS_MAJOR, False, True, "1.0.0"),
+                ],
+                # Latest version for repo_with_single_branch is currently 0.1.1
+                # Note repo_with_single_branch isn't modelled with prereleases
+                (
+                    "repo_with_single_branch_emoji_commits",
+                    "default_emoji_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, False, major_on_zero, "0.1.1")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (EMOJI_COMMITS_PATCH, False, major_on_zero, "0.1.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (EMOJI_COMMITS_MINOR, False, major_on_zero, "0.2.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    (EMOJI_COMMITS_MAJOR, False, False, "0.2.0"),
+                    (EMOJI_COMMITS_MAJOR, False, True, "1.0.0"),
+                ],
+                # Latest version for repo_with_single_branch_and_prereleases is currently 0.2.0
+                (
+                    "repo_with_single_branch_and_prereleases_emoji_commits",
+                    "default_emoji_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, prerelease, major_on_zero, "0.2.0")
+                        for prerelease in (True, False)
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (EMOJI_COMMITS_PATCH, False, major_on_zero, "0.2.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (EMOJI_COMMITS_PATCH, True, major_on_zero, "0.2.1-rc.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (EMOJI_COMMITS_MINOR, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (EMOJI_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    (EMOJI_COMMITS_MAJOR, False, True, "1.0.0"),
+                    (EMOJI_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
+                    (EMOJI_COMMITS_MAJOR, False, False, "0.3.0"),
+                    (EMOJI_COMMITS_MAJOR, True, False, "0.3.0-rc.1"),
+                ],
+                # Latest version for repo_with_main_and_feature_branches is currently 0.3.0-beta.1.
+                # The last full release version was 0.2.0, so it's had a minor prerelease
+                (
+                    "repo_with_main_and_feature_branches_emoji_commits",
+                    "default_emoji_parser",
+                    VersionTranslator(prerelease_token="beta"),
+                ): [
+                    *(
+                        (commits, True, major_on_zero, "0.3.0-beta.1")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *(
+                        (commits, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (EMOJI_COMMITS_PATCH, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (EMOJI_COMMITS_PATCH, True, major_on_zero, "0.3.0-beta.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (EMOJI_COMMITS_MINOR, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (EMOJI_COMMITS_MINOR, True, major_on_zero, "0.3.0-beta.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    (EMOJI_COMMITS_MAJOR, False, True, "1.0.0"),
+                    (EMOJI_COMMITS_MAJOR, True, True, "1.0.0-beta.1"),
+                    (EMOJI_COMMITS_MAJOR, False, False, "0.3.0"),
+                    # Note - since breaking changes are absorbed into the minor digit
+                    # with major_on_zero = False, and that's already been incremented
+                    # since the last full release, the breaking change here will only
+                    # trigger a prerelease revision
+                    (EMOJI_COMMITS_MAJOR, True, False, "0.3.0-beta.2"),
+                ],
+            }.items()
+            for (
+                commit_messages,
+                prerelease,
+                major_on_zero,
+                expected_new_version,
+            ) in values
+        ]
+    ),
 )
 def test_algorithm_with_zero_dot_versions_emoji(
     repo,
     file_in_repo,
     commit_parser,
     translator,
     commit_messages,
@@ -679,168 +713,205 @@
         expected_new_version, prerelease_token=translator.prerelease_token
     )
 
 
 @pytest.mark.parametrize(
     "repo, commit_parser, translator, commit_messages,"
     "prerelease, major_on_zero, expected_new_version",
-    [
-        (
-            lazy_fixture(repo_fixture_name),
-            lazy_fixture(parser_fixture_name),
-            translator,
-            commit_messages,
-            prerelease,
-            major_on_zero,
-            expected_new_version,
-        )
-        for (repo_fixture_name, parser_fixture_name, translator), values in {
-            # Latest version for repo_with_no_tags is currently 0.0.0 (default)
-            # It's biggest change type is minor, so the next version should be 0.1.0
-            (
-                "repo_with_no_tags_scipy_commits",
-                "default_scipy_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, False, major_on_zero, "0.1.0")
-                    for major_on_zero in (True, False)
-                    for commits in (
-                        [],
-                        ["uninteresting"],
-                        lazy_fixture("scipy_commits_patch"),
-                        lazy_fixture("scipy_commits_minor"),
-                    )
-                ),
-                (lazy_fixture("scipy_commits_major"), False, False, "0.1.0"),
-                (lazy_fixture("scipy_commits_major"), False, True, "1.0.0"),
-            ],
-            # Latest version for repo_with_single_branch is currently 0.1.1
-            # Note repo_with_single_branch isn't modelled with prereleases
-            (
-                "repo_with_single_branch_scipy_commits",
-                "default_scipy_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, False, major_on_zero, "0.1.1")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (lazy_fixture("scipy_commits_patch"), False, major_on_zero, "0.1.2")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (lazy_fixture("scipy_commits_minor"), False, major_on_zero, "0.2.0")
-                    for major_on_zero in (True, False)
-                ),
-                (lazy_fixture("scipy_commits_major"), False, False, "0.2.0"),
-                (lazy_fixture("scipy_commits_major"), False, True, "1.0.0"),
-            ],
-            # Latest version for repo_with_single_branch_and_prereleases is currently 0.2.0
+    xdist_sort_hack(
+        [
             (
-                "repo_with_single_branch_and_prereleases_scipy_commits",
-                "default_scipy_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, prerelease, major_on_zero, "0.2.0")
-                    for prerelease in (True, False)
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (lazy_fixture("scipy_commits_patch"), False, major_on_zero, "0.2.1")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (
-                        lazy_fixture("scipy_commits_patch"),
-                        True,
-                        major_on_zero,
-                        "0.2.1-rc.1",
-                    )
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (lazy_fixture("scipy_commits_minor"), False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (
-                        lazy_fixture("scipy_commits_minor"),
-                        True,
-                        major_on_zero,
-                        "0.3.0-rc.1",
-                    )
-                    for major_on_zero in (True, False)
-                ),
-                (lazy_fixture("scipy_commits_major"), False, True, "1.0.0"),
-                (lazy_fixture("scipy_commits_major"), True, True, "1.0.0-rc.1"),
-                (lazy_fixture("scipy_commits_major"), False, False, "0.3.0"),
-                (lazy_fixture("scipy_commits_major"), True, False, "0.3.0-rc.1"),
-            ],
-            # Latest version for repo_with_main_and_feature_branches is currently 0.3.0-rc.1.
-            # The last full release version was 0.2.0, so it's had a minor prerelease
-            (
-                "repo_with_main_and_feature_branches_scipy_commits",
-                "default_scipy_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, True, major_on_zero, "0.3.0-rc.1")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *(
-                    (commits, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (lazy_fixture("scipy_commits_patch"), False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (
-                        lazy_fixture("scipy_commits_patch"),
-                        True,
-                        major_on_zero,
-                        "0.3.0-rc.2",
-                    )
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (lazy_fixture("scipy_commits_minor"), False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (
-                        lazy_fixture("scipy_commits_minor"),
-                        True,
-                        major_on_zero,
-                        "0.3.0-rc.2",
-                    )
-                    for major_on_zero in (True, False)
-                ),
-                (lazy_fixture("scipy_commits_major"), False, True, "1.0.0"),
-                (lazy_fixture("scipy_commits_major"), True, True, "1.0.0-rc.1"),
-                (lazy_fixture("scipy_commits_major"), False, False, "0.3.0"),
-                # Note - since breaking changes are absorbed into the minor digit
-                # with major_on_zero = False, and that's already been incremented
-                # since the last full release, the breaking change here will only
-                # trigger a prerelease revision
-                (lazy_fixture("scipy_commits_major"), True, False, "0.3.0-rc.2"),
-            ],
-        }.items()
-        for (commit_messages, prerelease, major_on_zero, expected_new_version) in values
-    ],
+                lazy_fixture(repo_fixture_name),
+                lazy_fixture(parser_fixture_name),
+                translator,
+                commit_messages,
+                prerelease,
+                major_on_zero,
+                expected_new_version,
+            )
+            for (repo_fixture_name, parser_fixture_name, translator), values in {
+                # Latest version for repo_with_no_tags is currently 0.0.0 (default)
+                # It's biggest change type is minor, so the next version should be 0.1.0
+                (
+                    "repo_with_no_tags_scipy_commits",
+                    "default_scipy_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, False, major_on_zero, "0.1.0")
+                        for major_on_zero in (True, False)
+                        for commits in (
+                            [],
+                            ["uninteresting"],
+                            lazy_fixture("scipy_commits_patch"),
+                            lazy_fixture("scipy_commits_minor"),
+                        )
+                    ),
+                    (lazy_fixture("scipy_commits_major"), False, False, "0.1.0"),
+                    (lazy_fixture("scipy_commits_major"), False, True, "1.0.0"),
+                ],
+                # Latest version for repo_with_single_branch is currently 0.1.1
+                # Note repo_with_single_branch isn't modelled with prereleases
+                (
+                    "repo_with_single_branch_scipy_commits",
+                    "default_scipy_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, False, major_on_zero, "0.1.1")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_patch"),
+                            False,
+                            major_on_zero,
+                            "0.1.2",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_minor"),
+                            False,
+                            major_on_zero,
+                            "0.2.0",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    (lazy_fixture("scipy_commits_major"), False, False, "0.2.0"),
+                    (lazy_fixture("scipy_commits_major"), False, True, "1.0.0"),
+                ],
+                # Latest version for repo_with_single_branch_and_prereleases is currently 0.2.0
+                (
+                    "repo_with_single_branch_and_prereleases_scipy_commits",
+                    "default_scipy_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, prerelease, major_on_zero, "0.2.0")
+                        for prerelease in (True, False)
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_patch"),
+                            False,
+                            major_on_zero,
+                            "0.2.1",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_patch"),
+                            True,
+                            major_on_zero,
+                            "0.2.1-rc.1",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_minor"),
+                            False,
+                            major_on_zero,
+                            "0.3.0",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_minor"),
+                            True,
+                            major_on_zero,
+                            "0.3.0-rc.1",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    (lazy_fixture("scipy_commits_major"), False, True, "1.0.0"),
+                    (lazy_fixture("scipy_commits_major"), True, True, "1.0.0-rc.1"),
+                    (lazy_fixture("scipy_commits_major"), False, False, "0.3.0"),
+                    (lazy_fixture("scipy_commits_major"), True, False, "0.3.0-rc.1"),
+                ],
+                # Latest version for repo_with_main_and_feature_branches is currently 0.3.0-rc.1.
+                # The last full release version was 0.2.0, so it's had a minor prerelease
+                (
+                    "repo_with_main_and_feature_branches_scipy_commits",
+                    "default_scipy_parser",
+                    VersionTranslator(prerelease_token="beta"),
+                ): [
+                    *(
+                        (commits, True, major_on_zero, "0.3.0-beta.1")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *(
+                        (commits, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_patch"),
+                            False,
+                            major_on_zero,
+                            "0.3.0",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_patch"),
+                            True,
+                            major_on_zero,
+                            "0.3.0-beta.2",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_minor"),
+                            False,
+                            major_on_zero,
+                            "0.3.0",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (
+                            lazy_fixture("scipy_commits_minor"),
+                            True,
+                            major_on_zero,
+                            "0.3.0-beta.2",
+                        )
+                        for major_on_zero in (True, False)
+                    ),
+                    (lazy_fixture("scipy_commits_major"), False, True, "1.0.0"),
+                    (lazy_fixture("scipy_commits_major"), True, True, "1.0.0-beta.1"),
+                    (lazy_fixture("scipy_commits_major"), False, False, "0.3.0"),
+                    # Note - since breaking changes are absorbed into the minor digit
+                    # with major_on_zero = False, and that's already been incremented
+                    # since the last full release, the breaking change here will only
+                    # trigger a prerelease revision
+                    (lazy_fixture("scipy_commits_major"), True, False, "0.3.0-beta.2"),
+                ],
+            }.items()
+            for (
+                commit_messages,
+                prerelease,
+                major_on_zero,
+                expected_new_version,
+            ) in values
+        ],
+    ),
 )
 def test_algorithm_with_zero_dot_versions_scipy(
     repo,
     file_in_repo,
     commit_parser,
     translator,
     commit_messages,
@@ -860,148 +931,155 @@
         expected_new_version, prerelease_token=translator.prerelease_token
     )
 
 
 @pytest.mark.parametrize(
     "repo, commit_parser, translator, commit_messages,"
     "prerelease, major_on_zero, expected_new_version",
-    [
-        (
-            lazy_fixture(repo_fixture_name),
-            lazy_fixture(parser_fixture_name),
-            translator,
-            commit_messages,
-            prerelease,
-            major_on_zero,
-            expected_new_version,
-        )
-        for (repo_fixture_name, parser_fixture_name, translator), values in {
-            # Latest version for repo_with_no_tags is currently 0.0.0 (default)
-            # It's biggest change type is minor, so the next version should be 0.1.0
-            (
-                "repo_with_no_tags_tag_commits",
-                "default_tag_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, False, major_on_zero, "0.1.0")
-                    for major_on_zero in (True, False)
-                    for commits in (
-                        [],
-                        ["uninteresting"],
-                        TAG_COMMITS_PATCH,
-                        TAG_COMMITS_MINOR,
-                    )
-                ),
-                (TAG_COMMITS_MAJOR, False, False, "0.1.0"),
-                (TAG_COMMITS_MAJOR, False, True, "1.0.0"),
-            ],
-            # Latest version for repo_with_single_branch is currently 0.1.1
-            # Note repo_with_single_branch isn't modelled with prereleases
-            (
-                "repo_with_single_branch_tag_commits",
-                "default_tag_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, False, major_on_zero, "0.1.1")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (TAG_COMMITS_PATCH, False, major_on_zero, "0.1.2")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (TAG_COMMITS_MINOR, False, major_on_zero, "0.2.0")
-                    for major_on_zero in (True, False)
-                ),
-                (TAG_COMMITS_MAJOR, False, False, "0.2.0"),
-                (TAG_COMMITS_MAJOR, False, True, "1.0.0"),
-            ],
-            # Latest version for repo_with_single_branch_and_prereleases is currently 0.2.0
-            (
-                "repo_with_single_branch_and_prereleases_tag_commits",
-                "default_tag_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, prerelease, major_on_zero, "0.2.0")
-                    for prerelease in (True, False)
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (TAG_COMMITS_PATCH, False, major_on_zero, "0.2.1")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (TAG_COMMITS_PATCH, True, major_on_zero, "0.2.1-rc.1")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (TAG_COMMITS_MINOR, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (TAG_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.1")
-                    for major_on_zero in (True, False)
-                ),
-                (TAG_COMMITS_MAJOR, False, True, "1.0.0"),
-                (TAG_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
-                (TAG_COMMITS_MAJOR, False, False, "0.3.0"),
-                (TAG_COMMITS_MAJOR, True, False, "0.3.0-rc.1"),
-            ],
-            # Latest version for repo_with_main_and_feature_branches is currently 0.3.0-rc.1.
-            # The last full release version was 0.2.0, so it's had a minor prerelease
+    xdist_sort_hack(
+        [
             (
-                "repo_with_main_and_feature_branches_tag_commits",
-                "default_tag_parser",
-                VersionTranslator(),
-            ): [
-                *(
-                    (commits, True, major_on_zero, "0.3.0-rc.1")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                # Models a merge of commits from the branch to the main branch, now
-                # that prerelease=False
-                *(
-                    (commits, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                    for commits in ([], ["uninteresting"])
-                ),
-                *(
-                    (TAG_COMMITS_PATCH, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (TAG_COMMITS_PATCH, True, major_on_zero, "0.3.0-rc.2")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (TAG_COMMITS_MINOR, False, major_on_zero, "0.3.0")
-                    for major_on_zero in (True, False)
-                ),
-                *(
-                    (TAG_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.2")
-                    for major_on_zero in (True, False)
-                ),
-                (TAG_COMMITS_MAJOR, False, True, "1.0.0"),
-                (TAG_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
-                (TAG_COMMITS_MAJOR, False, False, "0.3.0"),
-                # Note - since breaking changes are absorbed into the minor digit
-                # with major_on_zero = False, and that's already been incremented
-                # since the last full release, the breaking change here will only
-                # trigger a prerelease revision
-                (TAG_COMMITS_MAJOR, True, False, "0.3.0-rc.2"),
-            ],
-        }.items()
-        for (commit_messages, prerelease, major_on_zero, expected_new_version) in values
-    ],
+                lazy_fixture(repo_fixture_name),
+                lazy_fixture(parser_fixture_name),
+                translator,
+                commit_messages,
+                prerelease,
+                major_on_zero,
+                expected_new_version,
+            )
+            for (repo_fixture_name, parser_fixture_name, translator), values in {
+                # Latest version for repo_with_no_tags is currently 0.0.0 (default)
+                # It's biggest change type is minor, so the next version should be 0.1.0
+                (
+                    "repo_with_no_tags_tag_commits",
+                    "default_tag_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, False, major_on_zero, "0.1.0")
+                        for major_on_zero in (True, False)
+                        for commits in (
+                            [],
+                            ["uninteresting"],
+                            TAG_COMMITS_PATCH,
+                            TAG_COMMITS_MINOR,
+                        )
+                    ),
+                    (TAG_COMMITS_MAJOR, False, False, "0.1.0"),
+                    (TAG_COMMITS_MAJOR, False, True, "1.0.0"),
+                ],
+                # Latest version for repo_with_single_branch is currently 0.1.1
+                # Note repo_with_single_branch isn't modelled with prereleases
+                (
+                    "repo_with_single_branch_tag_commits",
+                    "default_tag_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, False, major_on_zero, "0.1.1")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (TAG_COMMITS_PATCH, False, major_on_zero, "0.1.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (TAG_COMMITS_MINOR, False, major_on_zero, "0.2.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    (TAG_COMMITS_MAJOR, False, False, "0.2.0"),
+                    (TAG_COMMITS_MAJOR, False, True, "1.0.0"),
+                ],
+                # Latest version for repo_with_single_branch_and_prereleases is currently 0.2.0
+                (
+                    "repo_with_single_branch_and_prereleases_tag_commits",
+                    "default_tag_parser",
+                    VersionTranslator(),
+                ): [
+                    *(
+                        (commits, prerelease, major_on_zero, "0.2.0")
+                        for prerelease in (True, False)
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (TAG_COMMITS_PATCH, False, major_on_zero, "0.2.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (TAG_COMMITS_PATCH, True, major_on_zero, "0.2.1-rc.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (TAG_COMMITS_MINOR, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (TAG_COMMITS_MINOR, True, major_on_zero, "0.3.0-rc.1")
+                        for major_on_zero in (True, False)
+                    ),
+                    (TAG_COMMITS_MAJOR, False, True, "1.0.0"),
+                    (TAG_COMMITS_MAJOR, True, True, "1.0.0-rc.1"),
+                    (TAG_COMMITS_MAJOR, False, False, "0.3.0"),
+                    (TAG_COMMITS_MAJOR, True, False, "0.3.0-rc.1"),
+                ],
+                # Latest version for repo_with_main_and_feature_branches is currently 0.3.0-beta.1.
+                # The last full release version was 0.2.0, so it's had a minor prerelease
+                (
+                    "repo_with_main_and_feature_branches_tag_commits",
+                    "default_tag_parser",
+                    VersionTranslator(prerelease_token="beta"),
+                ): [
+                    *(
+                        (commits, True, major_on_zero, "0.3.0-beta.1")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    # Models a merge of commits from the branch to the main branch, now
+                    # that prerelease=False
+                    *(
+                        (commits, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                        for commits in ([], ["uninteresting"])
+                    ),
+                    *(
+                        (TAG_COMMITS_PATCH, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (TAG_COMMITS_PATCH, True, major_on_zero, "0.3.0-beta.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (TAG_COMMITS_MINOR, False, major_on_zero, "0.3.0")
+                        for major_on_zero in (True, False)
+                    ),
+                    *(
+                        (TAG_COMMITS_MINOR, True, major_on_zero, "0.3.0-beta.2")
+                        for major_on_zero in (True, False)
+                    ),
+                    (TAG_COMMITS_MAJOR, False, True, "1.0.0"),
+                    (TAG_COMMITS_MAJOR, True, True, "1.0.0-beta.1"),
+                    (TAG_COMMITS_MAJOR, False, False, "0.3.0"),
+                    # Note - since breaking changes are absorbed into the minor digit
+                    # with major_on_zero = False, and that's already been incremented
+                    # since the last full release, the breaking change here will only
+                    # trigger a prerelease revision
+                    (TAG_COMMITS_MAJOR, True, False, "0.3.0-beta.2"),
+                ],
+            }.items()
+            for (
+                commit_messages,
+                prerelease,
+                major_on_zero,
+                expected_new_version,
+            ) in values
+        ],
+    ),
 )
 def test_algorithm_with_zero_dot_versions_tag(
     repo,
     file_in_repo,
     commit_parser,
     translator,
     commit_messages,
```

### Comparing `python-semantic-release-8.0.0a4/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.0a5/tests/scenario/test_release_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 from datetime import datetime
 
 import pytest
 from git import Actor
 from pytest_lazyfixture import lazy_fixture
 
 from semantic_release.changelog.release_history import ReleaseHistory
-from semantic_release.commit_parser.angular import AngularCommitParser
-from semantic_release.version import translator
 from semantic_release.version.translator import VersionTranslator
 from semantic_release.version.version import Version
 
 from tests.const import ANGULAR_COMMITS_MINOR, COMMIT_MESSAGE
-from tests.helper import add_text_to_file
+from tests.util import add_text_to_file
 
 # NOTE: not testing parser correctness here, just that the right commits end up
 # in the right places. So we only compare that the commits with the messages
 # we anticipate are in the right place, rather than by hash
 # So we are only using the angular parser
 
 # We are also currently only testing that the "elements" key of the releases
@@ -87,17 +85,17 @@
                 "feature": ["feat: add some more text\n"],
                 "unknown": [COMMIT_MESSAGE.format(version="0.2.0-rc.1")],
             },
             Version.parse("0.2.0"): {
                 "feature": ["feat: add some more text\n"],
                 "unknown": [COMMIT_MESSAGE.format(version="0.2.0")],
             },
-            Version.parse("0.3.0-rc.1"): {
+            Version.parse("0.3.0-beta.1"): {
                 "feature": ["feat: (feature) add some more text\n"],
-                "unknown": [COMMIT_MESSAGE.format(version="0.3.0-rc.1")],
+                "unknown": [COMMIT_MESSAGE.format(version="0.3.0-beta.1")],
             },
         },
     )
 )
 
 REPO_WITH_GIT_FLOW_EXPECTED_RELEASE_HISTORY = FakeReleaseHistoryElements(
     unreleased={},
@@ -121,22 +119,22 @@
             "feature": ["feat: (dev) add some more text\n"],
             "unknown": [COMMIT_MESSAGE.format(version="1.1.0")],
         },
         Version.parse("1.1.1"): {
             "fix": ["fix: (dev) add some more text\n"],
             "unknown": [COMMIT_MESSAGE.format(version="1.1.1")],
         },
-        Version.parse("1.2.0-rc.1"): {
+        Version.parse("1.2.0-alpha.1"): {
             "feature": ["feat: (feature) add some more text\n"],
-            "unknown": [COMMIT_MESSAGE.format(version="1.2.0-rc.1")],
+            "unknown": [COMMIT_MESSAGE.format(version="1.2.0-alpha.1")],
         },
-        Version.parse("1.2.0-rc.2"): {
+        Version.parse("1.2.0-alpha.2"): {
             "feature": ["feat: (feature) add some more text\n"],
             "fix": ["fix: (feature) add some missing text\n"],
-            "unknown": [COMMIT_MESSAGE.format(version="1.2.0-rc.2")],
+            "unknown": [COMMIT_MESSAGE.format(version="1.2.0-alpha.2")],
         },
     },
 )
 
 REPO_WITH_GIT_FLOW_AND_RELEASE_CHANNELS_EXPECTED_RELEASE_HISTORY = (
     FakeReleaseHistoryElements(
         unreleased={},
```

### Comparing `python-semantic-release-8.0.0a4/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.0a5/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import requests_mock
 from requests import HTTPError, Response, Session
 
 from semantic_release.hvcs.gitea import Gitea
 from semantic_release.hvcs.token_auth import TokenAuth
 
 from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER
-from tests.helper import netrc_file
+from tests.util import netrc_file
 
 
 @pytest.fixture
 def default_gitea_client():
     remote_url = f"git@gitea.com:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git"
     yield Gitea(remote_url=remote_url)
```

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import requests_mock
 from requests import HTTPError, Response, Session
 
 from semantic_release.hvcs.github import Github
 from semantic_release.hvcs.token_auth import TokenAuth
 
 from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER
-from tests.helper import netrc_file
+from tests.util import netrc_file
 
 
 @pytest.fixture
 def default_gh_client():
     remote_url = f"git@github.com:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git"
     yield Github(remote_url=remote_url)
```

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_declaration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+import difflib
 from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 
 import pytest
 from pytest_lazyfixture import lazy_fixture
 
 from semantic_release.version.declaration import (
     PatternVersionDeclaration,
     TomlVersionDeclaration,
 )
 from semantic_release.version.version import Version
 
 from tests.const import EXAMPLE_PROJECT_VERSION
-from tests.helper import diff_strings
 
 
 def test_pyproject_toml_version_found(example_pyproject_toml):
     decl = TomlVersionDeclaration(
         example_pyproject_toml.resolve(), "tool.poetry.version"
     )
     versions = decl.parse()
@@ -54,20 +54,32 @@
     orig_content = decl.content
     new_content = decl.replace(new_version=new_version)
     decl.write(new_content)
 
     new_decl = decl_cls(config_file.resolve(), search_text)
     assert new_decl.parse() == {new_version}
 
-    deleted, added = diff_strings(orig_content, new_decl.content)
-    # Expecting only the version to have changed
-    deleted_text = "".join(c for _, c in deleted)
-    added_text = "".join(c for _, c in added)
-    assert deleted_text == EXAMPLE_PROJECT_VERSION.replace(".", "")
-    assert added_text == str(new_version).replace(".", "")
+    d = difflib.Differ()
+    diff = list(
+        d.compare(
+            orig_content.splitlines(keepends=True),
+            new_decl.content.splitlines(keepends=True),
+        )
+    )
+    added = [line[2:] for line in diff if line.startswith("+ ")]
+    removed = [line[2:] for line in diff if line.startswith("- ")]
+
+    assert len(removed) == 1
+    assert len(added) == 1
+
+    (removed_line,) = removed
+    (added_line,) = added
+
+    # Line is unchanged apart from new version added
+    assert removed_line.replace(EXAMPLE_PROJECT_VERSION, str(new_version)) == added_line
 
 
 @pytest.mark.parametrize(
     "search_text",
     [r"^version = (.*)$", r"^version = (?P<Version>.*)", r"(?P<vrsion>.*)"],
 )
 def test_bad_version_regex_fails(search_text):
```

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a4/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

