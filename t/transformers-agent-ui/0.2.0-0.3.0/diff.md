# Comparing `tmp/transformers-agent-ui-0.2.0.tar.gz` & `tmp/transformers-agent-ui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers-agent-ui-0.2.0.tar", last modified: Sun May 14 09:27:00 2023, max compression
+gzip compressed data, was "transformers-agent-ui-0.3.0.tar", last modified: Sun May 14 14:19:20 2023, max compression
```

## Comparing `transformers-agent-ui-0.2.0.tar` & `transformers-agent-ui-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 09:27:00.670714 transformers-agent-ui-0.2.0/
--rw-r--r--   0 jovyan    (1000) users      (100)      119 2023-05-13 18:34:40.000000 transformers-agent-ui-0.2.0/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     7397 2023-05-14 09:27:00.670714 transformers-agent-ui-0.2.0/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     5768 2023-05-14 09:18:16.000000 transformers-agent-ui-0.2.0/README.md
--rw-r--r--   0 jovyan    (1000) users      (100)     3580 2023-05-14 08:16:30.000000 transformers-agent-ui-0.2.0/pyproject.toml
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-14 09:27:00.670714 transformers-agent-ui-0.2.0/setup.cfg
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 09:27:00.662714 transformers-agent-ui-0.2.0/src/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 09:27:00.662714 transformers-agent-ui-0.2.0/src/transformers_agent_ui/
--rw-r--r--   0 jovyan    (1000) users      (100)      237 2023-05-14 09:25:18.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/__init__.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 09:27:00.666714 transformers-agent-ui-0.2.0/src/transformers_agent_ui/assets/
--rw-r--r--   0 jovyan    (1000) users      (100)      110 2023-05-13 18:33:44.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/assets/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)   583422 2023-05-13 18:32:19.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/assets/image.png
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 09:27:00.670714 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/
--rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:44:24.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     5107 2023-05-14 09:11:25.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/agent.py
--rw-r--r--   0 jovyan    (1000) users      (100)      813 2023-05-14 03:02:42.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/config.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3322 2023-05-14 08:38:27.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/custom_run.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1389 2023-05-14 07:43:57.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/run_input.py
--rw-r--r--   0 jovyan    (1000) users      (100)      243 2023-05-14 04:38:41.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/run_output.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4431 2023-05-14 07:41:15.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/store.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2166 2023-05-14 02:54:11.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/token.py
--rw-r--r--   0 jovyan    (1000) users      (100)       63 2023-05-13 16:01:28.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/py.typed
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 09:27:00.670714 transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/
--rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:38:23.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1050 2023-05-14 05:19:49.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/asset_editor.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2146 2023-05-14 05:05:11.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/config.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1598 2023-05-14 02:39:37.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/token_manager.py
--rw-r--r--   0 jovyan    (1000) users      (100)     7293 2023-05-14 09:12:45.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/transformers_agent_ui.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 09:27:00.666714 transformers-agent-ui-0.2.0/src/transformers_agent_ui.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     7397 2023-05-14 09:27:00.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     1020 2023-05-14 09:27:00.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-14 09:27:00.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      147 2023-05-14 09:27:00.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-05-14 09:27:00.000000 transformers-agent-ui-0.2.0/src/transformers_agent_ui.egg-info/top_level.txt
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/
+-rw-r--r--   0 jovyan    (1000) users      (100)      119 2023-05-13 18:34:40.000000 transformers-agent-ui-0.3.0/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     7603 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     5974 2023-05-14 14:02:08.000000 transformers-agent-ui-0.3.0/README.md
+-rw-r--r--   0 jovyan    (1000) users      (100)     3580 2023-05-14 08:16:30.000000 transformers-agent-ui-0.3.0/pyproject.toml
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/setup.cfg
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.730807 transformers-agent-ui-0.3.0/src/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.730807 transformers-agent-ui-0.3.0/src/transformers_agent_ui/
+-rw-r--r--   0 jovyan    (1000) users      (100)      237 2023-05-14 14:18:14.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/__init__.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.734807 transformers-agent-ui-0.3.0/src/transformers_agent_ui/assets/
+-rw-r--r--   0 jovyan    (1000) users      (100)      110 2023-05-13 18:33:44.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/assets/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)   583422 2023-05-13 18:32:19.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/assets/image.png
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/
+-rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:44:24.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     5103 2023-05-14 14:02:35.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/agent.py
+-rw-r--r--   0 jovyan    (1000) users      (100)      813 2023-05-14 03:02:42.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/config.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     3322 2023-05-14 08:38:27.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/custom_run.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1389 2023-05-14 07:43:57.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/run_input.py
+-rw-r--r--   0 jovyan    (1000) users      (100)      243 2023-05-14 04:38:41.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/run_output.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     4431 2023-05-14 07:41:15.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/store.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     2166 2023-05-14 02:54:11.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/token.py
+-rw-r--r--   0 jovyan    (1000) users      (100)       63 2023-05-13 16:01:28.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/py.typed
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/
+-rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:38:23.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1050 2023-05-14 05:19:49.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/asset_editor.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     2146 2023-05-14 05:05:11.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/config.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1598 2023-05-14 02:39:37.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/token_manager.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     8043 2023-05-14 14:15:06.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/transformers_agent_ui.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.734807 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     7603 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     1020 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      147 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/top_level.txt
```

### Comparing `transformers-agent-ui-0.2.0/PKG-INFO` & `transformers-agent-ui-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-agent-ui
-Version: 0.2.0
+Version: 0.3.0
 Summary: This package makes it super simple to do exploratory data analysis and develop high-quality Panel data apps ...
 Author: awesome-panel
 Project-URL: repository, https://github.com/awesome-panel/transformers-agent-ui
 Keywords: python,huggingface,transformers,deeplearning,ai,agent,holoviz,panel
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -159,28 +159,31 @@
   - [x] As inputs to .run
   - [ ] Create/ Update from file
   - [ ] Create/ Update from output
   - [ ] Delete/ Remove
 - [ ] Get better feedback on run exceptions back
 - [ ] Test it on lots of examples
   - [ ] Add specific support for reading and writing more types. Currently most things are pickled.
+    - torch.Tensor is often returned and can be saved
 - [ ] Add three examples to make it easy to get started
 - [ ] Support enabled `remote` parameter setting. Currently we only support `remote`.
 - [ ] Don't save asset if from cache. Instead reuse.
 - [ ] Make the Cache/ Store useful by providing an interface
 - [ ] Multi user support
   - [ ] Restrict logs to user session
     - See also [hf #23354](https://github.com/huggingface/transformers/issues/23354)
   - [ ] Restrict store to user session
 - [ ] Deploy to Hugging Face
 - [ ] Build a sample store and collect data on runs
 - [ ] Enable downloading the output value
 - [ ] Help the app and/ or Panel display the outputs. For example when a tensor is returned Panel
+- [ ] Specifically test that the output of each tool is supported
 does not know how to display that. And the agent fails if we ask it to return the value wrapped in
 a HoloViz Panel Audio Pane. See [Panel #4836](https://github.com/holoviz/panel/issues/4836)
+- [ ] Profile the `run` and figure out if for example agents should be reused/ cached
 
 ## Maybe list
 
 - [ ] Make the project more specific by calling it hfagent-ui and providing HFAgentUI,
 - [ ] Make the project more general as in agent-ui. We could provide HFAgentUI,
 LangChainAgentUI etc. Or maybe even just AgentUI. Much of the code would be reusable.
 - [ ] Run inference async to make app more performant if possible
```

### Comparing `transformers-agent-ui-0.2.0/README.md` & `transformers-agent-ui-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -124,28 +124,31 @@
   - [x] As inputs to .run
   - [ ] Create/ Update from file
   - [ ] Create/ Update from output
   - [ ] Delete/ Remove
 - [ ] Get better feedback on run exceptions back
 - [ ] Test it on lots of examples
   - [ ] Add specific support for reading and writing more types. Currently most things are pickled.
+    - torch.Tensor is often returned and can be saved
 - [ ] Add three examples to make it easy to get started
 - [ ] Support enabled `remote` parameter setting. Currently we only support `remote`.
 - [ ] Don't save asset if from cache. Instead reuse.
 - [ ] Make the Cache/ Store useful by providing an interface
 - [ ] Multi user support
   - [ ] Restrict logs to user session
     - See also [hf #23354](https://github.com/huggingface/transformers/issues/23354)
   - [ ] Restrict store to user session
 - [ ] Deploy to Hugging Face
 - [ ] Build a sample store and collect data on runs
 - [ ] Enable downloading the output value
 - [ ] Help the app and/ or Panel display the outputs. For example when a tensor is returned Panel
+- [ ] Specifically test that the output of each tool is supported
 does not know how to display that. And the agent fails if we ask it to return the value wrapped in
 a HoloViz Panel Audio Pane. See [Panel #4836](https://github.com/holoviz/panel/issues/4836)
+- [ ] Profile the `run` and figure out if for example agents should be reused/ cached
 
 ## Maybe list
 
 - [ ] Make the project more specific by calling it hfagent-ui and providing HFAgentUI,
 - [ ] Make the project more general as in agent-ui. We could provide HFAgentUI,
 LangChainAgentUI etc. Or maybe even just AgentUI. Much of the code would be reusable.
 - [ ] Run inference async to make app more performant if possible
```

### Comparing `transformers-agent-ui-0.2.0/pyproject.toml` & `transformers-agent-ui-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/assets/image.png` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/assets/image.png`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/agent.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def _get_run_kwargs(self):
         """Returns the kwargs with the 'output' added"""
         if self.kwargs:
             kwargs = self.kwargs.copy()
         else:
             kwargs = {}
-        if self.value and "value" not in kwargs:
+        if self.value is not None and "value" not in kwargs:
             kwargs["value"] = self.value
         return kwargs
 
     def run(self):
         """Runs the agent, model on the `value`"""
         exception_raised = False
 
@@ -127,15 +127,15 @@
                 value=self.value,
             )
             print(self.value)
         elif not exception_raised:
             self._handle_no_result()
 
         if self.value is None or self.value == "":
-            self.value = "No output generated. Check the logs"
+            self.value = "No output generated"
 
         self.is_running = False
         return self.value
 
     def _handle_no_result(self):
         print("No result returned")
```

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/config.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/config.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/custom_run.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/custom_run.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/run_input.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/run_input.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/store.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/store.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/domain/token.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/token.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/asset_editor.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/asset_editor.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/config.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/config.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/token_manager.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/token_manager.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui/ui/transformers_agent_ui.py` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/transformers_agent_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Provides the TransformersAgentUI"""
+import numpy as np
 import panel as pn
 import param
+from torch import Tensor
 
 from transformers_agent_ui.domain.agent import TransformersAgent
 from transformers_agent_ui.ui.asset_editor import AssetEditor
 from transformers_agent_ui.ui.config import (
     CONFIG,
     STYLES,
     TransformersAgentUIConfig,
@@ -171,41 +173,62 @@
             ("CODE", pn.widgets.Terminal(self.code)),
             ("EXPLANATION", self.explanation),
             ("PROMPT", self.prompt),
             align="center",
             sizing_mode="stretch_width",
         )
 
+    def _get_last_tool(self) -> str:
+        """Returns the last tool used in the code"""
+        code = self.code
+
+        if not code:
+            return "NA"
+
+        lines = code.splitlines()
+        if "text_reader" in lines[-1]:
+            return "text_reader"
+        return ""
+
     def get_value_pane(self):
         """Returns a converted value that can be displayed by Panel"""
         # Here we should help the agent return something that can be displayed
-        return self.value
+        value = self.value
+        tool = self._get_last_tool()
+
+        if tool == "text_reader":
+            if isinstance(value, Tensor) and hasattr(value, "numpy"):
+                value = value.numpy()  # pylint: disable=no-member
+            if isinstance(value, np.ndarray) and value.dtype in (np.float32,):
+                value = (value * 32768.0).astype(np.int16)
+            if isinstance(value, np.ndarray):
+                return pn.pane.Audio(value, sample_rate=16000)
+
+        return value
 
     @pn.depends("submit", watch=True)
     def _submit(self):
         self.run()
 
     def _handle_no_token(self, agent):
         message = f"No token found for agent '{agent}'. Please provide one."
         print(message)
         if pn.state.notifications:
-            pn.state.notifications.error(message, duration=0)
+            pn.state.notifications.error(message, duration=12000)
 
     def _handle_run_exception(self, exc: Exception):
         # openai.error.RateLimitError: You exceeded your current quota, please check your plan
         # and billing details.
         print(exc)
         if pn.state.notifications:
-            pn.state.notifications.error(  # type: ignore
-                f"The run failed: {exc}." + " Check the logs.", duration=0
-            )
+            pn.state.notifications.error(f"The run failed: {exc}.", duration=12000)  # type: ignore
 
     def _handle_no_result(self):
         message = "No result returned"
         print(message)
         if pn.state.notifications:
-            pn.state.notifications.error(message + " Check the logs.", duration=0)
+            pn.state.notifications.error(message, duration=12000)
 
 
 if pn.state.served:
     pn.extension("terminal", "notifications", notifications=True, design="bootstrap")
     TransformersAgentUI().servable()
```

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui.egg-info/PKG-INFO` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-agent-ui
-Version: 0.2.0
+Version: 0.3.0
 Summary: This package makes it super simple to do exploratory data analysis and develop high-quality Panel data apps ...
 Author: awesome-panel
 Project-URL: repository, https://github.com/awesome-panel/transformers-agent-ui
 Keywords: python,huggingface,transformers,deeplearning,ai,agent,holoviz,panel
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -159,28 +159,31 @@
   - [x] As inputs to .run
   - [ ] Create/ Update from file
   - [ ] Create/ Update from output
   - [ ] Delete/ Remove
 - [ ] Get better feedback on run exceptions back
 - [ ] Test it on lots of examples
   - [ ] Add specific support for reading and writing more types. Currently most things are pickled.
+    - torch.Tensor is often returned and can be saved
 - [ ] Add three examples to make it easy to get started
 - [ ] Support enabled `remote` parameter setting. Currently we only support `remote`.
 - [ ] Don't save asset if from cache. Instead reuse.
 - [ ] Make the Cache/ Store useful by providing an interface
 - [ ] Multi user support
   - [ ] Restrict logs to user session
     - See also [hf #23354](https://github.com/huggingface/transformers/issues/23354)
   - [ ] Restrict store to user session
 - [ ] Deploy to Hugging Face
 - [ ] Build a sample store and collect data on runs
 - [ ] Enable downloading the output value
 - [ ] Help the app and/ or Panel display the outputs. For example when a tensor is returned Panel
+- [ ] Specifically test that the output of each tool is supported
 does not know how to display that. And the agent fails if we ask it to return the value wrapped in
 a HoloViz Panel Audio Pane. See [Panel #4836](https://github.com/holoviz/panel/issues/4836)
+- [ ] Profile the `run` and figure out if for example agents should be reused/ cached
 
 ## Maybe list
 
 - [ ] Make the project more specific by calling it hfagent-ui and providing HFAgentUI,
 - [ ] Make the project more general as in agent-ui. We could provide HFAgentUI,
 LangChainAgentUI etc. Or maybe even just AgentUI. Much of the code would be reusable.
 - [ ] Run inference async to make app more performant if possible
```

### Comparing `transformers-agent-ui-0.2.0/src/transformers_agent_ui.egg-info/SOURCES.txt` & `transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

