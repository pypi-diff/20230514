# Comparing `tmp/cognite_gql_pygen-0.7.0.tar.gz` & `tmp/cognite_gql_pygen-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.7.0.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.8.0.tar", max compression
```

## Comparing `cognite_gql_pygen-0.7.0.tar` & `cognite_gql_pygen-0.8.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11349 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/LICENSE
--rw-r--r--   0        0        0     4493 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/README.md
--rw-r--r--   0        0        0     8651 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      167 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    19000 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3909 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2593 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/cdf/get_client.py
--rwxr-xr-x   0        0        0      399 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6471 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     4065 2023-05-13 21:48:05.698499 cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    19106 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     5929 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     7060 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0     3595 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/testing.py
--rw-r--r--   0        0        0     1423 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0       76 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0     1904 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/data_classes.py
--rw-r--r--   0        0        0     1560 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/generator.py
--rw-r--r--   0        0        0     7890 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0      596 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/misc.py
--rw-r--r--   0        0        0     1425 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/parser.py
--rw-r--r--   0        0        0     1334 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/templates/client.txt
--rw-r--r--   0        0        0      807 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/templates/schema.txt
--rw-r--r--   0        0        0       22 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     2230 2023-05-13 21:48:05.702499 cognite_gql_pygen-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5286 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/README.md
+-rw-r--r--   0        0        0     8651 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19000 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3909 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2593 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      399 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6471 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     4065 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    19106 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     5929 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7060 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0     3595 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/testing.py
+-rw-r--r--   0        0        0     1423 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0      146 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0     1904 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/data_classes.py
+-rw-r--r--   0        0        0     1634 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/generator.py
+-rw-r--r--   0        0        0     9042 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0      596 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/misc.py
+-rw-r--r--   0        0        0     1425 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/parser.py
+-rw-r--r--   0        0        0     1334 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/templates/client.txt
+-rw-r--r--   0        0        0      807 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-05-14 14:38:30.218309 cognite_gql_pygen-0.8.0/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     1946 2023-05-14 14:38:30.222308 cognite_gql_pygen-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6370 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.8.0/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.7.0/LICENSE` & `cognite_gql_pygen-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/README.md` & `cognite_gql_pygen-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -20,28 +20,38 @@
   * Reduced typing errors in development.
 * Keeping the language domain specific for the developer. Instead of working with generic concepts such as instances,
   nodes, edges, the developer can work with the concepts in the data model.
 
 
 ## Installation
 
-To install this package:
+### Without any optional dependencies
+
+To install this package without CLI support:
 ```bash
-$ pip install cognite-gql-pygen
+pip install cognite-gql-pygen
+```
+
+### With optional dependencies
+
+* `cli` This includes CLI support such that you can run the package from the command line.
+
+```bash
+pip install cognite-gql-pygen[cli]
 ```
 
 ## Usage
 
 The goal of the package is to have representations of all the types in a given data model with API calls to *.list()*,
 *.apply()*, *.delete()*, and *.retrieve()* individuals for each type.
 
 ![image](https://user-images.githubusercontent.com/60234212/234041823-f72a27e3-6450-4f05-99dc-50e87f762d0f.png)
 
 
-
+### With CLI
 You can specify the data models either as a `.graphql` schema or a `pydantic` classes in a `.py` file. Then, you can
 use the CLI to automatically generate the other representation as well as the `client.py` file which creates
 the API and the convenience method get_[client_name]_client().
 
 To generate from a `.graphql` schema you use the following command.
 
 ```bash
@@ -72,14 +82,36 @@
 it consists of four files.
 
 * `schema.graphql` The schema defined in GraphQL language.
 * `schema.py` The schema defined in `pydantic` classes.
 * `client.py` Which sets up the client for the data model.
 * `usage.py` Demonstrates the usage of the client.
 
+### Without CLI
+You can run this package directly in Python code. This can be useful, for example, a notebook.
+When you run the function `to_client_sdk` you get a `PythonSDK` object back which has the `pydantic`
+classes in a `PythonSDK.schema` and the client in the `PythonSDK.client`.
+
+
+```python
+from cognite.gqlpygen import to_client_sdk
+my_schema = """type Case {
+  scenario: Scenario
+  start_time: String!
+  end_time: String!
+ }
+
+type Scenario {
+  name: String!
+}
+"""
+sdk = to_client_sdk(my_schema, "MyClient", "my_schema")
+print(sdk.schema)
+```
+
 
 ### Settings File
 
 `dm togql` and `dm topython` take their defaults form `settings.toml` if present. See
 [settings.toml](./cognite/dm_clients/settings.toml) for an example, section `[local]` is relevant for `togql` and
 `topython` commands.
```

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/relationship_api.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/relationship_api.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/domain_modeling/testing.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/domain_modeling/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.8.0/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/gqlpygen/data_classes.py` & `cognite_gql_pygen-0.8.0/cognite/gqlpygen/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/gqlpygen/generator.py` & `cognite_gql_pygen-0.8.0/cognite/gqlpygen/generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
+
 from jinja2 import Environment, PackageLoader, select_autoescape
 
 from cognite.dm_clients.misc import to_snake
 from cognite.gqlpygen.parser import parse_graphql
 
 
-def to_client_sdk(schema_raw: str, client_name: str, schema_name: str) -> dict[str, str]:
+@dataclass
+class PythonSDK:
+    client: str
+    schema: str
+
+
+def to_client_sdk(schema_raw: str, client_name: str, schema_name: str) -> PythonSDK:
     """
     Converts a GraphQL schema to a client-side SDK.
 
     :param schema_raw: GraphQL schema.
     :param client_name: Name of the client.
     :param schema_name: Name of the schema.
     :return: Client-side SDK
@@ -37,16 +45,15 @@
     schema_tmp = env.get_template("schema.txt")
     ordered = models.topological_order
     ordered[-1].is_root_node = True
     schema_py = schema_tmp.render(
         schema_name=schema_name,
         models=ordered,
     )
-
-    return {"client.py": _clean_rendered_template(client_py), "schema.py": _clean_rendered_template(schema_py)}
+    return PythonSDK(_clean_rendered_template(client_py), _clean_rendered_template(schema_py))
 
 
 def _clean_rendered_template(rendered_template: str) -> str:
     """
     Clean up, adjust new lines and indent.
     """
     return rendered_template.replace("    \n", "\n") + "\n"
```

### Comparing `cognite_gql_pygen-0.7.0/cognite/gqlpygen/main.py` & `cognite_gql_pygen-0.8.0/cognite/gqlpygen/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,25 +4,39 @@
 import subprocess
 import sys
 from contextlib import suppress
 from pathlib import Path
 from typing import Optional
 
 import click
-import typer
-import yaml
-from packaging import version
+import toml
+
+try:
+    import typer
+except ImportError:
+    _has_typer = False
+    typer = None
+else:
+    _has_typer = True
+
+import dataclasses
+
+try:
+    from packaging import version
+except ImportError:
+    _has_packaging = False
+    version = None
+else:
+    _has_packaging = True
 
 from cognite.dm_clients.config import settings
 from cognite.dm_clients.domain_modeling.schema import Schema
 from cognite.gqlpygen.generator import to_client_sdk
 from cognite.gqlpygen.misc import to_client_name, to_schema_name
 
-app = typer.Typer()
-
 
 def _hide_pw(secret: str, value: Optional[str] = None) -> str:
     """
     Hide secret from value:
 
     >>> _hide_pw("SeCrEt", "Here is my SeCrEt password!")
     'Here is my SeC*****... password!'
@@ -42,171 +56,181 @@
     cdf_version_proc = subprocess.run("cdf --version", shell=True, capture_output=True)
     if cdf_version_proc.returncode:
         typer.echo(
             "Error calling 'cdf' command, please see https://docs.cognite.com/cdf/cli/ for installation instructions.",
             err=True,
         )
         sys.exit(1)
-
+    if not _has_packaging:
+        raise ImportError("packaging is required for this feature, install with `pip install cognite-gql-pygen[cli]")
     min_version = version.Version("2.0.0")
     installed_version = version.parse(cdf_version_proc.stdout.decode())
     if installed_version < min_version:
         typer.echo(
             f"Too old version of 'cdf' ({installed_version}), at least {min_version} is needed."
             f" Please see https://docs.cognite.com/cdf/cli/ for installation instructions.",
             err=True,
         )
         sys.exit(1)
 
 
-@app.command("topython", help="Create pydantic schema and Python DM client from a .graphql schema.")
-def to_python(
-    graphql_schema: Path = typer.Argument(settings.get("local.graphql_schema", ...), help="GraphQL schema to convert"),
-    output_dir: Path = typer.Option(
-        Path(_graphql_schema).parent if (_graphql_schema := settings.get("local.graphql_schema")) else Path.cwd(),
-        help="Directory to write schema.py and client.py to.",
-    ),
-    name: str = typer.Option(
-        settings.get("local.name", ""),
-        help="Name of the client and schema, expected to be in pascal case.",
-    ),
-):
-    schema_raw = graphql_schema.read_text()
-    client_name = to_client_name(name)
-    schema_name = to_schema_name(name)
-    sdk = to_client_sdk(schema_raw, client_name, schema_name)
-    output_dir = (output_dir or graphql_schema.parent).absolute()
-    output_dir.mkdir(exist_ok=True)
-
-    for name, content in sdk.items():
-        output = output_dir / name
-        output.write_text(content)
-        with suppress(ValueError):
-            # Will raise a ValueError of output is not relative to cwd.
-            output = output.relative_to(Path.cwd())
-        click.echo(f"Wrote file '{output}'")
-
-
-@app.command(
-    "settings",
-    help="Display configuration values from settings.toml, .secrets.toml and/or environment variables."
-    " Meant for troubleshooting. Partially hides value of 'client_secret' for security reasons.",
-)
-def check_settings():
-    typer.echo(_hide_pw(settings.get("cognite.client_secret", ""), yaml.safe_dump(settings.as_dict())))
-
-
-@app.command("togql", help="Input a pydantic schema to create .graphql schema")
-def to_gql(
-    schema_module: Path = typer.Argument(
-        settings.get("local.schema_module", ...),
-        help="Pydantic schema to convert. Path to a .py file or Python dot notation ",
-    ),
-    graphql_schema: Path = typer.Option(settings.get("local.graphql_schema", ...), help="File path for the output."),
-    name: Optional[str] = typer.Option(
-        settings.get("local.name"),
-        help="Name of the client and schema, expected to be in pascal case.",
-    ),
-):
-    if schema_module.suffix == ".py":
-        click.echo(f"Got file '{schema_module}', trying to import it...")
-        module_name = schema_module.stem
-        spec = importlib.util.spec_from_file_location(module_name, schema_module)
-        module = importlib.util.module_from_spec(spec)  # type:ignore[arg-type]
-        sys.modules[module_name] = module
-        spec.loader.exec_module(module)  # type:ignore[union-attr]
-    else:
-        module_name = settings.local.get("schema_module", default=schema_module.stem)
-        click.echo(f"Got module '{schema_module}', trying to import it...")
-        module = importlib.import_module(module_name)
-    click.echo("Import successful")
-
-    if name is None:
-        click.echo("Searching for a schema...")
-        for schema_name, instance in inspect.getmembers(module):
-            if isinstance(instance, Schema):
-                click.echo(f"Found schema '{schema_name}'")
-                break
-        else:
-            click.echo("Failed to find schema, exiting..")
-            exit(1)
-    else:
+if _has_typer:
+    app = typer.Typer()
+
+    @app.command("topython", help="Create pydantic schema and Python DM client from a .graphql schema.")
+    def to_python(
+        graphql_schema: Path = typer.Argument(
+            settings.get("local.graphql_schema", ...), help="GraphQL schema to convert"
+        ),
+        output_dir: Path = typer.Option(
+            Path(_graphql_schema).parent if (_graphql_schema := settings.get("local.graphql_schema")) else Path.cwd(),
+            help="Directory to write schema.py and client.py to.",
+        ),
+        name: str = typer.Option(
+            settings.get("local.name", ""),
+            help="Name of the client and schema, expected to be in pascal case.",
+        ),
+    ):
+        schema_raw = graphql_schema.read_text()
+        client_name = to_client_name(name)
         schema_name = to_schema_name(name)
-        click.echo(f"Got schema name '{schema_name}'")
-        try:
-            instance = getattr(module, schema_name)
-        except AttributeError as exc:
-            typer.echo(f"Error: {exc}. Check the --name option and 'schema_module' argument.")
-            sys.exit(1)
-
-    graphql_schema.write_text(instance.as_str())
-    click.echo(f"Wrote file '{graphql_schema}'")
-
-
-@app.command("signin", help="Upload a GQL schema to CDF DM data model.")
-def signin(
-    cdf_cluster: str = typer.Option(settings.get("cognite.cdf_cluster", ...), help="CDF cluster name."),
-    tenant_id: str = typer.Option(settings.get("cognite.tenant_id", ...), help="AD tenant ID."),
-    client_id: str = typer.Option(settings.get("cognite.client_id", ...), help="AD client ID."),
-    project: str = typer.Option(settings.get("cognite.project", ...), help="Name of CDF project."),
-):
-    client_secret_none = "None (use device flow)"
-    client_secret = settings.get("cognite.client_secret")
-    if client_secret is None:
-        if sys.stdin.isatty():
-            client_secret = typer.prompt(
-                "Client secret",
-                default=client_secret_none,
-                type=str,
-                hide_input=True,
-            )
+        sdk = to_client_sdk(schema_raw, client_name, schema_name)
+        output_dir = (output_dir or graphql_schema.parent).absolute()
+        output_dir.mkdir(exist_ok=True)
+
+        for name, content in dataclasses.asdict(sdk).items():
+            output = output_dir / f"{name}.py"
+            output.write_text(content)
+            with suppress(ValueError):
+                # Will raise a ValueError of output is not relative to cwd.
+                output = output.relative_to(Path.cwd())
+            click.echo(f"Wrote file '{output}'")
+
+    @app.command(
+        "settings",
+        help="Display configuration values from settings.toml, .secrets.toml and/or environment variables."
+        " Meant for troubleshooting. Partially hides value of 'client_secret' for security reasons.",
+    )
+    def check_settings():
+        typer.echo(_hide_pw(settings.get("cognite.client_secret", ""), toml.dumps(settings.as_dict())))
+
+    @app.command("togql", help="Input a pydantic schema to create .graphql schema")
+    def to_gql(
+        schema_module: Path = typer.Argument(
+            settings.get("local.schema_module", ...),
+            help="Pydantic schema to convert. Path to a .py file or Python dot notation ",
+        ),
+        graphql_schema: Path = typer.Option(
+            settings.get("local.graphql_schema", ...), help="File path for the output."
+        ),
+        name: Optional[str] = typer.Option(
+            settings.get("local.name"),
+            help="Name of the client and schema, expected to be in pascal case.",
+        ),
+    ):
+        if schema_module.suffix == ".py":
+            click.echo(f"Got file '{schema_module}', trying to import it...")
+            module_name = schema_module.stem
+            spec = importlib.util.spec_from_file_location(module_name, schema_module)
+            module = importlib.util.module_from_spec(spec)  # type:ignore[arg-type]
+            sys.modules[module_name] = module
+            spec.loader.exec_module(module)  # type:ignore[union-attr]
+        else:
+            module_name = settings.local.get("schema_module", default=schema_module.stem)
+            click.echo(f"Got module '{schema_module}', trying to import it...")
+            module = importlib.import_module(module_name)
+        click.echo("Import successful")
+
+        if name is None:
+            click.echo("Searching for a schema...")
+            for schema_name, instance in inspect.getmembers(module):
+                if isinstance(instance, Schema):
+                    click.echo(f"Found schema '{schema_name}'")
+                    break
+            else:
+                click.echo("Failed to find schema, exiting..")
+                exit(1)
         else:
-            client_secret = sys.stdin.readline().rstrip()
-    if client_secret == client_secret_none:
-        client_secret = ""
-    _check_cdf_cli()
-    command = [
-        "cdf",
-        "signin",
-        f"'{project}'",
-        f"--cluster='{cdf_cluster}'",
-        f"--tenant='{tenant_id}'",
-        f"--client-id='{client_id}'",
-        (f"--client-secret='{client_secret}'" if client_secret else "--device-code"),
-    ]
-    typer.echo(f"Executing:\n{_hide_pw(client_secret, ' '.join(command))}")
-    subprocess.run(" ".join(command), shell=True)
-
-
-@app.command("upload", help="Upload a GQL schema to CDF DM data model.")
-def upload(
-    graphql_schema: Path = typer.Argument(settings.get("local.graphql_schema", ...), help="GraphQL schema to upload."),
-    space: str = typer.Option(settings.get("dm_clients.space", ...), help="Space ID in CDF Domain Modeling"),
-    data_model: str = typer.Option(
-        settings.get("dm_clients.datamodel", ...),
-        help="ID of Data Model in CDF Domain Modeling",
-    ),
-    schema_version: int = typer.Option(
-        settings.get("dm_clients.schema_version", ...),
-        help="Version of the schema to app or update.",
-    ),
-):
-    _check_cdf_cli()
-    command = [
-        "cdf",
-        "data-models",
-        "publish",
-        f"--file='{graphql_schema}'",
-        f"--space='{space}'",
-        f"--external-id='{data_model}'",
-        f"--version='{schema_version}'",
-    ]
-    typer.echo(f"Executing:\n{' '.join(command)}")
-    subprocess.run(" ".join(command), shell=True)
+            schema_name = to_schema_name(name)
+            click.echo(f"Got schema name '{schema_name}'")
+            try:
+                instance = getattr(module, schema_name)
+            except AttributeError as exc:
+                typer.echo(f"Error: {exc}. Check the --name option and 'schema_module' argument.")
+                sys.exit(1)
+
+        graphql_schema.write_text(instance.as_str())
+        click.echo(f"Wrote file '{graphql_schema}'")
+
+    @app.command("signin", help="Upload a GQL schema to CDF DM data model.")
+    def signin(
+        cdf_cluster: str = typer.Option(settings.get("cognite.cdf_cluster", ...), help="CDF cluster name."),
+        tenant_id: str = typer.Option(settings.get("cognite.tenant_id", ...), help="AD tenant ID."),
+        client_id: str = typer.Option(settings.get("cognite.client_id", ...), help="AD client ID."),
+        project: str = typer.Option(settings.get("cognite.project", ...), help="Name of CDF project."),
+    ):
+        client_secret_none = "None (use device flow)"
+        client_secret = settings.get("cognite.client_secret")
+        if client_secret is None:
+            if sys.stdin.isatty():
+                client_secret = typer.prompt(
+                    "Client secret",
+                    default=client_secret_none,
+                    type=str,
+                    hide_input=True,
+                )
+            else:
+                client_secret = sys.stdin.readline().rstrip()
+        if client_secret == client_secret_none:
+            client_secret = ""
+        _check_cdf_cli()
+        command = [
+            "cdf",
+            "signin",
+            f"'{project}'",
+            f"--cluster='{cdf_cluster}'",
+            f"--tenant='{tenant_id}'",
+            f"--client-id='{client_id}'",
+            (f"--client-secret='{client_secret}'" if client_secret else "--device-code"),
+        ]
+        typer.echo(f"Executing:\n{_hide_pw(client_secret, ' '.join(command))}")
+        subprocess.run(" ".join(command), shell=True)
+
+    @app.command("upload", help="Upload a GQL schema to CDF DM data model.")
+    def upload(
+        graphql_schema: Path = typer.Argument(
+            settings.get("local.graphql_schema", ...), help="GraphQL schema to upload."
+        ),
+        space: str = typer.Option(settings.get("dm_clients.space", ...), help="Space ID in CDF Domain Modeling"),
+        data_model: str = typer.Option(
+            settings.get("dm_clients.datamodel", ...),
+            help="ID of Data Model in CDF Domain Modeling",
+        ),
+        schema_version: int = typer.Option(
+            settings.get("dm_clients.schema_version", ...),
+            help="Version of the schema to app or update.",
+        ),
+    ):
+        _check_cdf_cli()
+        command = [
+            "cdf",
+            "data-models",
+            "publish",
+            f"--file='{graphql_schema}'",
+            f"--space='{space}'",
+            f"--external-id='{data_model}'",
+            f"--version='{schema_version}'",
+        ]
+        typer.echo(f"Executing:\n{' '.join(command)}")
+        subprocess.run(" ".join(command), shell=True)
+
+    def main():
+        app()
 
+else:
 
-def main():
-    app()
+    def main():
+        print("THE CLI requires typer to be available, install with `pip install cognite-gql-pygen[cli]")  # noqa
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cognite_gql_pygen-0.7.0/cognite/gqlpygen/misc.py` & `cognite_gql_pygen-0.8.0/cognite/gqlpygen/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/gqlpygen/parser.py` & `cognite_gql_pygen-0.8.0/cognite/gqlpygen/parser.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/gqlpygen/templates/client.txt` & `cognite_gql_pygen-0.8.0/cognite/gqlpygen/templates/client.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/cognite/gqlpygen/templates/schema.txt` & `cognite_gql_pygen-0.8.0/cognite/gqlpygen/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.7.0/pyproject.toml` & `cognite_gql_pygen-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.7.0"
-description = "Cognite graphQL Python generation SDK"
+version = "0.8.0"
+description = "Cognite GraphQL Python Generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache-2.0"
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
 
@@ -26,35 +26,35 @@
 dm = "cognite.gqlpygen.main:main"
 dm_clients = "cognite.dm_clients.main:main"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = ">=1.10"
-typer = {version = "*", extras = ["all"] }
-PyYAML = "^6.0"
-arrow = "^1.2.2"
-cognite-sdk = {version = ">5.9.0", extras = ["pandas"]}
-msal = ">=1.16.0"
-numpy = "^1.23.2"
-strawberry-graphql = "^0.156.4"
-docopt = "^0.6.2"
-cachelib = "^0.10.2"
-retry = "^0.9.2"
-loguru = "^0.6.0"
-dynaconf = "^3.1.12"
 graphql-core = ">=3.2"
 Jinja2 = ">=3.1"
-packaging = ">=21.3"
+cognite-sdk = {version = ">5.9.0"}
+msal = ">=1.16.0"
+retry = ">=0.9.2"
+strawberry-graphql = "^0.156.4"
+cachelib = ">=0.10.2"
 typing-extensions = ">=4.4.0"
+dynaconf = {version=">=3.1.12"}
+toml = {version=">=0.10"}
+
+packaging = {version=">=21.3", optional=true}
+typer = {version = ">=0.9", extras = ["rich"], optional=true }
+
+[tool.poetry.extras]
+cli = ["packaging", "typer"]
+all = ["packaging", "typer"]
 
 [tool.poetry.dev-dependencies]
 twine = "*"
 pre-commit = "*"
-toml = "*"
 python-dotenv = "*"
 pytest = "*"
 pytest-cov = "*"
 pytest-mock = "*"
 faker = "*"
 mkdocs = "*"
 mkdocs-jupyter = "*"
@@ -64,31 +64,15 @@
 mkdocs-gitbook = "*"
 
 [tool.pytest.ini_options]
 filterwarnings = [
   "ignore::DeprecationWarning:pkg_resources",  # TODO check again with dynaconf>=3.2.0 (introduced in setuptools==67.5.0)
 ]
 addopts = "--doctest-modules"
-
-[tool.mypy]
-plugins = [
-  "pydantic.mypy"
+markers = [
+    "full: Requiers all optional dependencies to run.",
 ]
-explicit_package_bases = true
-follow_imports = "normal"
-warn_redundant_casts = true
-warn_unused_ignores = true
-check_untyped_defs = true
-#disallow_any_generics = true
-#no_implicit_reexport = true
-#disallow_untyped_defs = true
-
 
-[tool.pydantic-mypy]
-init_forbid_extra = true
-init_typed = true
-warn_required_dynamic_aliases = true
-warn_untyped_fields = true
 
 [build-system]
 requires = ["poetry-core>=1.3"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cognite_gql_pygen-0.7.0/PKG-INFO` & `cognite_gql_pygen-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.7.0
-Summary: Cognite graphQL Python generation SDK
+Version: 0.8.0
+Summary: Cognite GraphQL Python Generation SDK
 License: Apache-2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: cli
 Requires-Dist: Jinja2 (>=3.1)
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: arrow (>=1.2.2,<2.0.0)
-Requires-Dist: cachelib (>=0.10.2,<0.11.0)
-Requires-Dist: cognite-sdk[pandas] (>5.9.0)
-Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
+Requires-Dist: cachelib (>=0.10.2)
+Requires-Dist: cognite-sdk (>5.9.0)
+Requires-Dist: dynaconf (>=3.1.12)
 Requires-Dist: graphql-core (>=3.2)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: msal (>=1.16.0)
-Requires-Dist: numpy (>=1.23.2,<2.0.0)
-Requires-Dist: packaging (>=21.3)
+Requires-Dist: packaging (>=21.3) ; extra == "cli" or extra == "all"
 Requires-Dist: pydantic (>=1.10)
-Requires-Dist: retry (>=0.9.2,<0.10.0)
+Requires-Dist: retry (>=0.9.2)
 Requires-Dist: strawberry-graphql (>=0.156.4,<0.157.0)
-Requires-Dist: typer[all]
+Requires-Dist: toml (>=0.10)
+Requires-Dist: typer[rich] (>=0.9) ; extra == "cli" or extra == "all"
 Requires-Dist: typing-extensions (>=4.4.0)
 Description-Content-Type: text/markdown
 
 Cognite GraphQL Python Generator
 ==========================
 [![build](https://github.com/cognitedata/cognite-gql-pygen/actions/workflows/release.yaml/badge.svg)](https://github.com/cognitedata/cognite-gql-pygen/actions/workflows/release.yaml)
 [![GitHub](https://img.shields.io/github/license/cognitedata/cognite-gql-pygen)](https://github.com/cognitedata/cognite-gql-pygen/blob/master/LICENSE)
@@ -52,28 +50,38 @@
   * Reduced typing errors in development.
 * Keeping the language domain specific for the developer. Instead of working with generic concepts such as instances,
   nodes, edges, the developer can work with the concepts in the data model.
 
 
 ## Installation
 
-To install this package:
+### Without any optional dependencies
+
+To install this package without CLI support:
 ```bash
-$ pip install cognite-gql-pygen
+pip install cognite-gql-pygen
+```
+
+### With optional dependencies
+
+* `cli` This includes CLI support such that you can run the package from the command line.
+
+```bash
+pip install cognite-gql-pygen[cli]
 ```
 
 ## Usage
 
 The goal of the package is to have representations of all the types in a given data model with API calls to *.list()*,
 *.apply()*, *.delete()*, and *.retrieve()* individuals for each type.
 
 ![image](https://user-images.githubusercontent.com/60234212/234041823-f72a27e3-6450-4f05-99dc-50e87f762d0f.png)
 
 
-
+### With CLI
 You can specify the data models either as a `.graphql` schema or a `pydantic` classes in a `.py` file. Then, you can
 use the CLI to automatically generate the other representation as well as the `client.py` file which creates
 the API and the convenience method get_[client_name]_client().
 
 To generate from a `.graphql` schema you use the following command.
 
 ```bash
@@ -104,14 +112,36 @@
 it consists of four files.
 
 * `schema.graphql` The schema defined in GraphQL language.
 * `schema.py` The schema defined in `pydantic` classes.
 * `client.py` Which sets up the client for the data model.
 * `usage.py` Demonstrates the usage of the client.
 
+### Without CLI
+You can run this package directly in Python code. This can be useful, for example, a notebook.
+When you run the function `to_client_sdk` you get a `PythonSDK` object back which has the `pydantic`
+classes in a `PythonSDK.schema` and the client in the `PythonSDK.client`.
+
+
+```python
+from cognite.gqlpygen import to_client_sdk
+my_schema = """type Case {
+  scenario: Scenario
+  start_time: String!
+  end_time: String!
+ }
+
+type Scenario {
+  name: String!
+}
+"""
+sdk = to_client_sdk(my_schema, "MyClient", "my_schema")
+print(sdk.schema)
+```
+
 
 ### Settings File
 
 `dm togql` and `dm topython` take their defaults form `settings.toml` if present. See
 [settings.toml](./cognite/dm_clients/settings.toml) for an example, section `[local]` is relevant for `togql` and
 `topython` commands.
```

