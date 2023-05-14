# Comparing `tmp/poetry_core-1.5.1.tar.gz` & `tmp/poetry_core-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_core-1.5.1.tar", max compression
+gzip compressed data, was "poetry_core-1.5.2.tar", max compression
```

## Comparing `poetry_core-1.5.1.tar` & `poetry_core-1.5.2.tar`

### file list

```diff
@@ -1,562 +1,562 @@
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.190241 poetry_core-1.5.1/LICENSE
--rw-r--r--   0        0        0     2403 2023-02-20 16:27:54.190241 poetry_core-1.5.1/README.md
--rw-r--r--   0        0        0     2605 2023-02-20 16:27:54.190241 poetry_core-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      394 2023-02-20 16:27:54.190241 poetry_core-1.5.1/src/poetry/core/__init__.py
--rw-r--r--   0        0        0       23 2023-02-20 16:27:54.190241 poetry_core-1.5.1/src/poetry/core/_vendor/_pyrsistent_version.py
--rw-r--r--   0        0        0     1947 2023-02-20 16:27:54.190241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/__init__.py
--rw-r--r--   0        0        0     4094 2023-02-20 16:27:54.190241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/_cmp.py
--rw-r--r--   0        0        0     5435 2023-02-20 16:27:54.190241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/_compat.py
--rw-r--r--   0        0        0      826 2023-02-20 16:27:54.190241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/_config.py
--rw-r--r--   0        0        0    14545 2023-02-20 16:27:54.190241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/_funcs.py
--rw-r--r--   0        0        0    96087 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/_make.py
--rw-r--r--   0        0        0     6059 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/_next_gen.py
--rw-r--r--   0        0        0     2121 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/_version_info.py
--rw-r--r--   0        0        0     3602 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/converters.py
--rw-r--r--   0        0        0     1915 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/exceptions.py
--rw-r--r--   0        0        0     1038 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/filters.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/py.typed
--rw-r--r--   0        0        0     1400 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/setters.py
--rw-r--r--   0        0        0    20501 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attr/validators.py
--rw-r--r--   0        0        0     1109 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attrs/LICENSE
--rw-r--r--   0        0        0     1149 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attrs/__init__.py
--rw-r--r--   0        0        0       70 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attrs/converters.py
--rw-r--r--   0        0        0       70 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attrs/exceptions.py
--rw-r--r--   0        0        0       67 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attrs/filters.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attrs/py.typed
--rw-r--r--   0        0        0       67 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attrs/setters.py
--rw-r--r--   0        0        0       70 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/attrs/validators.py
--rw-r--r--   0        0        0     1057 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/COPYING
--rw-r--r--   0        0        0     2187 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/__init__.py
--rw-r--r--   0        0        0       40 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/__main__.py
--rw-r--r--   0        0        0    14575 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_format.py
--rw-r--r--   0        0        0    10549 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_legacy_validators.py
--rw-r--r--   0        0        0     5425 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_types.py
--rw-r--r--   0        0        0    10254 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_utils.py
--rw-r--r--   0        0        0    15956 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_validators.py
--rw-r--r--   0        0        0       70 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/benchmarks/__init__.py
--rw-r--r--   0        0        0   117105 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/benchmarks/issue232/issue.json
--rw-r--r--   0        0        0      506 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/benchmarks/issue232.py
--rw-r--r--   0        0        0      320 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/benchmarks/json_schema_test_suite.py
--rw-r--r--   0        0        0     8518 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/cli.py
--rw-r--r--   0        0        0    11336 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/exceptions.py
--rw-r--r--   0        0        0     7295 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/protocols.py
--rw-r--r--   0        0        0     1785 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft2019-09.json
--rw-r--r--   0        0        0     2452 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft2020-12.json
--rw-r--r--   0        0        0     2600 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft3.json
--rw-r--r--   0        0        0     4357 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft4.json
--rw-r--r--   0        0        0     4437 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft6.json
--rw-r--r--   0        0        0     4819 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft7.json
--rw-r--r--   0        0        0     1860 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/applicator
--rw-r--r--   0        0        0      517 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/content
--rw-r--r--   0        0        0     1531 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/core
--rw-r--r--   0        0        0      892 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/meta-data
--rw-r--r--   0        0        0     2834 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/validation
--rw-r--r--   0        0        0     1659 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/applicator
--rw-r--r--   0        0        0      519 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/content
--rw-r--r--   0        0        0     1564 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/core
--rw-r--r--   0        0        0      403 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format
--rw-r--r--   0        0        0      448 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format-annotation
--rw-r--r--   0        0        0      445 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format-assertion
--rw-r--r--   0        0        0      892 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/meta-data
--rw-r--r--   0        0        0      506 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/unevaluated
--rw-r--r--   0        0        0     2834 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/validation
--rw-r--r--   0        0        0    38171 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/validators.py
--rw-r--r--   0        0        0     1073 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/LICENSE
--rw-r--r--   0        0        0      744 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/__init__.py
--rw-r--r--   0        0        0      182 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      599 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py
--rw-r--r--   0        0        0     2092 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/ast_utils.py
--rw-r--r--   0        0        0     2814 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/common.py
--rw-r--r--   0        0        0    10940 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/exceptions.py
--rw-r--r--   0        0        0     3427 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammars/__init__.py
--rw-r--r--   0        0        0      944 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammars/common.lark
--rw-r--r--   0        0        0     1467 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammars/lark.lark
--rw-r--r--   0        0        0    10995 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammars/python.lark
--rw-r--r--   0        0        0      103 2023-02-20 16:27:54.194241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammars/unicode.lark
--rw-r--r--   0        0        0     3076 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/indenter.py
--rw-r--r--   0        0        0    27483 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/lark.py
--rw-r--r--   0        0        0    20633 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/lexer.py
--rw-r--r--   0        0        0    53453 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/load_grammar.py
--rw-r--r--   0        0        0    14112 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parse_tree_builder.py
--rw-r--r--   0        0        0     9338 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parser_frontends.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/__init__.py
--rw-r--r--   0        0        0    12251 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/cyk.py
--rw-r--r--   0        0        0    13990 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/earley.py
--rw-r--r--   0        0        0     1581 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/earley_common.py
--rw-r--r--   0        0        0    31391 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/earley_forest.py
--rw-r--r--   0        0        0     6421 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/grammar_analysis.py
--rw-r--r--   0        0        0    10614 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/lalr_analysis.py
--rw-r--r--   0        0        0     5296 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/lalr_interactive_parser.py
--rw-r--r--   0        0        0     7216 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/lalr_parser.py
--rw-r--r--   0        0        0     2497 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/resolve_ambig.py
--rw-r--r--   0        0        0     7505 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/xearley.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/py.typed
--rw-r--r--   0        0        0     3728 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/reconstruct.py
--rw-r--r--   0        0        0     2319 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/tools/__init__.py
--rw-r--r--   0        0        0     6265 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/tools/nearley.py
--rw-r--r--   0        0        0     1014 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/tools/serialize.py
--rw-r--r--   0        0        0     5550 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/tools/standalone.py
--rw-r--r--   0        0        0     8178 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/tree.py
--rw-r--r--   0        0        0     6004 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/tree_matcher.py
--rw-r--r--   0        0        0     5958 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/tree_templates.py
--rw-r--r--   0        0        0    11089 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/utils.py
--rw-r--r--   0        0        0    21096 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/lark/visitors.py
--rw-r--r--   0        0        0      197 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/LICENSE
--rw-r--r--   0        0        0    10174 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/LICENSE.APACHE
--rw-r--r--   0        0        0     1344 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/LICENSE.BSD
--rw-r--r--   0        0        0      501 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/markers.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/py.typed
--rw-r--r--   0        0        0     3264 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39046 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16295 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/packaging/version.py
--rw-r--r--   0        0        0     1060 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/LICENSE.mit
--rw-r--r--   0        0        0     1479 2023-02-20 16:27:54.198241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/__init__.py
--rw-r--r--   0        0        0    18372 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_checked_types.py
--rw-r--r--   0        0        0    11963 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_field_common.py
--rw-r--r--   0        0        0     3232 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_helpers.py
--rw-r--r--   0        0        0     3287 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_immutable.py
--rw-r--r--   0        0        0     6730 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pbag.py
--rw-r--r--   0        0        0     9702 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pclass.py
--rw-r--r--   0        0        0    12203 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pdeque.py
--rw-r--r--   0        0        0     8293 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_plist.py
--rw-r--r--   0        0        0    18781 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pmap.py
--rw-r--r--   0        0        0     7032 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_precord.py
--rw-r--r--   0        0        0     5693 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pset.py
--rw-r--r--   0        0        0    22694 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pvector.py
--rw-r--r--   0        0        0     3425 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_toolz.py
--rw-r--r--   0        0        0     3800 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_transformations.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/py.typed
--rw-r--r--   0        0        0     1767 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/typing.py
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/LICENSE
--rw-r--r--   0        0        0     1148 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/__init__.py
--rw-r--r--   0        0        0      532 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/_compat.py
--rw-r--r--   0        0        0     4015 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/_utils.py
--rw-r--r--   0        0        0     7120 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/api.py
--rw-r--r--   0        0        0    29687 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/container.py
--rw-r--r--   0        0        0     5486 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/exceptions.py
--rw-r--r--   0        0        0    51976 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/items.py
--rw-r--r--   0        0        0    37694 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/parser.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/py.typed
--rw-r--r--   0        0        0     4882 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/source.py
--rw-r--r--   0        0        0     1291 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/toml_char.py
--rw-r--r--   0        0        0      110 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/toml_document.py
--rw-r--r--   0        0        0     1599 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/toml_file.py
--rw-r--r--   0        0        0    12787 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/typing_extensions.LICENSE
--rw-r--r--   0        0        0    80078 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      574 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/_vendor/vendor.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/constraints/__init__.py
--rw-r--r--   0        0        0      719 2023-02-20 16:27:54.202241 poetry_core-1.5.1/src/poetry/core/constraints/generic/__init__.py
--rw-r--r--   0        0        0     1162 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/generic/any_constraint.py
--rw-r--r--   0        0        0     1055 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/generic/base_constraint.py
--rw-r--r--   0        0        0     4488 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/generic/constraint.py
--rw-r--r--   0        0        0     1068 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/generic/empty_constraint.py
--rw-r--r--   0        0        0     3689 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/generic/multi_constraint.py
--rw-r--r--   0        0        0     2036 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/generic/parser.py
--rw-r--r--   0        0        0     5880 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/generic/union_constraint.py
--rw-r--r--   0        0        0      832 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/__init__.py
--rw-r--r--   0        0        0     1416 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/empty_constraint.py
--rw-r--r--   0        0        0       86 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/exceptions.py
--rw-r--r--   0        0        0     5724 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/parser.py
--rw-r--r--   0        0        0      913 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/patterns.py
--rw-r--r--   0        0        0     1543 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/util.py
--rw-r--r--   0        0        0     5047 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/version.py
--rw-r--r--   0        0        0     1731 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/version_constraint.py
--rw-r--r--   0        0        0    13641 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/version_range.py
--rw-r--r--   0        0        0     2383 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/version_range_constraint.py
--rw-r--r--   0        0        0    14643 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/constraints/version/version_union.py
--rw-r--r--   0        0        0      132 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/exceptions/__init__.py
--rw-r--r--   0        0        0       84 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/exceptions/base.py
--rw-r--r--   0        0        0    16981 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/factory.py
--rw-r--r--   0        0        0      998 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/json/__init__.py
--rw-r--r--   0        0        0    18190 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/json/schemas/poetry-schema.json
--rw-r--r--   0        0        0      255 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/__init__.py
--rw-r--r--   0        0        0     2682 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/api.py
--rw-r--r--   0        0        0      994 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/builder.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/builders/__init__.py
--rw-r--r--   0        0        0    12795 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/builders/builder.py
--rw-r--r--   0        0        0    15020 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/builders/sdist.py
--rw-r--r--   0        0        0    14573 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/builders/wheel.py
--rw-r--r--   0        0        0     3012 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/metadata.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/utils/__init__.py
--rw-r--r--   0        0        0     3066 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/utils/helpers.py
--rw-r--r--   0        0        0     1100 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/utils/include.py
--rw-r--r--   0        0        0     3697 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/utils/module.py
--rw-r--r--   0        0        0     2720 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/masonry/utils/package_include.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/__init__.py
--rw-r--r--   0        0        0      910 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/constraints/__init__.py
--rw-r--r--   0        0        0    17882 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/dependency.py
--rw-r--r--   0        0        0     1479 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/dependency_group.py
--rw-r--r--   0        0        0     1801 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/directory_dependency.py
--rw-r--r--   0        0        0     1525 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/file_dependency.py
--rw-r--r--   0        0        0    20951 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/package.py
--rw-r--r--   0        0        0     2492 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/path_dependency.py
--rw-r--r--   0        0        0     2868 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/project_package.py
--rw-r--r--   0        0        0     6355 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/specification.py
--rw-r--r--   0        0        0     1531 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/url_dependency.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/utils/__init__.py
--rw-r--r--   0        0        0     6890 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/utils/link.py
--rw-r--r--   0        0        0    13198 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/utils/utils.py
--rw-r--r--   0        0        0     3053 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/packages/vcs_dependency.py
--rw-r--r--   0        0        0     1145 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/poetry.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/py.typed
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/pyproject/__init__.py
--rw-r--r--   0        0        0      149 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/pyproject/exceptions.py
--rw-r--r--   0        0        0     2127 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/pyproject/tables.py
--rw-r--r--   0        0        0     3254 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/pyproject/toml.py
--rw-r--r--   0        0        0      199 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/__init__.py
--rw-r--r--   0        0        0      128 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/empty_constraint.py
--rw-r--r--   0        0        0      149 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/exceptions.py
--rw-r--r--   0        0        0      239 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/helpers.py
--rw-r--r--   0        0        0      622 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/patterns.py
--rw-r--r--   0        0        0      134 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/util.py
--rw-r--r--   0        0        0      112 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/version.py
--rw-r--r--   0        0        0      132 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/version_constraint.py
--rw-r--r--   0        0        0      122 2023-02-20 16:27:54.206241 poetry_core-1.5.1/src/poetry/core/semver/version_range.py
--rw-r--r--   0        0        0      142 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/semver/version_range_constraint.py
--rw-r--r--   0        0        0      122 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/semver/version_union.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/spdx/__init__.py
--rw-r--r--   0        0        0    30125 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/spdx/data/licenses.json
--rw-r--r--   0        0        0     1352 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/spdx/helpers.py
--rw-r--r--   0        0        0     5639 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/spdx/license.py
--rw-r--r--   0        0        0     1107 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/spdx/updater.py
--rw-r--r--   0        0        0      167 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/toml/__init__.py
--rw-r--r--   0        0        0      221 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/toml/exceptions.py
--rw-r--r--   0        0        0     1086 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/toml/file.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/utils/__init__.py
--rw-r--r--   0        0        0       83 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/utils/_compat.py
--rw-r--r--   0        0        0     2526 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/utils/helpers.py
--rw-r--r--   0        0        0      252 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/utils/patterns.py
--rw-r--r--   0        0        0      624 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/utils/toml_file.py
--rw-r--r--   0        0        0      722 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/vcs/__init__.py
--rw-r--r--   0        0        0    11234 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/vcs/git.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/__init__.py
--rw-r--r--   0        0        0       80 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/exceptions.py
--rw-r--r--   0        0        0      214 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/grammars/__init__.py
--rw-r--r--   0        0        0      972 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/grammars/markers.lark
--rw-r--r--   0        0        0     1398 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/grammars/pep508.lark
--rw-r--r--   0        0        0     1606 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/helpers.py
--rw-r--r--   0        0        0    29673 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/markers.py
--rw-r--r--   0        0        0      752 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/parser.py
--rw-r--r--   0        0        0      352 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/pep440/__init__.py
--rw-r--r--   0        0        0     2874 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/pep440/parser.py
--rw-r--r--   0        0        0     4826 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/pep440/segments.py
--rw-r--r--   0        0        0    10844 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/pep440/version.py
--rw-r--r--   0        0        0     3501 2023-02-20 16:27:54.210241 poetry_core-1.5.1/src/poetry/core/version/requirements.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/__init__.py
--rw-r--r--   0        0        0     2687 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/generic/__init__.py
--rw-r--r--   0        0        0    12991 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/generic/test_constraint.py
--rw-r--r--   0        0        0     1800 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/generic/test_main.py
--rw-r--r--   0        0        0     1187 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/generic/test_multi_constraint.py
--rw-r--r--   0        0        0     1169 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/generic/test_union_constraint.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/version/__init__.py
--rw-r--r--   0        0        0    13374 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/version/test_helpers.py
--rw-r--r--   0        0        0     7518 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/version/test_parse_constraint.py
--rw-r--r--   0        0        0     2925 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/version/test_utils.py
--rw-r--r--   0        0        0    17288 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/version/test_version.py
--rw-r--r--   0        0        0      943 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/version/test_version_constraint.py
--rw-r--r--   0        0        0    14171 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/constraints/version/test_version_range.py
--rw-r--r--   0        0        0     1329 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/complete.toml
--rw-r--r--   0        0        0     1116 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0      961 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/distributions/demo-0.1.0.tar.gz
--rw-r--r--   0        0        0      209 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/invalid_pyproject/pyproject.toml
--rw-r--r--   0        0        0      110 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/pep_517_backend/README.md
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/pep_517_backend/foo/__init__.py
--rw-r--r--   0        0        0     1190 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/pep_517_backend/pyproject.toml
--rw-r--r--   0        0        0      634 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_failing_strict_validation/pyproject.toml
--rw-r--r--   0        0        0      407 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_build_system_requires/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_groups_and_explicit_main/README.rst
--rw-r--r--   0        0        0      326 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_groups_and_explicit_main/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_groups_and_explicit_main/simple_project/__init__.py
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_groups_and_legacy_dev/README.rst
--rw-r--r--   0        0        0      376 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_groups_and_legacy_dev/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_groups_and_legacy_dev/simple_project/__init__.py
--rw-r--r--   0        0        0      278 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_invalid_dev_deps/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_markers_and_extras/project/__init__.py
--rw-r--r--   0        0        0      602 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_markers_and_extras/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
--rw-r--r--   0        0        0      394 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
--rw-r--r--   0        0        0      255 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_pep517_non_poetry/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_setup/my_package/__init__.py
--rw-r--r--   0        0        0      346 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_setup/setup.py
--rw-r--r--   0        0        0      444 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/project_with_setup_cfg_only/setup.cfg
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/sample_project/README.rst
--rw-r--r--   0        0        0     2261 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/sample_project/pyproject.toml
--rw-r--r--   0        0        0       83 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/script-files/sample_script.py
--rw-r--r--   0        0        0       41 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/script-files/sample_script.sh
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/simple_project/README.rst
--rw-r--r--   0        0        0     1320 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1106 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
--rw-r--r--   0        0        0      590 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/simple_project/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/simple_project/simple_project/__init__.py
--rw-r--r--   0        0        0       28 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/with_readme_files/README-1.rst
--rw-r--r--   0        0        0       20 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/with_readme_files/README-2.rst
--rw-r--r--   0        0        0       79 2023-02-20 16:27:54.210241 poetry_core-1.5.1/tests/fixtures/with_readme_files/my_package/__init__.py
--rw-r--r--   0        0        0      300 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/fixtures/with_readme_files/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     2720 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/integration/test_pep517.py
--rw-r--r--   0        0        0     1499 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/integration/test_pep517_backend.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/json/__init__.py
--rw-r--r--   0        0        0     2277 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/json/test_poetry_schema.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/__init__.py
--rw-r--r--   0        0        0      294 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/build_script_in_subdir/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/build_script_in_subdir/scripts/build.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/build_script_in_subdir/src/foo.py
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/LICENSE
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/README.rst
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/Bar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/IncludedBar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/SecondBar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/lowercasebar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/FooBar/Bar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/FooBar/lowercasebar.py
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/bar/CapitalFoo.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/bar/foo.py
--rw-r--r--   0        0        0     1160 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/comma_file/comma_file/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/comma_file/comma_file/a,b.py
--rw-r--r--   0        0        0      224 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/comma_file/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/LICENSE
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/README.rst
--rw-r--r--   0        0        0       40 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/bin/script.sh
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/my_package/__init__.py
--rw-r--r--   0        0        0        3 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/my_package/data1/test.json
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg1/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg1/extra_file.xml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg2/__init__.py
--rw-r--r--   0        0        0        3 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg2/data2/data.json
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/my_package/sub_pkg3/foo.py
--rw-r--r--   0        0        0     1348 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/LICENSE
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/README.rst
--rw-r--r--   0        0        0      874 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/data1.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/sub_data/data2.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/sub_data/data3.txt
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/LICENSE
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/README.rst
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/data1.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/sub_data/data2.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/sub_data/data3.txt
--rw-r--r--   0        0        0      874 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/LICENSE
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/README.rst
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/data1.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/sub_data/data2.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/sub_data/data3.txt
--rw-r--r--   0        0        0      915 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/disable_setup_py/README.rst
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/disable_setup_py/my_package/__init__.py
--rw-r--r--   0        0        0      740 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/disable_setup_py/pyproject.toml
--rw-r--r--   0        0        0       12 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/epoch/README.rst
--rw-r--r--   0        0        0       44 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/epoch/epoch.py
--rw-r--r--   0        0        0      223 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/epoch/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/compiled/source.c
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/compiled/source.h
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/cython_code.pyx
--rw-r--r--   0        0        0      474 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude-whl-include-sdist/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/LICENSE
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/README.rst
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/data1.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/data2.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/sub_data/data2.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.214241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/sub_data/data3.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item1/itemdata1.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item1/subitem/subitemdata.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item2/itemdata2.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/publicdata.txt
--rw-r--r--   0        0        0      952 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/pyproject.toml
--rw-r--r--   0        0        0       21 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
--rw-r--r--   0        0        0      148 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
--rw-r--r--   0        0        0      329 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
--rw-r--r--   0        0        0       18 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended/README.rst
--rw-r--r--   0        0        0      186 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended/build.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended/extended/__init__.py
--rw-r--r--   0        0        0      888 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended/extended/extended.c
--rw-r--r--   0        0        0      292 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended/pyproject.toml
--rw-r--r--   0        0        0      539 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended/setup.py
--rw-r--r--   0        0        0       18 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended_with_no_setup/README.rst
--rw-r--r--   0        0        0      753 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended_with_no_setup/build.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended_with_no_setup/extended/__init__.py
--rw-r--r--   0        0        0      888 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended_with_no_setup/extended/extended.c
--rw-r--r--   0        0        0      293 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/extended_with_no_setup/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/include_excluded_code/lib/my_package/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/include_excluded_code/lib/my_package/generated.py
--rw-r--r--   0        0        0      485 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/include_excluded_code/pyproject.toml
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/LICENSE
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/README.rst
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Bar/foo/bar/Foo.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/Bar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/IncludedBar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/SecondBar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/lowercasebar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/FooBar/Bar.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/FooBar/lowercasebar.py
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/__init__.py
--rw-r--r--   0        0        0     1011 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/COPYING
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/COPYING.txt
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE.md
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/BSD-3.md
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/CUSTOM-LICENSE
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/MIT.txt
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/README.rst
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/my_package/__init__.py
--rw-r--r--   0        0        0     1231 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/pyproject.toml
--rw-r--r--   0        0        0       74 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/localversionlabel/localversionlabel.py
--rw-r--r--   0        0        0      133 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/localversionlabel/pyproject.toml
--rw-r--r--   0        0        0       18 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/module1/README.rst
--rw-r--r--   0        0        0       42 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/module1/module1.py
--rw-r--r--   0        0        0      265 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/module1/pyproject.toml
--rw-r--r--   0        0        0      261 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
--rw-r--r--   0        0        0        8 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
--rw-r--r--   0        0        0      291 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
--rw-r--r--   0        0        0        8 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pkg-stubs/subpkg/py.typed
--rw-r--r--   0        0        0      306 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pyproject.toml
--rw-r--r--   0        0        0      294 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/prerelease/README.rst
--rw-r--r--   0        0        0       42 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/prerelease/prerelease.py
--rw-r--r--   0        0        0      233 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/prerelease/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_callable_legacy_string/README.rst
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_callable_legacy_string/my_package/__init__.py
--rw-r--r--   0        0        0      346 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_callable_legacy_string/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_callable_legacy_table/README.rst
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_callable_legacy_table/my_package/__init__.py
--rw-r--r--   0        0        0      471 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_callable_legacy_table/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_console/README.rst
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_console/my_package/__init__.py
--rw-r--r--   0        0        0      481 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_console/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file/README.rst
--rw-r--r--   0        0        0       40 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file/bin/script.sh
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file/my_package/__init__.py
--rw-r--r--   0        0        0      371 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/README.rst
--rw-r--r--   0        0        0       40 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/bin/script.sh
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/my_package/__init__.py
--rw-r--r--   0        0        0      384 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file_missing/README.rst
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file_missing/my_package/__init__.py
--rw-r--r--   0        0        0      371 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/script_reference_file_missing/pyproject.toml
--rw-r--r--   0        0        0       18 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/simple_version/README.rst
--rw-r--r--   0        0        0      217 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/simple_version/pyproject.toml
--rw-r--r--   0        0        0       42 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/simple_version/simple_version.py
--rw-r--r--   0        0        0       28 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/single_python/README.rst
--rw-r--r--   0        0        0      276 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/single_python/pyproject.toml
--rw-r--r--   0        0        0       42 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/single_python/single_python.py
--rw-r--r--   0        0        0       18 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/source_file/README.rst
--rw-r--r--   0        0        0      268 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/source_file/pyproject.toml
--rw-r--r--   0        0        0       42 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/source_file/src/module_src.py
--rw-r--r--   0        0        0       18 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/source_package/README.rst
--rw-r--r--   0        0        0      268 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/source_package/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/source_package/src/package_src/__init__.py
--rw-r--r--   0        0        0       42 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/source_package/src/package_src/module.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/split_source/lib_a/module_a/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/split_source/lib_b/module_b/__init__.py
--rw-r--r--   0        0        0      331 2023-02-20 16:27:54.218241 poetry_core-1.5.1/tests/masonry/builders/fixtures/split_source/pyproject.toml
--rw-r--r--   0        0        0       18 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/src_extended/README.rst
--rw-r--r--   0        0        0      190 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/src_extended/build.py
--rw-r--r--   0        0        0      292 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/src_extended/pyproject.toml
--rw-r--r--   0        0        0      598 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/src_extended/setup.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/src_extended/src/extended/__init__.py
--rw-r--r--   0        0        0      888 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/src_extended/src/extended/extended.c
--rw-r--r--   0        0        0     1062 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/LICENSE
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/README.rst
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/extra_dir/README.md
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/extra_dir/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/extra_dir/sub_pkg/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/extra_dir/vcs_excluded.txt
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/for_wheel_only/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/my_module.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/notes.txt
--rw-r--r--   0        0        0       22 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/package_with_include/__init__.py
--rw-r--r--   0        0        0     1259 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/src/src_package/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/tests/__init__.py
--rw-r--r--   0        0        0      238 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_bad_path_dep/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_bad_path_dep/with_bad_path_dep/__init__.py
--rw-r--r--   0        0        0      274 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_bad_path_dev_dep/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_bad_path_dev_dep/with_bad_path_dev_dep/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_include_inline_table/both.txt
--rw-r--r--   0        0        0     1050 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_include_inline_table/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_include_inline_table/src/src_package/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_include_inline_table/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_include_inline_table/tests/test_foo/test.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_include_inline_table/wheel_only.txt
--rw-r--r--   0        0        0      656 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_url_dependency/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_url_dependency/with_url_dependency/__init__.py
--rw-r--r--   0        0        0      641 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_vcs_dependency/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_vcs_dependency/with_vcs_dependency/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_wildcard_dependency_constraint/my_package/__init__.py
--rw-r--r--   0        0        0      236 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/fixtures/with_wildcard_dependency_constraint/pyproject.toml
--rw-r--r--   0        0        0     8986 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/test_builder.py
--rw-r--r--   0        0        0    18699 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/test_complete.py
--rw-r--r--   0        0        0    20426 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/test_sdist.py
--rw-r--r--   0        0        0    11300 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/builders/test_wheel.py
--rw-r--r--   0        0        0    10197 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/test_api.py
--rw-r--r--   0        0        0     2202 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/test_builder.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/__init__.py
--rw-r--r--   0        0        0        8 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/fixtures/pep_561_stub_only_partial_namespace/good-stubs/subpkg/py.typed
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/fixtures/with_includes/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/fixtures/with_includes/bar/baz.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/fixtures/with_includes/extra_package/some_dir/foo.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/fixtures/with_includes/extra_package/some_dir/quux.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/fixtures/with_includes/not_a_python_pkg/baz.txt
--rw-r--r--   0        0        0      530 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/test_helpers.py
--rw-r--r--   0        0        0     3047 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/masonry/utils/test_package_include.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/__init__.py
--rw-r--r--   0        0        0    12255 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_dependency.py
--rw-r--r--   0        0        0      948 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_dependency_group.py
--rw-r--r--   0        0        0     6036 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_directory_dependency.py
--rw-r--r--   0        0        0     8481 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_file_dependency.py
--rw-r--r--   0        0        0    10865 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_main.py
--rw-r--r--   0        0        0    20447 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_package.py
--rw-r--r--   0        0        0     3814 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_specification.py
--rw-r--r--   0        0        0     2588 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_url_dependency.py
--rw-r--r--   0        0        0     5052 2023-02-20 16:27:54.222241 poetry_core-1.5.1/tests/packages/test_vcs_dependency.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/packages/utils/__init__.py
--rw-r--r--   0        0        0     9196 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/packages/utils/test_utils.py
--rw-r--r--   0        0        0     3873 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/packages/utils/test_utils_link.py
--rw-r--r--   0        0        0     2248 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/packages/utils/test_utils_urls.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/pyproject/__init__.py
--rw-r--r--   0        0        0      813 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/pyproject/conftest.py
--rw-r--r--   0        0        0     3641 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/pyproject/test_pyproject_toml.py
--rw-r--r--   0        0        0     1056 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/pyproject/test_pyproject_toml_file.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/spdx/__init__.py
--rw-r--r--   0        0        0     1413 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/spdx/test_helpers.py
--rw-r--r--   0        0        0     1497 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/spdx/test_license.py
--rw-r--r--   0        0        0      343 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/test_core_version.py
--rw-r--r--   0        0        0    14536 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/test_factory.py
--rw-r--r--   0        0        0     2601 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/testutils.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     3800 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/utils/test_helpers.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/vcs/__init__.py
--rw-r--r--   0        0        0    15077 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/vcs/test_vcs.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/version/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/version/pep440/__init__.py
--rw-r--r--   0        0        0     4523 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/version/pep440/test_segments.py
--rw-r--r--   0        0        0     9801 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/version/pep440/test_version.py
--rw-r--r--   0        0        0    63190 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/version/test_markers.py
--rw-r--r--   0        0        0     4452 2023-02-20 16:27:54.226241 poetry_core-1.5.1/tests/version/test_requirements.py
--rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 poetry_core-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.384417 poetry_core-1.5.2/LICENSE
+-rw-r--r--   0        0        0     2403 2023-03-13 20:55:41.384417 poetry_core-1.5.2/README.md
+-rw-r--r--   0        0        0     2612 2023-03-13 20:55:41.388417 poetry_core-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      394 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/__init__.py
+-rw-r--r--   0        0        0       23 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/_pyrsistent_version.py
+-rw-r--r--   0        0        0     1947 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/__init__.py
+-rw-r--r--   0        0        0     4094 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/_cmp.py
+-rw-r--r--   0        0        0     5435 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/_compat.py
+-rw-r--r--   0        0        0      826 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/_config.py
+-rw-r--r--   0        0        0    14545 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/_funcs.py
+-rw-r--r--   0        0        0    96087 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/_make.py
+-rw-r--r--   0        0        0     6059 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/_next_gen.py
+-rw-r--r--   0        0        0     2121 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/_version_info.py
+-rw-r--r--   0        0        0     3602 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/converters.py
+-rw-r--r--   0        0        0     1915 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/exceptions.py
+-rw-r--r--   0        0        0     1038 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/filters.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/py.typed
+-rw-r--r--   0        0        0     1400 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/setters.py
+-rw-r--r--   0        0        0    20501 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attr/validators.py
+-rw-r--r--   0        0        0     1109 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attrs/LICENSE
+-rw-r--r--   0        0        0     1149 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attrs/__init__.py
+-rw-r--r--   0        0        0       70 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attrs/converters.py
+-rw-r--r--   0        0        0       70 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attrs/exceptions.py
+-rw-r--r--   0        0        0       67 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attrs/filters.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attrs/py.typed
+-rw-r--r--   0        0        0       67 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attrs/setters.py
+-rw-r--r--   0        0        0       70 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/attrs/validators.py
+-rw-r--r--   0        0        0     1057 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/COPYING
+-rw-r--r--   0        0        0     2187 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/__init__.py
+-rw-r--r--   0        0        0       40 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/__main__.py
+-rw-r--r--   0        0        0    14575 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_format.py
+-rw-r--r--   0        0        0    10549 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_legacy_validators.py
+-rw-r--r--   0        0        0     5425 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_types.py
+-rw-r--r--   0        0        0    10254 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_utils.py
+-rw-r--r--   0        0        0    15956 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_validators.py
+-rw-r--r--   0        0        0       70 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/benchmarks/__init__.py
+-rw-r--r--   0        0        0   117105 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/benchmarks/issue232/issue.json
+-rw-r--r--   0        0        0      506 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/benchmarks/issue232.py
+-rw-r--r--   0        0        0      320 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/benchmarks/json_schema_test_suite.py
+-rw-r--r--   0        0        0     8518 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/cli.py
+-rw-r--r--   0        0        0    11336 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/exceptions.py
+-rw-r--r--   0        0        0     7295 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/protocols.py
+-rw-r--r--   0        0        0     1785 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft2019-09.json
+-rw-r--r--   0        0        0     2452 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft2020-12.json
+-rw-r--r--   0        0        0     2600 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft3.json
+-rw-r--r--   0        0        0     4357 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft4.json
+-rw-r--r--   0        0        0     4437 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft6.json
+-rw-r--r--   0        0        0     4819 2023-03-13 20:55:41.388417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft7.json
+-rw-r--r--   0        0        0     1860 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/applicator
+-rw-r--r--   0        0        0      517 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/content
+-rw-r--r--   0        0        0     1531 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/core
+-rw-r--r--   0        0        0      892 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/meta-data
+-rw-r--r--   0        0        0     2834 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/validation
+-rw-r--r--   0        0        0     1659 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/applicator
+-rw-r--r--   0        0        0      519 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/content
+-rw-r--r--   0        0        0     1564 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/core
+-rw-r--r--   0        0        0      403 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format
+-rw-r--r--   0        0        0      448 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format-annotation
+-rw-r--r--   0        0        0      445 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/format-assertion
+-rw-r--r--   0        0        0      892 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/meta-data
+-rw-r--r--   0        0        0      506 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/unevaluated
+-rw-r--r--   0        0        0     2834 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/validation
+-rw-r--r--   0        0        0    38171 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/validators.py
+-rw-r--r--   0        0        0     1073 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/LICENSE
+-rw-r--r--   0        0        0      744 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/__init__.py
+-rw-r--r--   0        0        0      182 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      599 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py
+-rw-r--r--   0        0        0     2092 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/ast_utils.py
+-rw-r--r--   0        0        0     2814 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/common.py
+-rw-r--r--   0        0        0    10940 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/exceptions.py
+-rw-r--r--   0        0        0     3427 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammars/__init__.py
+-rw-r--r--   0        0        0      944 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammars/common.lark
+-rw-r--r--   0        0        0     1467 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammars/lark.lark
+-rw-r--r--   0        0        0    10995 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammars/python.lark
+-rw-r--r--   0        0        0      103 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammars/unicode.lark
+-rw-r--r--   0        0        0     3076 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/indenter.py
+-rw-r--r--   0        0        0    27483 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/lark.py
+-rw-r--r--   0        0        0    20633 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/lexer.py
+-rw-r--r--   0        0        0    53453 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/load_grammar.py
+-rw-r--r--   0        0        0    14112 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parse_tree_builder.py
+-rw-r--r--   0        0        0     9338 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parser_frontends.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/__init__.py
+-rw-r--r--   0        0        0    12251 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/cyk.py
+-rw-r--r--   0        0        0    13990 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/earley.py
+-rw-r--r--   0        0        0     1581 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/earley_common.py
+-rw-r--r--   0        0        0    31391 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/earley_forest.py
+-rw-r--r--   0        0        0     6421 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/grammar_analysis.py
+-rw-r--r--   0        0        0    10614 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/lalr_analysis.py
+-rw-r--r--   0        0        0     5296 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/lalr_interactive_parser.py
+-rw-r--r--   0        0        0     7216 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/lalr_parser.py
+-rw-r--r--   0        0        0     2497 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/resolve_ambig.py
+-rw-r--r--   0        0        0     7505 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/xearley.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/py.typed
+-rw-r--r--   0        0        0     3728 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/reconstruct.py
+-rw-r--r--   0        0        0     2319 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/tools/__init__.py
+-rw-r--r--   0        0        0     6265 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/tools/nearley.py
+-rw-r--r--   0        0        0     1014 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/tools/serialize.py
+-rw-r--r--   0        0        0     5550 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/tools/standalone.py
+-rw-r--r--   0        0        0     8178 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/tree.py
+-rw-r--r--   0        0        0     6004 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/tree_matcher.py
+-rw-r--r--   0        0        0     5958 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/tree_templates.py
+-rw-r--r--   0        0        0    11089 2023-03-13 20:55:41.392417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/utils.py
+-rw-r--r--   0        0        0    21096 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/lark/visitors.py
+-rw-r--r--   0        0        0      197 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/LICENSE
+-rw-r--r--   0        0        0    10174 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/LICENSE.BSD
+-rw-r--r--   0        0        0      501 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8813 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     9399 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5148 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8161 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/py.typed
+-rw-r--r--   0        0        0     3264 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39046 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18065 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16295 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     1060 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/LICENSE.mit
+-rw-r--r--   0        0        0     1479 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/__init__.py
+-rw-r--r--   0        0        0    18372 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_checked_types.py
+-rw-r--r--   0        0        0    11963 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_field_common.py
+-rw-r--r--   0        0        0     3232 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_helpers.py
+-rw-r--r--   0        0        0     3287 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_immutable.py
+-rw-r--r--   0        0        0     6730 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pbag.py
+-rw-r--r--   0        0        0     9702 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pclass.py
+-rw-r--r--   0        0        0    12203 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pdeque.py
+-rw-r--r--   0        0        0     8293 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_plist.py
+-rw-r--r--   0        0        0    18781 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pmap.py
+-rw-r--r--   0        0        0     7032 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_precord.py
+-rw-r--r--   0        0        0     5693 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pset.py
+-rw-r--r--   0        0        0    22694 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pvector.py
+-rw-r--r--   0        0        0     3425 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_toolz.py
+-rw-r--r--   0        0        0     3800 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_transformations.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/py.typed
+-rw-r--r--   0        0        0     1767 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/typing.py
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/LICENSE
+-rw-r--r--   0        0        0     1148 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/__init__.py
+-rw-r--r--   0        0        0      532 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/_compat.py
+-rw-r--r--   0        0        0     4015 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/_utils.py
+-rw-r--r--   0        0        0     7120 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/api.py
+-rw-r--r--   0        0        0    29687 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/container.py
+-rw-r--r--   0        0        0     5486 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/exceptions.py
+-rw-r--r--   0        0        0    51976 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/items.py
+-rw-r--r--   0        0        0    37694 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/parser.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/py.typed
+-rw-r--r--   0        0        0     4882 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/source.py
+-rw-r--r--   0        0        0     1291 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/toml_char.py
+-rw-r--r--   0        0        0      110 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/toml_document.py
+-rw-r--r--   0        0        0     1599 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/toml_file.py
+-rw-r--r--   0        0        0    12787 2023-03-13 20:55:41.396417 poetry_core-1.5.2/src/poetry/core/_vendor/typing_extensions.LICENSE
+-rw-r--r--   0        0        0    80078 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      574 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/_vendor/vendor.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/__init__.py
+-rw-r--r--   0        0        0      719 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/generic/__init__.py
+-rw-r--r--   0        0        0     1162 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/generic/any_constraint.py
+-rw-r--r--   0        0        0     1055 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/generic/base_constraint.py
+-rw-r--r--   0        0        0     4524 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/generic/constraint.py
+-rw-r--r--   0        0        0     1068 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/generic/empty_constraint.py
+-rw-r--r--   0        0        0     3689 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/generic/multi_constraint.py
+-rw-r--r--   0        0        0     2036 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/generic/parser.py
+-rw-r--r--   0        0        0     5880 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/generic/union_constraint.py
+-rw-r--r--   0        0        0      832 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/__init__.py
+-rw-r--r--   0        0        0     1416 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/empty_constraint.py
+-rw-r--r--   0        0        0       86 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/exceptions.py
+-rw-r--r--   0        0        0     5724 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/parser.py
+-rw-r--r--   0        0        0      913 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/patterns.py
+-rw-r--r--   0        0        0     1543 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/util.py
+-rw-r--r--   0        0        0     5047 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/version.py
+-rw-r--r--   0        0        0     1731 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/version_constraint.py
+-rw-r--r--   0        0        0    13641 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/version_range.py
+-rw-r--r--   0        0        0     2383 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/version_range_constraint.py
+-rw-r--r--   0        0        0    14643 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/constraints/version/version_union.py
+-rw-r--r--   0        0        0      132 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/exceptions/__init__.py
+-rw-r--r--   0        0        0       84 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/exceptions/base.py
+-rw-r--r--   0        0        0    16981 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/factory.py
+-rw-r--r--   0        0        0      975 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/json/__init__.py
+-rw-r--r--   0        0        0    18190 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/json/schemas/poetry-schema.json
+-rw-r--r--   0        0        0      255 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/__init__.py
+-rw-r--r--   0        0        0     2682 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/api.py
+-rw-r--r--   0        0        0      994 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/builder.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/builders/__init__.py
+-rw-r--r--   0        0        0    12881 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/builders/builder.py
+-rw-r--r--   0        0        0    15020 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/builders/sdist.py
+-rw-r--r--   0        0        0    14441 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/builders/wheel.py
+-rw-r--r--   0        0        0     3012 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/metadata.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/utils/__init__.py
+-rw-r--r--   0        0        0     3094 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/utils/helpers.py
+-rw-r--r--   0        0        0     1100 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/utils/include.py
+-rw-r--r--   0        0        0     3697 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/utils/module.py
+-rw-r--r--   0        0        0     2720 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/masonry/utils/package_include.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/__init__.py
+-rw-r--r--   0        0        0      930 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/constraints/__init__.py
+-rw-r--r--   0        0        0    17918 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/dependency.py
+-rw-r--r--   0        0        0     1479 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/dependency_group.py
+-rw-r--r--   0        0        0     1801 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/directory_dependency.py
+-rw-r--r--   0        0        0     1525 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/file_dependency.py
+-rw-r--r--   0        0        0    21119 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/package.py
+-rw-r--r--   0        0        0     2492 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/path_dependency.py
+-rw-r--r--   0        0        0     2912 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/project_package.py
+-rw-r--r--   0        0        0     6355 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/specification.py
+-rw-r--r--   0        0        0     1531 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/url_dependency.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/utils/__init__.py
+-rw-r--r--   0        0        0     6890 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/utils/link.py
+-rw-r--r--   0        0        0    13198 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/utils/utils.py
+-rw-r--r--   0        0        0     3053 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/packages/vcs_dependency.py
+-rw-r--r--   0        0        0     1145 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/poetry.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/py.typed
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/pyproject/__init__.py
+-rw-r--r--   0        0        0      149 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/pyproject/exceptions.py
+-rw-r--r--   0        0        0     2127 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/pyproject/tables.py
+-rw-r--r--   0        0        0     3254 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/pyproject/toml.py
+-rw-r--r--   0        0        0      199 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/semver/__init__.py
+-rw-r--r--   0        0        0      128 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/semver/empty_constraint.py
+-rw-r--r--   0        0        0      149 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/semver/exceptions.py
+-rw-r--r--   0        0        0      239 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/semver/helpers.py
+-rw-r--r--   0        0        0      622 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/semver/patterns.py
+-rw-r--r--   0        0        0      134 2023-03-13 20:55:41.400417 poetry_core-1.5.2/src/poetry/core/semver/util.py
+-rw-r--r--   0        0        0      112 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/semver/version.py
+-rw-r--r--   0        0        0      132 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/semver/version_constraint.py
+-rw-r--r--   0        0        0      122 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/semver/version_range.py
+-rw-r--r--   0        0        0      142 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/semver/version_range_constraint.py
+-rw-r--r--   0        0        0      122 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/semver/version_union.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/spdx/__init__.py
+-rw-r--r--   0        0        0    30125 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/spdx/data/licenses.json
+-rw-r--r--   0        0        0     1352 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/spdx/helpers.py
+-rw-r--r--   0        0        0     5639 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/spdx/license.py
+-rw-r--r--   0        0        0     1107 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/spdx/updater.py
+-rw-r--r--   0        0        0      167 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/toml/__init__.py
+-rw-r--r--   0        0        0      221 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/toml/exceptions.py
+-rw-r--r--   0        0        0     1086 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/toml/file.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/utils/__init__.py
+-rw-r--r--   0        0        0       83 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/utils/_compat.py
+-rw-r--r--   0        0        0     2526 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/utils/helpers.py
+-rw-r--r--   0        0        0      252 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/utils/patterns.py
+-rw-r--r--   0        0        0      624 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/utils/toml_file.py
+-rw-r--r--   0        0        0      722 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/vcs/__init__.py
+-rw-r--r--   0        0        0    11234 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/vcs/git.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/__init__.py
+-rw-r--r--   0        0        0       80 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/exceptions.py
+-rw-r--r--   0        0        0      214 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/grammars/__init__.py
+-rw-r--r--   0        0        0      972 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/grammars/markers.lark
+-rw-r--r--   0        0        0     1398 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/grammars/pep508.lark
+-rw-r--r--   0        0        0     1606 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/helpers.py
+-rw-r--r--   0        0        0    29613 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/markers.py
+-rw-r--r--   0        0        0      752 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/parser.py
+-rw-r--r--   0        0        0      352 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/pep440/__init__.py
+-rw-r--r--   0        0        0     2874 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/pep440/parser.py
+-rw-r--r--   0        0        0     4870 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/pep440/segments.py
+-rw-r--r--   0        0        0    10979 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/pep440/version.py
+-rw-r--r--   0        0        0     3501 2023-03-13 20:55:41.404417 poetry_core-1.5.2/src/poetry/core/version/requirements.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     2687 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/generic/__init__.py
+-rw-r--r--   0        0        0    12991 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/generic/test_constraint.py
+-rw-r--r--   0        0        0     1800 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/generic/test_main.py
+-rw-r--r--   0        0        0     1187 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/generic/test_multi_constraint.py
+-rw-r--r--   0        0        0     1169 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/generic/test_union_constraint.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/version/__init__.py
+-rw-r--r--   0        0        0    13374 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/version/test_helpers.py
+-rw-r--r--   0        0        0     7518 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/version/test_parse_constraint.py
+-rw-r--r--   0        0        0     2925 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/version/test_utils.py
+-rw-r--r--   0        0        0    17288 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/version/test_version.py
+-rw-r--r--   0        0        0      943 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/version/test_version_constraint.py
+-rw-r--r--   0        0        0    14171 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/constraints/version/test_version_range.py
+-rw-r--r--   0        0        0     1329 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/complete.toml
+-rw-r--r--   0        0        0     1116 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0      961 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/distributions/demo-0.1.0.tar.gz
+-rw-r--r--   0        0        0      209 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/invalid_pyproject/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/pep_517_backend/README.md
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/pep_517_backend/foo/__init__.py
+-rw-r--r--   0        0        0     1190 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/pep_517_backend/pyproject.toml
+-rw-r--r--   0        0        0      634 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_failing_strict_validation/pyproject.toml
+-rw-r--r--   0        0        0      407 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_build_system_requires/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_groups_and_explicit_main/README.rst
+-rw-r--r--   0        0        0      326 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_groups_and_explicit_main/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_groups_and_explicit_main/simple_project/__init__.py
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_groups_and_legacy_dev/README.rst
+-rw-r--r--   0        0        0      376 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_groups_and_legacy_dev/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_groups_and_legacy_dev/simple_project/__init__.py
+-rw-r--r--   0        0        0      278 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_invalid_dev_deps/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_markers_and_extras/project/__init__.py
+-rw-r--r--   0        0        0      602 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_markers_and_extras/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_multi_constraints_dependency/project/__init__.py
+-rw-r--r--   0        0        0      394 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_multi_constraints_dependency/pyproject.toml
+-rw-r--r--   0        0        0      255 2023-03-13 20:55:41.404417 poetry_core-1.5.2/tests/fixtures/project_with_pep517_non_poetry/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/project_with_setup/my_package/__init__.py
+-rw-r--r--   0        0        0      346 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/project_with_setup/setup.py
+-rw-r--r--   0        0        0      444 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/project_with_setup_cfg_only/setup.cfg
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/sample_project/README.rst
+-rw-r--r--   0        0        0     2261 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/sample_project/pyproject.toml
+-rw-r--r--   0        0        0       83 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/script-files/sample_script.py
+-rw-r--r--   0        0        0       41 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/script-files/sample_script.sh
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/simple_project/README.rst
+-rw-r--r--   0        0        0     1320 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1106 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz
+-rw-r--r--   0        0        0      590 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/simple_project/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/simple_project/simple_project/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/with_readme_files/README-1.rst
+-rw-r--r--   0        0        0       20 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/with_readme_files/README-2.rst
+-rw-r--r--   0        0        0       79 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/with_readme_files/my_package/__init__.py
+-rw-r--r--   0        0        0      300 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/fixtures/with_readme_files/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2720 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/integration/test_pep517.py
+-rw-r--r--   0        0        0     1499 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/integration/test_pep517_backend.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/json/__init__.py
+-rw-r--r--   0        0        0     2277 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/json/test_poetry_schema.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/__init__.py
+-rw-r--r--   0        0        0      294 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/build_script_in_subdir/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/build_script_in_subdir/scripts/build.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/build_script_in_subdir/src/foo.py
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/README.rst
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/Bar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/IncludedBar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/SecondBar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/Foo/lowercasebar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/FooBar/Bar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/FooBar/lowercasebar.py
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/bar/CapitalFoo.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/my_package/bar/foo.py
+-rw-r--r--   0        0        0     1160 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/comma_file/comma_file/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/comma_file/comma_file/a,b.py
+-rw-r--r--   0        0        0      224 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/comma_file/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/README.rst
+-rw-r--r--   0        0        0       40 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/bin/script.sh
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/my_package/__init__.py
+-rw-r--r--   0        0        0        3 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/my_package/data1/test.json
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/my_package/sub_pkg1/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/my_package/sub_pkg1/extra_file.xml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/my_package/sub_pkg2/__init__.py
+-rw-r--r--   0        0        0        3 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/my_package/sub_pkg2/data2/data.json
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/my_package/sub_pkg3/foo.py
+-rw-r--r--   0        0        0     1348 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/README.rst
+-rw-r--r--   0        0        0      874 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/data1.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/sub_data/data2.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/src/my_package/data/sub_data/data3.txt
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/README.rst
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/data1.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/sub_data/data2.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/my_package/data/sub_data/data3.txt
+-rw-r--r--   0        0        0      874 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/README.rst
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/data1.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/sub_data/data2.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/my_package/data/sub_data/data3.txt
+-rw-r--r--   0        0        0      915 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/disable_setup_py/README.rst
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/disable_setup_py/my_package/__init__.py
+-rw-r--r--   0        0        0      740 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/disable_setup_py/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/epoch/README.rst
+-rw-r--r--   0        0        0       44 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/epoch/epoch.py
+-rw-r--r--   0        0        0      223 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/epoch/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/compiled/source.c
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/compiled/source.h
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude-whl-include-sdist/exclude_whl_include_sdist/cython_code.pyx
+-rw-r--r--   0        0        0      474 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude-whl-include-sdist/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.408417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/README.rst
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/data1.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/data2.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/sub_data/data2.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/data/sub_data/data3.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item1/itemdata1.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item1/subitem/subitemdata.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/item2/itemdata2.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/my_package/puplic/publicdata.txt
+-rw-r--r--   0        0        0      952 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/excluded_subpackage/README.rst
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/excluded_subpackage/example/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/excluded_subpackage/example/test/__init__.py
+-rw-r--r--   0        0        0      148 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/excluded_subpackage/example/test/excluded.py
+-rw-r--r--   0        0        0      329 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/excluded_subpackage/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended/README.rst
+-rw-r--r--   0        0        0      186 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended/build.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended/extended/__init__.py
+-rw-r--r--   0        0        0      888 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended/extended/extended.c
+-rw-r--r--   0        0        0      292 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended/setup.py
+-rw-r--r--   0        0        0       18 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended_with_no_setup/README.rst
+-rw-r--r--   0        0        0      753 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended_with_no_setup/build.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended_with_no_setup/extended/__init__.py
+-rw-r--r--   0        0        0      888 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended_with_no_setup/extended/extended.c
+-rw-r--r--   0        0        0      293 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/extended_with_no_setup/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/include_excluded_code/lib/my_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/include_excluded_code/lib/my_package/generated.py
+-rw-r--r--   0        0        0      485 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/include_excluded_code/pyproject.toml
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/README.rst
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Bar/foo/bar/Foo.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/Bar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/IncludedBar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/SecondBar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/Foo/lowercasebar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/FooBar/Bar.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/FooBar/lowercasebar.py
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/my_package/__init__.py
+-rw-r--r--   0        0        0     1011 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/COPYING
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/COPYING.txt
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/BSD-3.md
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/CUSTOM-LICENSE
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/LICENSES/MIT.txt
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/README.rst
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/my_package/__init__.py
+-rw-r--r--   0        0        0     1231 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/localversionlabel/localversionlabel.py
+-rw-r--r--   0        0        0      133 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/localversionlabel/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/module1/README.rst
+-rw-r--r--   0        0        0       42 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/module1/module1.py
+-rw-r--r--   0        0        0      265 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/module1/pyproject.toml
+-rw-r--r--   0        0        0      261 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/pep_561_stub_only/pyproject.toml
+-rw-r--r--   0        0        0        8 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pkg-stubs/py.typed
+-rw-r--r--   0        0        0      291 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial/pyproject.toml
+-rw-r--r--   0        0        0        8 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pkg-stubs/subpkg/py.typed
+-rw-r--r--   0        0        0      306 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/pep_561_stub_only_partial_namespace/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/pep_561_stub_only_src/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/prerelease/README.rst
+-rw-r--r--   0        0        0       42 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/prerelease/prerelease.py
+-rw-r--r--   0        0        0      233 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/prerelease/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_callable_legacy_string/README.rst
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_callable_legacy_string/my_package/__init__.py
+-rw-r--r--   0        0        0      346 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_callable_legacy_string/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_callable_legacy_table/README.rst
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_callable_legacy_table/my_package/__init__.py
+-rw-r--r--   0        0        0      471 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_callable_legacy_table/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_console/README.rst
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_console/my_package/__init__.py
+-rw-r--r--   0        0        0      481 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_console/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file/README.rst
+-rw-r--r--   0        0        0       40 2023-03-13 20:55:41.412417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file/bin/script.sh
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file/my_package/__init__.py
+-rw-r--r--   0        0        0      371 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/README.rst
+-rw-r--r--   0        0        0       40 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/bin/script.sh
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/my_package/__init__.py
+-rw-r--r--   0        0        0      384 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file_invalid_definition/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file_missing/README.rst
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file_missing/my_package/__init__.py
+-rw-r--r--   0        0        0      371 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/script_reference_file_missing/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/simple_version/README.rst
+-rw-r--r--   0        0        0      217 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/simple_version/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/simple_version/simple_version.py
+-rw-r--r--   0        0        0       28 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/single_python/README.rst
+-rw-r--r--   0        0        0      276 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/single_python/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/single_python/single_python.py
+-rw-r--r--   0        0        0       18 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/source_file/README.rst
+-rw-r--r--   0        0        0      268 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/source_file/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/source_file/src/module_src.py
+-rw-r--r--   0        0        0       18 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/source_package/README.rst
+-rw-r--r--   0        0        0      268 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/source_package/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/source_package/src/package_src/__init__.py
+-rw-r--r--   0        0        0       42 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/source_package/src/package_src/module.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/split_source/lib_a/module_a/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/split_source/lib_b/module_b/__init__.py
+-rw-r--r--   0        0        0      331 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/split_source/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/src_extended/README.rst
+-rw-r--r--   0        0        0      190 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/src_extended/build.py
+-rw-r--r--   0        0        0      292 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/src_extended/pyproject.toml
+-rw-r--r--   0        0        0      598 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/src_extended/setup.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/src_extended/src/extended/__init__.py
+-rw-r--r--   0        0        0      888 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/src_extended/src/extended/extended.c
+-rw-r--r--   0        0        0     1062 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/LICENSE
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/README.rst
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/extra_dir/README.md
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/extra_dir/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/extra_dir/sub_pkg/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/extra_dir/sub_pkg/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/extra_dir/vcs_excluded.txt
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/for_wheel_only/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/my_module.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/notes.txt
+-rw-r--r--   0        0        0       22 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/package_with_include/__init__.py
+-rw-r--r--   0        0        0     1259 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/src/src_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/tests/__init__.py
+-rw-r--r--   0        0        0      238 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_bad_path_dep/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_bad_path_dep/with_bad_path_dep/__init__.py
+-rw-r--r--   0        0        0      274 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_bad_path_dev_dep/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_bad_path_dev_dep/with_bad_path_dev_dep/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_include_inline_table/both.txt
+-rw-r--r--   0        0        0     1050 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_include_inline_table/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_include_inline_table/src/src_package/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_include_inline_table/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_include_inline_table/tests/test_foo/test.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_include_inline_table/wheel_only.txt
+-rw-r--r--   0        0        0      656 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_url_dependency/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_url_dependency/with_url_dependency/__init__.py
+-rw-r--r--   0        0        0      641 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_vcs_dependency/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_vcs_dependency/with_vcs_dependency/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_wildcard_dependency_constraint/my_package/__init__.py
+-rw-r--r--   0        0        0      236 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/fixtures/with_wildcard_dependency_constraint/pyproject.toml
+-rw-r--r--   0        0        0     8986 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/test_builder.py
+-rw-r--r--   0        0        0    12863 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/test_complete.py
+-rw-r--r--   0        0        0    20426 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/test_sdist.py
+-rw-r--r--   0        0        0    11300 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/builders/test_wheel.py
+-rw-r--r--   0        0        0    10197 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/test_api.py
+-rw-r--r--   0        0        0     2202 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/test_builder.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/utils/__init__.py
+-rw-r--r--   0        0        0        8 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/utils/fixtures/pep_561_stub_only_partial_namespace/good-stubs/subpkg/py.typed
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/utils/fixtures/with_includes/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.416417 poetry_core-1.5.2/tests/masonry/utils/fixtures/with_includes/bar/baz.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/masonry/utils/fixtures/with_includes/extra_package/some_dir/foo.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/masonry/utils/fixtures/with_includes/extra_package/some_dir/quux.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/masonry/utils/fixtures/with_includes/not_a_python_pkg/baz.txt
+-rw-r--r--   0        0        0      530 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/masonry/utils/test_helpers.py
+-rw-r--r--   0        0        0     3047 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/masonry/utils/test_package_include.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/__init__.py
+-rw-r--r--   0        0        0    12255 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_dependency.py
+-rw-r--r--   0        0        0      948 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_dependency_group.py
+-rw-r--r--   0        0        0     6036 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_directory_dependency.py
+-rw-r--r--   0        0        0     8481 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_file_dependency.py
+-rw-r--r--   0        0        0    10865 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_main.py
+-rw-r--r--   0        0        0    20447 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_package.py
+-rw-r--r--   0        0        0     3814 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_specification.py
+-rw-r--r--   0        0        0     2588 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_url_dependency.py
+-rw-r--r--   0        0        0     5052 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/test_vcs_dependency.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/utils/__init__.py
+-rw-r--r--   0        0        0     9196 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/utils/test_utils.py
+-rw-r--r--   0        0        0     3929 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/utils/test_utils_link.py
+-rw-r--r--   0        0        0     2248 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/packages/utils/test_utils_urls.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/pyproject/__init__.py
+-rw-r--r--   0        0        0      813 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/pyproject/conftest.py
+-rw-r--r--   0        0        0     3641 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/pyproject/test_pyproject_toml.py
+-rw-r--r--   0        0        0     1056 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/pyproject/test_pyproject_toml_file.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/spdx/__init__.py
+-rw-r--r--   0        0        0     1413 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/spdx/test_helpers.py
+-rw-r--r--   0        0        0     1497 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/spdx/test_license.py
+-rw-r--r--   0        0        0      343 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/test_core_version.py
+-rw-r--r--   0        0        0    14536 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/test_factory.py
+-rw-r--r--   0        0        0     2601 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/testutils.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3800 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/utils/test_helpers.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/vcs/__init__.py
+-rw-r--r--   0        0        0    15077 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/vcs/test_vcs.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/version/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/version/pep440/__init__.py
+-rw-r--r--   0        0        0     4523 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/version/pep440/test_segments.py
+-rw-r--r--   0        0        0     9801 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/version/pep440/test_version.py
+-rw-r--r--   0        0        0    63210 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/version/test_markers.py
+-rw-r--r--   0        0        0     4452 2023-03-13 20:55:41.420417 poetry_core-1.5.2/tests/version/test_requirements.py
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 poetry_core-1.5.2/PKG-INFO
```

### Comparing `poetry_core-1.5.1/LICENSE` & `poetry_core-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/README.md` & `poetry_core-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/pyproject.toml` & `poetry_core-1.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-core"
-version = "1.5.1"
+version = "1.5.2"
 description = "Poetry PEP 517 Build Backend"
 authors = ["Sébastien Eustace <sebastien@eustace.io>"]
 
 license = "MIT"
 
 readme = "README.md"
 
@@ -38,23 +38,23 @@
 [tool.poetry.dependencies]
 python = "^3.7"
 
 # required for compatibility
 importlib-metadata = {version = ">=1.7.0", python = "<3.8"}
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^2.15.0"
-pyrsistent = "^0.18.0"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-pytest-mock = "^3.5"
-tox = "^3.0"
-vendoring = {version = "^1.0", python = "^3.8"}
-build = "^0.7.0"
-mypy = ">=0.960"
+pre-commit = ">=2.15.0"
+pyrsistent = ">=0.18.0"
+pytest = ">=7.1.2"
+pytest-cov = ">=3.0.0"
+pytest-mock = ">=3.5"
+tox = ">=3.0"
+vendoring = {version = ">=1.0", python = "^3.8"}
+build = ">=0.10.0"
+mypy = ">=1.0"
 setuptools = ">=60"
 types-jsonschema = ">=4.4.4"
 types-setuptools = ">=57.4.14"
 
 [tool.black]
 line-length = 88
 preview = true
```

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/__init__.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/_cmp.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/_cmp.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/_compat.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/_compat.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/_config.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/_config.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/_funcs.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/_funcs.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/_make.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/_make.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/_next_gen.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/_next_gen.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/_version_info.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/_version_info.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/converters.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/converters.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/exceptions.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/filters.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/filters.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/setters.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/setters.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attr/validators.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attr/validators.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attrs/LICENSE` & `poetry_core-1.5.2/src/poetry/core/_vendor/attrs/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/attrs/__init__.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/attrs/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/COPYING` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/COPYING`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/__init__.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_format.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_format.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_legacy_validators.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_legacy_validators.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_types.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_types.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_utils.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/_validators.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/_validators.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/benchmarks/issue232/issue.json` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/benchmarks/issue232/issue.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/cli.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/cli.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/exceptions.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/protocols.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/protocols.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft2019-09.json` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft2019-09.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft2020-12.json` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft2020-12.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft3.json` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft3.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft4.json` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft4.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft6.json` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft6.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/draft7.json` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/draft7.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/applicator` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/applicator`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/content` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/content`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/core` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/core`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/meta-data` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/meta-data`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/validation` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2019-09/validation`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/applicator` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/applicator`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/content` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/content`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/core` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/core`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/meta-data` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/meta-data`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/validation` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/schemas/vocabularies/draft2020-12/validation`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/jsonschema/validators.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/jsonschema/validators.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/LICENSE` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/__init__.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/__pyinstaller/hook-lark.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/ast_utils.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/ast_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/common.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/common.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/exceptions.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammar.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammar.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammars/common.lark` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammars/common.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammars/lark.lark` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammars/lark.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/grammars/python.lark` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/grammars/python.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/indenter.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/indenter.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/lark.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/lark.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/lexer.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/lexer.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/load_grammar.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/load_grammar.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parse_tree_builder.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parse_tree_builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parser_frontends.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parser_frontends.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/cyk.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/cyk.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/earley.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/earley.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/earley_common.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/earley_common.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/earley_forest.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/earley_forest.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/grammar_analysis.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/grammar_analysis.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/lalr_analysis.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/lalr_analysis.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/lalr_interactive_parser.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/lalr_interactive_parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/lalr_parser.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/lalr_parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/resolve_ambig.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/resolve_ambig.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/parsers/xearley.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/parsers/xearley.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/reconstruct.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/reconstruct.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/tools/__init__.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/tools/nearley.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/tools/nearley.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/tools/serialize.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/tools/serialize.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/tools/standalone.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/tools/standalone.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/tree.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/tree.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/tree_matcher.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/tree_matcher.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/tree_templates.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/tree_templates.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/utils.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/lark/visitors.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/lark/visitors.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/LICENSE.APACHE` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/LICENSE.BSD` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_elffile.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_manylinux.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_musllinux.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_parser.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_structures.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/_tokenizer.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/markers.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/requirements.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/specifiers.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/tags.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/utils.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/packaging/version.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/LICENSE.mit` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/__init__.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_checked_types.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_checked_types.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_field_common.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_field_common.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_helpers.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_immutable.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_immutable.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pbag.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pbag.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pclass.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pclass.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pdeque.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pdeque.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_plist.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_plist.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pmap.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pmap.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_precord.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_precord.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pset.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pset.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_pvector.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_pvector.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_toolz.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_toolz.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/_transformations.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/_transformations.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/pyrsistent/typing.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/pyrsistent/typing.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/LICENSE` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/__init__.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/_compat.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/_compat.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/_utils.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/api.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/api.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/container.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/container.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/exceptions.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/items.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/items.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/parser.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/source.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/source.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/toml_char.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/toml_char.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/tomlkit/toml_file.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/tomlkit/toml_file.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/typing_extensions.LICENSE` & `poetry_core-1.5.2/src/poetry/core/_vendor/typing_extensions.LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/typing_extensions.py` & `poetry_core-1.5.2/src/poetry/core/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/_vendor/vendor.txt` & `poetry_core-1.5.2/src/poetry/core/_vendor/vendor.txt`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/generic/__init__.py` & `poetry_core-1.5.2/src/poetry/core/constraints/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/generic/any_constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/generic/any_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/generic/base_constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/generic/base_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/generic/constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/generic/constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,18 @@
     @property
     def value(self) -> str:
         return self._value
 
     @property
     def version(self) -> str:
         warnings.warn(
-            "The property 'version' is deprecated and will be removed. "
-            "Please use the property 'value' instead.",
+            (
+                "The property 'version' is deprecated and will be removed. "
+                "Please use the property 'value' instead."
+            ),
             DeprecationWarning,
             stacklevel=2,
         )
         return self.value
 
     @property
     def operator(self) -> str:
```

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/generic/empty_constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/generic/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/generic/multi_constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/generic/multi_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/generic/parser.py` & `poetry_core-1.5.2/src/poetry/core/constraints/generic/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/generic/union_constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/generic/union_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/__init__.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/empty_constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/empty_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/parser.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/patterns.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/patterns.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/util.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/util.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/version.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/version_constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/version_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/version_range.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/version_range.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/version_range_constraint.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/version_range_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/constraints/version/version_union.py` & `poetry_core-1.5.2/src/poetry/core/constraints/version/version_union.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/factory.py` & `poetry_core-1.5.2/src/poetry/core/factory.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/json/__init__.py` & `poetry_core-1.5.2/src/poetry/core/json/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 
 import json
-import os
 
+from pathlib import Path
 from typing import Any
 
 
-SCHEMA_DIR = os.path.join(os.path.dirname(__file__), "schemas")
+SCHEMA_DIR = Path(__file__).parent / "schemas"
 
 
 class ValidationError(ValueError):
     pass
 
 
 def validate_object(obj: dict[str, Any], schema_name: str) -> list[str]:
-    schema_file = os.path.join(SCHEMA_DIR, f"{schema_name}.json")
+    schema_file = SCHEMA_DIR / f"{schema_name}.json"
 
-    if not os.path.exists(schema_file):
+    if not schema_file.exists():
         raise ValueError(f"Schema {schema_name} does not exist.")
 
-    with open(schema_file, encoding="utf-8") as f:
+    with schema_file.open(encoding="utf-8") as f:
         schema = json.loads(f.read())
 
     from jsonschema import Draft7Validator
 
     validator = Draft7Validator(schema)
     validation_errors = sorted(validator.iter_errors(obj), key=lambda e: e.path)  # type: ignore[no-any-return]
```

### Comparing `poetry_core-1.5.1/src/poetry/core/json/schemas/poetry-schema.json` & `poetry_core-1.5.2/src/poetry/core/json/schemas/poetry-schema.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/api.py` & `poetry_core-1.5.2/src/poetry/core/masonry/api.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/builder.py` & `poetry_core-1.5.2/src/poetry/core/masonry/builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/builders/builder.py` & `poetry_core-1.5.2/src/poetry/core/masonry/builders/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,17 +279,20 @@
         for name, specification in self._poetry.local_config.get("scripts", {}).items():
             if isinstance(specification, str):
                 # TODO: deprecate this in favour or reference
                 specification = {"reference": specification, "type": "console"}
 
             if "callable" in specification:
                 warnings.warn(
-                    f"Use of callable in script specification ({name}) is deprecated."
-                    " Use reference instead.",
+                    (
+                        f"Use of callable in script specification ({name}) is"
+                        " deprecated. Use reference instead."
+                    ),
                     DeprecationWarning,
+                    stacklevel=2,
                 )
                 specification = {
                     "reference": specification["callable"],
                     "type": "console",
                 }
 
             if specification.get("type") != "console":
```

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/builders/sdist.py` & `poetry_core-1.5.2/src/poetry/core/masonry/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/builders/wheel.py` & `poetry_core-1.5.2/src/poetry/core/masonry/builders/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,27 +159,27 @@
     def _build(self, wheel: zipfile.ZipFile) -> None:
         if self._package.build_script:
             if not self._poetry.package.build_should_generate_setup():
                 # Since we have a build script but no setup.py generation is required,
                 # we assume that the build script will build and copy the files
                 # directly.
                 # That way they will be picked up when adding files to the wheel.
-                current_path = os.getcwd()
+                current_path = Path.cwd()
                 try:
-                    os.chdir(str(self._path))
+                    os.chdir(self._path)
                     self._run_build_script(self._package.build_script)
                 finally:
                     os.chdir(current_path)
             else:
                 with SdistBuilder(poetry=self._poetry).setup_py() as setup:
                     # We need to place ourselves in the temporary
                     # directory in order to build the package
-                    current_path = os.getcwd()
+                    current_path = Path.cwd()
                     try:
-                        os.chdir(str(self._path))
+                        os.chdir(self._path)
                         self._run_build_command(setup)
                     finally:
                         os.chdir(current_path)
 
                     build_dir = self._path / "build"
                     libs: list[Path] = list(build_dir.glob("lib.*"))
                     if not libs:
@@ -190,31 +190,31 @@
 
                     lib = libs[0]
 
                     for pkg in sorted(lib.glob("**/*")):
                         if pkg.is_dir() or self.is_excluded(pkg):
                             continue
 
-                        rel_path = str(pkg.relative_to(lib))
+                        rel_path = pkg.relative_to(lib)
 
-                        if rel_path in wheel.namelist():
+                        if rel_path.as_posix() in wheel.namelist():
                             continue
 
                         logger.debug(f"Adding: {rel_path}")
 
                         self._add_file(wheel, pkg, rel_path)
 
     def _copy_file_scripts(self, wheel: zipfile.ZipFile) -> None:
         file_scripts = self.convert_script_files()
 
         for abs_path in file_scripts:
             self._add_file(
                 wheel,
                 abs_path,
-                Path.joinpath(Path(self.wheel_data_folder), "scripts", abs_path.name),
+                Path(self.wheel_data_folder) / "scripts" / abs_path.name,
             )
 
     def _run_build_command(self, setup: Path) -> None:
         subprocess.check_call(
             [
                 self.executable.as_posix(),
                 str(setup),
@@ -264,15 +264,15 @@
 
         for license_file in license_files:
             if not license_file.is_file():
                 logger.debug(f"Skipping: {license_file.as_posix()}")
                 continue
 
             dest = dist_info / license_file.relative_to(self._path)
-            os.makedirs(dest.parent, exist_ok=True)
+            dest.parent.mkdir(parents=True, exist_ok=True)
             shutil.copy(license_file, dest)
 
         return dist_info
 
     def _write_record(self, wheel: zipfile.ZipFile) -> None:
         # Write a record of the files in the wheel
         with self._write_to_zip(wheel, self.dist_info + "/RECORD") as f:
@@ -341,27 +341,23 @@
             tag = (impl, "none", platform)
 
         return "-".join(tag)
 
     def _add_file(
         self,
         wheel: zipfile.ZipFile,
-        full_path: Path | str,
-        rel_path: Path | str,
+        full_path: Path,
+        rel_path: Path,
     ) -> None:
-        full_path, rel_path = str(full_path), str(rel_path)
-        if os.sep != "/":
-            # We always want to have /-separated paths in the zip file and in
-            # RECORD
-            rel_path = rel_path.replace(os.sep, "/")
-
-        zinfo = zipfile.ZipInfo(rel_path)
+        # We always want to have /-separated paths in the zip file and in RECORD
+        rel_path_name = rel_path.as_posix()
+        zinfo = zipfile.ZipInfo(rel_path_name)
 
         # Normalize permission bits to either 755 (executable) or 644
-        st_mode = os.stat(full_path).st_mode
+        st_mode = full_path.stat().st_mode
         new_mode = normalize_file_permissions(st_mode)
         zinfo.external_attr = (new_mode & 0xFFFF) << 16  # Unix attributes
 
         if stat.S_ISDIR(st_mode):
             zinfo.external_attr |= 0x10  # MS-DOS directory flag
 
         hashsum = hashlib.sha256()
@@ -371,18 +367,18 @@
                 if not buf:
                     break
                 hashsum.update(buf)
 
             src.seek(0)
             wheel.writestr(zinfo, src.read(), compress_type=zipfile.ZIP_DEFLATED)
 
-        size = os.stat(full_path).st_size
+        size = full_path.stat().st_size
         hash_digest = urlsafe_b64encode(hashsum.digest()).decode("ascii").rstrip("=")
 
-        self._records.append((rel_path, hash_digest, size))
+        self._records.append((rel_path_name, hash_digest, size))
 
     @contextlib.contextmanager
     def _write_to_zip(
         self, wheel: zipfile.ZipFile, rel_path: str
     ) -> Iterator[StringIO]:
         sio = StringIO()
         yield sio
```

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/metadata.py` & `poetry_core-1.5.2/src/poetry/core/masonry/metadata.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/utils/helpers.py` & `poetry_core-1.5.2/src/poetry/core/masonry/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,18 @@
 
 def escape_name(name: str) -> str:
     """
     Escaped wheel name as specified in https://packaging.python.org/en/latest/specifications/binary-distribution-format/#escaping-and-unicode.
     This function should only be used for the generation of artifact names, and not to normalize or filter existing artifact names.
     """
     warnings.warn(
-        "escape_name() is deprecated. Use packaging.utils.canonicalize_name() and"
-        " distribution_name() instead.",
+        (
+            "escape_name() is deprecated. Use packaging.utils.canonicalize_name() and"
+            " distribution_name() instead."
+        ),
         DeprecationWarning,
         stacklevel=2,
     )
     return re.sub(r"[-_.]+", "_", name, flags=re.UNICODE).lower()
 
 
 def distribution_name(name: NormalizedName) -> DistributionName:
```

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/utils/include.py` & `poetry_core-1.5.2/src/poetry/core/masonry/utils/include.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/utils/module.py` & `poetry_core-1.5.2/src/poetry/core/masonry/utils/module.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/masonry/utils/package_include.py` & `poetry_core-1.5.2/src/poetry/core/masonry/utils/package_include.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/constraints/__init__.py` & `poetry_core-1.5.2/src/poetry/core/packages/constraints/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 from poetry.core.constraints.generic import MultiConstraint
 from poetry.core.constraints.generic import UnionConstraint
 from poetry.core.constraints.generic import parse_constraint
 from poetry.core.constraints.generic.parser import parse_single_constraint
 
 
 warnings.warn(
-    "poetry.core.packages.constraints is deprecated."
-    " Use poetry.core.constraints.generic instead.",
+    (
+        "poetry.core.packages.constraints is deprecated."
+        " Use poetry.core.constraints.generic instead."
+    ),
     DeprecationWarning,
     stacklevel=2,
 )
 
 
 __all__ = [
     "AnyConstraint",
```

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/dependency.py` & `poetry_core-1.5.2/src/poetry/core/packages/dependency.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,16 +101,18 @@
         else:
             self._constraint = constraint
 
         self._pretty_constraint = str(constraint)
 
     def set_constraint(self, constraint: str | VersionConstraint) -> None:
         warnings.warn(
-            "Calling method 'set_constraint' is deprecated and will be removed. "
-            "It has been replaced by the property 'constraint' for consistency.",
+            (
+                "Calling method 'set_constraint' is deprecated and will be removed. "
+                "It has been replaced by the property 'constraint' for consistency."
+            ),
             DeprecationWarning,
             stacklevel=2,
         )
         self.constraint = constraint  # type: ignore[assignment]
 
     @property
     def pretty_constraint(self) -> str:
```

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/dependency_group.py` & `poetry_core-1.5.2/src/poetry/core/packages/dependency_group.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/directory_dependency.py` & `poetry_core-1.5.2/src/poetry/core/packages/directory_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/file_dependency.py` & `poetry_core-1.5.2/src/poetry/core/packages/file_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/package.py` & `poetry_core-1.5.2/src/poetry/core/packages/package.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,18 @@
         """
         Creates a new in memory package.
         """
         from poetry.core.version.markers import AnyMarker
 
         if pretty_version is not None:
             warnings.warn(
-                "The `pretty_version` parameter is deprecated and will be removed"
-                " in a future release.",
+                (
+                    "The `pretty_version` parameter is deprecated and will be removed"
+                    " in a future release."
+                ),
                 DeprecationWarning,
                 stacklevel=2,
             )
 
         super().__init__(
             name,
             source_type=source_type,
@@ -371,26 +373,32 @@
             urls["Documentation"] = self.documentation_url
 
         return urls
 
     @property
     def readme(self) -> Path | None:
         warnings.warn(
-            "`readme` is deprecated: you are getting only the first readme file. Please"
-            " use the plural form `readmes`.",
+            (
+                "`readme` is deprecated: you are getting only the first readme file."
+                " Please use the plural form `readmes`."
+            ),
             DeprecationWarning,
+            stacklevel=2,
         )
         return next(iter(self.readmes), None)
 
     @readme.setter
     def readme(self, path: Path) -> None:
         warnings.warn(
-            "`readme` is deprecated. Please assign a tuple to the plural form"
-            " `readmes`.",
+            (
+                "`readme` is deprecated. Please assign a tuple to the plural form"
+                " `readmes`."
+            ),
             DeprecationWarning,
+            stacklevel=2,
         )
         self.readmes = (path,)
 
     @property
     def yanked(self) -> bool:
         return isinstance(self._yanked, str) or bool(self._yanked)
```

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/path_dependency.py` & `poetry_core-1.5.2/src/poetry/core/packages/path_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/project_package.py` & `poetry_core-1.5.2/src/poetry/core/packages/project_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,18 @@
         self,
         name: str,
         version: str | Version,
         pretty_version: str | None = None,
     ) -> None:
         if pretty_version is not None:
             warnings.warn(
-                "The `pretty_version` parameter is deprecated and will be removed"
-                " in a future release.",
+                (
+                    "The `pretty_version` parameter is deprecated and will be removed"
+                    " in a future release."
+                ),
                 DeprecationWarning,
                 stacklevel=2,
             )
 
         super().__init__(name, version)
 
         self.build_config: dict[str, Any] = {}
```

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/specification.py` & `poetry_core-1.5.2/src/poetry/core/packages/specification.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/url_dependency.py` & `poetry_core-1.5.2/src/poetry/core/packages/url_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/utils/link.py` & `poetry_core-1.5.2/src/poetry/core/packages/utils/link.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/utils/utils.py` & `poetry_core-1.5.2/src/poetry/core/packages/utils/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/packages/vcs_dependency.py` & `poetry_core-1.5.2/src/poetry/core/packages/vcs_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/poetry.py` & `poetry_core-1.5.2/src/poetry/core/poetry.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/pyproject/tables.py` & `poetry_core-1.5.2/src/poetry/core/pyproject/tables.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/pyproject/toml.py` & `poetry_core-1.5.2/src/poetry/core/pyproject/toml.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/semver/patterns.py` & `poetry_core-1.5.2/src/poetry/core/semver/patterns.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/spdx/data/licenses.json` & `poetry_core-1.5.2/src/poetry/core/spdx/data/licenses.json`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/spdx/helpers.py` & `poetry_core-1.5.2/src/poetry/core/spdx/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/spdx/license.py` & `poetry_core-1.5.2/src/poetry/core/spdx/license.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/spdx/updater.py` & `poetry_core-1.5.2/src/poetry/core/spdx/updater.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/toml/file.py` & `poetry_core-1.5.2/src/poetry/core/toml/file.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/utils/helpers.py` & `poetry_core-1.5.2/src/poetry/core/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/utils/toml_file.py` & `poetry_core-1.5.2/src/poetry/core/utils/toml_file.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/vcs/__init__.py` & `poetry_core-1.5.2/src/poetry/core/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/vcs/git.py` & `poetry_core-1.5.2/src/poetry/core/vcs/git.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/version/grammars/markers.lark` & `poetry_core-1.5.2/src/poetry/core/version/grammars/markers.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/version/grammars/pep508.lark` & `poetry_core-1.5.2/src/poetry/core/version/grammars/pep508.lark`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/version/helpers.py` & `poetry_core-1.5.2/src/poetry/core/version/helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/version/markers.py` & `poetry_core-1.5.2/src/poetry/core/version/markers.py`

 * *Files 0% similar despite different names*

```diff
@@ -779,18 +779,15 @@
                 token.children, tree_prefix=tree_prefix, top_level=False
             )
             groups[-1].append(sub_marker)
 
         elif token.data == f"{tree_prefix}item":
             name, op, value = token.children
             if value.type == f"{tree_prefix}MARKER_NAME":
-                name, value, = (
-                    value,
-                    name,
-                )
+                name, value = value, name
 
             value = value[1:-1]
             sub_marker = SingleMarker(str(name), f"{op}{value}")
             groups[-1].append(sub_marker)
 
         elif token.data == f"{tree_prefix}BOOL_OP" and token.children[0] == "or":
             groups.append([])
@@ -829,16 +826,18 @@
         dnf_markers = [dnf(m) for m in marker.markers]
         sub_marker_lists = [
             m.markers if isinstance(m, MarkerUnion) else [m] for m in dnf_markers
         ]
         return MarkerUnion.of(
             *[MultiMarker.of(*c) for c in itertools.product(*sub_marker_lists)]
         )
+
     if isinstance(marker, MarkerUnion):
         return MarkerUnion.of(*[dnf(m) for m in marker.markers])
+
     return marker
 
 
 def intersection(*markers: BaseMarker) -> BaseMarker:
     return dnf(MultiMarker(*markers))
```

### Comparing `poetry_core-1.5.1/src/poetry/core/version/parser.py` & `poetry_core-1.5.2/src/poetry/core/version/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/version/pep440/parser.py` & `poetry_core-1.5.2/src/poetry/core/version/pep440/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/src/poetry/core/version/pep440/segments.py` & `poetry_core-1.5.2/src/poetry/core/version/pep440/segments.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,18 @@
         )
 
     def to_string(self, short: bool = False) -> str:
         if short:
             import warnings
 
             warnings.warn(
-                "Parameter 'short' has no effect and will be removed. "
-                "(Release tags are always normalized according to PEP 440 now.)",
+                (
+                    "Parameter 'short' has no effect and will be removed. "
+                    "(Release tags are always normalized according to PEP 440 now.)"
+                ),
                 DeprecationWarning,
                 stacklevel=2,
             )
 
         return f"{self.phase}{self.number}"
 
     def next(self) -> ReleaseTag:
```

### Comparing `poetry_core-1.5.1/src/poetry/core/version/pep440/version.py` & `poetry_core-1.5.2/src/poetry/core/version/pep440/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,16 +115,16 @@
             # the sorting rules in PEP440.
             # - Alpha numeric segments sort before numeric segments
             # - Alpha numeric segments sort lexicographically
             # - Numeric segments sort numerically
             # - Shorter versions sort before longer versions when the prefixes
             #   match exactly
             assert isinstance(self.local, tuple)
+            # We convert strings that are integers so that they can be compared
             _local = tuple(
-                # We typecast strings that are integers so that they can be compared
                 (int(i), "") if str(i).isnumeric() else (NegativeInfinity(), i)
                 for i in self.local
             )
         return self.epoch, self.release, _pre, _post, _dev, _local
 
     @property
     def major(self) -> int:
@@ -144,16 +144,18 @@
         return self.release.extra
 
     def to_string(self, short: bool = False) -> str:
         if short:
             import warnings
 
             warnings.warn(
-                "Parameter 'short' has no effect and will be removed. "
-                "(Versions are always normalized according to PEP 440 now.)",
+                (
+                    "Parameter 'short' has no effect and will be removed. "
+                    "(Versions are always normalized according to PEP 440 now.)"
+                ),
                 DeprecationWarning,
                 stacklevel=2,
             )
 
         version_string = self.release.to_string()
 
         if self.epoch:
@@ -228,17 +230,19 @@
         ):
             release = release.next_patch()
         return self.__class__(epoch=self.epoch, release=release)
 
     def next_prerelease(self: T, next_phase: bool = False) -> PEP440Version:
         if self.is_stable():
             warnings.warn(
-                "Calling next_prerelease() on a stable release is deprecated for its"
-                " ambiguity. Use next_major(), next_minor(), etc. together with"
-                " first_prerelease()",
+                (
+                    "Calling next_prerelease() on a stable release is deprecated for"
+                    " its ambiguity. Use next_major(), next_minor(), etc. together with"
+                    " first_prerelease()"
+                ),
                 DeprecationWarning,
                 stacklevel=2,
             )
         if self.is_prerelease():
             assert self.pre is not None
             if not self.is_devrelease() or self.is_postrelease():
                 pre = self.pre.next_phase() if next_phase else self.pre.next()
@@ -263,17 +267,19 @@
 
     def next_devrelease(self: T) -> T:
         if self.is_devrelease():
             assert self.dev is not None
             dev = self.dev.next()
         else:
             warnings.warn(
-                "Calling next_devrelease() on a non dev release is deprecated for its"
-                " ambiguity. Use next_major(), next_minor(), etc. together with"
-                " first_devrelease()",
+                (
+                    "Calling next_devrelease() on a non dev release is deprecated for"
+                    " its ambiguity. Use next_major(), next_minor(), etc. together with"
+                    " first_devrelease()"
+                ),
                 DeprecationWarning,
                 stacklevel=2,
             )
             dev = ReleaseTag(RELEASE_PHASE_ID_DEV)
         return self.__class__(
             epoch=self.epoch,
             release=self.release,
```

### Comparing `poetry_core-1.5.1/src/poetry/core/version/requirements.py` & `poetry_core-1.5.2/src/poetry/core/version/requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/conftest.py` & `poetry_core-1.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/generic/test_constraint.py` & `poetry_core-1.5.2/tests/constraints/generic/test_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/generic/test_main.py` & `poetry_core-1.5.2/tests/constraints/generic/test_main.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/generic/test_multi_constraint.py` & `poetry_core-1.5.2/tests/constraints/generic/test_multi_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/generic/test_union_constraint.py` & `poetry_core-1.5.2/tests/constraints/generic/test_union_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/version/test_helpers.py` & `poetry_core-1.5.2/tests/constraints/version/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/version/test_parse_constraint.py` & `poetry_core-1.5.2/tests/constraints/version/test_parse_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/version/test_utils.py` & `poetry_core-1.5.2/tests/constraints/version/test_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/version/test_version.py` & `poetry_core-1.5.2/tests/constraints/version/test_version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/version/test_version_constraint.py` & `poetry_core-1.5.2/tests/constraints/version/test_version_constraint.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/constraints/version/test_version_range.py` & `poetry_core-1.5.2/tests/constraints/version/test_version_range.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/complete.toml` & `poetry_core-1.5.2/tests/fixtures/complete.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl` & `poetry_core-1.5.2/tests/fixtures/distributions/demo-0.1.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/distributions/demo-0.1.0.tar.gz` & `poetry_core-1.5.2/tests/fixtures/distributions/demo-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/pep_517_backend/pyproject.toml` & `poetry_core-1.5.2/tests/fixtures/pep_517_backend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/project_failing_strict_validation/pyproject.toml` & `poetry_core-1.5.2/tests/fixtures/project_failing_strict_validation/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/project_with_markers_and_extras/pyproject.toml` & `poetry_core-1.5.2/tests/fixtures/project_with_markers_and_extras/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/sample_project/pyproject.toml` & `poetry_core-1.5.2/tests/fixtures/sample_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl` & `poetry_core-1.5.2/tests/fixtures/simple_project/dist/simple_project-1.2.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz` & `poetry_core-1.5.2/tests/fixtures/simple_project/dist/simple_project-1.2.3.tar.gz`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/fixtures/simple_project/pyproject.toml` & `poetry_core-1.5.2/tests/fixtures/simple_project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/integration/test_pep517.py` & `poetry_core-1.5.2/tests/integration/test_pep517.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/integration/test_pep517_backend.py` & `poetry_core-1.5.2/tests/integration/test_pep517_backend.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/json/test_poetry_schema.py` & `poetry_core-1.5.2/tests/json/test_poetry_schema.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/case_sensitive_exclusions/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/case_sensitive_exclusions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/complete/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/complete/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/default_src_with_excluded_data/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/default_src_with_excluded_data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/default_with_excluded_data_toml/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/default_with_excluded_data_toml/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/disable_setup_py/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/disable_setup_py/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/exclude_nested_data_toml/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/exclude_nested_data_toml/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/extended/extended/extended.c` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/extended/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/extended/setup.py` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/extended/setup.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/extended_with_no_setup/build.py` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/extended_with_no_setup/build.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/extended_with_no_setup/extended/extended.c` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/extended_with_no_setup/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/invalid_case_sensitive_exclusions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/licenses_and_copying/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/licenses_and_copying/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/src_extended/setup.py` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/src_extended/setup.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/src_extended/src/extended/extended.c` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/src_extended/src/extended/extended.c`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/LICENSE` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/with-include/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/with-include/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/with_include_inline_table/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/with_include_inline_table/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/with_url_dependency/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/with_url_dependency/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/fixtures/with_vcs_dependency/pyproject.toml` & `poetry_core-1.5.2/tests/masonry/builders/fixtures/with_vcs_dependency/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/test_builder.py` & `poetry_core-1.5.2/tests/masonry/builders/test_builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/test_complete.py` & `poetry_core-1.5.2/tests/masonry/builders/test_complete.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import csv
 import os
 import platform
 import re
 import shutil
 import sys
 import tarfile
 import tempfile
@@ -38,348 +39,142 @@
 def clear_samples_dist() -> None:
     for dist in fixtures_dir.glob("**/dist"):
         if dist.is_dir():
             shutil.rmtree(str(dist))
 
 
 @pytest.mark.skipif(
-    sys.platform == "win32"
-    and sys.version_info <= (3, 6)
-    or platform.python_implementation().lower() == "pypy",
-    reason="Disable test on Windows for Python <=3.6 and for PyPy",
+    platform.python_implementation().lower() == "pypy", reason="Disable test for PyPy"
 )
-def test_wheel_c_extension() -> None:
-    module_path = fixtures_dir / "extended"
-    builder = Builder(Factory().create_poetry(module_path))
-    builder.build(fmt="all")
-
-    sdist = fixtures_dir / "extended" / "dist" / "extended-0.1.tar.gz"
-
-    assert sdist.exists()
-
-    with tarfile.open(str(sdist), "r") as tar:
-        assert "extended-0.1/build.py" in tar.getnames()
-        assert "extended-0.1/extended/extended.c" in tar.getnames()
-
-    whl = list((module_path / "dist").glob("extended-0.1-cp*-cp*-*.whl"))[0]
-
-    assert whl.exists()
-
-    zip = zipfile.ZipFile(str(whl))
-
-    has_compiled_extension = False
-    for name in zip.namelist():
-        if name.startswith("extended/extended") and name.endswith((".so", ".pyd")):
-            has_compiled_extension = True
-
-    assert has_compiled_extension
-
-    try:
-        wheel_data = zip.read("extended-0.1.dist-info/WHEEL").decode()
-
-        assert (
-            re.match(
-                f"""(?m)^\
-Wheel-Version: 1.0
-Generator: poetry-core {__version__}
-Root-Is-Purelib: false
-Tag: cp[23]_?\\d+-cp[23]_?\\d+m?u?-.+
-$""",
-                wheel_data,
-            )
-            is not None
-        )
-
-        records = zip.read("extended-0.1.dist-info/RECORD").decode()
-
-        assert re.search(r"\s+extended/extended.*\.(so|pyd)", records) is not None
-    finally:
-        zip.close()
-
-
-@pytest.mark.skipif(
-    sys.platform == "win32"
-    and sys.version_info <= (3, 6)
-    or platform.python_implementation().lower() == "pypy",
-    reason="Disable test on Windows for Python <=3.6 and for PyPy",
+@pytest.mark.parametrize(
+    ["project", "exptected_c_dir"],
+    [
+        ("extended", "extended"),
+        ("extended_with_no_setup", "extended"),
+        ("src_extended", "src/extended"),
+    ],
 )
-def test_wheel_c_extension_with_no_setup() -> None:
-    module_path = fixtures_dir / "extended_with_no_setup"
+def test_wheel_c_extension(project: str, exptected_c_dir: str) -> None:
+    module_path = fixtures_dir / project
     builder = Builder(Factory().create_poetry(module_path))
     builder.build(fmt="all")
 
-    sdist = fixtures_dir / "extended_with_no_setup" / "dist" / "extended-0.1.tar.gz"
-
+    sdist = fixtures_dir / project / "dist" / "extended-0.1.tar.gz"
     assert sdist.exists()
 
-    with tarfile.open(str(sdist), "r") as tar:
+    with tarfile.open(sdist, "r") as tar:
         assert "extended-0.1/build.py" in tar.getnames()
-        assert "extended-0.1/extended/extended.c" in tar.getnames()
+        assert f"extended-0.1/{exptected_c_dir}/extended.c" in tar.getnames()
 
     whl = list((module_path / "dist").glob("extended-0.1-cp*-cp*-*.whl"))[0]
-
     assert whl.exists()
 
-    zip = zipfile.ZipFile(str(whl))
-
-    has_compiled_extension = False
-    for name in zip.namelist():
-        if name.startswith("extended/extended") and name.endswith((".so", ".pyd")):
-            has_compiled_extension = True
-
-    assert has_compiled_extension
-
-    try:
-        wheel_data = zip.read("extended-0.1.dist-info/WHEEL").decode()
+    with zipfile.ZipFile(whl) as zipf:
+        has_compiled_extension = False
+        for name in zipf.namelist():
+            if name.startswith("extended/extended") and name.endswith((".so", ".pyd")):
+                has_compiled_extension = True
+        assert has_compiled_extension
 
+        wheel_data = zipf.read("extended-0.1.dist-info/WHEEL").decode()
         assert (
             re.match(
                 f"""(?m)^\
 Wheel-Version: 1.0
 Generator: poetry-core {__version__}
 Root-Is-Purelib: false
 Tag: cp[23]_?\\d+-cp[23]_?\\d+m?u?-.+
 $""",
                 wheel_data,
             )
             is not None
         )
 
-        records = zip.read("extended-0.1.dist-info/RECORD").decode()
-
-        assert re.search(r"\s+extended/extended.*\.(so|pyd)", records) is not None
-    finally:
-        zip.close()
-
+        record = zipf.read("extended-0.1.dist-info/RECORD").decode()
+        records = csv.reader(record.splitlines())
+        record_files = [row[0] for row in records]
+        assert re.search(r"\s+extended/extended.*\.(so|pyd)", record) is not None
+
+        # Files in RECORD should match files in wheel.
+        assert zipf.namelist() == record_files
+        assert len(set(record_files)) == len(record_files)
 
-@pytest.mark.skipif(
-    sys.platform == "win32"
-    and sys.version_info <= (3, 6)
-    or platform.python_implementation().lower() == "pypy",
-    reason="Disable test on Windows for Python <=3.6 and for PyPy",
-)
-def test_wheel_c_extension_src_layout() -> None:
-    module_path = fixtures_dir / "src_extended"
-    builder = Builder(Factory().create_poetry(module_path))
-    builder.build(fmt="all")
-
-    sdist = fixtures_dir / "src_extended" / "dist" / "extended-0.1.tar.gz"
-
-    assert sdist.exists()
-
-    with tarfile.open(str(sdist), "r") as tar:
-        assert "extended-0.1/build.py" in tar.getnames()
-        assert "extended-0.1/src/extended/extended.c" in tar.getnames()
-
-    whl = list((module_path / "dist").glob("extended-0.1-cp*-cp*-*.whl"))[0]
-
-    assert whl.exists()
-
-    zip = zipfile.ZipFile(str(whl))
-
-    has_compiled_extension = False
-    for name in zip.namelist():
-        if name.startswith("extended/extended") and name.endswith((".so", ".pyd")):
-            has_compiled_extension = True
-
-    assert has_compiled_extension
-
-    try:
-        wheel_data = zip.read("extended-0.1.dist-info/WHEEL").decode()
-
-        assert (
-            re.match(
-                f"""(?m)^\
-Wheel-Version: 1.0
-Generator: poetry-core {__version__}
-Root-Is-Purelib: false
-Tag: cp[23]_?\\d+-cp[23]_?\\d+m?u?-.+
-$""",
-                wheel_data,
-            )
-            is not None
-        )
-
-        records = zip.read("extended-0.1.dist-info/RECORD").decode()
 
-        assert re.search(r"\s+extended/extended.*\.(so|pyd)", records) is not None
-    finally:
-        zip.close()
+@pytest.mark.parametrize("no_vcs", [False, True])
+def test_complete(no_vcs: bool) -> None:
+    module_path = fixtures_dir / "complete"
 
+    if no_vcs:
+        # Copy the complete fixtures dir to a temporary directory
+        temporary_dir = Path(tempfile.mkdtemp()) / "complete"
+        shutil.copytree(module_path.as_posix(), temporary_dir.as_posix())
+        module_path = temporary_dir
 
-def test_complete() -> None:
-    module_path = fixtures_dir / "complete"
     builder = Builder(Factory().create_poetry(module_path))
     builder.build(fmt="all")
 
     whl = module_path / "dist" / "my_package-1.2.3-py3-none-any.whl"
 
     assert whl.exists()
     if sys.platform != "win32":
         assert (os.stat(str(whl)).st_mode & 0o777) == 0o644
 
-    zip = zipfile.ZipFile(str(whl))
-
-    try:
-        assert "my_package/sub_pgk1/extra_file.xml" not in zip.namelist()
-        assert "my_package-1.2.3.data/scripts/script.sh" in zip.namelist()
-        assert (
-            "Hello World"
-            in zip.read("my_package-1.2.3.data/scripts/script.sh").decode()
-        )
-
-        entry_points = zip.read("my_package-1.2.3.dist-info/entry_points.txt")
-
-        assert (
-            entry_points.decode()
-            == """\
-[console_scripts]
-extra-script=my_package.extra:main[time]
-my-2nd-script=my_package:main2
-my-script=my_package:main
-
-"""
-        )
-        wheel_data = zip.read("my_package-1.2.3.dist-info/WHEEL").decode()
-
-        assert (
-            wheel_data
-            == f"""\
-Wheel-Version: 1.0
-Generator: poetry-core {__version__}
-Root-Is-Purelib: true
-Tag: py3-none-any
-"""
-        )
-        wheel_data = zip.read("my_package-1.2.3.dist-info/METADATA").decode()
-
-        assert (
-            wheel_data
-            == """\
-Metadata-Version: 2.1
-Name: my-package
-Version: 1.2.3
-Summary: Some description.
-Home-page: https://python-poetry.org/
-License: MIT
-Keywords: packaging,dependency,poetry
-Author: Sébastien Eustace
-Author-email: sebastien@eustace.io
-Maintainer: People Everywhere
-Maintainer-email: people@everywhere.com
-Requires-Python: >=3.6,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: time
-Requires-Dist: cachy[msgpack] (>=0.2.0,<0.3.0)
-Requires-Dist: cleo (>=0.6,<0.7)
-Requires-Dist: pendulum (>=1.4,<2.0) ; (python_version ~= "2.7" and sys_platform == "win32" or python_version in "3.4 3.5") and (extra == "time")
-Project-URL: Documentation, https://python-poetry.org/docs
-Project-URL: Issue Tracker, https://github.com/python-poetry/poetry/issues
-Project-URL: Repository, https://github.com/python-poetry/poetry
-Description-Content-Type: text/x-rst
-
-My Package
-==========
-
-"""
-        )
-        actual_records = zip.read("my_package-1.2.3.dist-info/RECORD").decode()
-
-        # For some reason, the ordering of the files and the SHA hashes
-        # vary per operating systems and Python versions.
-        # So instead of 1:1 assertion, let's do a bit clunkier one:
-
-        expected_records = [
+    expected_name_list = (
+        [
             "my_package/__init__.py",
             "my_package/data1/test.json",
             "my_package/sub_pkg1/__init__.py",
             "my_package/sub_pkg2/__init__.py",
             "my_package/sub_pkg2/data2/data.json",
-            "my_package-1.2.3.dist-info/entry_points.txt",
-            "my_package-1.2.3.dist-info/LICENSE",
-            "my_package-1.2.3.dist-info/WHEEL",
-            "my_package-1.2.3.dist-info/METADATA",
+            "my_package/sub_pkg3/foo.py",
+            "my_package-1.2.3.data/scripts/script.sh",
         ]
+        + sorted(
+            [
+                "my_package-1.2.3.dist-info/entry_points.txt",
+                "my_package-1.2.3.dist-info/LICENSE",
+                "my_package-1.2.3.dist-info/METADATA",
+                "my_package-1.2.3.dist-info/WHEEL",
+            ],
+            key=lambda x: Path(x),
+        )
+        + ["my_package-1.2.3.dist-info/RECORD"]
+    )
 
-        for expected_record in expected_records:
-            assert expected_record in actual_records
-
-    finally:
-        zip.close()
-
-
-def test_complete_no_vcs() -> None:
-    # Copy the complete fixtures dir to a temporary directory
-    module_path = fixtures_dir / "complete"
-    temporary_dir = Path(tempfile.mkdtemp()) / "complete"
-
-    shutil.copytree(module_path.as_posix(), temporary_dir.as_posix())
-
-    builder = Builder(Factory().create_poetry(temporary_dir))
-    builder.build(fmt="all")
-
-    whl = temporary_dir / "dist" / "my_package-1.2.3-py3-none-any.whl"
-
-    assert whl.exists()
-
-    zip = zipfile.ZipFile(str(whl))
-
-    # Check the zipped file to be sure that included and excluded files are
-    # correctly taken account of without vcs
-    expected_name_list = [
-        "my_package/__init__.py",
-        "my_package/data1/test.json",
-        "my_package/sub_pkg1/__init__.py",
-        "my_package/sub_pkg2/__init__.py",
-        "my_package/sub_pkg2/data2/data.json",
-        "my_package-1.2.3.data/scripts/script.sh",
-        "my_package/sub_pkg3/foo.py",
-        "my_package-1.2.3.dist-info/entry_points.txt",
-        "my_package-1.2.3.dist-info/LICENSE",
-        "my_package-1.2.3.dist-info/WHEEL",
-        "my_package-1.2.3.dist-info/METADATA",
-        "my_package-1.2.3.dist-info/RECORD",
-    ]
-
-    assert sorted(zip.namelist()) == sorted(expected_name_list)
+    with zipfile.ZipFile(str(whl)) as zipf:
+        assert zipf.namelist() == expected_name_list
+        assert (
+            "Hello World"
+            in zipf.read("my_package-1.2.3.data/scripts/script.sh").decode()
+        )
 
-    try:
-        entry_points = zip.read("my_package-1.2.3.dist-info/entry_points.txt")
+        entry_points = zipf.read("my_package-1.2.3.dist-info/entry_points.txt")
 
         assert (
             entry_points.decode()
             == """\
 [console_scripts]
 extra-script=my_package.extra:main[time]
 my-2nd-script=my_package:main2
 my-script=my_package:main
 
 """
         )
-        wheel_data = zip.read("my_package-1.2.3.dist-info/WHEEL").decode()
+        wheel_data = zipf.read("my_package-1.2.3.dist-info/WHEEL").decode()
 
         assert (
             wheel_data
             == f"""\
 Wheel-Version: 1.0
 Generator: poetry-core {__version__}
 Root-Is-Purelib: true
 Tag: py3-none-any
 """
         )
-        wheel_data = zip.read("my_package-1.2.3.dist-info/METADATA").decode()
+        wheel_data = zipf.read("my_package-1.2.3.dist-info/METADATA").decode()
 
         assert (
             wheel_data
             == """\
 Metadata-Version: 2.1
 Name: my-package
 Version: 1.2.3
@@ -401,27 +196,33 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: time
 Requires-Dist: cachy[msgpack] (>=0.2.0,<0.3.0)
 Requires-Dist: cleo (>=0.6,<0.7)
-Requires-Dist: pendulum (>=1.4,<2.0) ; (python_version ~= "2.7" and sys_platform == "win32" or python_version in "3.4 3.5") and (extra == "time")
+Requires-Dist: pendulum (>=1.4,<2.0) ; (python_version ~= "2.7"\
+ and sys_platform == "win32" or python_version in "3.4 3.5") and (extra == "time")
 Project-URL: Documentation, https://python-poetry.org/docs
 Project-URL: Issue Tracker, https://github.com/python-poetry/poetry/issues
 Project-URL: Repository, https://github.com/python-poetry/poetry
 Description-Content-Type: text/x-rst
 
 My Package
 ==========
 
 """
         )
-    finally:
-        zip.close()
+        actual_records = zipf.read("my_package-1.2.3.dist-info/RECORD").decode()
+
+        # The SHA hashes vary per operating systems.
+        # So instead of 1:1 assertion, let's do a bit clunkier one:
+        actual_files = [row[0] for row in csv.reader(actual_records.splitlines())]
+
+        assert actual_files == expected_name_list
 
 
 def test_module_src() -> None:
     module_path = fixtures_dir / "source_file"
     builder = Builder(Factory().create_poetry(module_path))
     builder.build(fmt="all")
 
@@ -432,20 +233,16 @@
     with tarfile.open(str(sdist), "r") as tar:
         assert "module_src-0.1/src/module_src.py" in tar.getnames()
 
     whl = module_path / "dist" / "module_src-0.1-py2.py3-none-any.whl"
 
     assert whl.exists()
 
-    zip = zipfile.ZipFile(str(whl))
-
-    try:
-        assert "module_src.py" in zip.namelist()
-    finally:
-        zip.close()
+    with zipfile.ZipFile(str(whl)) as zipf:
+        assert "module_src.py" in zipf.namelist()
 
 
 def test_package_src() -> None:
     module_path = fixtures_dir / "source_package"
     builder = Builder(Factory().create_poetry(module_path))
     builder.build(fmt="all")
 
@@ -456,21 +253,17 @@
     with tarfile.open(str(sdist), "r") as tar:
         assert "package_src-0.1/src/package_src/module.py" in tar.getnames()
 
     whl = module_path / "dist" / "package_src-0.1-py2.py3-none-any.whl"
 
     assert whl.exists()
 
-    zip = zipfile.ZipFile(str(whl))
-
-    try:
-        assert "package_src/__init__.py" in zip.namelist()
-        assert "package_src/module.py" in zip.namelist()
-    finally:
-        zip.close()
+    with zipfile.ZipFile(str(whl)) as zipf:
+        assert "package_src/__init__.py" in zipf.namelist()
+        assert "package_src/module.py" in zipf.namelist()
 
 
 def test_split_source() -> None:
     module_path = fixtures_dir / "split_source"
     builder = Builder(Factory().create_poetry(module_path))
     builder.build(fmt="all")
 
@@ -482,21 +275,17 @@
         assert "split_source-0.1/lib_a/module_a/__init__.py" in tar.getnames()
         assert "split_source-0.1/lib_b/module_b/__init__.py" in tar.getnames()
 
     whl = module_path / "dist" / "split_source-0.1-py3-none-any.whl"
 
     assert whl.exists()
 
-    zip = zipfile.ZipFile(str(whl))
-
-    try:
-        assert "module_a/__init__.py" in zip.namelist()
-        assert "module_b/__init__.py" in zip.namelist()
-    finally:
-        zip.close()
+    with zipfile.ZipFile(str(whl)) as zipf:
+        assert "module_a/__init__.py" in zipf.namelist()
+        assert "module_b/__init__.py" in zipf.namelist()
 
 
 def test_package_with_include(mocker: MockerFixture) -> None:
     module_path = fixtures_dir / "with-include"
 
     # Patch git module to return specific excluded files
     p = mocker.patch("poetry.core.vcs.git.Git.get_ignored_files")
```

### Comparing `poetry_core-1.5.1/tests/masonry/builders/test_sdist.py` & `poetry_core-1.5.2/tests/masonry/builders/test_sdist.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/builders/test_wheel.py` & `poetry_core-1.5.2/tests/masonry/builders/test_wheel.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/test_api.py` & `poetry_core-1.5.2/tests/masonry/test_api.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/test_builder.py` & `poetry_core-1.5.2/tests/masonry/test_builder.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/utils/test_helpers.py` & `poetry_core-1.5.2/tests/masonry/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/masonry/utils/test_package_include.py` & `poetry_core-1.5.2/tests/masonry/utils/test_package_include.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_dependency.py` & `poetry_core-1.5.2/tests/packages/test_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_dependency_group.py` & `poetry_core-1.5.2/tests/packages/test_dependency_group.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_directory_dependency.py` & `poetry_core-1.5.2/tests/packages/test_directory_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_file_dependency.py` & `poetry_core-1.5.2/tests/packages/test_file_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_main.py` & `poetry_core-1.5.2/tests/packages/test_main.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_package.py` & `poetry_core-1.5.2/tests/packages/test_package.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_specification.py` & `poetry_core-1.5.2/tests/packages/test_specification.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_url_dependency.py` & `poetry_core-1.5.2/tests/packages/test_url_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/test_vcs_dependency.py` & `poetry_core-1.5.2/tests/packages/test_vcs_dependency.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/utils/test_utils.py` & `poetry_core-1.5.2/tests/packages/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/packages/utils/test_utils_link.py` & `poetry_core-1.5.2/tests/packages/utils/test_utils_link.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,18 @@
 
 
 def make_url(
     ext: str, file_checksum: str | None = None, metadata_checksum: str | None = None
 ) -> Link:
     file_checksum = file_checksum or make_checksum()
     return Link(
-        "https://files.pythonhosted.org/packages/16/52/dead/"
-        f"demo-1.0.0.{ext}#sha256={file_checksum}",
+        (
+            "https://files.pythonhosted.org/packages/16/52/dead/"
+            f"demo-1.0.0.{ext}#sha256={file_checksum}"
+        ),
         metadata=f"sha256={metadata_checksum}" if metadata_checksum else None,
     )
 
 
 def test_package_link_hash(file_checksum: str) -> None:
     link = make_url(ext="whl", file_checksum=file_checksum)
     assert link.hash_name == "sha256"
@@ -100,16 +102,18 @@
         ("", False),
     ],
 )
 def test_package_link_pep653_non_hash_metadata_value(
     file_checksum: str, metadata: str | bool, has_metadata: bool
 ) -> None:
     link = Link(
-        "https://files.pythonhosted.org/packages/16/52/dead/"
-        f"demo-1.0.0.whl#sha256={file_checksum}",
+        (
+            "https://files.pythonhosted.org/packages/16/52/dead/"
+            f"demo-1.0.0.whl#sha256={file_checksum}"
+        ),
         metadata=metadata,
     )
 
     if has_metadata:
         assert link.has_metadata
         assert link.metadata_url == f"{link.url_without_fragment}.metadata"
     else:
```

### Comparing `poetry_core-1.5.1/tests/packages/utils/test_utils_urls.py` & `poetry_core-1.5.2/tests/packages/utils/test_utils_urls.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/pyproject/conftest.py` & `poetry_core-1.5.2/tests/pyproject/conftest.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/pyproject/test_pyproject_toml.py` & `poetry_core-1.5.2/tests/pyproject/test_pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/pyproject/test_pyproject_toml_file.py` & `poetry_core-1.5.2/tests/pyproject/test_pyproject_toml_file.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/spdx/test_helpers.py` & `poetry_core-1.5.2/tests/spdx/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/spdx/test_license.py` & `poetry_core-1.5.2/tests/spdx/test_license.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/test_factory.py` & `poetry_core-1.5.2/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/testutils.py` & `poetry_core-1.5.2/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/utils/test_helpers.py` & `poetry_core-1.5.2/tests/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/vcs/test_vcs.py` & `poetry_core-1.5.2/tests/vcs/test_vcs.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/version/pep440/test_segments.py` & `poetry_core-1.5.2/tests/version/pep440/test_segments.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/version/pep440/test_version.py` & `poetry_core-1.5.2/tests/version/pep440/test_version.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/tests/version/test_markers.py` & `poetry_core-1.5.2/tests/version/test_markers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1612,16 +1612,18 @@
         str(dnf(intersection(*markers).invert()))
         == 'platform_system == "Darwin" and platform_machine == "arm64"'
         ' and python_version >= "3.6" or python_version >= "3.10"'
     )
 
 
 @pytest.mark.parametrize(
-    "python_version, python_full_version, "
-    "expected_intersection_version, expected_union_version",
+    (
+        "python_version, python_full_version, "
+        "expected_intersection_version, expected_union_version"
+    ),
     [
         # python_version > 3.6 (equal to python_full_version >= 3.7.0)
         ('> "3.6"', '> "3.5.2"', '> "3.6"', '> "3.5.2"'),
         ('> "3.6"', '>= "3.5.2"', '> "3.6"', '>= "3.5.2"'),
         ('> "3.6"', '> "3.6.2"', '> "3.6"', '> "3.6.2"'),
         ('> "3.6"', '>= "3.6.2"', '> "3.6"', '>= "3.6.2"'),
         ('> "3.6"', '> "3.7.0"', '> "3.7.0"', '> "3.6"'),
```

### Comparing `poetry_core-1.5.1/tests/version/test_requirements.py` & `poetry_core-1.5.2/tests/version/test_requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_core-1.5.1/PKG-INFO` & `poetry_core-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-core
-Version: 1.5.1
+Version: 1.5.2
 Summary: Poetry PEP 517 Build Backend
 Home-page: https://github.com/python-poetry/poetry-core
 License: MIT
 Keywords: packaging,dependency,poetry
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Requires-Python: >=3.7,<4.0
```

