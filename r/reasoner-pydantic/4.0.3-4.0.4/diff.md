# Comparing `tmp/reasoner-pydantic-4.0.3.tar.gz` & `tmp/reasoner-pydantic-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.0.3.tar", last modified: Fri May 12 22:46:32 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.0.4.tar", last modified: Sun May 14 21:42:53 2023, max compression
```

## Comparing `reasoner-pydantic-4.0.3.tar` & `reasoner-pydantic-4.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:46:32.166085 reasoner-pydantic-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-12 22:46:32.166085 reasoner-pydantic-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:46:32.162085 reasoner-pydantic-4.0.3/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 22:46:32.162085 reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-12 22:46:32.000000 reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-12 22:46:32.000000 reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:46:32.000000 reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 22:46:32.000000 reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 22:46:32.000000 reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 22:46:32.000000 reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 22:46:32.166085 reasoner-pydantic-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-12 22:46:28.000000 reasoner-pydantic-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:42:53.836713 reasoner-pydantic-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-14 21:42:53.836713 reasoner-pydantic-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:42:53.836713 reasoner-pydantic-4.0.4/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:42:53.836713 reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-14 21:42:53.000000 reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-14 21:42:53.000000 reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:42:53.000000 reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:42:53.000000 reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 21:42:53.000000 reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 21:42:53.000000 reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 21:42:53.836713 reasoner-pydantic-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-14 21:42:48.000000 reasoner-pydantic-4.0.4/setup.py
```

### Comparing `reasoner-pydantic-4.0.3/PKG-INFO` & `reasoner-pydantic-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.3
+Version: 4.0.4
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.3/README.md` & `reasoner-pydantic-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .results import Result, NodeBinding, EdgeBinding, Results, Analysis
 from .auxgraphs import AuxiliaryGraphs, AuxiliaryGraph
 from .message import (
     Message,
     Query,
     Response,
     AsyncQuery,
+    AsyncQueryResponse,
+    AsyncQueryStatusResponse,
 )
 from .workflow import (
     Operation,
     Workflow,
 )
 from .shared import (
     Attribute,
@@ -51,14 +53,16 @@
     QEdge,
     QNode,
     Query,
     QueryGraph,
     AsyncQuery,
     Result,
     Response,
+    AsyncQueryResponse,
+    AsyncQueryStatusResponse,
     LogLevel,
     AttributeConstraint,
     MetaEdge,
     MetaNode,
     MetaKnowledgeGraph,
     MetaAttribute,
     Results,
```

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/message.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,16 @@
             auxgraphs = AuxiliaryGraphs.parse_obj(obj["auxiliary_graphs"])
         m = Message(
             query_graph=qgraph,
             knowledge_graph=kgraph,
             results=results,
             auxiliary_graphs=auxgraphs,
         )
-        m._normalize_kg_edge_ids()
+        if m.knowledge_graph:
+            m._normalize_kg_edge_ids()
         m.update(message)
         return m
 
     def update(self, other: "Message"):
         if hash(self.query_graph) != hash(other.query_graph):
             raise NotImplementedError("Query graph merging not supported yet")
         # Make a copy because normalization will modify results
@@ -123,15 +124,17 @@
 
         # Update auxiliary graphs
         if self.auxiliary_graphs:
             for auxiliary_graph in self.auxiliary_graphs.__root__.values():
                 if auxiliary_graph.edges:
                     for aux_edge in auxiliary_graph.edges:
                         auxiliary_graph.edges.discard(aux_edge)
-                        auxiliary_graph.edges.add(edge_id_mapping[aux_edge])
+                        auxiliary_graph.edges.add(
+                            edge_id_mapping.get(aux_edge, aux_edge)
+                        )
 
         # Update results
         if self.results:
             for result in self.results.__root__:
                 if result and result.analyses:
                     for analysis in result.analyses:
                         for edge_binding_list in analysis.edge_bindings.values():
@@ -193,7 +196,37 @@
     status: Optional[str] = Field(None, nullable=True)
 
     workflow: Optional[Workflow]
 
     class Config:
         title = "response"
         extra = "allow"
+
+
+class AsyncQueryResponse(BaseModel):
+    """ "Async Query Response."""
+
+    status: Optional[str] = Field(None, nullable=True)
+
+    description: Optional[str] = Field(None, nullable=True)
+
+    job_id: str = Field(..., title="job id")
+
+    class Config:
+        title = "async query response"
+        extra = "allow"
+
+
+class AsyncQueryStatusResponse(BaseModel):
+    """Async Query Status Response."""
+
+    status: str = Field(..., title="status")
+
+    description: str = Field(..., title="description")
+
+    logs: Optional[HashableSet[LogEntry]] = Field(None, nullable=True)
+
+    response_url: Optional[str] = Field(None, nullable=True)
+
+    class Config:
+        title = "async query status response"
+        extra = "allow"
```

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/results.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/results.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.0.4/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.3
+Version: 4.0.4
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.3/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.0.4/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.3/setup.py` & `reasoner-pydantic-4.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.0.3",
+    version="4.0.4",
     author="Kenneth Morton",
     author_email="kenny@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

