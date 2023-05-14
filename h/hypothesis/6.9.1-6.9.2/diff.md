# Comparing `tmp/hypothesis-6.9.1.tar.gz` & `tmp/hypothesis-6.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis-6.9.1.tar", last modified: Mon Apr 12 07:16:19 2021, max compression
+gzip compressed data, was "hypothesis-6.9.2.tar", last modified: Thu Apr 15 03:58:37 2021, max compression
```

## Comparing `hypothesis-6.9.1.tar` & `hypothesis-6.9.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.259216 hypothesis-6.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    17141 2021-04-12 07:15:42.000000 hypothesis-6.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-04-12 07:15:42.000000 hypothesis-6.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-12 07:16:19.259216 hypothesis-6.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2021-04-12 07:15:42.000000 hypothesis-6.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-04-12 07:16:19.259216 hypothesis-6.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4976 2021-04-12 07:15:42.000000 hypothesis-6.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.247215 hypothesis-6.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.251216 hypothesis-6.9.1/src/hypothesis/
--rw-r--r--   0 runner    (1001) docker     (121)     1726 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/_error_if_old.py
--rw-r--r--   0 runner    (1001) docker     (121)    24218 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     7312 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/control.py
--rw-r--r--   0 runner    (1001) docker     (121)    53552 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    11964 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (121)     5733 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/executors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.251216 hypothesis-6.9.1/src/hypothesis/extra/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9209 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     8546 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/codemods.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/dateutil.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.251216 hypothesis-6.9.1/src/hypothesis/extra/django/
--rw-r--r--   0 runner    (1001) docker     (121)      957 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12290 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/django/_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     8805 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/django/_impl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/dpcontracts.py
--rw-r--r--   0 runner    (1001) docker     (121)    45489 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/ghostwriter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9203 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/lark.py
--rw-r--r--   0 runner    (1001) docker     (121)    61961 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.251216 hypothesis-6.9.1/src/hypothesis/extra/pandas/
--rw-r--r--   0 runner    (1001) docker     (121)      836 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25023 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/pandas/impl.py
--rw-r--r--   0 runner    (1001) docker     (121)    12577 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/pytz.py
--rw-r--r--   0 runner    (1001) docker     (121)     3019 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/extra/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.255216 hypothesis-6.9.1/src/hypothesis/internal/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9574 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/cathetus.py
--rw-r--r--   0 runner    (1001) docker     (121)    13068 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/charmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     7535 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.255216 hypothesis-6.9.1/src/hypothesis/internal/conjecture/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4519 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/choicetree.py
--rw-r--r--   0 runner    (1001) docker     (121)    36398 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    16695 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/datatree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.255216 hypothesis-6.9.1/src/hypothesis/internal/conjecture/dfa/
--rw-r--r--   0 runner    (1001) docker     (121)    24097 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/dfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19512 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/dfa/lstar.py
--rw-r--r--   0 runner    (1001) docker     (121)    44863 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     7818 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/floats.py
--rw-r--r--   0 runner    (1001) docker     (121)     9898 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/junkdrawer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7545 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/optimiser.py
--rw-r--r--   0 runner    (1001) docker     (121)    14559 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/pareto.py
--rw-r--r--   0 runner    (1001) docker     (121)    58461 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.255216 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/
--rw-r--r--   0 runner    (1001) docker     (121)      949 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5648 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    12080 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/dfas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3351 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/floats.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/integer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2051 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/learned_dfas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2054 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/lexical.py
--rw-r--r--   0 runner    (1001) docker     (121)     3744 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/ordering.py
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/conjecture/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3475 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/coverage.py
--rw-r--r--   0 runner    (1001) docker     (121)      820 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/detection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/entropy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4134 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/escalation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4963 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)     2889 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/floats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/intervalsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/lazyformat.py
--rw-r--r--   0 runner    (1001) docker     (121)    19891 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4726 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/scrutineer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4324 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/internal/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     6611 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/provisional.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/reporting.py
--rw-r--r--   0 runner    (1001) docker     (121)    30138 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/stateful.py
--rw-r--r--   0 runner    (1001) docker     (121)     5284 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.255216 hypothesis-6.9.1/src/hypothesis/strategies/
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.259216 hypothesis-6.9.1/src/hypothesis/strategies/_internal/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6776 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/attrs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9836 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/collections.py
--rw-r--r--   0 runner    (1001) docker     (121)    75301 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    20361 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/deferred.py
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/featureflags.py
--rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/flatmapped.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/ipaddress.py
--rw-r--r--   0 runner    (1001) docker     (121)     5851 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/lazy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3876 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    17420 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/numbers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13063 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/random.py
--rw-r--r--   0 runner    (1001) docker     (121)     3962 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/recursive.py
--rw-r--r--   0 runner    (1001) docker     (121)    18063 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/regex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/shared.py
--rw-r--r--   0 runner    (1001) docker     (121)    36513 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/strategies.py
--rw-r--r--   0 runner    (1001) docker     (121)     4256 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/strings.py
--rw-r--r--   0 runner    (1001) docker     (121)    28517 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/strategies/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.259216 hypothesis-6.9.1/src/hypothesis/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      761 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/utils/conventions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/utils/dynamicvariables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.259216 hypothesis-6.9.1/src/hypothesis/vendor/
--rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27443 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/vendor/pretty.py
--rw-r--r--   0 runner    (1001) docker     (121)    10309 2021-04-12 07:15:42.000000 hypothesis-6.9.1/src/hypothesis/vendor/tlds-alpha-by-domain.txt
--rw-r--r--   0 runner    (1001) docker     (121)      699 2021-04-12 07:16:18.000000 hypothesis-6.9.1/src/hypothesis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-12 07:16:19.251216 hypothesis-6.9.1/src/hypothesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-12 07:16:19.000000 hypothesis-6.9.1/src/hypothesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4242 2021-04-12 07:16:19.000000 hypothesis-6.9.1/src/hypothesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-12 07:16:19.000000 hypothesis-6.9.1/src/hypothesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-04-12 07:16:19.000000 hypothesis-6.9.1/src/hypothesis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-12 07:16:19.000000 hypothesis-6.9.1/src/hypothesis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      971 2021-04-12 07:16:19.000000 hypothesis-6.9.1/src/hypothesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-04-12 07:16:19.000000 hypothesis-6.9.1/src/hypothesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.878723 hypothesis-6.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    17141 2021-04-15 03:57:57.000000 hypothesis-6.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-04-15 03:57:57.000000 hypothesis-6.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-15 03:58:37.878723 hypothesis-6.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2131 2021-04-15 03:57:57.000000 hypothesis-6.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-04-15 03:58:37.878723 hypothesis-6.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4976 2021-04-15 03:57:57.000000 hypothesis-6.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.862722 hypothesis-6.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.866722 hypothesis-6.9.2/src/hypothesis/
+-rw-r--r--   0 runner    (1001) docker     (121)     1726 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/_error_if_old.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24218 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7312 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/control.py
+-rw-r--r--   0 runner    (1001) docker     (121)    53552 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11964 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5733 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2036 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/executors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.866722 hypothesis-6.9.2/src/hypothesis/extra/
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9209 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8546 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/codemods.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2432 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/dateutil.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.870722 hypothesis-6.9.2/src/hypothesis/extra/django/
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12290 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/django/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8805 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/django/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1997 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/dpcontracts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48572 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/ghostwriter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9203 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/lark.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61961 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.870722 hypothesis-6.9.2/src/hypothesis/extra/pandas/
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25023 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/pandas/impl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12577 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2077 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/pytz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3019 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/extra/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.870722 hypothesis-6.9.2/src/hypothesis/internal/
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9574 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2442 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/cathetus.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13068 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/charmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7535 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.874723 hypothesis-6.9.2/src/hypothesis/internal/conjecture/
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4519 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/choicetree.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36398 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16695 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/datatree.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.874723 hypothesis-6.9.2/src/hypothesis/internal/conjecture/dfa/
+-rw-r--r--   0 runner    (1001) docker     (121)    24097 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/dfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19512 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/dfa/lstar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44863 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7818 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/floats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9898 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/junkdrawer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7545 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/optimiser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14559 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (121)    58461 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.874723 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/
+-rw-r--r--   0 runner    (1001) docker     (121)      949 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5648 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12080 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/dfas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3351 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/floats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/integer.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2051 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/learned_dfas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2054 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/lexical.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3744 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/conjecture/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3475 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (121)      820 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/detection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3756 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4134 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4963 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2889 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/floats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/intervalsets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1237 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/lazyformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20011 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4726 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/scrutineer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4324 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/internal/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6611 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/provisional.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30138 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5284 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.874723 hypothesis-6.9.2/src/hypothesis/strategies/
+-rw-r--r--   0 runner    (1001) docker     (121)     3026 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.878723 hypothesis-6.9.2/src/hypothesis/strategies/_internal/
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6776 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9836 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)    75301 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20361 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3314 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4642 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/featureflags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1734 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/flatmapped.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2113 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4477 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/ipaddress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5851 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3876 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17420 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13063 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/random.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3962 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18063 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/regex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36513 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4256 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/strings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28517 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4280 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/strategies/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.878723 hypothesis-6.9.2/src/hypothesis/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/utils/conventions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1182 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/utils/dynamicvariables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.878723 hypothesis-6.9.2/src/hypothesis/vendor/
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27443 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/vendor/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10309 2021-04-15 03:57:57.000000 hypothesis-6.9.2/src/hypothesis/vendor/tlds-alpha-by-domain.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      699 2021-04-15 03:58:36.000000 hypothesis-6.9.2/src/hypothesis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-15 03:58:37.866722 hypothesis-6.9.2/src/hypothesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-04-15 03:58:37.000000 hypothesis-6.9.2/src/hypothesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4242 2021-04-15 03:58:37.000000 hypothesis-6.9.2/src/hypothesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-15 03:58:37.000000 hypothesis-6.9.2/src/hypothesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-04-15 03:58:37.000000 hypothesis-6.9.2/src/hypothesis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-15 03:58:37.000000 hypothesis-6.9.2/src/hypothesis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2021-04-15 03:58:37.000000 hypothesis-6.9.2/src/hypothesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-04-15 03:58:37.000000 hypothesis-6.9.2/src/hypothesis.egg-info/top_level.txt
```

### Comparing `hypothesis-6.9.1/LICENSE.txt` & `hypothesis-6.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/PKG-INFO` & `hypothesis-6.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis
-Version: 6.9.1
+Version: 6.9.2
 Summary: A library for property-based testing
 Home-page: https://github.com/HypothesisWorks/hypothesis/tree/master/hypothesis-python
 Author: David R. MacIver
 Author-email: david@drmaciver.com
 License: MPL v2
 Project-URL: Website, https://hypothesis.works
 Project-URL: Documentation, https://hypothesis.readthedocs.io
```

### Comparing `hypothesis-6.9.1/README.rst` & `hypothesis-6.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/setup.py` & `hypothesis-6.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/__init__.py` & `hypothesis-6.9.2/src/hypothesis/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/_error_if_old.py` & `hypothesis-6.9.2/src/hypothesis/_error_if_old.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/_settings.py` & `hypothesis-6.9.2/src/hypothesis/_settings.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/configuration.py` & `hypothesis-6.9.2/src/hypothesis/configuration.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/control.py` & `hypothesis-6.9.2/src/hypothesis/control.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/core.py` & `hypothesis-6.9.2/src/hypothesis/core.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/database.py` & `hypothesis-6.9.2/src/hypothesis/database.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/entry_points.py` & `hypothesis-6.9.2/src/hypothesis/entry_points.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/errors.py` & `hypothesis-6.9.2/src/hypothesis/errors.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/executors.py` & `hypothesis-6.9.2/src/hypothesis/executors.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/__init__.py` & `hypothesis-6.9.2/src/hypothesis/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/cli.py` & `hypothesis-6.9.2/src/hypothesis/extra/cli.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/codemods.py` & `hypothesis-6.9.2/src/hypothesis/extra/codemods.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/dateutil.py` & `hypothesis-6.9.2/src/hypothesis/extra/dateutil.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/django/__init__.py` & `hypothesis-6.9.2/src/hypothesis/extra/django/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/django/_fields.py` & `hypothesis-6.9.2/src/hypothesis/extra/django/_fields.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/django/_impl.py` & `hypothesis-6.9.2/src/hypothesis/extra/django/_impl.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/dpcontracts.py` & `hypothesis-6.9.2/src/hypothesis/extra/dpcontracts.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/ghostwriter.py` & `hypothesis-6.9.2/src/hypothesis/extra/ghostwriter.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 from hypothesis.strategies._internal.lazy import LazyStrategy, unwrap_strategies
 from hypothesis.strategies._internal.strategies import (
     FilteredStrategy,
     MappedSearchStrategy,
     OneOfStrategy,
     SampledFromStrategy,
 )
-from hypothesis.strategies._internal.types import _global_type_lookup
+from hypothesis.strategies._internal.types import _global_type_lookup, is_generic_type
 from hypothesis.utils.conventions import InferType, infer
 
 IMPORT_SECTION = """
 # This test code was written by the `hypothesis.extra.ghostwriter` module
 # and is provided under the Creative Commons Zero public domain dedication.
 
 {imports}
@@ -125,20 +125,31 @@
 """
 
 SUPPRESS_BLOCK = """\
 try:
 {test_body}
 except {exceptions}:
     reject()
-"""
+""".rstrip()
 
 Except = Union[Type[Exception], Tuple[Type[Exception], ...]]
 RE_TYPES = (type(re.compile(".")), type(re.match(".", "abc")))
 
 
+def _dedupe_exceptions(exc: Tuple[Type[Exception], ...]) -> Tuple[Type[Exception], ...]:
+    # This is reminiscent of de-duplication logic I wrote for flake8-bugbear,
+    # but with access to the actual objects we can just check for subclasses.
+    # This lets us print e.g. `Exception` instead of `(Exception, OSError)`.
+    uniques = list(exc)
+    for a, b in permutations(exc, 2):
+        if a in uniques and issubclass(a, b):
+            uniques.remove(a)
+    return tuple(sorted(uniques, key=lambda e: e.__name__))
+
+
 def _check_except(except_: Except) -> Tuple[Type[Exception], ...]:
     if isinstance(except_, tuple):
         for i, e in enumerate(except_):
             if not isinstance(e, type) or not issubclass(e, Exception):
                 raise InvalidArgument(
                     f"Expected an Exception but got except_[{i}]={e!r}"
                     f" (type={_get_qualname(type(e))})"
@@ -153,14 +164,32 @@
 
 
 def _check_style(style: str) -> None:
     if style not in ("pytest", "unittest"):
         raise InvalidArgument(f"Valid styles are 'pytest' or 'unittest', got {style!r}")
 
 
+def _exceptions_from_docstring(doc: str) -> Tuple[Type[Exception], ...]:
+    """Return a tuple of exceptions that the docstring says may be raised.
+
+    Note that we ignore non-builtin exception types for simplicity, as this is
+    used directly in _write_call() and passing import sets around would be really
+    really annoying.
+    """
+    # TODO: it would be great to handle Google- and Numpy-style docstrings
+    #       (e.g. by using the Napoleon Sphinx extension)
+    assert isinstance(doc, str), doc
+    raises = []
+    for excname in re.compile(r"\:raises\s+(\w+)\:", re.MULTILINE).findall(doc):
+        exc_type = getattr(builtins, excname, None)
+        if isinstance(exc_type, type) and issubclass(exc_type, Exception):
+            raises.append(exc_type)
+    return tuple(_dedupe_exceptions(tuple(raises)))
+
+
 # Simple strategies to guess for common argument names - we wouldn't do this in
 # builds() where strict correctness is required, but we only use these guesses
 # when the alternative is nothing() to force user edits anyway.
 #
 # This table was constructed manually after skimming through the documentation
 # for the builtins and a few stdlib modules.  Future enhancements could be based
 # on analysis of type-annotated code to detect arguments which almost always
@@ -298,28 +327,33 @@
     # If there is only one function, we pass arguments to @given in the order of
     # that function's signature.  Otherwise, we use alphabetical order.
     if len(funcs) == 1:
         return {name: given_strategies[name] for name in _get_params(f)}
     return dict(sorted(given_strategies.items()))
 
 
-def _assert_eq(style, a, b):
+def _assert_eq(style: str, a: str, b: str) -> str:
     if style == "unittest":
         return f"self.assertEqual({a}, {b})"
     assert style == "pytest"
     if a.isidentifier() and b.isidentifier():
         return f"assert {a} == {b}, ({a}, {b})"
     return f"assert {a} == {b}"
 
 
 def _imports_for_object(obj):
     """Return the imports for `obj`, which may be empty for e.g. lambdas"""
     if isinstance(obj, RE_TYPES):
         return {"re"}
     try:
+        if is_generic_type(obj):
+            if isinstance(obj, TypeVar):
+                return {(obj.__module__, obj.__name__)}
+            with contextlib.suppress(Exception):
+                return set().union(*map(_imports_for_object, obj.__args__))
         if (not callable(obj)) or obj.__name__ == "<lambda>":
             return set()
         name = _get_qualname(obj).split(".")[0]
         return {(_get_module(obj), name)}
     except Exception:
         with contextlib.suppress(AttributeError):
             if obj.__module__ == "typing":  # only on CPython 3.6
@@ -434,27 +468,46 @@
     qname = getattr(obj, "__qualname__", obj.__name__)
     qname = qname.replace("<", "_").replace(">", "_").replace(" ", "")
     if include_module:
         return _get_module(obj) + "." + qname
     return qname
 
 
-def _write_call(func: Callable, *pass_variables: str) -> str:
+def _write_call(
+    func: Callable, *pass_variables: str, except_: Except, assign: str = ""
+) -> str:
     """Write a call to `func` with explicit and implicit arguments.
 
     >>> _write_call(sorted, "my_seq", "func")
     "builtins.sorted(my_seq, key=func, reverse=reverse)"
+
+    >>> write_call(f, assign="var1")
+    "var1 = f()"
+
+    The fancy part is that we'll check the docstring for any known exceptions
+    which `func` might raise, and catch-and-reject on them... *unless* they're
+    subtypes of `except_`, which will be handled in an outer try-except block.
     """
     args = ", ".join(
         (v or p.name)
         if p.kind is inspect.Parameter.POSITIONAL_ONLY
         else f"{p.name}={v or p.name}"
         for v, p in zip_longest(pass_variables, _get_params(func).values())
     )
-    return f"{_get_qualname(func, include_module=True)}({args})"
+    call = f"{_get_qualname(func, include_module=True)}({args})"
+    if assign:
+        call = f"{assign} = {call}"
+    raises = _exceptions_from_docstring(getattr(func, "__doc__", "") or "")
+    exnames = [ex.__name__ for ex in raises if not issubclass(ex, except_)]
+    if not exnames:
+        return call
+    return SUPPRESS_BLOCK.format(
+        test_body=indent(call, prefix="    "),
+        exceptions="(" + ", ".join(exnames) + ")" if len(exnames) > 1 else exnames[0],
+    )
 
 
 def _st_strategy_names(s: str) -> str:
     """Replace strategy name() with st.name().
 
     Uses a tricky re.sub() to avoid problems with frozensets() matching
     sets() too.
@@ -464,14 +517,15 @@
 
 
 def _make_test_body(
     *funcs: Callable,
     ghost: str,
     test_body: str,
     except_: Tuple[Type[Exception], ...],
+    assertions: str = "",
     style: str,
     given_strategies: Optional[Mapping[str, Union[str, st.SearchStrategy]]] = None,
 ) -> Tuple[Set[Union[str, Tuple[str, str]]], str]:
     # A set of modules to import - we might add to this later.  The import code
     # is written later, so we can have one import section for multiple magic()
     # test functions.
     imports = {_get_module(f) for f in funcs}
@@ -483,38 +537,34 @@
         )
         reprs = [((k,) + _valid_syntax_repr(v)) for k, v in given_strategies.items()]
         imports = imports.union(*(imp for _, imp, _ in reprs))
         given_args = ", ".join(f"{k}={v}" for k, _, v in reprs)
     given_args = _st_strategy_names(given_args)
 
     if except_:
-        # This is reminiscent of de-duplication logic I wrote for flake8-bugbear,
-        # but with access to the actual objects we can just check for subclasses.
-        # This lets us print e.g. `Exception` instead of `(Exception, OSError)`.
-        uniques = list(except_)
-        for a, b in permutations(except_, 2):
-            if a in uniques and issubclass(a, b):
-                uniques.remove(a)
-        # Then convert to strings, either builtin names or qualified names.
+        # Convert to strings, either builtin names or qualified names.
         exceptions = []
-        for ex in uniques:
+        for ex in _dedupe_exceptions(except_):
             if ex.__qualname__ in dir(builtins):
                 exceptions.append(ex.__qualname__)
             else:
                 imports.add(ex.__module__)
                 exceptions.append(_get_qualname(ex, include_module=True))
         # And finally indent the existing test body into a try-except block
         # which catches these exceptions and calls `hypothesis.reject()`.
         test_body = SUPPRESS_BLOCK.format(
             test_body=indent(test_body, prefix="    "),
             exceptions="(" + ", ".join(exceptions) + ")"
             if len(exceptions) > 1
             else exceptions[0],
         )
 
+    if assertions:
+        test_body = f"{test_body}\n{assertions}"
+
     # Indent our test code to form the body of a function or method.
     argnames = (["self"] if style == "unittest" else []) + list(given_strategies)
     body = TEMPLATE.format(
         given_args=given_args,
         test_kind=ghost,
         func_name="_".join(_get_qualname(f).replace(".", "_") for f in funcs),
         arg_names=", ".join(argnames),
@@ -731,15 +781,17 @@
                 make_(_make_ufunc_body, func)
                 del by_name[name]
 
     # For all remaining callables, just write a fuzz-test.  In principle we could
     # guess at equivalence or idempotence; but it doesn't seem accurate enough to
     # be worth the trouble when it's so easy for the user to specify themselves.
     for _, f in sorted(by_name.items()):
-        make_(_make_test_body, f, test_body=_write_call(f), ghost="fuzz")
+        make_(
+            _make_test_body, f, test_body=_write_call(f, except_=except_), ghost="fuzz"
+        )
     return _make_test(imports, "\n".join(parts))
 
 
 def fuzz(func: Callable, *, except_: Except = (), style: str = "pytest") -> str:
     """Write source code for a property-based test of ``func``.
 
     The resulting test checks that valid input only leads to expected exceptions.
@@ -780,15 +832,19 @@
     """
     if not callable(func):
         raise InvalidArgument(f"Got non-callable func={func!r}")
     except_ = _check_except(except_)
     _check_style(style)
 
     imports, body = _make_test_body(
-        func, test_body=_write_call(func), except_=except_, ghost="fuzz", style=style
+        func,
+        test_body=_write_call(func, except_=except_),
+        except_=except_,
+        ghost="fuzz",
+        style=style,
     )
     return _make_test(imports, body)
 
 
 def idempotent(func: Callable, *, except_: Except = (), style: str = "pytest") -> str:
     """Write source code for a property-based test of ``func``.
 
@@ -825,40 +881,42 @@
             assert result == repeat, (result, repeat)
     """
     if not callable(func):
         raise InvalidArgument(f"Got non-callable func={func!r}")
     except_ = _check_except(except_)
     _check_style(style)
 
-    test_body = "result = {}\nrepeat = {}\n{}".format(
-        _write_call(func),
-        _write_call(func, "result"),
-        _assert_eq(style, "result", "repeat"),
-    )
-
     imports, body = _make_test_body(
-        func, test_body=test_body, except_=except_, ghost="idempotent", style=style
+        func,
+        test_body="result = {}\nrepeat = {}".format(
+            _write_call(func, except_=except_),
+            _write_call(func, "result", except_=except_),
+        ),
+        except_=except_,
+        assertions=_assert_eq(style, "result", "repeat"),
+        ghost="idempotent",
+        style=style,
     )
     return _make_test(imports, body)
 
 
 def _make_roundtrip_body(funcs, except_, style):
     first_param = next(iter(_get_params(funcs[0])))
     test_lines = [
-        "value0 = " + _write_call(funcs[0]),
+        _write_call(funcs[0], assign="value0", except_=except_),
         *(
-            f"value{i + 1} = " + _write_call(f, f"value{i}")
+            _write_call(f, f"value{i}", assign=f"value{i + 1}", except_=except_)
             for i, f in enumerate(funcs[1:])
         ),
-        _assert_eq(style, first_param, f"value{len(funcs) - 1}"),
     ]
     return _make_test_body(
         *funcs,
         test_body="\n".join(test_lines),
         except_=except_,
+        assertions=_assert_eq(style, first_param, f"value{len(funcs) - 1}"),
         ghost="roundtrip",
         style=style,
     )
 
 
 def roundtrip(*funcs: Callable, except_: Except = (), style: str = "pytest") -> str:
     """Write source code for a property-based test of ``funcs``.
@@ -885,21 +943,26 @@
 
 
 def _make_equiv_body(funcs, except_, style):
     var_names = [f"result_{f.__name__}" for f in funcs]
     if len(set(var_names)) < len(var_names):
         var_names = [f"result_{i}_{ f.__name__}" for i, f in enumerate(funcs)]
     test_lines = [
-        vname + " = " + _write_call(f) for vname, f in zip(var_names, funcs)
-    ] + [_assert_eq(style, var_names[0], vname) for vname in var_names[1:]]
+        _write_call(f, assign=vname, except_=except_)
+        for vname, f in zip(var_names, funcs)
+    ]
+    assertions = "\n".join(
+        _assert_eq(style, var_names[0], vname) for vname in var_names[1:]
+    )
 
     return _make_test_body(
         *funcs,
         test_body="\n".join(test_lines),
         except_=except_,
+        assertions=assertions,
         ghost="equivalent",
         style=style,
     )
 
 
 def equivalent(*funcs: Callable, except_: Except = (), style: str = "pytest") -> str:
     """Write source code for a property-based test of ``funcs``.
@@ -996,16 +1059,14 @@
     associative: bool = True,
     commutative: bool = True,
     identity: Union[X, InferType, None] = infer,
     distributes_over: Optional[Callable[[X, X], X]] = None,
     except_: Tuple[Type[Exception], ...],
     style: str,
 ) -> Tuple[Set[Union[str, Tuple[str, str]]], str]:
-    # TODO: collapse together first two strategies, keep any others (for flags etc.)
-    # assign this as a global variable, which will be prepended to the test bodies
     strategies = _get_strategies(func)
     operands, b = [strategies.pop(p) for p in list(_get_params(func))[:2]]
     if repr(operands) != repr(b):
         operands |= b
     operands_name = func.__name__ + "_operands"
 
     all_imports = set()
@@ -1013,43 +1074,59 @@
 
     def maker(
         sub_property: str,
         args: str,
         body: str,
         right: Optional[str] = None,
     ) -> None:
-        if right is not None:
-            body = f"left={body}\nright={right}\n" + _assert_eq(style, "left", "right")
+        if right is None:
+            assertions = ""
+        else:
+            body = f"{body}\n{right}"
+            assertions = _assert_eq(style, "left", "right")
         imports, body = _make_test_body(
             func,
             test_body=body,
             ghost=sub_property + "_binary_operation",
             except_=except_,
+            assertions=assertions,
             style=style,
             given_strategies={**strategies, **{n: operands_name for n in args}},
         )
         all_imports.update(imports)
         if style == "unittest":
             endline = "(unittest.TestCase):\n"
             body = body[body.index(endline) + len(endline) + 1 :]
         parts.append(body)
 
     if associative:
         maker(
             "associative",
             "abc",
-            _write_call(func, "a", _write_call(func, "b", "c")),
-            _write_call(func, _write_call(func, "a", "b"), "c"),
+            _write_call(
+                func,
+                "a",
+                _write_call(func, "b", "c", except_=Exception),
+                except_=Exception,
+                assign="left",
+            ),
+            _write_call(
+                func,
+                _write_call(func, "a", "b", except_=Exception),
+                "c",
+                except_=Exception,
+                assign="right",
+            ),
         )
     if commutative:
         maker(
             "commutative",
             "ab",
-            _write_call(func, "a", "b"),
-            _write_call(func, "b", "a"),
+            _write_call(func, "a", "b", except_=Exception, assign="left"),
+            _write_call(func, "b", "a", except_=Exception, assign="right"),
         )
     if identity is not None:
         # Guess that the identity element is the minimal example from our operands
         # strategy.  This is correct often enough to be worthwhile, and close enough
         # that it's a good starting point to edit much of the rest.
         if identity is infer:
             try:
@@ -1066,26 +1143,38 @@
             # executed; so you still shouldn't ghostwrite for hostile code.
             compile(repr(identity), "<string>", "exec")
         except SyntaxError:
             identity = repr(identity)  # type: ignore
         maker(
             "identity",
             "a",
-            _assert_eq(style, "a", _write_call(func, "a", repr(identity))),
+            _assert_eq(
+                style,
+                "a",
+                _write_call(func, "a", repr(identity), except_=Exception),
+            ),
         )
     if distributes_over:
         maker(
             distributes_over.__name__ + "_distributes_over",
             "abc",
             _write_call(
                 distributes_over,
-                _write_call(func, "a", "b"),
-                _write_call(func, "a", "c"),
+                _write_call(func, "a", "b", except_=Exception),
+                _write_call(func, "a", "c", except_=Exception),
+                except_=Exception,
+                assign="left",
+            ),
+            _write_call(
+                func,
+                "a",
+                _write_call(distributes_over, "b", "c", except_=Exception),
+                except_=Exception,
+                assign="right",
             ),
-            _write_call(func, "a", _write_call(distributes_over, "b", "c")),
         )
 
     _, operands_repr = _valid_syntax_repr(operands)
     operands_repr = _st_strategy_names(operands_repr)
     classdef = ""
     if style == "unittest":
         classdef = f"class TestBinaryOperation{func.__name__}(unittest.TestCase):\n    "
@@ -1126,29 +1215,29 @@
     body = """
     input_shapes, expected_shape = shapes
     input_dtypes, expected_dtype = types.split("->")
     array_st = [npst.arrays(d, s) for d, s in zip(input_dtypes, input_shapes)]
 
     {array_names} = data.draw(st.tuples(*array_st))
     result = {call}
-
-    {shape_assert}
-    {type_assert}
     """.format(
         array_names=", ".join(ascii_lowercase[: func.nin]),
-        call=_write_call(func, *ascii_lowercase[: func.nin]),
+        call=_write_call(func, *ascii_lowercase[: func.nin], except_=except_),
+    )
+    assertions = "\n{shape_assert}\n{type_assert}".format(
         shape_assert=_assert_eq(style, "result.shape", "expected_shape"),
         type_assert=_assert_eq(style, "result.dtype.char", "expected_dtype"),
     )
 
     qname = _get_qualname(func, include_module=True)
     return _make_test_body(
         func,
         test_body=dedent(body).strip(),
         except_=except_,
+        assertions=assertions,
         ghost="ufunc" if func.signature is None else "gufunc",
         style=style,
         given_strategies={
             "data": st.data(),
             "shapes": shapes,
             "types": f"sampled_from([sig for sig in {qname}.types if 'O' not in sig])",
         },
```

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/lark.py` & `hypothesis-6.9.2/src/hypothesis/extra/lark.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/numpy.py` & `hypothesis-6.9.2/src/hypothesis/extra/numpy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/pandas/__init__.py` & `hypothesis-6.9.2/src/hypothesis/extra/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/pandas/impl.py` & `hypothesis-6.9.2/src/hypothesis/extra/pandas/impl.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/pytestplugin.py` & `hypothesis-6.9.2/src/hypothesis/extra/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/pytz.py` & `hypothesis-6.9.2/src/hypothesis/extra/pytz.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/extra/redis.py` & `hypothesis-6.9.2/src/hypothesis/extra/redis.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/__init__.py` & `hypothesis-6.9.2/src/hypothesis/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/cache.py` & `hypothesis-6.9.2/src/hypothesis/internal/cache.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/cathetus.py` & `hypothesis-6.9.2/src/hypothesis/internal/cathetus.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/charmap.py` & `hypothesis-6.9.2/src/hypothesis/internal/charmap.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/compat.py` & `hypothesis-6.9.2/src/hypothesis/internal/compat.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/__init__.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/choicetree.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/choicetree.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/data.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/data.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/datatree.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/datatree.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/dfa/__init__.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/dfa/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/dfa/lstar.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/dfa/lstar.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/engine.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/engine.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/floats.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/floats.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/junkdrawer.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/junkdrawer.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/optimiser.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/optimiser.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/pareto.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/pareto.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinker.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinker.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/__init__.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/common.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/common.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/dfas.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/dfas.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/floats.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/floats.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/integer.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/integer.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/learned_dfas.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/learned_dfas.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/lexical.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/lexical.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/shrinking/ordering.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/shrinking/ordering.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/conjecture/utils.py` & `hypothesis-6.9.2/src/hypothesis/internal/conjecture/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/coverage.py` & `hypothesis-6.9.2/src/hypothesis/internal/coverage.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/detection.py` & `hypothesis-6.9.2/src/hypothesis/internal/detection.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/entropy.py` & `hypothesis-6.9.2/src/hypothesis/internal/entropy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/escalation.py` & `hypothesis-6.9.2/src/hypothesis/internal/escalation.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/filtering.py` & `hypothesis-6.9.2/src/hypothesis/internal/filtering.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/floats.py` & `hypothesis-6.9.2/src/hypothesis/internal/floats.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/healthcheck.py` & `hypothesis-6.9.2/src/hypothesis/internal/healthcheck.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/intervalsets.py` & `hypothesis-6.9.2/src/hypothesis/internal/intervalsets.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/lazyformat.py` & `hypothesis-6.9.2/src/hypothesis/internal/lazyformat.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/reflection.py` & `hypothesis-6.9.2/src/hypothesis/internal/reflection.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,15 +404,16 @@
 
 def nicerepr(v):
     if inspect.isfunction(v):
         return get_pretty_function_description(v)
     elif isinstance(v, type):
         return v.__name__
     else:
-        return pretty(v)
+        # With TypeVar T, show List[T] instead of TypeError on List[~T]
+        return re.sub(r"(\[)~([A-Z][a-z]*\])", r"\g<1>\g<2>", pretty(v))
 
 
 def arg_string(f, args, kwargs, reorder=True):
     if reorder:
         args, kwargs = convert_positional_arguments(f, args, kwargs)
 
     argspec = inspect.getfullargspec(f)
```

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/scrutineer.py` & `hypothesis-6.9.2/src/hypothesis/internal/scrutineer.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/internal/validation.py` & `hypothesis-6.9.2/src/hypothesis/internal/validation.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/provisional.py` & `hypothesis-6.9.2/src/hypothesis/provisional.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/reporting.py` & `hypothesis-6.9.2/src/hypothesis/reporting.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/stateful.py` & `hypothesis-6.9.2/src/hypothesis/stateful.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/statistics.py` & `hypothesis-6.9.2/src/hypothesis/statistics.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/__init__.py` & `hypothesis-6.9.2/src/hypothesis/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/__init__.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/attrs.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/attrs.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/collections.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/collections.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/core.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/core.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/datetime.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/datetime.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/deferred.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/deferred.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/featureflags.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/featureflags.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/flatmapped.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/flatmapped.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/functions.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/functions.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/ipaddress.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/ipaddress.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/lazy.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/lazy.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/misc.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/misc.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/numbers.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/numbers.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/random.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/random.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/recursive.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/recursive.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/regex.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/regex.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/shared.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/shared.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/strategies.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/strategies.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/strings.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/strings.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/types.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/types.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/strategies/_internal/utils.py` & `hypothesis-6.9.2/src/hypothesis/strategies/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/utils/__init__.py` & `hypothesis-6.9.2/src/hypothesis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/utils/conventions.py` & `hypothesis-6.9.2/src/hypothesis/utils/conventions.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/utils/dynamicvariables.py` & `hypothesis-6.9.2/src/hypothesis/utils/dynamicvariables.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/vendor/__init__.py` & `hypothesis-6.9.2/src/hypothesis/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/vendor/pretty.py` & `hypothesis-6.9.2/src/hypothesis/vendor/pretty.py`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/vendor/tlds-alpha-by-domain.txt` & `hypothesis-6.9.2/src/hypothesis/vendor/tlds-alpha-by-domain.txt`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis/version.py` & `hypothesis-6.9.2/src/hypothesis/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public License,
 # v. 2.0. If a copy of the MPL was not distributed with this file, You can
 # obtain one at https://mozilla.org/MPL/2.0/.
 #
 # END HEADER
 
-__version_info__ = (6, 9, 1)
+__version_info__ = (6, 9, 2)
 __version__ = ".".join(map(str, __version_info__))
```

### Comparing `hypothesis-6.9.1/src/hypothesis.egg-info/PKG-INFO` & `hypothesis-6.9.2/src/hypothesis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis
-Version: 6.9.1
+Version: 6.9.2
 Summary: A library for property-based testing
 Home-page: https://github.com/HypothesisWorks/hypothesis/tree/master/hypothesis-python
 Author: David R. MacIver
 Author-email: david@drmaciver.com
 License: MPL v2
 Project-URL: Website, https://hypothesis.works
 Project-URL: Documentation, https://hypothesis.readthedocs.io
```

### Comparing `hypothesis-6.9.1/src/hypothesis.egg-info/SOURCES.txt` & `hypothesis-6.9.2/src/hypothesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypothesis-6.9.1/src/hypothesis.egg-info/requires.txt` & `hypothesis-6.9.2/src/hypothesis.egg-info/requires.txt`

 * *Files identical despite different names*

