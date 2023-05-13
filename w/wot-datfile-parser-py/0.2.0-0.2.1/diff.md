# Comparing `tmp/wot_datfile_parser_py-0.2.0.tar.gz` & `tmp/wot_datfile_parser_py-0.2.1.tar.gz`

## Comparing `wot_datfile_parser_py-0.2.0.tar` & `wot_datfile_parser_py-0.2.1.tar`

### file list

```diff
@@ -1,720 +1,14 @@
--rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 wot_datfile_parser_py-0.2.0/Cargo.toml
--rw-r--r--   0     1000     1000     1683 2023-01-27 07:12:36.000000 wot_datfile_parser_py-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      685 2023-01-12 08:19:57.000000 wot_datfile_parser_py-0.2.0/.gitignore
--rw-r--r--   0     1000     1000      324 2023-01-27 06:23:51.000000 wot_datfile_parser_py-0.2.0/.rustfmt.toml
--rw-r--r--   0     1000     1000      873 2023-03-02 05:59:50.000000 wot_datfile_parser_py-0.2.0/README.md
--rw-r--r--   0     1000     1000     3759 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0     1000     1000       44 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/_distutils_hack/override.py
--rw-r--r--   0     1000     1000      152 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/distutils-precedence.pth
--rw-r--r--   0     1000     1000     5748 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/maturin/__init__.py
--rw-r--r--   0     1000     1000      953 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/maturin/__main__.py
--rw-r--r--   0     1000     1000     4835 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/maturin/import_hook.py
--rw-r--r--   0     1000     1000        4 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/maturin-0.14.9.dist-info/INSTALLER
--rw-r--r--   0     1000     1000    17736 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/maturin-0.14.9.dist-info/METADATA
--rw-r--r--   0     1000     1000      854 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/maturin-0.14.9.dist-info/RECORD
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/maturin-0.14.9.dist-info/REQUESTED
--rw-r--r--   0     1000     1000      148 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/maturin-0.14.9.dist-info/WHEEL
--rw-r--r--   0     1000     1000      357 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/__init__.py
--rw-r--r--   0     1000     1000     1198 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/__main__.py
--rw-r--r--   0     1000     1000      573 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/__init__.py
--rw-r--r--   0     1000     1000     9739 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/build_env.py
--rw-r--r--   0     1000     1000     9441 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cache.py
--rw-r--r--   0     1000     1000      132 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0     1000     1000     6676 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0     1000     1000     8037 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0     1000     1000    28525 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0     1000     1000      760 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0     1000     1000     2472 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0     1000     1000     2614 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0     1000     1000    10788 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0     1000     1000    10339 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0     1000     1000    18669 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0     1000     1000     5076 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0     1000     1000      116 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0     1000     1000     3736 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0     1000     1000     7524 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0     1000     1000     1685 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0     1000     1000     2958 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0     1000     1000     8944 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0     1000     1000     6629 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0     1000     1000     4942 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0     1000     1000     2968 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0     1000     1000     1703 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0     1000     1000     1132 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0     1000     1000     4849 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0     1000     1000    27893 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0     1000     1000    12318 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0     1000     1000     5697 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0     1000     1000     5859 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0     1000     1000     3526 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0     1000     1000     6206 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0     1000     1000    13171 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/configuration.py
--rw-r--r--   0     1000     1000      858 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0     1000     1000     1172 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0     1000     1000      680 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0     1000     1000     5499 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0     1000     1000     1115 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0     1000     1000    20912 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0     1000     1000       30 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0     1000     1000    21392 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0     1000     1000    36783 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0     1000     1000     6557 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0     1000     1000    17362 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0     1000     1000     5871 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0     1000     1000     7918 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0     1000     1000     1579 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0     1000     1000      340 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/main.py
--rw-r--r--   0     1000     1000     2036 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0     1000     1000    19429 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0     1000     1000     9456 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0     1000     1000       63 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0     1000     1000      990 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0     1000     1000     6350 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0     1000     1000     2520 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0     1000     1000     1030 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/index.py
--rw-r--r--   0     1000     1000     9817 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/link.py
--rw-r--r--   0     1000     1000      738 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0     1000     1000     4520 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0     1000     1000     1907 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0     1000     1000     3858 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0     1000     1000     3500 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0     1000     1000       50 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0     1000     1000    12190 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0     1000     1000     2131 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0     1000     1000     6062 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/network/download.py
--rw-r--r--   0     1000     1000     7627 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0     1000     1000    16729 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/network/session.py
--rw-r--r--   0     1000     1000     4059 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0     1000     1000     1791 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0     1000     1000     1404 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0     1000     1000     1456 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0     1000     1000     2198 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0     1000     1000     1063 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0     1000     1000     1405 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0     1000     1000     3064 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0     1000     1000     5109 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0     1000     1000     9770 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0     1000     1000       51 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0     1000     1000     1354 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0     1000     1000     4091 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0     1000     1000    27412 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0     1000     1000    24145 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0     1000     1000     6722 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0     1000     1000     2793 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0     1000     1000    16094 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0     1000     1000    17421 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0     1000     1000    32524 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0     1000     1000     7584 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0     1000     1000     4117 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/req/req_tracker.py
--rw-r--r--   0     1000     1000    23814 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0     1000     1000      583 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0     1000     1000    18288 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0     1000     1000     5220 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0     1000     1000    18357 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0     1000     1000    28298 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0     1000     1000     5705 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0     1000     1000     9915 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0     1000     1000     2526 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0     1000     1000     5455 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0     1000     1000    11335 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0     1000     1000     6849 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0     1000     1000     1015 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0     1000     1000     1665 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0     1000     1000     1884 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0     1000     1000     5377 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0     1000     1000      242 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0     1000     1000     3627 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0     1000     1000     3206 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0     1000     1000     1249 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0     1000     1000     2203 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0     1000     1000     1169 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0     1000     1000     1055 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0     1000     1000     5893 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0     1000     1000      716 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0     1000     1000     3110 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0     1000     1000     4811 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0     1000     1000      795 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0     1000     1000    11522 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0     1000     1000    19359 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0     1000     1000     1193 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0     1000     1000     2108 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0     1000     1000     5652 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0     1000     1000     9182 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0     1000     1000     7662 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0     1000     1000     8906 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0     1000     1000     1759 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0     1000     1000     3459 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0     1000     1000     4549 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0     1000     1000      596 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0     1000     1000     3047 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0     1000     1000    18116 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0     1000     1000     5238 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0     1000     1000    11718 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0     1000     1000    22811 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0     1000     1000    12307 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0     1000     1000     4708 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0     1000     1000      465 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0     1000     1000     1379 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0     1000     1000     5033 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0     1000     1000      917 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0     1000     1000      170 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0     1000     1000     4251 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0     1000     1000      940 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0     1000     1000      778 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0     1000     1000    15625 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0     1000     1000     3946 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0     1000     1000     4154 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0     1000     1000     6783 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0     1000     1000      774 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0     1000     1000       62 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0     1000     1000      255 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0     1000     1000   265969 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0     1000     1000     2791 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0     1000     1000     3271 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0     1000     1000    31254 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0     1000     1000     1757 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0     1000     1000     9411 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0     1000     1000     3839 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0     1000     1000     5110 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0     1000     1000        1 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0     1000     1000     2747 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0     1000     1000     3590 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0     1000     1000     1200 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/compat.py
--rw-r--r--   0     1000     1000     1855 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0     1000     1000     1661 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0     1000     1000     3950 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0     1000     1000    10510 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0     1000     1000     3749 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0     1000     1000    13546 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0     1000     1000     1748 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0     1000     1000    31621 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0     1000     1000     1747 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0     1000     1000    20715 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0     1000     1000     1754 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0     1000     1000    13838 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0     1000     1000    25777 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0     1000     1000    19643 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0     1000     1000   105697 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0     1000     1000    99571 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0     1000     1000    98776 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0     1000     1000   102498 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0     1000     1000   131180 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0     1000     1000   103312 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0     1000     1000    95946 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0     1000     1000     5370 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0     1000     1000     3413 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0     1000     1000     2012 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0     1000     1000    25481 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0     1000     1000    19474 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0     1000     1000     6136 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0     1000     1000     4309 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0     1000     1000     3774 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0     1000     1000    12503 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0     1000     1000     2766 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0     1000     1000      242 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0     1000     1000      239 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0     1000     1000     2522 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0     1000     1000    10517 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0     1000     1000     1915 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0     1000     1000     5404 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0     1000     1000     6438 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0     1000     1000      581 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0     1000     1000    41259 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0     1000     1000    51456 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0     1000     1000    20739 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0     1000     1000    51963 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0     1000     1000    14811 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0     1000     1000     5058 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0     1000     1000    39109 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0     1000     1000    10820 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0     1000     1000    17720 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/scripts.py
--rw-r--r--   0     1000     1000    66262 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0     1000     1000    23513 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/version.py
--rw-r--r--   0     1000     1000    42943 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0     1000     1000    48414 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/distro.py
--rw-r--r--   0     1000     1000     1160 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/__init__.py
--rw-r--r--   0     1000     1000    16728 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/_ihatexml.py
--rw-r--r--   0     1000     1000    32353 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/_inputstream.py
--rw-r--r--   0     1000     1000    77040 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/_tokenizer.py
--rw-r--r--   0     1000     1000      109 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/_trie/__init__.py
--rw-r--r--   0     1000     1000     1013 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/_trie/_base.py
--rw-r--r--   0     1000     1000     1775 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/_trie/py.py
--rw-r--r--   0     1000     1000     4931 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/_utils.py
--rw-r--r--   0     1000     1000    83464 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/constants.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/filters/__init__.py
--rw-r--r--   0     1000     1000      919 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-r--r--   0     1000     1000      286 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/filters/base.py
--rw-r--r--   0     1000     1000     2945 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-r--r--   0     1000     1000     3643 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/filters/lint.py
--rw-r--r--   0     1000     1000    10588 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
--rw-r--r--   0     1000     1000    26897 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
--rw-r--r--   0     1000     1000     1214 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/filters/whitespace.py
--rw-r--r--   0     1000     1000   117186 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/html5parser.py
--rw-r--r--   0     1000     1000    15759 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/serializer.py
--rw-r--r--   0     1000     1000      679 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-r--r--   0     1000     1000     1715 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-r--r--   0     1000     1000     1776 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
--rw-r--r--   0     1000     1000     3592 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-r--r--   0     1000     1000    14565 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/base.py
--rw-r--r--   0     1000     1000     8925 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
--rw-r--r--   0     1000     1000    12836 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
--rw-r--r--   0     1000     1000    14766 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
--rw-r--r--   0     1000     1000     5719 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-r--r--   0     1000     1000     7476 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/base.py
--rw-r--r--   0     1000     1000     1413 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
--rw-r--r--   0     1000     1000     4551 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
--rw-r--r--   0     1000     1000     6357 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-r--r--   0     1000     1000     2309 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
--rw-r--r--   0     1000     1000      849 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0     1000     1000     3374 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0     1000     1000      321 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0     1000     1000    12795 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0     1000     1000    44025 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0     1000     1000     1881 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0     1000     1000       21 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0     1000     1000   204400 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0     1000     1000     1118 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0     1000     1000       20 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/msgpack/_version.py
--rw-r--r--   0     1000     1000     1081 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0     1000     1000     6088 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0     1000     1000    34475 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0     1000     1000      661 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0     1000     1000      497 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0     1000     1000    11488 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0     1000     1000     4378 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0     1000     1000     1431 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0     1000     1000     8487 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0     1000     1000     4676 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0     1000     1000    30110 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0     1000     1000    15699 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0     1000     1000     4200 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0     1000     1000    14665 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0     1000     1000      130 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0     1000     1000     3457 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/build.py
--rw-r--r--   0     1000     1000     6084 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/check.py
--rw-r--r--   0     1000     1000     4098 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0     1000     1000     1253 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/compat.py
--rw-r--r--   0     1000     1000     1129 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0     1000     1000     6100 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
--rw-r--r--   0     1000     1000      563 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-r--r--   0     1000     1000    11201 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-r--r--   0     1000     1000     2463 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/meta.py
--rw-r--r--   0     1000     1000    13429 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
--rw-r--r--   0     1000     1000   108287 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0     1000     1000      562 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0     1000     1000    12676 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0     1000     1000     1176 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0     1000     1000     4012 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0     1000     1000     4910 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0     1000     1000     2655 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0     1000     1000     6910 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0     1000     1000       80 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0     1000     1000     6439 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0     1000     1000     5294 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/progress/__init__.py
--rw-r--r--   0     1000     1000     2942 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/progress/bar.py
--rw-r--r--   0     1000     1000     2655 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/progress/colors.py
--rw-r--r--   0     1000     1000     1613 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/progress/counter.py
--rw-r--r--   0     1000     1000     1461 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/progress/spinner.py
--rw-r--r--   0     1000     1000     3002 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0     1000     1000      353 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0     1000     1000    23408 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0     1000     1000     1697 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0     1000     1000     1938 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0     1000     1000    40292 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0     1000     1000     2917 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0     1000     1000     5119 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0     1000     1000     6516 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0     1000     1000     3314 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0     1000     1000     5005 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0     1000     1000    35330 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0     1000     1000    21819 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0     1000     1000     5871 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0     1000     1000    18930 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0     1000     1000     5073 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0     1000     1000     2212 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0     1000     1000     5014 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0     1000     1000     7335 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0     1000     1000     4674 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0     1000     1000    11753 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0     1000     1000    31937 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0     1000     1000    11307 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0     1000     1000    70032 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0     1000     1000    52776 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0     1000     1000      986 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0     1000     1000     1727 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0     1000     1000     3072 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0     1000     1000     3091 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0     1000     1000     4630 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0     1000     1000     6257 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0     1000     1000     3252 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0     1000     1000     6143 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0     1000     1000    63188 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0     1000     1000     9123 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0     1000     1000     9107 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0     1000     1000     6429 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0     1000     1000    12936 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0     1000     1000   212248 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0     1000     1000    22165 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0     1000     1000     9030 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0     1000     1000    38299 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0     1000     1000    25339 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0     1000     1000    13388 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0     1000     1000    10381 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0     1000     1000     6805 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0     1000     1000     5130 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0     1000     1000      441 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0     1000     1000     1096 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0     1000     1000    21861 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0     1000     1000     6402 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0     1000     1000    10207 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0     1000     1000      465 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0     1000     1000     2114 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0     1000     1000    18430 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0     1000     1000     3446 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0     1000     1000     3972 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0     1000     1000      757 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0     1000     1000    35116 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0     1000     1000      695 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0     1000     1000    29835 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0     1000     1000     4188 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0     1000     1000     3005 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0     1000     1000    33301 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0     1000     1000      537 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0     1000     1000      156 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0     1000     1000     5872 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0     1000     1000     1583 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0     1000     1000    17592 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0     1000     1000     4794 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0     1000     1000     5804 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0     1000     1000     8810 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0     1000     1000    10096 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0     1000     1000   140235 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0     1000     1000     1064 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0     1000     1000      265 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0     1000     1000     7444 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0     1000     1000     3225 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0     1000     1000     1236 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0     1000     1000     1246 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_lru_cache.py
--rw-r--r--   0     1000     1000     7063 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0     1000     1000      423 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0     1000     1000     5472 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0     1000     1000    26521 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0     1000     1000      351 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0     1000     1000      417 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0     1000     1000     2065 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0     1000     1000     1804 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0     1000     1000      890 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0     1000     1000    10425 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0     1000     1000     6676 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0     1000     1000     3264 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0     1000     1000     9069 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0     1000     1000     4285 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0     1000     1000    17285 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0     1000     1000     1054 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0     1000     1000     7131 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0     1000     1000    81236 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0     1000     1000     1288 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0     1000     1000     5497 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0     1000     1000     5298 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0     1000     1000     7614 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0     1000     1000      183 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0     1000     1000     2501 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0     1000     1000      642 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0     1000     1000     1613 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0     1000     1000     2511 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0     1000     1000     4894 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0     1000     1000     5051 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0     1000     1000     3025 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0     1000     1000    14048 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0     1000     1000    13711 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0     1000     1000     3667 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0     1000     1000    10868 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0     1000     1000     8058 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0     1000     1000     5258 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0     1000     1000     4970 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0     1000     1000      838 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0     1000     1000     3396 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0     1000     1000     8637 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0     1000     1000    32572 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0     1000     1000    35926 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0     1000     1000     7762 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0     1000     1000    11307 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0     1000     1000     1401 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0     1000     1000      166 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0     1000     1000     4309 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0     1000     1000     4197 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0     1000     1000     2842 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0     1000     1000     1591 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0     1000     1000    23916 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0     1000     1000     4312 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0     1000     1000     4425 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0     1000     1000    26469 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0     1000     1000     1258 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0     1000     1000    26994 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0     1000     1000    36757 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0     1000     1000     1700 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/tabulate.py
--rw-r--r--   0     1000     1000     1459 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0     1000     1000    44424 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0     1000     1000     3627 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0     1000     1000      102 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0     1000     1000    25935 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0     1000     1000     9122 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0     1000     1000    34549 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/six.py
--rw-r--r--   0     1000     1000    18257 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0     1000     1000     3314 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0     1000     1000     1944 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0     1000     1000     1496 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0     1000     1000     1376 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0     1000     1000     1908 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0     1000     1000     1383 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0     1000     1000     6645 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0     1000     1000     2790 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0     1000     1000     2145 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0     1000     1000     6691 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0     1000     1000      230 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0     1000     1000    22415 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0     1000     1000     2681 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0     1000     1000    87149 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0     1000     1000     2763 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0     1000     1000    10811 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0     1000     1000       63 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0     1000     1000    20076 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0     1000     1000    39013 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0     1000     1000      957 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0     1000     1000    17632 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0     1000     1000    13922 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0     1000     1000    11034 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0     1000     1000     4538 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0     1000     1000    16900 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0     1000     1000    34449 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0     1000     1000     7097 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0     1000     1000     8217 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0     1000     1000     8579 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0     1000     1000     2440 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0     1000     1000     1417 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0     1000     1000    34666 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0     1000     1000    19763 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0     1000     1000     5985 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0     1000     1000    28203 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0     1000     1000     1155 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0     1000     1000     4901 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0     1000     1000     1605 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0     1000     1000      498 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0     1000     1000     4123 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0     1000     1000     3510 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0     1000     1000    22001 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0     1000     1000    17177 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0     1000     1000     5751 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0     1000     1000     6895 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0     1000     1000    10003 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0     1000     1000    14047 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0     1000     1000     5404 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0     1000     1000      496 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0     1000     1000    10579 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0     1000     1000     8979 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0     1000     1000     1305 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0     1000     1000     6563 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0     1000     1000     4307 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0     1000     1000      286 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip/py.typed
--rw-r--r--   0     1000     1000        4 2023-01-12 08:19:25.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip-22.0.2.dist-info/INSTALLER
--rw-r--r--   0     1000     1000     1093 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip-22.0.2.dist-info/LICENSE.txt
--rw-r--r--   0     1000     1000     4166 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip-22.0.2.dist-info/METADATA
--rw-r--r--   0     1000     1000    79775 2023-01-12 08:19:25.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip-22.0.2.dist-info/RECORD
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:25.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip-22.0.2.dist-info/REQUESTED
--rw-r--r--   0     1000     1000       92 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip-22.0.2.dist-info/WHEEL
--rw-r--r--   0     1000     1000      126 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip-22.0.2.dist-info/entry_points.txt
--rw-r--r--   0     1000     1000        4 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pip-22.0.2.dist-info/top_level.txt
--rw-r--r--   0     1000     1000   108573 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/__init__.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0     1000     1000    24701 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0     1000     1000      661 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0     1000     1000      497 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0     1000     1000    11488 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0     1000     1000     4378 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0     1000     1000     1629 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0     1000     1000     8496 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0     1000     1000     4706 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0     1000     1000    30964 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0     1000     1000    15710 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0     1000     1000     4200 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0     1000     1000    14665 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0     1000     1000   232055 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py
--rw-r--r--   0     1000     1000     2362 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0     1000     1000      104 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
--rw-r--r--   0     1000     1000     7448 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/__init__.py
--rw-r--r--   0     1000     1000      218 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0     1000     1000      536 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0     1000     1000    20813 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0     1000     1000     8572 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0     1000     1000    14894 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0     1000     1000    47644 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0     1000     1000    18079 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0     1000     1000      799 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0     1000     1000     5562 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0     1000     1000     4913 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0     1000     1000    35579 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py
--rw-r--r--   0     1000     1000    21537 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0     1000     1000    16030 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rw-r--r--   0     1000     1000     5773 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0     1000     1000     8022 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0     1000     1000    31612 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0     1000     1000    16495 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0     1000     1000     5963 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0     1000     1000     5637 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0     1000     1000     2776 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0     1000     1000    13117 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0     1000     1000    28970 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0     1000     1000     2822 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0     1000     1000     2753 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0     1000     1000     1298 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0     1000     1000     8397 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0     1000     1000     2017 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0     1000     1000      671 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0     1000     1000    11712 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0     1000     1000    19005 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0     1000     1000     7597 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0     1000     1000     4827 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0     1000     1000     9282 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0     1000     1000    17330 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0     1000     1000      139 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0     1000     1000     3491 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0     1000     1000     7778 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0     1000     1000    50421 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0     1000     1000     3577 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0     1000     1000    10515 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0     1000     1000    17784 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0     1000     1000     8148 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0     1000     1000    13407 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0     1000     1000     1969 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0     1000     1000    30453 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0     1000     1000    23540 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0     1000     1000      455 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/py35compat.py
--rw-r--r--   0     1000     1000      212 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0     1000     1000     3498 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0     1000     1000    22151 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0     1000     1000    12483 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0     1000     1000    14538 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0     1000     1000    20655 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0     1000     1000    13015 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0     1000     1000     5277 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0     1000     1000     2392 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_imp.py
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0     1000     1000       82 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0     1000     1000   117968 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0     1000     1000    16256 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0     1000     1000    15130 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0     1000     1000      661 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0     1000     1000      497 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0     1000     1000    11488 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0     1000     1000     4378 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0     1000     1000     1629 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0     1000     1000     8493 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0     1000     1000     4700 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0     1000     1000    30964 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0     1000     1000    15710 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0     1000     1000     4200 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0     1000     1000    14665 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0     1000     1000   232055 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/_vendor/pyparsing.py
--rw-r--r--   0     1000     1000     7077 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/archive_util.py
--rw-r--r--   0     1000     1000    10536 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/build_meta.py
--rw-r--r--   0     1000     1000    65536 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/cli-32.exe
--rw-r--r--   0     1000     1000    74752 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/cli-64.exe
--rw-r--r--   0     1000     1000   137216 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/cli-arm64.exe
--rw-r--r--   0     1000     1000    65536 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/cli.exe
--rw-r--r--   0     1000     1000      217 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/__init__.py
--rw-r--r--   0     1000     1000     2381 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/alias.py
--rw-r--r--   0     1000     1000    16604 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0     1000     1000     1182 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0     1000     1000     4415 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0     1000     1000    13212 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0     1000     1000     8751 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/build_py.py
--rw-r--r--   0     1000     1000     7012 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/develop.py
--rw-r--r--   0     1000     1000      960 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0     1000     1000    87973 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0     1000     1000    26134 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0     1000     1000     4906 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/install.py
--rw-r--r--   0     1000     1000     3195 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0     1000     1000     5036 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0     1000     1000     2593 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0     1000     1000      628 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0     1000     1000     4946 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0     1000     1000      468 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/register.py
--rw-r--r--   0     1000     1000     2128 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/rotate.py
--rw-r--r--   0     1000     1000      658 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0     1000     1000     6413 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/sdist.py
--rw-r--r--   0     1000     1000     5086 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/setopt.py
--rw-r--r--   0     1000     1000     8088 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/test.py
--rw-r--r--   0     1000     1000      462 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/upload.py
--rw-r--r--   0     1000     1000     7218 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0     1000     1000    23153 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/config.py
--rw-r--r--   0     1000     1000      949 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/dep_util.py
--rw-r--r--   0     1000     1000     5499 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/depends.py
--rw-r--r--   0     1000     1000    43162 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/dist.py
--rw-r--r--   0     1000     1000     1555 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/errors.py
--rw-r--r--   0     1000     1000     1684 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/extension.py
--rw-r--r--   0     1000     1000     2407 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0     1000     1000     4873 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/glob.py
--rw-r--r--   0     1000     1000    65536 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/gui-32.exe
--rw-r--r--   0     1000     1000    75264 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/gui-64.exe
--rw-r--r--   0     1000     1000   137728 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/gui-arm64.exe
--rw-r--r--   0     1000     1000    65536 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/gui.exe
--rw-r--r--   0     1000     1000     3824 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/installer.py
--rw-r--r--   0     1000     1000      812 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/launch.py
--rw-r--r--   0     1000     1000     5217 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/monkey.py
--rw-r--r--   0     1000     1000    50561 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/msvc.py
--rw-r--r--   0     1000     1000     3093 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/namespaces.py
--rw-r--r--   0     1000     1000    40092 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/package_index.py
--rw-r--r--   0     1000     1000      245 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/py34compat.py
--rw-r--r--   0     1000     1000    14348 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/sandbox.py
--rw-r--r--   0     1000     1000      218 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0     1000     1000      138 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/script.tmpl
--rw-r--r--   0     1000     1000      941 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0     1000     1000      144 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/version.py
--rw-r--r--   0     1000     1000     8288 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/wheel.py
--rw-r--r--   0     1000     1000      714 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools/windows_support.py
--rw-r--r--   0     1000     1000        4 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools-59.6.0.dist-info/INSTALLER
--rw-r--r--   0     1000     1000     1050 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools-59.6.0.dist-info/LICENSE
--rw-r--r--   0     1000     1000     4963 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools-59.6.0.dist-info/METADATA
--rw-r--r--   0     1000     1000    23275 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools-59.6.0.dist-info/RECORD
--rw-r--r--   0     1000     1000        0 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools-59.6.0.dist-info/REQUESTED
--rw-r--r--   0     1000     1000       92 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools-59.6.0.dist-info/WHEEL
--rw-r--r--   0     1000     1000     2636 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools-59.6.0.dist-info/entry_points.txt
--rw-r--r--   0     1000     1000       48 2023-01-12 08:19:24.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/setuptools-59.6.0.dist-info/top_level.txt
--rw-r--r--   0     1000     1000      396 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli/__init__.py
--rw-r--r--   0     1000     1000    22633 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli/_parser.py
--rw-r--r--   0     1000     1000     2943 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli/_re.py
--rw-r--r--   0     1000     1000      254 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli/_types.py
--rw-r--r--   0     1000     1000       26 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli/py.typed
--rw-r--r--   0     1000     1000        4 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/INSTALLER
--rw-r--r--   0     1000     1000     1072 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/LICENSE
--rw-r--r--   0     1000     1000     8875 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/METADATA
--rw-r--r--   0     1000     1000      913 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/RECORD
--rw-r--r--   0     1000     1000       81 2023-01-12 08:19:51.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/tomli-2.0.1.dist-info/WHEEL
--rw-r--r--   0     1000     1000        4 2023-03-02 06:01:38.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/wot_datfile_parser_py-0.2.0.dist-info/INSTALLER
--rw-r--r--   0     1000     1000     1213 2023-03-02 06:01:38.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/wot_datfile_parser_py-0.2.0.dist-info/METADATA
--rw-r--r--   0     1000     1000      647 2023-03-02 06:01:38.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/wot_datfile_parser_py-0.2.0.dist-info/RECORD
--rw-r--r--   0     1000     1000        0 2023-03-02 06:01:38.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/wot_datfile_parser_py-0.2.0.dist-info/REQUESTED
--rw-r--r--   0     1000     1000      100 2023-03-02 06:01:38.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/wot_datfile_parser_py-0.2.0.dist-info/WHEEL
--rw-r--r--   0     1000     1000      110 2023-03-02 06:01:38.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/wot_datfile_parser_py-0.2.0.dist-info/direct_url.json
--rw-r--r--   0     1000     1000       43 2023-03-02 06:01:38.000000 wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/wot_datfile_parser_py.pth
--rw-r--r--   0     1000     1000       70 2023-01-12 08:19:23.000000 wot_datfile_parser_py-0.2.0/dp/pyvenv.cfg
--rw-r--r--   0     1000     1000     5704 2023-03-02 05:59:30.000000 wot_datfile_parser_py-0.2.0/example/9252658313363554.dat
--rw-r--r--   0     1000     1000      231 2023-03-02 06:03:23.000000 wot_datfile_parser_py-0.2.0/example/simple.py
--rw-r--r--   0     1000     1000       53 2023-01-27 07:12:03.000000 wot_datfile_parser_py-0.2.0/justfile
--rw-r--r--   0     1000     1000      329 2023-01-27 06:39:00.000000 wot_datfile_parser_py-0.2.0/pyproject.toml
--rw-r--r--   0     1000     1000      791 2023-01-27 06:24:02.000000 wot_datfile_parser_py-0.2.0/src/lib.rs
--rw-r--r--   0     1000     1000      350 2023-01-27 06:54:13.000000 wot_datfile_parser_py-0.2.0/wot_datfile_parser_py/__init__.py
--rw-r--r--   0     1000     1000    27367 2023-03-02 06:01:29.000000 wot_datfile_parser_py-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1213 1970-01-01 00:00:00.000000 wot_datfile_parser_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 wot_datfile_parser_py-0.2.1/Cargo.toml
+-rw-r--r--   0     1000     1000     1683 2023-01-27 07:12:36.000000 wot_datfile_parser_py-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      690 2023-03-02 06:14:20.000000 wot_datfile_parser_py-0.2.1/.gitignore
+-rw-r--r--   0     1000     1000      324 2023-01-27 06:23:51.000000 wot_datfile_parser_py-0.2.1/.rustfmt.toml
+-rw-r--r--   0     1000     1000      867 2023-03-02 06:13:29.000000 wot_datfile_parser_py-0.2.1/README.md
+-rw-r--r--   0     1000     1000     5447 2023-05-13 21:51:27.000000 wot_datfile_parser_py-0.2.1/example/20243720148301877.dat
+-rw-r--r--   0     1000     1000     5704 2023-03-02 05:59:30.000000 wot_datfile_parser_py-0.2.1/example/9252658313363554.dat
+-rw-r--r--   0     1000     1000      232 2023-05-13 21:51:32.000000 wot_datfile_parser_py-0.2.1/example/simple.py
+-rw-r--r--   0     1000     1000       53 2023-01-27 07:12:03.000000 wot_datfile_parser_py-0.2.1/justfile
+-rw-r--r--   0     1000     1000      329 2023-01-27 06:39:00.000000 wot_datfile_parser_py-0.2.1/pyproject.toml
+-rw-r--r--   0     1000     1000      791 2023-01-27 06:24:02.000000 wot_datfile_parser_py-0.2.1/src/lib.rs
+-rw-r--r--   0     1000     1000      350 2023-01-27 06:54:13.000000 wot_datfile_parser_py-0.2.1/wot_datfile_parser_py/__init__.py
+-rw-r--r--   0     1000     1000    27367 2023-05-13 21:56:56.000000 wot_datfile_parser_py-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 wot_datfile_parser_py-0.2.1/PKG-INFO
```

### Comparing `wot_datfile_parser_py-0.2.0/.github/workflows/CI.yml` & `wot_datfile_parser_py-0.2.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `wot_datfile_parser_py-0.2.0/.gitignore` & `wot_datfile_parser_py-0.2.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -65,8 +65,10 @@
 # PyCharm
 .idea/
 
 # VSCode
 .vscode/
 
 # Pyenv
-.python-version
+.python-version
+
+dp/
```

### Comparing `wot_datfile_parser_py-0.2.0/README.md` & `wot_datfile_parser_py-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# World of Tanks Datfile Parser (Python) `WIP`
+# World of Tanks Datfile Parser (Python)
 A parser for `.dat` battle result files generated by the game World of Tanks. `.dat` files are generated whenever a battle's results are viewed in-game. For Windows, these files are found in a location like:
 ```
 C:\Users\<YOUR_USER_NAME>\AppData\Roaming\Wargaming.net\WorldOfTanks\battle_results
 ```
 This project simply provides python bindings for the Rust library: [`wot_datfile_parser`](https://github.com/dacite/wot-battle-results-parser/tree/main/datfile_parser)
 
 Install with:
```

### Comparing `wot_datfile_parser_py-0.2.0/dp/lib64/python3.10/site-packages/wot_datfile_parser_py-0.2.0.dist-info/METADATA` & `wot_datfile_parser_py-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: wot_datfile_parser_py
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# World of Tanks Datfile Parser (Python) `WIP`
+# World of Tanks Datfile Parser (Python)
 A parser for `.dat` battle result files generated by the game World of Tanks. `.dat` files are generated whenever a battle's results are viewed in-game. For Windows, these files are found in a location like:
 ```
 C:\Users\<YOUR_USER_NAME>\AppData\Roaming\Wargaming.net\WorldOfTanks\battle_results
 ```
 This project simply provides python bindings for the Rust library: [`wot_datfile_parser`](https://github.com/dacite/wot-battle-results-parser/tree/main/datfile_parser)
 
 Install with:
```

### Comparing `wot_datfile_parser_py-0.2.0/example/9252658313363554.dat` & `wot_datfile_parser_py-0.2.1/example/9252658313363554.dat`

 * *Files identical despite different names*

### Comparing `wot_datfile_parser_py-0.2.0/src/lib.rs` & `wot_datfile_parser_py-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `wot_datfile_parser_py-0.2.0/Cargo.lock` & `wot_datfile_parser_py-0.2.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1014,17 +1014,17 @@
  "serde",
  "serde-pickle",
  "thiserror",
 ]
 
 [[package]]
 name = "wot_datfile_parser"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12fcfc0121bd29e1a1a862a6c762e174022402a3b034aa6743ed032a787dea66"
+checksum = "46d887e9ad74fa48005fdeac103902cca58190a19e4c3935ea7f3a9d7fad5340"
 dependencies = [
  "byteorder",
  "crc",
  "hex",
  "itertools",
  "miniz_oxide",
  "nom",
@@ -1036,15 +1036,15 @@
  "thiserror",
  "wot-battle-results-parser-utils",
  "wot_types",
 ]
 
 [[package]]
 name = "wot_datfile_parser_py"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "pyo3",
  "serde_json",
  "wot_datfile_parser",
 ]
 
 [[package]]
```

