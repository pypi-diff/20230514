# Comparing `tmp/requests-mock-flask-2023.3.5.1.tar.gz` & `tmp/requests-mock-flask-2023.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests-mock-flask-2023.3.5.1.tar", last modified: Sun Mar  5 17:42:02 2023, max compression
+gzip compressed data, was "requests-mock-flask-2023.5.14.tar", last modified: Sun May 14 14:01:22 2023, max compression
```

## Comparing `requests-mock-flask-2023.3.5.1.tar` & `requests-mock-flask-2023.5.14.tar`

### file list

```diff
@@ -1,51 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.213890 requests-mock-flask-2023.3.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-05 17:41:42.000000 requests-mock-flask-2023.3.5.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/docs/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/docs/source/api-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/docs/source/changelog.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2159 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/docs/source/release-process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/lint.mk
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/requirements/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/requirements/setup-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/spelling_private_dict.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.213890 requests-mock-flask-2023.3.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/src/requests_mock_flask/
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/src/requests_mock_flask/_type_check_imports/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask/_type_check_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-03-05 17:42:02.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-05 17:42:02.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 17:42:02.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 17:42:02.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-05 17:42:02.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-05 17:42:02.000000 requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:42:02.217890 requests-mock-flask-2023.3.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29108 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/tests/test_requests_mock_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-03-05 17:41:39.000000 requests-mock-flask-2023.3.5.1/tests/test_usage_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.233736 requests-mock-flask-2023.5.14/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.229736 requests-mock-flask-2023.5.14/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.229736 requests-mock-flask-2023.5.14/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.229736 requests-mock-flask-2023.5.14/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-14 14:01:08.000000 requests-mock-flask-2023.5.14/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-14 14:01:22.233736 requests-mock-flask-2023.5.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.229736 requests-mock-flask-2023.5.14/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.229736 requests-mock-flask-2023.5.14/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/docs/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/docs/source/api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/docs/source/changelog.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2142 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/docs/source/release-process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/lint.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:01:22.233736 requests-mock-flask-2023.5.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/spelling_private_dict.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.229736 requests-mock-flask-2023.5.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.229736 requests-mock-flask-2023.5.14/src/requests_mock_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.233736 requests-mock-flask-2023.5.14/src/requests_mock_flask/_type_check_imports/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask/_type_check_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.233736 requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-14 14:01:22.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-14 14:01:22.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:01:22.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:01:21.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-14 14:01:22.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-14 14:01:22.000000 requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:01:22.233736 requests-mock-flask-2023.5.14/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30397 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/tests/test_requests_mock_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-14 14:01:06.000000 requests-mock-flask-2023.5.14/tests/test_usage_patterns.py
```

### Comparing `requests-mock-flask-2023.3.5.1/.github/workflows/ci.yml` & `requests-mock-flask-2023.5.14/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -27,18 +27,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - uses: actions/cache@v3
         with:
           path: ~/.cache/pip
-          # This is like the example but we use ``*requirements.txt`` rather
-          # than ``requirements.txt`` because we have multiple requirements
-          # files.
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/*requirements.txt') }}
+          key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             ${{ runner.os }}-pip-
 
       - name: "Install dependencies"
         run: |
           python -m pip install --upgrade pip setuptools wheel
           # We use '--ignore-installed' to avoid GitHub's cache which can cause
@@ -48,11 +45,13 @@
 
       - name: "Lint"
         run: |
           make lint
 
       - name: "Run tests"
         run: |
-          pytest -s -vvv --cov-fail-under 100 --cov=src/ --cov=tests tests/ --cov-report=xml
+          # We run tests against "." and not the tests directory as we test the README
+          # and documentation.
+          pytest -s -vvv --cov-fail-under 100 --cov=src/ --cov=tests . --cov-report=xml
 
       - name: "Upload coverage to Codecov"
         uses: "codecov/codecov-action@v3"
```

### Comparing `requests-mock-flask-2023.3.5.1/.github/workflows/release.yml` & `requests-mock-flask-2023.5.14/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `requests-mock-flask-2023.3.5.1/.gitignore` & `requests-mock-flask-2023.5.14/.gitignore`

 * *Files identical despite different names*

### Comparing `requests-mock-flask-2023.3.5.1/CHANGELOG.rst` & `requests-mock-flask-2023.5.14/CHANGELOG.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Changelog
 =========
 
 Next
 ----
 
+2023.05.14
+------------
+
 2023.03.05.1
 ------------
 
 2023.03.05
 ------------
 
 2022.04.03
```

### Comparing `requests-mock-flask-2023.3.5.1/LICENSE` & `requests-mock-flask-2023.5.14/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-mock-flask-2023.3.5.1/Makefile` & `requests-mock-flask-2023.5.14/Makefile`

 * *Files identical despite different names*

### Comparing `requests-mock-flask-2023.3.5.1/PKG-INFO` & `requests-mock-flask-2023.5.14/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-mock-flask
-Version: 2023.3.5.1
+Version: 2023.5.14
 Summary: Helpers to use requests_mock and responses with a Flask test client.
 Author-email: Adam Dangoor <adamdangoor@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Adam Dangoor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,15 +66,15 @@
    import flask
    import requests
    import responses
    import requests_mock
 
    from requests_mock_flask import add_flask_app_to_mock
 
-   app = flask.Flask(__name__)
+   app = flask.Flask("test_app")
 
    @app.route('/')
    def _() -> str:
        return 'Hello, World!'
 
    @responses.activate
    def test_responses_decorator() -> None:
@@ -125,15 +125,15 @@
            response = requests.get('http://www.example.com')
 
        assert response.status_code == 200
        assert response.text == 'Hello, World!'
 
    def test_requests_mock_adapter() -> None:
        """
-       It is possible to use the helper with a ``requests_mock`` adapter.
+       It is possible to use the helper with a ``requests_mock`` fixture.
        """
        session = requests.Session()
        adapter = requests_mock.Adapter()
        session.mount('mock', adapter)
 
        add_flask_app_to_mock(
            mock_obj=adapter,
@@ -142,29 +142,28 @@
        )
 
        response = session.get('mock://www.example.com')
 
        assert response.status_code == 200
        assert response.text == 'Hello, World!'
 
-   @httpretty.activate
-   def test_httpretty_decorator() -> None:
-       """
-       It is possible to use the helper with HTTPretty.
-       """
-       add_flask_app_to_mock(
-           mock_obj=httpretty,
-           flask_app=app,
-           base_url='http://www.example.com',
-       )
+.. -> test_src
 
-       response = requests.get('http://www.example.com')
+.. invisible-code-block: python
 
-       assert response.status_code == 200
-       assert response.text == 'Hello, World!'
+   import pathlib
+   import subprocess
+   import tempfile
+
+   import pytest
+
+   with tempfile.TemporaryDirectory() as tmp_dir:
+       test_file = pathlib.Path(tmp_dir) / 'test_src.py'
+       test_file.write_text(test_src)
+       subprocess.check_output(["python", "-m", "pytest", test_file, "--basetemp", test_file.parent])
 
 
 Use cases
 ---------
 
 * Use ``requests`` or other Python APIs for testing Flask applications.
 * Create a test suite which can test a Flask application as well as a live web application, to make a verified fake.
```

### Comparing `requests-mock-flask-2023.3.5.1/README.rst` & `requests-mock-flask-2023.5.14/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -26,15 +26,15 @@
    import flask
    import requests
    import responses
    import requests_mock
 
    from requests_mock_flask import add_flask_app_to_mock
 
-   app = flask.Flask(__name__)
+   app = flask.Flask("test_app")
 
    @app.route('/')
    def _() -> str:
        return 'Hello, World!'
 
    @responses.activate
    def test_responses_decorator() -> None:
@@ -85,15 +85,15 @@
            response = requests.get('http://www.example.com')
 
        assert response.status_code == 200
        assert response.text == 'Hello, World!'
 
    def test_requests_mock_adapter() -> None:
        """
-       It is possible to use the helper with a ``requests_mock`` adapter.
+       It is possible to use the helper with a ``requests_mock`` fixture.
        """
        session = requests.Session()
        adapter = requests_mock.Adapter()
        session.mount('mock', adapter)
 
        add_flask_app_to_mock(
            mock_obj=adapter,
@@ -102,29 +102,28 @@
        )
 
        response = session.get('mock://www.example.com')
 
        assert response.status_code == 200
        assert response.text == 'Hello, World!'
 
-   @httpretty.activate
-   def test_httpretty_decorator() -> None:
-       """
-       It is possible to use the helper with HTTPretty.
-       """
-       add_flask_app_to_mock(
-           mock_obj=httpretty,
-           flask_app=app,
-           base_url='http://www.example.com',
-       )
+.. -> test_src
 
-       response = requests.get('http://www.example.com')
+.. invisible-code-block: python
 
-       assert response.status_code == 200
-       assert response.text == 'Hello, World!'
+   import pathlib
+   import subprocess
+   import tempfile
+
+   import pytest
+
+   with tempfile.TemporaryDirectory() as tmp_dir:
+       test_file = pathlib.Path(tmp_dir) / 'test_src.py'
+       test_file.write_text(test_src)
+       subprocess.check_output(["python", "-m", "pytest", test_file, "--basetemp", test_file.parent])
 
 
 Use cases
 ---------
 
 * Use ``requests`` or other Python APIs for testing Flask applications.
 * Create a test suite which can test a Flask application as well as a live web application, to make a verified fake.
```

### Comparing `requests-mock-flask-2023.3.5.1/docs/Makefile` & `requests-mock-flask-2023.5.14/docs/Makefile`

 * *Files identical despite different names*

### Comparing `requests-mock-flask-2023.3.5.1/docs/source/conf.py` & `requests-mock-flask-2023.5.14/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 """
 Configuration for Sphinx.
 """
 
 import datetime
-
-from pkg_resources import get_distribution
+import importlib.metadata
 
 # pylint: disable=invalid-name
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
@@ -20,26 +19,25 @@
 
 project = "requests-mock-flask"
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # General information about the project.
-project = "Requests-Mock-Flask"
 year = datetime.datetime.now(tz=datetime.UTC).year
 author = "Adam Dangoor"
 project_copyright = f"{year}, {author}"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# Use ``pkg_resources`` as per
+# Use ``importlib.metadata.version`` as per
 # https://github.com/pypa/setuptools_scm#usage-from-sphinx.
-version = get_distribution(project).version
+version = importlib.metadata.version(distribution_name=project)
 _month, _day, _year, *_ = version.split(".")
 release = f"{_month}.{_day}.{_year}"
 
 html_theme = "furo"
 html_title = project
 html_show_copyright = False
 html_show_sphinx = False
```

### Comparing `requests-mock-flask-2023.3.5.1/docs/source/contributing.rst` & `requests-mock-flask-2023.5.14/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `requests-mock-flask-2023.3.5.1/lint.mk` & `requests-mock-flask-2023.5.14/lint.mk`

 * *Files 14% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
 .PHONY: fix-ruff
 fix-ruff:
 	ruff --fix .
 
 .PHONY: pip-extra-reqs
 pip-extra-reqs:
-	pip-extra-reqs --requirements-file=requirements/requirements.txt src/
+	pip-extra-reqs --requirements-file=<(pdm export --pyproject) src/
 
 .PHONY: pip-missing-reqs
 pip-missing-reqs:
 	pip-missing-reqs \
-		--requirements-file=requirements/requirements.txt \
+		--requirements-file=<(pdm export --pyproject) \
 		--ignore-file=src/requests_mock_flask/_type_check_imports/__init__.py \
 		src/
 
 .PHONY: pylint
 pylint:
 	pylint *.py src/ tests/ docs/
```

### Comparing `requests-mock-flask-2023.3.5.1/pyproject.toml` & `requests-mock-flask-2023.5.14/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -102,43 +102,44 @@
 xfail_strict = true
 log_cli = true
 
 [tool.check-manifest]
 
 ignore = [
   "*.enc",
+  ".vscode/*.json",
   "readthedocs.yaml",
+  "conftest.py",
   "CHANGELOG.rst",
   "CODE_OF_CONDUCT.rst",
   "CONTRIBUTING.rst",
   "LICENSE",
   "Makefile",
   "ci",
   "ci/**",
   "codecov.yaml",
   "docs",
   "docs/**",
   ".git_archival.txt",
   "spelling_private_dict.txt",
   "tests",
-  "tests-pylintrc",
   "tests/**",
-  "vuforia_secrets.env.example",
   "lint.mk",
 ]
 
 [tool.mypy]
 
 strict = true
 
 [[tool.mypy.overrides]]
 
 module = [
-    "flask_negotiate",
     "httpretty",
+    "sybil",
+    "sybil.parsers.rest",
 ]
 
 ignore_missing_imports = true
 
 
 [tool.doc8]
 
@@ -149,15 +150,21 @@
     "./docs/build/spelling/output.txt",
     "./node_modules",
     "./src/*.egg-info/",
     "./src/*/_setuptools_scm_version.txt",
 ]
 
 [build-system]
-requires = ["setuptools", "pip", "wheel"]
+requires = [
+     "pip",
+     "setuptools",
+     "setuptools-scm-git-archive==1.4",
+     "setuptools_scm[toml]==7.1.0",
+     "wheel",
+ ]
 build-backend = "setuptools.build_meta"
 
 [tool.ruff]
 select = ["ALL"]
 
 ignore = [
     # We do not annotate the type of 'self'.
@@ -175,32 +182,23 @@
     "D301",
     # It is too much work to make every docstring imperative.
     "D401",
     # We ignore some docstyle errors which do not apply to Google style
     # docstrings.
     "D406",
     "D407",
-    # We have an existing interface to support and so we do not want to change
-    # exception names.
-    "N818",
-    # Ignore "too-many-*" errors as they seem to get in the way more than
-    # helping.
-    "PLR0912",
-    "PLR0913",
     # Allow 'assert' as we use it for tests.
     "S101",
-    # Allow imports which are only used for type checking to be outside type
-    # checking blocks.
-    "TCH002",
-    "TCH003",
-    # We use quoted annotations so that we can use types from packages which
-    # may not be installed.
-    "UP037",
 ]
 
+# Do not automatically remove commented out code.
+# We comment out code during development, and with VSCode auto-save, this code
+# is sometimes annoyingly removed.
+unfixable = ["ERA001"]
+
 [tool.ruff.per-file-ignores]
 "tests/test_*.py" = [
     # Do not require tests to have a one-line summary.
     "D205",
 ]
 
 [tool.distutils.bdist_wheel]
@@ -219,20 +217,50 @@
 description = "Helpers to use requests_mock and responses with a Flask test client."
 dynamic = ["version"]
 keywords = ["requests", "mock", "flask"]
 license = { file = "LICENSE" }
 name = "requests-mock-flask"
 readme = { file = "README.rst", content-type = "text/x-rst"}
 requires-python = ">=3.10"
+dependencies = ["Werkzeug>=2.3.0"]
+
+[project.optional-dependencies]
+dev = [
+    "Flask==2.3.2",
+    "Sphinx-Substitution-Extensions==2022.2.16",
+    "black==23.3.0",
+    "check-manifest==0.49",
+    "doc8==1.1.1",
+    "furo==2023.3.27",
+    "httpretty==1.1.4",
+    "mypy==1.3.0",
+    "pdm==2.6.1",
+    "pip_check_reqs==2.4.4",
+    "pylint==2.17.4",
+    "pyroma==4.2",
+    "pytest-cov==4.0.0",
+    "pytest==7.3.1",
+    "requests-mock==1.10.0",
+    "requests==2.30.0",
+    "responses==0.23.1",
+    "ruff==0.0.267",
+    "sphinx-autodoc-typehints==1.23.0",
+    "sphinx-prompt==1.5.0",
+    "sphinxcontrib.spelling==8.0.0",
+    "sybil==5.0.1",
+    "types-requests==2.30.0.0",
+    "vulture==2.7",
+]
 
 [project.urls]
 Source = "https://github.com/adamtheturtle/requests-mock-flask"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 requests_mock_flask = ["py.typed"]
 
+[tool.setuptools_scm]
```

### Comparing `requests-mock-flask-2023.3.5.1/src/requests_mock_flask/__init__.py` & `requests-mock-flask-2023.5.14/src/requests_mock_flask/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,63 +24,63 @@
     HTTPRETTY = auto()
 
 
 def add_flask_app_to_mock(
     # We allow an `Any` type here, as we do not want to add all mocker types
     # as requirements.
     mock_obj: Any,  # noqa: ANN401
-    flask_app: "flask.Flask",
+    flask_app: flask.Flask,
     base_url: str,
 ) -> None:
     """
     Make it so that requests sent to the ``base_url`` are forwarded to the
     ``Flask`` app, when in the context of the ``mock_obj``.
     """
     # We use hasattr here rather than checking the type of ``mock_obj``.
     #
     # This is so that we do not need to add responses etc. as requirements.
     if hasattr(mock_obj, "add_callback"):
         mock_obj_type = _MockObjTypes.RESPONSES
 
         def responses_callback(
-            request: "requests.PreparedRequest",
+            request: requests.PreparedRequest,
         ) -> tuple[int, dict[str, str | int | bool | None], bytes]:
             return _responses_callback(request=request, flask_app=flask_app)
 
     elif hasattr(mock_obj, "request_history"):
         mock_obj_type = _MockObjTypes.REQUESTS_MOCK
 
         def requests_mock_callback(
             # We ignore SLF001 here, as we prefer to have this typed with
             # private types than to have it untyped.
-            request: "requests_mock.request._RequestObjectProxy",  # noqa: SLF001
-            context: "requests_mock.response._Context",  # noqa: SLF001
+            request: requests_mock.request._RequestObjectProxy,  # noqa: SLF001
+            context: requests_mock.response._Context,  # noqa: SLF001
         ) -> str:
             return _requests_mock_callback(
                 request=request,
                 context=context,
                 flask_app=flask_app,
             )
 
     elif hasattr(mock_obj, "HTTPretty"):
         mock_obj_type = _MockObjTypes.HTTPRETTY
 
         def httpretty_callback(
-            request: "httpretty.HTTPrettyRequest",
+            request: httpretty.HTTPrettyRequest,
             uri: str,
             headers: dict[str, Any],
         ) -> tuple[int, dict[str, str | int | bool | None], bytes]:
             return _httpretty_callback(
                 request=request,
                 uri=uri,
                 headers=headers,
                 flask_app=flask_app,
             )
 
-    else:  # pragma: no cover
+    else:
         message = (
             "Expected a HTTPretty, ``requests_mock``, or ``responses`` "
             f"object, got {type(mock_obj)}."
         )
         raise TypeError(message)
 
     for rule in flask_app.url_map.iter_rules():
@@ -111,16 +111,16 @@
                     body=httpretty_callback,
                 )
             else:  # pragma: no cover
                 pass
 
 
 def _responses_callback(
-    request: "requests.PreparedRequest",
-    flask_app: "flask.Flask",
+    request: requests.PreparedRequest,
+    flask_app: flask.Flask,
 ) -> tuple[int, dict[str, str | int | bool | None], bytes]:
     """
     Given a request to the flask app, send an equivalent request to an in
     memory fake of the flask app and return some key details of the
     response.
 
     :param request: The incoming request to pass onto the flask app.
@@ -138,15 +138,15 @@
         list(parse_cookie(cookie).items())[0]
         for cookie in cookie_list_no_empty
     ]
     cookies_dict = dict(request_cookies)
 
     for key, value in cookies_dict.items():
         test_client.set_cookie(
-            server_name="",
+            domain="localhost",
             key=key,
             value=value,
         )
 
     environ_overrides = {}
     if "Content-Length" in request.headers:
         environ_overrides["CONTENT_LENGTH"] = request.headers["Content-Length"]
@@ -165,18 +165,18 @@
     result_headers: dict[str, str | int | bool | None] = dict(
         response.headers,
     )
     return (response.status_code, result_headers, bytes(response.data))
 
 
 def _httpretty_callback(
-    request: "httpretty.HTTPrettyRequest",
+    request: httpretty.HTTPrettyRequest,
     uri: str,
     headers: dict[str, Any],
-    flask_app: "flask.Flask",
+    flask_app: flask.Flask,
 ) -> tuple[int, dict[str, str | int | bool | None], bytes]:
     # We make this assertion to satisfy linters.
     # The parameters are given to httpretty callbacks, but we do not use them.
     assert [uri, headers]
 
     test_client = flask_app.test_client()
     # See parameters at
@@ -188,15 +188,15 @@
         list(parse_cookie(cookie).items())[0]
         for cookie in cookie_list_no_empty
     ]
     cookies_dict = dict(request_cookies)
 
     for key, value in cookies_dict.items():
         test_client.set_cookie(
-            server_name="",
+            domain=request.host,
             key=key,
             value=value,
         )
 
     environ_overrides = {}
     if "Content-Length" in request.headers:
         environ_overrides["CONTENT_LENGTH"] = request.headers["Content-Length"]
@@ -214,17 +214,17 @@
     )
     return (response.status_code, result_headers, response.data)
 
 
 def _requests_mock_callback(
     # We ignore SLF001 here, as we prefer to have this typed with
     # private types than to have it untyped.
-    request: "requests_mock.request._RequestObjectProxy",  # noqa: SLF001
-    context: "requests_mock.response._Context",  # noqa: SLF001
-    flask_app: "flask.Flask",
+    request: requests_mock.request._RequestObjectProxy,  # noqa: SLF001
+    context: requests_mock.response._Context,  # noqa: SLF001
+    flask_app: flask.Flask,
 ) -> str:
     """
     Given a request to the flask app, send an equivalent request to an in
     memory fake of the flask app and return some key details of the
     response.
 
     :param request: The incoming request to pass onto the flask app.
@@ -244,15 +244,15 @@
         list(parse_cookie(cookie).items())[0]
         for cookie in cookie_list_no_empty
     ]
     cookies_dict = dict(request_cookies)
 
     for key, value in cookies_dict.items():
         test_client.set_cookie(
-            server_name="",
+            domain="localhost",
             key=key,
             value=value,
         )
 
     environ_overrides = {}
     if "Content-Length" in request.headers:
         environ_overrides["CONTENT_LENGTH"] = request.headers["Content-Length"]
```

### Comparing `requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/PKG-INFO` & `requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-mock-flask
-Version: 2023.3.5.1
+Version: 2023.5.14
 Summary: Helpers to use requests_mock and responses with a Flask test client.
 Author-email: Adam Dangoor <adamdangoor@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Adam Dangoor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -66,15 +66,15 @@
    import flask
    import requests
    import responses
    import requests_mock
 
    from requests_mock_flask import add_flask_app_to_mock
 
-   app = flask.Flask(__name__)
+   app = flask.Flask("test_app")
 
    @app.route('/')
    def _() -> str:
        return 'Hello, World!'
 
    @responses.activate
    def test_responses_decorator() -> None:
@@ -125,15 +125,15 @@
            response = requests.get('http://www.example.com')
 
        assert response.status_code == 200
        assert response.text == 'Hello, World!'
 
    def test_requests_mock_adapter() -> None:
        """
-       It is possible to use the helper with a ``requests_mock`` adapter.
+       It is possible to use the helper with a ``requests_mock`` fixture.
        """
        session = requests.Session()
        adapter = requests_mock.Adapter()
        session.mount('mock', adapter)
 
        add_flask_app_to_mock(
            mock_obj=adapter,
@@ -142,29 +142,28 @@
        )
 
        response = session.get('mock://www.example.com')
 
        assert response.status_code == 200
        assert response.text == 'Hello, World!'
 
-   @httpretty.activate
-   def test_httpretty_decorator() -> None:
-       """
-       It is possible to use the helper with HTTPretty.
-       """
-       add_flask_app_to_mock(
-           mock_obj=httpretty,
-           flask_app=app,
-           base_url='http://www.example.com',
-       )
+.. -> test_src
 
-       response = requests.get('http://www.example.com')
+.. invisible-code-block: python
 
-       assert response.status_code == 200
-       assert response.text == 'Hello, World!'
+   import pathlib
+   import subprocess
+   import tempfile
+
+   import pytest
+
+   with tempfile.TemporaryDirectory() as tmp_dir:
+       test_file = pathlib.Path(tmp_dir) / 'test_src.py'
+       test_file.write_text(test_src)
+       subprocess.check_output(["python", "-m", "pytest", test_file, "--basetemp", test_file.parent])
 
 
 Use cases
 ---------
 
 * Use ``requests`` or other Python APIs for testing Flask applications.
 * Create a test suite which can test a Flask application as well as a live web application, to make a verified fake.
```

### Comparing `requests-mock-flask-2023.3.5.1/src/requests_mock_flask.egg-info/SOURCES.txt` & `requests-mock-flask-2023.5.14/src/requests_mock_flask.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 .gitattributes
 .gitignore
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
+conftest.py
 lint.mk
 pyproject.toml
 readthedocs.yaml
-setup.py
 spelling_private_dict.txt
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/release.yml
+.vscode/extensions.json
+.vscode/settings.json
 docs/Makefile
 docs/source/__init__.py
 docs/source/api-reference.rst
 docs/source/changelog.rst
 docs/source/conf.py
 docs/source/contributing.rst
 docs/source/index.rst
 docs/source/release-process.rst
-requirements/dev-requirements.txt
-requirements/requirements.txt
-requirements/setup-requirements.txt
 src/requests_mock_flask/__init__.py
 src/requests_mock_flask/py.typed
 src/requests_mock_flask.egg-info/PKG-INFO
 src/requests_mock_flask.egg-info/SOURCES.txt
 src/requests_mock_flask.egg-info/dependency_links.txt
 src/requests_mock_flask.egg-info/not-zip-safe
 src/requests_mock_flask.egg-info/requires.txt
```

### Comparing `requests-mock-flask-2023.3.5.1/tests/test_requests_mock_flask.py` & `requests-mock-flask-2023.5.14/tests/test_requests_mock_flask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 """
 Tests for the ``requests_mock_flask`` package.
 
 Test with a bunch of route types as per:
 https://flask.palletsprojects.com/en/1.1.x/quickstart/#variable-rules
 """
 
+from __future__ import annotations
+
 import json
 import uuid
-from collections.abc import Iterator
 from contextlib import contextmanager
 from functools import partial
+from typing import TYPE_CHECKING, Final
 
 import httpretty
 import pytest
 import requests
 import requests_mock
 import responses
 import werkzeug
 from flask import Flask, Response, jsonify, make_response, request
-from flask_negotiate import consumes
 from requests_mock_flask import add_flask_app_to_mock
 
+if TYPE_CHECKING:
+    from collections.abc import Iterator
+
+# We use a high timeout to allow interactive debugging while requests are being
+# made.
+_TIMEOUT_SECONDS: Final[int] = 120
+
 
 @contextmanager
 def httpretty_context_manager() -> Iterator[type[httpretty]]:
     """
     Context manager for httpretty.
     """
     httpretty.enable()
@@ -69,15 +77,18 @@
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        mock_response = requests.get("http://www.example.com", timeout=1)
+        mock_response = requests.get(
+            url="http://www.example.com",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
 @pytest.mark.parametrize("mock_ctx", _MOCK_CTXS)
@@ -110,15 +121,15 @@
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com",
             headers={"hello": "world"},
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -147,15 +158,18 @@
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        mock_response = requests.get("http://www.example.com", timeout=1)
+        mock_response = requests.get(
+            "http://www.example.com",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.json() == expected_json
 
 
 @pytest.mark.parametrize("mock_ctx", _MOCK_CTXS)
@@ -185,15 +199,15 @@
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com/Frasier",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -224,15 +238,15 @@
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com/Frasier",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -261,15 +275,18 @@
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        mock_response = requests.get("http://www.example.com/4", timeout=1)
+        mock_response = requests.get(
+            "http://www.example.com/4",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
 @pytest.mark.parametrize("mock_ctx", _MOCK_CTXS)
@@ -297,15 +314,18 @@
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        mock_response = requests.get("http://www.example.com/4.0", timeout=1)
+        mock_response = requests.get(
+            "http://www.example.com/4.0",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
 @pytest.mark.parametrize("mock_ctx", _MOCK_CTXS)
@@ -335,15 +355,15 @@
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com/foo/bar",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -373,15 +393,15 @@
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com/foo/bar",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert "not found on the server" in mock_response.text
 
 
@@ -413,15 +433,15 @@
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             f"http://www.example.com/{random_uuid}",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -452,15 +472,15 @@
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com/users/4/posts",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -491,15 +511,15 @@
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com/users/cranes/frasier/posts",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -528,15 +548,18 @@
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        mock_response = requests.post("http://www.example.com/", timeout=1)
+        mock_response = requests.post(
+            "http://www.example.com/",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
 @pytest.mark.parametrize("custom_content_length", ["1", "100"])
@@ -622,18 +645,21 @@
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        mock_get_response = requests.get("http://www.example.com/", timeout=1)
+        mock_get_response = requests.get(
+            "http://www.example.com/",
+            timeout=_TIMEOUT_SECONDS,
+        )
         mock_post_response = requests.post(
             "http://www.example.com/",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_get_response.status_code == expected_status_code
     assert mock_get_response.headers["Content-Type"] == expected_content_type
     assert mock_get_response.text == expected_data.decode()
 
     assert mock_post_response.status_code == expected_status_code
@@ -665,15 +691,18 @@
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        mock_response = requests.get("http://www.example.com/a", timeout=1)
+        mock_response = requests.get(
+            "http://www.example.com/a",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert "not found on the server" in mock_response.text
 
 
 @pytest.mark.parametrize("mock_ctx", _MOCK_CTXS)
@@ -707,27 +736,27 @@
         with pytest.raises(
             expected_exception=(
                 requests.exceptions.ConnectionError,
                 requests_mock.exceptions.NoMockAddress,
                 ValueError,
             ),
         ):
-            requests.post("http://www.example.com/", timeout=1)
+            requests.post("http://www.example.com/", timeout=_TIMEOUT_SECONDS)
 
 
 @pytest.mark.parametrize("mock_ctx", _MOCK_CTXS)
 def test_request_needs_content_type(mock_ctx: _MockCtxType) -> None:
     """
     Routes which require a content type are supported.
     """
     app = Flask(__name__)
 
     @app.route("/")
-    @consumes("application/json")  # type: ignore[misc]
     def _() -> str:
+        assert request.mimetype == "application/json"
         return "Hello, World!"
 
     test_client = app.test_client()
     response = test_client.get("/", content_type="application/json")
 
     expected_status_code = 200
     expected_content_type = "text/html; charset=utf-8"
@@ -743,15 +772,15 @@
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com",
             headers={"Content-Type": "application/json"},
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -759,16 +788,16 @@
 def test_request_needs_data(mock_ctx: _MockCtxType) -> None:
     """
     Routes which require data are supported.
     """
     app = Flask(__name__)
 
     @app.route("/")
-    @consumes("application/json")  # type: ignore[misc]
     def _() -> str:
+        assert request.mimetype == "application/json"
         request_json = request.get_json()
         assert isinstance(request_json, dict)
         return str(request_json["hello"])
 
     test_client = app.test_client()
     response = test_client.get(
         "/",
@@ -791,15 +820,15 @@
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com",
             headers={"Content-Type": "application/json"},
             data=json.dumps({"hello": "world"}),
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -839,15 +868,18 @@
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        mock_response = requests.get("http://www.example.com/4", timeout=1)
+        mock_response = requests.get(
+            "http://www.example.com/4",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
 @pytest.mark.parametrize("mock_ctx", _MOCK_CTXS)
@@ -878,15 +910,15 @@
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
         mock_response = requests.get(
             "http://www.example.com?frasier=crane",
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
 
 
@@ -897,37 +929,44 @@
     """
     app = Flask(__name__)
 
     @app.route("/", methods=["POST"])
     def _() -> Response:
         response = make_response()
         response.set_cookie("frasier_set", "crane_set")
+        assert request.cookies, request
         assert request.cookies["frasier"] == "crane"
         assert request.cookies["frasier2"] == "crane2"
         response.data = "Hello, World!"
         assert isinstance(response, Response)
         return response
 
     test_client = app.test_client()
-    test_client.set_cookie(server_name="", key="frasier", value="crane")
-    test_client.set_cookie(server_name="", key="frasier2", value="crane2")
-    test_client_cookie_jar = test_client.cookie_jar
-    assert test_client_cookie_jar is not None
-    original_cookies = set(test_client_cookie_jar)
+    test_client.set_cookie(
+        domain="localhost",
+        key="frasier",
+        value="crane",
+    )
+    test_client.set_cookie(
+        domain="localhost",
+        key="frasier2",
+        value="crane2",
+    )
     response = test_client.post("/")
 
     expected_status_code = 200
     expected_content_type = "text/html; charset=utf-8"
     expected_data = b"Hello, World!"
 
-    (new_cookie,) = set(test_client_cookie_jar) - original_cookies
-    assert new_cookie.name == "frasier_set"
-    assert new_cookie.value == "crane_set"
-    assert response.status_code == expected_status_code
+    assert response.status_code == expected_status_code, response.data
     assert response.headers["Content-Type"] == expected_content_type
+    new_cookie = test_client.get_cookie(key="frasier_set")
+    assert new_cookie is not None
+    assert new_cookie.key == "frasier_set"
+    assert new_cookie.value == "crane_set"
     assert response.data == expected_data
 
     with mock_ctx() as mock_obj:
         add_flask_app_to_mock(
             mock_obj=mock_obj,
             flask_app=app,
             base_url="http://www.example.com",
@@ -935,14 +974,30 @@
 
         mock_response = requests.post(
             "http://www.example.com",
             cookies={
                 "frasier": "crane",
                 "frasier2": "crane2",
             },
-            timeout=1,
+            timeout=_TIMEOUT_SECONDS,
         )
 
     assert mock_response.status_code == expected_status_code
     assert mock_response.headers["Content-Type"] == expected_content_type
     assert mock_response.text == expected_data.decode()
     assert mock_response.cookies["frasier_set"] == "crane_set"
+
+
+def test_unknown_mock_type() -> None:
+    """
+    When an unknown mock type is passed in, an error is raised.
+    """
+    expected_error = (
+        "Expected a HTTPretty, ``requests_mock``, or ``responses`` object, "
+        "got <class 'object'>."
+    )
+    with pytest.raises(expected_exception=TypeError, match=expected_error):
+        add_flask_app_to_mock(
+            mock_obj=object(),
+            flask_app=Flask(__name__),
+            base_url="http://www.example.com",
+        )
```

### Comparing `requests-mock-flask-2023.3.5.1/tests/test_usage_patterns.py` & `requests-mock-flask-2023.5.14/tests/test_usage_patterns.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """
 Tests for ways the helper can be used.
 """
 
 from http import HTTPStatus
+from typing import Final
 
 import httpretty
 import requests
 import requests_mock
 import responses
 from flask import Flask
 from requests_mock_flask import add_flask_app_to_mock
 
+# We use a high timeout to allow interactive debugging while requests are being
+# made.
+_TIMEOUT_SECONDS: Final[int] = 120
+
 
 class TestResponses:
     """
     Tests for using the helper with ``responses``.
     """
 
     @staticmethod
@@ -33,15 +38,18 @@
         ) as resp_m:
             add_flask_app_to_mock(
                 mock_obj=resp_m,
                 flask_app=app,
                 base_url="http://www.example.com",
             )
 
-            response = requests.get("http://www.example.com", timeout=1)
+            response = requests.get(
+                url="http://www.example.com",
+                timeout=_TIMEOUT_SECONDS,
+            )
 
         assert response.status_code == HTTPStatus.OK
         assert response.text == "Hello, World!"
 
     @staticmethod
     @responses.activate
     def test_decorator() -> None:
@@ -56,15 +64,18 @@
 
         add_flask_app_to_mock(
             mock_obj=responses,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        response = requests.get("http://www.example.com", timeout=1)
+        response = requests.get(
+            url="http://www.example.com",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
         assert response.status_code == HTTPStatus.OK
         assert response.text == "Hello, World!"
 
 
 class TestRequestsMock:
     """
@@ -86,15 +97,18 @@
         with requests_mock.Mocker() as resp_m:
             add_flask_app_to_mock(
                 mock_obj=resp_m,
                 flask_app=app,
                 base_url="http://www.example.com",
             )
 
-            response = requests.get("http://www.example.com", timeout=1)
+            response = requests.get(
+                url="http://www.example.com",
+                timeout=_TIMEOUT_SECONDS,
+            )
 
         assert response.status_code == HTTPStatus.OK
         assert response.text == "Hello, World!"
 
     @staticmethod
     def test_fixture(  # pylint: disable=redefined-outer-name
         requests_mock: requests_mock.Mocker,
@@ -110,15 +124,18 @@
 
         add_flask_app_to_mock(
             mock_obj=requests_mock,
             flask_app=app,
             base_url="http://www.example.com",
         )
 
-        response = requests.get("http://www.example.com", timeout=1)
+        response = requests.get(
+            url="http://www.example.com",
+            timeout=_TIMEOUT_SECONDS,
+        )
 
         assert response.status_code == HTTPStatus.OK
 
     @staticmethod
     def test_adapter() -> None:
         """
         It is possible to use the helper with a ``requests_mock`` adapter.
@@ -167,11 +184,14 @@
         with httpretty.enabled():
             add_flask_app_to_mock(
                 mock_obj=httpretty,
                 flask_app=app,
                 base_url="http://www.example.com",
             )
 
-            response = requests.get("http://www.example.com", timeout=1)
+            response = requests.get(
+                "http://www.example.com",
+                timeout=_TIMEOUT_SECONDS,
+            )
 
         assert response.status_code == HTTPStatus.OK
         assert response.text == "Hello, World!"
```

