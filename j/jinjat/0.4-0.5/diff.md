# Comparing `tmp/jinjat-0.4.tar.gz` & `tmp/jinjat-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinjat-0.4.tar", max compression
+gzip compressed data, was "jinjat-0.5.tar", max compression
```

## Comparing `jinjat-0.4.tar` & `jinjat-0.5.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-05-02 00:00:49.669895 jinjat-0.4/LICENSE
--rw-r--r--   0        0        0     1612 2023-05-02 00:00:49.669895 jinjat-0.4/README.md
--rw-r--r--   0        0        0     2648 2023-05-02 00:01:01.405990 jinjat-0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/__init__.py
--rw-r--r--   0        0        0       93 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/__main__.py
--rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/dbt/__init__.py
--rw-r--r--   0        0        0     2348 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/dbt/config.py
--rw-r--r--   0        0        0    23495 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/dbt/dbt_project.py
--rw-r--r--   0        0        0      878 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/exceptions.py
--rw-r--r--   0        0        0     4486 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/generator.py
--rw-r--r--   0        0        0     2641 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/log_controller.py
--rw-r--r--   0        0        0     5373 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/models.py
--rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/routes/__init__.py
--rw-r--r--   0        0        0     8917 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/routes/admin.py
--rw-r--r--   0        0        0     9164 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/routes/analysis.py
--rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/schema/__init__.py
--rw-r--r--   0        0        0      693 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/schema/validator.py
--rw-r--r--   0        0        0     5947 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/server.py
--rw-r--r--   0        0        0        0 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/util/__init__.py
--rw-r--r--   0        0        0     6947 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/util/api.py
--rw-r--r--   0        0        0     1068 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/util/filesystem.py
--rw-r--r--   0        0        0     2068 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/core/util/jmespath.py
--rw-r--r--   0        0        0    12288 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/jaffle_shop.duckdb
--rw-r--r--   0        0        0     5853 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/main.py
--rw-r--r--   0        0        0    10094 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/playground.py
--rw-r--r--   0        0        0      210 2023-05-02 00:00:49.673895 jinjat-0.4/src/jinjat/requirements.txt
--rw-r--r--   0        0        0     3558 1970-01-01 00:00:00.000000 jinjat-0.4/setup.py
--rw-r--r--   0        0        0     4401 1970-01-01 00:00:00.000000 jinjat-0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-14 01:24:40.914393 jinjat-0.5/LICENSE
+-rw-r--r--   0        0        0     1347 2023-05-14 01:24:40.914393 jinjat-0.5/README.md
+-rw-r--r--   0        0        0     2783 2023-05-14 01:24:53.338441 jinjat-0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/dbt/__init__.py
+-rw-r--r--   0        0        0     2601 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/dbt/config.py
+-rw-r--r--   0        0        0    23560 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/dbt/dbt_project.py
+-rw-r--r--   0        0        0      878 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/exceptions.py
+-rw-r--r--   0        0        0     4486 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/generator.py
+-rw-r--r--   0        0        0     2641 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/log_controller.py
+-rw-r--r--   0        0        0     5381 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/models.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/routes/__init__.py
+-rw-r--r--   0        0        0     8917 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/routes/admin.py
+-rw-r--r--   0        0        0     9399 2023-05-14 01:24:53.338441 jinjat-0.5/src/jinjat/core/routes/analysis.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/schema/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/schema/validator.py
+-rw-r--r--   0        0        0     6220 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/server.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/util/__init__.py
+-rw-r--r--   0        0        0     8166 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/util/api.py
+-rw-r--r--   0        0        0     1068 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/util/filesystem.py
+-rw-r--r--   0        0        0     2068 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/core/util/jmespath.py
+-rw-r--r--   0        0        0        0 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/deploy/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/deploy/cloud-run.py
+-rw-r--r--   0        0        0      944 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/deploy/fal.py
+-rw-r--r--   0        0        0      338 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/deploy/modal-client.py
+-rw-r--r--   0        0        0    12288 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/jaffle_shop.duckdb
+-rw-r--r--   0        0        0     6058 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/main.py
+-rw-r--r--   0        0        0    10094 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/playground.py
+-rw-r--r--   0        0        0      210 2023-05-14 01:24:40.914393 jinjat-0.5/src/jinjat/requirements.txt
+-rw-r--r--   0        0        0     3398 1970-01-01 00:00:00.000000 jinjat-0.5/setup.py
+-rw-r--r--   0        0        0     4168 1970-01-01 00:00:00.000000 jinjat-0.5/PKG-INFO
```

### Comparing `jinjat-0.4/LICENSE` & `jinjat-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/README.md` & `jinjat-0.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -69,21 +69,8 @@
 #### Installation
 
 ```commandline
 pip install jinjat[playground]
 ```
 
 Jinjat Playground is a Streamlit app that lets you develop APIs in your browser.
-Once you write the template, you can save it to your dbt project as an analysis and expose the API.
-
-### [Refine.dev](https://refine.dev) Integration
-
-#### Installation
-
-```commandline
-pip install jinjat[refine]
-```
-
-Jinjat Refine integration creates a Refine app from your OpenAPI spec 
-
-
-> Jinjat is a fork of [dbt-osmosis](https://github.com/z3z1ma/dbt-osmosis)
+Once you write the template, you can save it to your dbt project as an analysis and expose the API.
```

### Comparing `jinjat-0.4/pyproject.toml` & `jinjat-0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jinjat"
-version = "0.4"
+version = "0.5"
 description = "A low-code data application framework that uses dbt Core and OpenAPI"
 authors = ["buremba <emrekabakci@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -17,17 +17,17 @@
     "Programming Language :: Python :: 3.10",
 ]
 keywords = ["dbt", "server", "streamlit", "git", "refine", "data-app", "snowflake"]
 documentation = "https://github.com/jinjat-data/jinjat"
 repository = "https://github.com/jinjat-data/jinjat"
 
 [tool.poetry.dependencies]
-python = ">=3.6,<4"
+python = ">=3.8.1,<4"
 click = ">7"
-dbt-core = "=1.4.5"
+dbt-core = "=1.5.0"
 watchdog = ">=2.2.1"
 "ruamel.yaml" = ">=0.17"
 rich = ">=10"
 pydantic = "^1.9.1"
 bottle = "^0.12.23"
 orjson = "^3.8.0"
 fastapi = "^0.85.0"
@@ -44,21 +44,25 @@
 graphviz = { version = ">=0.17", optional = true }
 pydot = { version = ">=1.4.2", optional = true }
 streamlit-agraph = { version = ">=0.0.35", optional = true }
 streamlit-pandas-profiling = { version = ">=0.1.3", optional = true }
 streamlit-aggrid = { version = ">=0.2.2", optional = true }
 scipy = { version = "^1.3.1", optional = true }
 feedparser = { version = "^6.0.10", optional = true }
-# Testing duckdb
+# Testing duck
 duckcli = { version = "^0.2.1", optional = true }
-dbt-duckdb = { version = "^1.4.1", optional = true }
+dbt-duckdb = { version = "^1.5.0", optional = true }
 pandas = "^1.5.3"
+# Deploy
+fal-serverless = "0.6.29"
+modal-client = "0.49.2059"
+sqlglot = "12.3.0"
 
 [tool.poetry.dev-dependencies]
-black = ">=21.9b0"
+black = ">=23.3.0"
 mypy = ">=0.910"
 pytest = ">=6.2.5"
 coverage = ">=5.5"
 pylint = ">=2.11.1"
 nox = ">=2021.6.12"
 pytest-mock = ">=3.6.1"
 viztracer = "^0.15.3"
@@ -72,14 +76,18 @@
     "pydot",
     "streamlit-agraph",
     "streamlit-pandas-profiling",
     "streamlit-aggrid",
     "scipy",
     "feedparser",
 ]
+deploy = [
+    "fal-serverless",
+    "modal-client"
+]
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `jinjat-0.4/src/jinjat/core/dbt/config.py` & `jinjat-0.5/src/jinjat/core/dbt/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from pathlib import Path
 from typing import (
     Optional, TypeVar,
 )
-from dbt.flags import DEFAULT_PROFILES_DIR
+
+from dbt.cli.resolvers import default_profiles_dir
 from dbt.tracking import disable_tracking
 from dbt.version import __version__ as dbt_version
 from ruamel.yaml import YAML
 
 CACHE = {}
 CACHE_VERSION = 1
 JINJAT_REQUEST_VAR_NAME = "jinjat_request"
@@ -23,14 +25,18 @@
     return any(seq in query for seq in JINJA_CONTROL_SEQS)
 
 
 disable_tracking()
 fire_event = lambda e: None
 
 
+def default_profiles_dir(project_path) -> Path:
+    return project_path if (project_path / "profiles.yml").exists() else Path.home() / ".dbt"
+
+
 class ConfigInterface:
     """This mimic dbt-core args based interface for dbt-core
     class instantiation"""
 
     def __init__(
             self,
             threads: Optional[int] = 1,
@@ -38,15 +44,16 @@
             profiles_dir: Optional[str] = None,
             project_dir: Optional[str] = None,
             vars: Optional[str] = "{}",
             profile: Optional[str] = None,
     ):
         self.threads = threads
         self.target = target
-        self.profiles_dir = profiles_dir or DEFAULT_PROFILES_DIR
+        self.profiles_dir = profiles_dir or default_profiles_dir(
+            Path(project_dir) if project_dir is not None else Path.cwd())
         self.project_dir = project_dir
         self.vars = vars  # json.dumps str
         self.dependencies = []
         self.single_threaded = threads == 1
         self.quiet = True
         self.profile = profile
```

### Comparing `jinjat-0.4/src/jinjat/core/dbt/dbt_project.py` & `jinjat-0.5/src/jinjat/core/dbt/dbt_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 from dbt.adapters.factory import Adapter, get_adapter_class_by_name
 from dbt.config.runtime import RuntimeConfig
 from dbt.context.providers import generate_runtime_model_context
 from dbt.contracts.connection import AdapterResponse
 from dbt.contracts.graph.manifest import ManifestNode, MaybeNonSource, MaybeParsedSource
 from dbt.flags import set_from_args
 from dbt.node_types import NodeType
-from dbt.parser.manifest import ManifestLoader, process_node
+from dbt.parser.manifest import ManifestLoader, process_node, MANIFEST_FILE_NAME
 from dbt.parser.sql import SqlBlockParser, SqlMacroParser
-from dbt.task.parse import MANIFEST_FILE_NAME
 from dbt.task.sql import SqlCompileRunner, SqlExecuteRunner
+from dbt.adapters.factory import register_adapter
 
 from jinjat.core.log_controller import logger
 
 
 class DbtProject:
     """Container for a dbt project. The dbt attribute is the primary interface for
     dbt-core. The adapter attribute is the primary interface for the dbt adapter"""
@@ -131,14 +131,15 @@
             self.init_adapter()
 
         project_parser = ManifestLoader(
             self.config, self.config.load_dependencies(), self.adapter.connections.set_query_header
         )
         # endpatched (https://github.com/dbt-labs/dbt-core/blob/main/core/dbt/parser/manifest.py#L545)
         try:
+            register_adapter(self.config)
             self.dbt = project_parser.load()
         except CompilationError as e:
             logger().error(f"Encountered an error loading dbt module:\n{e}")
             sys.exit(1)
         self.dbt.build_flat_graph()
         project_parser.save_macros_to_adapter(self.adapter)
         self._sql_parser = None
@@ -444,15 +445,15 @@
 
 class DbtTarget(BaseModel):
     target: Optional[str] = None
     profiles_dir: Optional[str] = None
     project_dir: Optional[str] = None
     refine: Optional[bool] = False
     threads: Optional[int] = 1
-    vars: Optional[str] = "{}"
+    vars: Optional[dict] = {}
 
 
 class DbtProjectContainer:
     """This class manages multiple DbtProjects which each correspond
     to a single dbt project on disk. This is mostly for jinjat server use"""
 
     def __init__(self):
```

### Comparing `jinjat-0.4/src/jinjat/core/exceptions.py` & `jinjat-0.5/src/jinjat/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/src/jinjat/core/generator.py` & `jinjat-0.5/src/jinjat/core/generator.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/src/jinjat/core/log_controller.py` & `jinjat-0.5/src/jinjat/core/log_controller.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/src/jinjat/core/models.py` & `jinjat-0.5/src/jinjat/core/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 from starlette.requests import Request
 
 LIMIT_QUERY_PARAM = '_limit'
 JSON_COLUMNS_QUERY_PARAM = '_json_columns'
 
 
 class CORS(BaseModel):
-    allowed_origins: Optional[str]
+    allowed_origins: Optional[List[str]]
 
 
 class JinjatProjectConfig(BaseModel):
-    cors: Optional[CORS] = CORS(allowed_origins="*")
+    cors: Optional[CORS] = CORS(allowed_origins=["*"])
     max_limit: Optional[int] = 50000
     default_limit: Optional[int] = 500
     refine: Optional[dict]
     openapi: Optional[dict]
 
     @validator('openapi')
     def validate_openapi(cls, openapi):
```

### Comparing `jinjat-0.4/src/jinjat/core/routes/admin.py` & `jinjat-0.5/src/jinjat/core/routes/admin.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/src/jinjat/core/routes/analysis.py` & `jinjat-0.5/src/jinjat/core/routes/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,19 +107,24 @@
                   include_in_schema=False)
 
     # api.add_route("/elements", functools.partial(elements_html, CustomButton("Admin APIs", "/")),
     #               include_in_schema=False)
 
     async def custom_openapi(req: Request) -> JSONResponse:
         extract_path = req.query_params.get("jmespath")
+        servers = [{"url": str(req.url).strip('/openapi.json')}]
+
         if api.openapi_schema:
+            api.openapi_schema['servers'] = servers
             return JSONResponse(extract_jmespath(extract_path, api.openapi_schema, project))
 
-        openapi_schema = get_openapi(title=project.project_name, version=project.config.version, routes=api.routes,
-                                     servers=[{"url": req.scope.get("root_path", "").rstrip("/")}])
+        openapi_schema = get_openapi(title=project.project_name,
+                                     version=project.config.version,
+                                     routes=api.routes,
+                                     servers=servers)
 
         component_schemas = create_components_from_nodes(project)
         components = openapi_schema.setdefault('components', {})
         existing_schemas = components.setdefault('schemas', {})
         components['schemas'] = {**existing_schemas, **component_schemas}
 
         if jinjat_project_config.openapi is not None:
@@ -169,28 +174,30 @@
         # inferred_schema_json = to_json_schema(inferred_schema)
         # if openapi.requestBody.content.get('application/json').schema()
 
         openapi_dict = openapi.dict(by_alias=True, exclude_none=True, exclude_unset=True)
         try:
             transform_request = compile_transform(jinjat_config.transform_request)
         except Exception as e:
-            raise InvalidJinjaConfig(node.original_file_path, None, f"Unable to parse `transform_request` jmespath expression {jinjat_config.transform_request}: {e}")
+            raise InvalidJinjaConfig(node.original_file_path, None,
+                                     f"Unable to parse `transform_request` jmespath expression {jinjat_config.transform_request}: {e}")
 
         try:
             transform_response = compile_transform(jinjat_config.transform_response)
         except Exception as e:
-            raise InvalidJinjaConfig(node.original_file_path, None, f"Unable to parse `transform_response` jmespath expression {jinjat_config.transform_response}: {e}")
+            raise InvalidJinjaConfig(node.original_file_path, None,
+                                     f"Unable to parse `transform_response` jmespath expression {jinjat_config.transform_response}: {e}")
 
         api.add_api_route(api_path,
                           endpoint=functools.partial(handle_analysis_api, project, sql, openapi_dict,
                                                      transform_request,
                                                      transform_response,
                                                      fetch_enabled,
                                                      jinjat_project_config),
                           tags=node.tags,
                           description=node.description,
                           summary=node.name,
                           methods=methods,
-                          operation_id=node.unique_id,
+                          operation_id=re.sub(r"\W", "_", node.name),
                           name=node.alias,
                           openapi_extra=openapi_dict)
     return api
```

### Comparing `jinjat-0.4/src/jinjat/core/schema/validator.py` & `jinjat-0.5/src/jinjat/core/schema/validator.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/src/jinjat/core/server.py` & `jinjat-0.5/src/jinjat/core/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,17 @@
 
 from jinjat.core.dbt.dbt_project import DbtProjectContainer, DbtProject, DbtTarget
 from jinjat.core.log_controller import logger
 from jinjat.core.models import JinjatProjectConfig
 from jinjat.core.routes.admin import app as admin_app
 from jinjat.core.routes.analysis import create_analysis_apps
 from jinjat.core.util.api import register_jsonapi_exception_handlers, rapidoc_html, CustomButton, DBT_PROJECT_HEADER, \
-    DBT_PROJECT_NAME
+    DBT_PROJECT_NAME, StaticFilesWithFallbackIndex, extract_host
 from jinjat.core.util.filesystem import get_project_root
 
-SERVER_OPT = "SERVER_OPT"
-
 app = FastAPI(redoc_url=None, docs_url=None)
 
 dbt_container = DbtProjectContainer()
 app.state.dbt_project_container = dbt_container
 admin_app.state.dbt_project_container = dbt_container
 
 
@@ -58,52 +56,46 @@
 
 def unmount_app(new_app: FastAPI):
     existing_apps = next(filter(lambda r: isinstance(r, Mount) and r.name == new_app.root_path, app.routes), None)
     if existing_apps is not None:
         app.routes.remove(existing_apps)
 
 
-"""Register default project, ugly (using envs?) but works. This will parse the project on disk and load it into memory"""
-if SERVER_OPT in os.environ:
-    dbt_target = DbtTarget.parse_raw(os.environ[SERVER_OPT])
-    logger().info("Registering project: {}".format(dbt_target.json()))
-    project = app.state.dbt_project_container.add_project(dbt_target)
+def custom_openapi(project, config):
+    if app.openapi_schema:
+        return app.openapi_schema
+
+    openapi_schema = get_openapi(title=project.project_name, version=project.config.version, routes=app.routes)
+    app.openapi_schema = openapi_schema
+    if config.openapi is not None:
+        always_merger.merge(app.openapi_schema.get('info'), config.openapi.get("info", {}))
+    return app.openapi_schema
+
 
+def mount_app(app: FastAPI, project, dbt_target: DbtTarget):
     config = get_jinjat_project_config(project.project_root)
 
     app.add_middleware(
         CORSMiddleware,
-        allow_origins=[
-            config.cors.allowed_origins
-        ],
+        allow_origins=config.cors.allowed_origins,
         allow_credentials=False,
         allow_methods=["*"],
         allow_headers=["*"],
         expose_headers=[DBT_PROJECT_HEADER, DBT_PROJECT_NAME]
     )
 
-
-    def custom_openapi():
-        if app.openapi_schema:
-            return app.openapi_schema
-
-        openapi_schema = get_openapi(title=project.project_name, version=project.config.version, routes=app.routes)
-        app.openapi_schema = openapi_schema
-        if config.openapi is not None:
-            always_merger.merge(app.openapi_schema.get('info'), config.openapi.get("info", {}))
-        return app.openapi_schema
-
-
     register_jsonapi_exception_handlers(app)
-
-    app.openapi = custom_openapi
+    app.openapi = lambda req: custom_openapi(project, config)
 
     analysis_app = create_analysis_apps(config, project)
 
-    logger().info("{} analysis found with `jinjat` config\n".format(len(analysis_app.routes)))
+    if len(analysis_app.routes) == 0:
+        logger().warning("Could not find any analysis found with `jinjat` config")
+    else:
+        logger().info(f"{len(analysis_app.routes)} analysis found with `jinjat` config")
 
     admin_app.router.add_route("/docs",
                                functools.partial(rapidoc_html,
                                                  CustomButton("Analysis APIs", f"/{project.config.version}/docs")),
                                include_in_schema=False)
     admin_app.version = project.config.version
     app.mount("/admin", admin_app)
@@ -116,37 +108,48 @@
     default_refine_project = os.path.join(get_project_root(), *["src", "jinjat", "jinjat-refine"])
     project_static_files = os.path.join(project.project_root, "static")
 
     static_files = main_directory = None
     if os.path.exists(project_static_files) and dbt_target.refine:
         static_files = StaticFiles(directory=project_static_files, html=True)
         static_files.all_directories = [project_static_files, default_refine_project]
-        main_directory = default_refine_project
     else:
         if os.path.exists(project_static_files):
             main_directory = project_static_files
         elif dbt_target.refine:
             main_directory = default_refine_project
 
         if main_directory is not None:
-            static_files = StaticFiles(directory=main_directory, html=True)
+            static_files = StaticFilesWithFallbackIndex(fallback_home_page_response=lambda scope: {
+                "analysis_api_docs": f"{extract_host(scope)}{project.config.version}/docs" if len(
+                    analysis_app.routes) > 0 else None,
+                "admin_api_docs": f"{extract_host(scope)}admin/docs",
+                "magic": "https://jinj.at",
+                "options": dbt_target.dict()
+            }, directory=main_directory, html=True)
 
     if static_files is not None:
         app.mount("/", static_files, name="static")
 
-    if main_directory is None or not os.path.exists(os.path.join(main_directory, "index.html")):
+    if static_files is None:
         app.router.add_route("/", lambda request: JSONResponse({
             "analysis_api_docs": f"{request.base_url}{project.config.version}/docs" if len(
                 analysis_app.routes) > 0 else None,
             "admin_api_docs": f"{request.base_url}admin/docs",
             "magic": "https://jin.jat",
             "options": dbt_target.dict()
         }))
 
 
+def get_multi_tenant_app(target: DbtTarget):
+    project = app.state.dbt_project_container.add_project(target)
+    mount_app(app, project, target)
+    return app
+
+
 # We use ambient reinitialization based on TTL now
 # loop = asyncio.get_running_loop()
 # project.heartbeat = loop.create_task(_adapter_heartbeat(project))
 async def _adapter_heartbeat(runner: DbtProject):
     """Equivalent of a keepalive for adapters such as Snowflake"""
     await asyncio.sleep(60 * 30)
     while runner.adapter_probe():
```

### Comparing `jinjat-0.4/src/jinjat/core/util/api.py` & `jinjat-0.5/src/jinjat/core/util/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import typing
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, List
 
+from starlette.exceptions import HTTPException as StarletteHttpException
 from fastapi.exceptions import HTTPException
 from pydantic import BaseModel, ValidationError
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, Response, JSONResponse
-
+from starlette.staticfiles import StaticFiles, PathLike
+from starlette.types import Scope
 
 DBT_PROJECT_HEADER = 'x-dbt-project-version'
 DBT_PROJECT_NAME = 'x-dbt-project-name'
 
 def get_human_readable_error(validation_error: ValidationError) -> str:
     error_str = "Validation errors:\n"
     for error in validation_error.errors():
@@ -181,8 +184,31 @@
 
     async def _serialize_error(request: Request, exc: Exception) -> Response:
         return serialize_error(exc)
 
     app.add_exception_handler(Exception, _serialize_error)
     app.add_exception_handler(HTTPException, _serialize_error)
 
+def extract_host(scope: dict):
+    for header in scope.get('headers'):
+        if header[0].lower() == 'host':
+            return header[0]
+    return "/"
+
+
+class StaticFilesWithFallbackIndex(StaticFiles):
+
+    def __init__(self, *, fallback_home_page_response : typing.Callable[[Scope], JSONResponse], directory: typing.Optional[PathLike] = None, packages: typing.Optional[
+        typing.List[typing.Union[str, typing.Tuple[str, str]]]
+    ] = None, html: bool = False, check_dir: bool = True) -> None:
+        super().__init__(directory=directory, packages=packages, html=html, check_dir=check_dir)
+        self.fallback_home_page_response = fallback_home_page_response
+
+    async def get_response(self, path: str, scope: Scope) -> Response:
+        response = None
+        try:
+            response = await super().get_response(path, scope)
+        except StarletteHttpException as e:
+            if e.status_code == 404 and path == '.':
+                return JSONResponse(self.fallback_home_page_response(scope))
+        return response
```

### Comparing `jinjat-0.4/src/jinjat/core/util/filesystem.py` & `jinjat-0.5/src/jinjat/core/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/src/jinjat/core/util/jmespath.py` & `jinjat-0.5/src/jinjat/core/util/jmespath.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/src/jinjat/main.py` & `jinjat-0.5/src/jinjat/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import functools
 import multiprocessing
-import os
 import subprocess
 import sys
 from pathlib import Path
 from typing import Callable, Optional
 
 import click
 import uvicorn
+import yaml
 from dbt.cli.option_types import YAML
 
-from jinjat.core.dbt.config import DEFAULT_PROFILES_DIR
 from jinjat.core.generator import compile_macro
 from jinjat.core.log_controller import logger
-from jinjat.core.server import DbtTarget, SERVER_OPT, app
+from jinjat.core.server import DbtTarget, get_multi_tenant_app
 
 CONTEXT = {"max_content_width": 800}
 
 
 @click.group()
 @click.version_option()
 def cli():
@@ -60,22 +59,23 @@
     return wrapper
 
 
 def shared_single_project_opts(func: Callable) -> Callable:
     @click.option(
         "--project-dir",
         type=click.Path(exists=True, dir_okay=True, file_okay=False),
+        envvar="DBT_PROJECT_DIR",
         default=str(Path.cwd()),
         help="Which directory to look in for the dbt_project.yml file. Default is the current working directory and its parents.",
     )
     @click.option(
         "--profiles-dir",
+        envvar="DBT_PROFILES_DIR",
         type=click.Path(exists=True, dir_okay=True, file_okay=False),
-        default=DEFAULT_PROFILES_DIR,
-        help="Which directory to look in for the profiles.yml file. Defaults to ~/.dbt",
+        help="Which directory to look in for the profiles.yml file. If not set, dbt will look in the current working directory first, then HOME/.dbt/",
     )
     @click.option(
         "-t",
         "--target",
         type=click.STRING,
         help="Which profile to load. Overrides setting in dbt_project.yml.",
     )
@@ -112,40 +112,42 @@
     is_flag=True
 )
 def generate(
         macro: str,
         args: dict,
         dry_run: bool,
         project_dir: str,
-        profiles_dir: str,
+        profiles_dir: Optional[str],
         target: Optional[str],
         vars: str
 ):
-    dbt_target = DbtTarget(project_dir=project_dir, profiles_dir=profiles_dir, target=target, vars=vars)
+    dbt_target = DbtTarget(project_dir=project_dir, profiles_dir=profiles_dir, target=target,
+                           vars=yaml.load(vars, Loader=yaml.Loader))
     compile_macro(dbt_target, macro, args, dry_run)
 
+
 @serve_project_opts
 @cli.command(context_settings=CONTEXT)
 @shared_single_project_opts
 @shared_server_opts
 def serve(
         project_dir: str,
-        profiles_dir: str,
+        profiles_dir: Optional[str],
         target: Optional[str],
         host: str,
         port: int,
         vars: str,
-        refine: bool,
+        refine: Optional[bool] = False,
 ) -> object:
-    logger().info(":water_wave: Executing jinjat in single-tenant mode")
+    logger().info(f":water_wave: Executing jinjat for dbt project in {project_dir}")
 
-    dbt_target = DbtTarget(project_dir=project_dir, profiles_dir=profiles_dir, target=target, vars=vars, refine=refine)
-    os.environ[SERVER_OPT] = dbt_target.json()
+    dbt_target = DbtTarget(project_dir=project_dir, profiles_dir=profiles_dir, target=target,
+                           vars=yaml.load(vars, Loader=yaml.Loader), refine=refine)
 
-    server = multiprocessing.Process(target=run_server, args=(host, port))
+    server = multiprocessing.Process(target=run_server, args=(host, port, dbt_target))
     server.start()
 
     import atexit
 
     atexit.register(lambda: server.terminate())
 
     server.join()
@@ -208,21 +210,21 @@
     subprocess.run(
         streamlit_command,
         env=os.environ,
         cwd=Path.cwd(),
     )
 
 
-def run_server(host="localhost", port=8581):
-    app.state.test = 1
+def run_server(host="localhost", port=8581, target=DbtTarget):
     uvicorn.run(
-        "jinjat.core.server:app",
+        lambda: get_multi_tenant_app(target),
         host=host,
         port=port,
         log_level="info",
         reload=False,
         workers=1,
+        factory=True
     )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `jinjat-0.4/src/jinjat/playground.py` & `jinjat-0.5/src/jinjat/playground.py`

 * *Files identical despite different names*

### Comparing `jinjat-0.4/setup.py` & `jinjat-0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,40 +6,43 @@
 
 packages = \
 ['jinjat',
  'jinjat.core',
  'jinjat.core.dbt',
  'jinjat.core.routes',
  'jinjat.core.schema',
- 'jinjat.core.util']
+ 'jinjat.core.util',
+ 'jinjat.deploy']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bottle>=0.12.23,<0.13.0',
  'click>7',
- 'dbt-core==1.4.5',
+ 'dbt-core==1.5.0',
  'deepmerge>=1.1.0,<2.0.0',
  'fastapi>=0.85.0,<0.86.0',
  'jinja2-simple-tags>=0.4.0,<0.5.0',
  'jmespath>=1.0.1,<2.0.0',
  'jsonref>=1.1.0,<2.0.0',
  'jsonschema>=3.0,<4.0',
  'openapi-schema-pydantic>=1.2.4,<2.0.0',
  'orjson>=3.8.0,<4.0.0',
  'pandas>=1.5.3,<2.0.0',
  'pydantic>=1.9.1,<2.0.0',
  'rich>=10',
  'ruamel.yaml>=0.17',
+ 'sqlglot==12.3.0',
  'uvicorn[standard]>=0.18.3,<0.19.0',
  'watchdog>=2.2.1']
 
 extras_require = \
-{'duckdb': ['duckcli>=0.2.1,<0.3.0', 'dbt-duckdb>=1.4.1,<2.0.0'],
+{':extra == "deploy"': ['fal-serverless==0.6.29', 'modal-client==0.49.2059'],
+ 'duckdb': ['duckcli>=0.2.1,<0.3.0', 'dbt-duckdb>=1.5.0,<2.0.0'],
  'playground': ['streamlit>=1.0.0',
                 'streamlit-ace>=0.1.0',
                 'graphviz>=0.17',
                 'pydot>=1.4.2',
                 'streamlit-agraph>=0.0.35',
                 'streamlit-pandas-profiling>=0.1.3',
                 'streamlit-aggrid>=0.2.2',
@@ -47,26 +50,26 @@
                 'feedparser>=6.0.10,<7.0.0']}
 
 entry_points = \
 {'console_scripts': ['jinjat = jinjat.main:cli']}
 
 setup_kwargs = {
     'name': 'jinjat',
-    'version': '0.4',
+    'version': '0.5',
     'description': 'A low-code data application framework that uses dbt Core and OpenAPI',
-    'long_description': '# Jinjat\n\n## Develop data applications with dbt, SQL, and OpenAPI\n\n### Installation\n\n```commandline\npip install jinjat\n```\n\n### Create your first API\n\nCreate an [analysis]() in `analysis/my_first_api.sql`:\n```sql\n{%- set query = request().query %}\n\nselect \'{{query.example}}\' as col1\n```\n\nAnd create a YML file in `analysis/schema.yml`:\n\n```yml\nversion: 2\n\nanalyses:\n  - name: my_first_api\n    config:\n      jinjat:\n        method: get\n        openapi:\n          parameters:\n            - in: query\n              name: example\n              schema:\n                type: number\n```\n\nStart Jinjat as follows:\n\n```commandline\njinjat serve --project-dir [YOUR_DBT_PROJECT_DIRECTORY]\n```\n\nAnd then run the following CURL command to test the API:\n\n```commandline\ncurl -XGET \'http://127.0.0.1:8581?example=value\'\n```\n\nIt should return the following response:\n\n```json\n[\n  "col1": "3"\n]\n```\n\nJinjat uses OpenAPI to validate the requests and create an API documentation automatically for your API.\n\n## Integrations\n\npoetry install --extras "duckdb"\n\n### Playground\n\npoetry install --extras "playground"\n\n\n#### Installation\n\n```commandline\npip install jinjat[playground]\n```\n\nJinjat Playground is a Streamlit app that lets you develop APIs in your browser.\nOnce you write the template, you can save it to your dbt project as an analysis and expose the API.\n\n### [Refine.dev](https://refine.dev) Integration\n\n#### Installation\n\n```commandline\npip install jinjat[refine]\n```\n\nJinjat Refine integration creates a Refine app from your OpenAPI spec \n\n\n> Jinjat is a fork of [dbt-osmosis](https://github.com/z3z1ma/dbt-osmosis)',
+    'long_description': '# Jinjat\n\n## Develop data applications with dbt, SQL, and OpenAPI\n\n### Installation\n\n```commandline\npip install jinjat\n```\n\n### Create your first API\n\nCreate an [analysis]() in `analysis/my_first_api.sql`:\n```sql\n{%- set query = request().query %}\n\nselect \'{{query.example}}\' as col1\n```\n\nAnd create a YML file in `analysis/schema.yml`:\n\n```yml\nversion: 2\n\nanalyses:\n  - name: my_first_api\n    config:\n      jinjat:\n        method: get\n        openapi:\n          parameters:\n            - in: query\n              name: example\n              schema:\n                type: number\n```\n\nStart Jinjat as follows:\n\n```commandline\njinjat serve --project-dir [YOUR_DBT_PROJECT_DIRECTORY]\n```\n\nAnd then run the following CURL command to test the API:\n\n```commandline\ncurl -XGET \'http://127.0.0.1:8581?example=value\'\n```\n\nIt should return the following response:\n\n```json\n[\n  "col1": "3"\n]\n```\n\nJinjat uses OpenAPI to validate the requests and create an API documentation automatically for your API.\n\n## Integrations\n\npoetry install --extras "duckdb"\n\n### Playground\n\npoetry install --extras "playground"\n\n\n#### Installation\n\n```commandline\npip install jinjat[playground]\n```\n\nJinjat Playground is a Streamlit app that lets you develop APIs in your browser.\nOnce you write the template, you can save it to your dbt project as an analysis and expose the API.',
     'author': 'buremba',
     'author_email': 'emrekabakci@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jinjat-data/jinjat',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.6,<4',
+    'python_requires': '>=3.8.1,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `jinjat-0.4/PKG-INFO` & `jinjat-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 Metadata-Version: 2.1
 Name: jinjat
-Version: 0.4
+Version: 0.5
 Summary: A low-code data application framework that uses dbt Core and OpenAPI
 Home-page: https://github.com/jinjat-data/jinjat
 License: Apache 2.0
 Keywords: dbt,server,streamlit,git,refine,data-app,snowflake
 Author: buremba
 Author-email: emrekabakci@gmail.com
-Requires-Python: >=3.6,<4
+Requires-Python: >=3.8.1,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Build Tools
+Provides-Extra: deploy
 Provides-Extra: duckdb
 Provides-Extra: playground
 Requires-Dist: bottle (>=0.12.23,<0.13.0)
 Requires-Dist: click (>7)
-Requires-Dist: dbt-core (==1.4.5)
-Requires-Dist: dbt-duckdb (>=1.4.1,<2.0.0) ; extra == "duckdb"
+Requires-Dist: dbt-core (==1.5.0)
+Requires-Dist: dbt-duckdb (>=1.5.0,<2.0.0) ; extra == "duckdb"
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: duckcli (>=0.2.1,<0.3.0) ; extra == "duckdb"
+Requires-Dist: fal-serverless (==0.6.29) ; extra == "deploy"
 Requires-Dist: fastapi (>=0.85.0,<0.86.0)
 Requires-Dist: feedparser (>=6.0.10,<7.0.0) ; extra == "playground"
 Requires-Dist: graphviz (>=0.17) ; extra == "playground"
 Requires-Dist: jinja2-simple-tags (>=0.4.0,<0.5.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
 Requires-Dist: jsonschema (>=3.0,<4.0)
+Requires-Dist: modal-client (==0.49.2059) ; extra == "deploy"
 Requires-Dist: openapi-schema-pydantic (>=1.2.4,<2.0.0)
 Requires-Dist: orjson (>=3.8.0,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pydot (>=1.4.2) ; extra == "playground"
 Requires-Dist: rich (>=10)
 Requires-Dist: ruamel.yaml (>=0.17)
 Requires-Dist: scipy (>=1.3.1,<2.0.0) ; extra == "playground"
+Requires-Dist: sqlglot (==12.3.0)
 Requires-Dist: streamlit (>=1.0.0) ; extra == "playground"
 Requires-Dist: streamlit-ace (>=0.1.0) ; extra == "playground"
 Requires-Dist: streamlit-aggrid (>=0.2.2) ; extra == "playground"
 Requires-Dist: streamlit-agraph (>=0.0.35) ; extra == "playground"
 Requires-Dist: streamlit-pandas-profiling (>=0.1.3) ; extra == "playground"
 Requires-Dist: uvicorn[standard] (>=0.18.3,<0.19.0)
 Requires-Dist: watchdog (>=2.2.1)
@@ -131,20 +132,7 @@
 
 ```commandline
 pip install jinjat[playground]
 ```
 
 Jinjat Playground is a Streamlit app that lets you develop APIs in your browser.
 Once you write the template, you can save it to your dbt project as an analysis and expose the API.
-
-### [Refine.dev](https://refine.dev) Integration
-
-#### Installation
-
-```commandline
-pip install jinjat[refine]
-```
-
-Jinjat Refine integration creates a Refine app from your OpenAPI spec 
-
-
-> Jinjat is a fork of [dbt-osmosis](https://github.com/z3z1ma/dbt-osmosis)
```

