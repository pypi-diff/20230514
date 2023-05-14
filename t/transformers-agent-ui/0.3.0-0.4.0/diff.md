# Comparing `tmp/transformers-agent-ui-0.3.0.tar.gz` & `tmp/transformers-agent-ui-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers-agent-ui-0.3.0.tar", last modified: Sun May 14 14:19:20 2023, max compression
+gzip compressed data, was "transformers-agent-ui-0.4.0.tar", last modified: Sun May 14 18:59:16 2023, max compression
```

## Comparing `transformers-agent-ui-0.3.0.tar` & `transformers-agent-ui-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/
--rw-r--r--   0 jovyan    (1000) users      (100)      119 2023-05-13 18:34:40.000000 transformers-agent-ui-0.3.0/MANIFEST.in
--rw-r--r--   0 jovyan    (1000) users      (100)     7603 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     5974 2023-05-14 14:02:08.000000 transformers-agent-ui-0.3.0/README.md
--rw-r--r--   0 jovyan    (1000) users      (100)     3580 2023-05-14 08:16:30.000000 transformers-agent-ui-0.3.0/pyproject.toml
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/setup.cfg
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.730807 transformers-agent-ui-0.3.0/src/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.730807 transformers-agent-ui-0.3.0/src/transformers_agent_ui/
--rw-r--r--   0 jovyan    (1000) users      (100)      237 2023-05-14 14:18:14.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/__init__.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.734807 transformers-agent-ui-0.3.0/src/transformers_agent_ui/assets/
--rw-r--r--   0 jovyan    (1000) users      (100)      110 2023-05-13 18:33:44.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/assets/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)   583422 2023-05-13 18:32:19.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/assets/image.png
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/
--rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:44:24.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     5103 2023-05-14 14:02:35.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/agent.py
--rw-r--r--   0 jovyan    (1000) users      (100)      813 2023-05-14 03:02:42.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/config.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3322 2023-05-14 08:38:27.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/custom_run.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1389 2023-05-14 07:43:57.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/run_input.py
--rw-r--r--   0 jovyan    (1000) users      (100)      243 2023-05-14 04:38:41.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/run_output.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4431 2023-05-14 07:41:15.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/store.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2166 2023-05-14 02:54:11.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/token.py
--rw-r--r--   0 jovyan    (1000) users      (100)       63 2023-05-13 16:01:28.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/py.typed
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.738807 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/
--rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:38:23.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1050 2023-05-14 05:19:49.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/asset_editor.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2146 2023-05-14 05:05:11.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/config.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1598 2023-05-14 02:39:37.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/token_manager.py
--rw-r--r--   0 jovyan    (1000) users      (100)     8043 2023-05-14 14:15:06.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/transformers_agent_ui.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 14:19:20.734807 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     7603 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     1020 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)      147 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-05-14 14:19:20.000000 transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/top_level.txt
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.541234 transformers-agent-ui-0.4.0/
+-rw-r--r--   0 jovyan    (1000) users      (100)      119 2023-05-13 18:34:40.000000 transformers-agent-ui-0.4.0/MANIFEST.in
+-rw-r--r--   0 jovyan    (1000) users      (100)     7849 2023-05-14 18:59:16.541234 transformers-agent-ui-0.4.0/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     6220 2023-05-14 18:43:25.000000 transformers-agent-ui-0.4.0/README.md
+-rw-r--r--   0 jovyan    (1000) users      (100)     3600 2023-05-14 18:08:48.000000 transformers-agent-ui-0.4.0/pyproject.toml
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-05-14 18:59:16.541234 transformers-agent-ui-0.4.0/setup.cfg
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.525234 transformers-agent-ui-0.4.0/src/
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.529234 transformers-agent-ui-0.4.0/src/transformers_agent_ui/
+-rw-r--r--   0 jovyan    (1000) users      (100)      237 2023-05-14 18:58:51.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/__init__.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.533234 transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/
+-rw-r--r--   0 jovyan    (1000) users      (100)      513 2023-05-14 18:38:27.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)   495733 2023-05-14 17:02:40.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/boat-in-water.png
+-rw-r--r--   0 jovyan    (1000) users      (100)   445847 2023-05-14 18:35:22.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/assets/capybara.png
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.537234 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/
+-rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:44:24.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     4993 2023-05-14 16:50:30.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/agent.py
+-rw-r--r--   0 jovyan    (1000) users      (100)      813 2023-05-14 03:02:42.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/config.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     3315 2023-05-14 16:51:53.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/custom_run.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1656 2023-05-14 18:56:46.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/examples.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1919 2023-05-14 17:46:18.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/run.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     4431 2023-05-14 07:41:15.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/store.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     2166 2023-05-14 02:54:11.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/token.py
+-rw-r--r--   0 jovyan    (1000) users      (100)       63 2023-05-13 16:01:28.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/py.typed
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.541234 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/
+-rw-r--r--   0 jovyan    (1000) users      (100)        0 2023-05-14 02:38:23.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/__init__.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1707 2023-05-14 18:17:54.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/components.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     2146 2023-05-14 05:05:11.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/config.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     1598 2023-05-14 02:39:37.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/token_manager.py
+-rw-r--r--   0 jovyan    (1000) users      (100)     8261 2023-05-14 18:15:17.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/transformers_agent_ui.py
+drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2023-05-14 18:59:16.529234 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)     7849 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)     1064 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)      147 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/requires.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       22 2023-05-14 18:59:16.000000 transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/top_level.txt
```

### Comparing `transformers-agent-ui-0.3.0/PKG-INFO` & `transformers-agent-ui-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-agent-ui
-Version: 0.3.0
+Version: 0.4.0
 Summary: This package makes it super simple to do exploratory data analysis and develop high-quality Panel data apps ...
 Author: awesome-panel
 Project-URL: repository, https://github.com/awesome-panel/transformers-agent-ui
 Keywords: python,huggingface,transformers,deeplearning,ai,agent,holoviz,panel
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -168,22 +168,26 @@
 - [ ] Support enabled `remote` parameter setting. Currently we only support `remote`.
 - [ ] Don't save asset if from cache. Instead reuse.
 - [ ] Make the Cache/ Store useful by providing an interface
 - [ ] Multi user support
   - [ ] Restrict logs to user session
     - See also [hf #23354](https://github.com/huggingface/transformers/issues/23354)
   - [ ] Restrict store to user session
-- [ ] Deploy to Hugging Face
+  - [ ] Make application non-blocking when used by multiple users
+- [ ] Deploy to Hugging Face. I probably wont be able to as the app needs a lot of power when
+running locally.
 - [ ] Build a sample store and collect data on runs
 - [ ] Enable downloading the output value
 - [ ] Help the app and/ or Panel display the outputs. For example when a tensor is returned Panel
 - [ ] Specifically test that the output of each tool is supported
 does not know how to display that. And the agent fails if we ask it to return the value wrapped in
 a HoloViz Panel Audio Pane. See [Panel #4836](https://github.com/holoviz/panel/issues/4836)
 - [ ] Profile the `run` and figure out if for example agents should be reused/ cached
+- [ ] Prompt seems to be cut of when displayed in the UI. Fix this
 
-## Maybe list
+## Maybe later list
 
 - [ ] Make the project more specific by calling it hfagent-ui and providing HFAgentUI,
 - [ ] Make the project more general as in agent-ui. We could provide HFAgentUI,
 LangChainAgentUI etc. Or maybe even just AgentUI. Much of the code would be reusable.
 - [ ] Run inference async to make app more performant if possible
+- [ ] Support chat mode.
```

### Comparing `transformers-agent-ui-0.3.0/README.md` & `transformers-agent-ui-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -133,22 +133,26 @@
 - [ ] Support enabled `remote` parameter setting. Currently we only support `remote`.
 - [ ] Don't save asset if from cache. Instead reuse.
 - [ ] Make the Cache/ Store useful by providing an interface
 - [ ] Multi user support
   - [ ] Restrict logs to user session
     - See also [hf #23354](https://github.com/huggingface/transformers/issues/23354)
   - [ ] Restrict store to user session
-- [ ] Deploy to Hugging Face
+  - [ ] Make application non-blocking when used by multiple users
+- [ ] Deploy to Hugging Face. I probably wont be able to as the app needs a lot of power when
+running locally.
 - [ ] Build a sample store and collect data on runs
 - [ ] Enable downloading the output value
 - [ ] Help the app and/ or Panel display the outputs. For example when a tensor is returned Panel
 - [ ] Specifically test that the output of each tool is supported
 does not know how to display that. And the agent fails if we ask it to return the value wrapped in
 a HoloViz Panel Audio Pane. See [Panel #4836](https://github.com/holoviz/panel/issues/4836)
 - [ ] Profile the `run` and figure out if for example agents should be reused/ cached
+- [ ] Prompt seems to be cut of when displayed in the UI. Fix this
 
-## Maybe list
+## Maybe later list
 
 - [ ] Make the project more specific by calling it hfagent-ui and providing HFAgentUI,
 - [ ] Make the project more general as in agent-ui. We could provide HFAgentUI,
 LangChainAgentUI etc. Or maybe even just AgentUI. Much of the code would be reusable.
 - [ ] Run inference async to make app more performant if possible
+- [ ] Support chat mode.
```

### Comparing `transformers-agent-ui-0.3.0/pyproject.toml` & `transformers-agent-ui-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 max-args=10
 
 [tool.pylint.format]
 max-module-lines = 1000
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 100
-disable = []
+disable = ["too-many-ancestors"]
 
 [tool.mypy]
 python_version = "3.9"
 namespace_packages = true
 explicit_package_bases = true
 mypy_path = "src"
 exclude = []
```

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/agent.py` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 from datetime import datetime
 
 import param
 from transformers import HfAgent, OpenAiAgent
 
 from transformers_agent_ui.domain.config import AGENT_CONFIGURATION
 from transformers_agent_ui.domain.custom_run import run
-from transformers_agent_ui.domain.run_input import RunInput
-from transformers_agent_ui.domain.run_output import RunOutput
+from transformers_agent_ui.domain.run import Run
 from transformers_agent_ui.domain.store import Store
 from transformers_agent_ui.domain.token import TokenManager
 
 log = logging.getLogger(__name__)
 
 
 def _get_agent(agent, model, token):
@@ -33,15 +32,15 @@
             **params,
             api_key=token,
         )
 
     raise ValueError(f"The agent {agent} and model {model} is not supported")
 
 
-class TransformersAgent(RunInput, RunOutput, param.Parameterized):
+class TransformersAgent(Run):
     """A wrapper of the Hugging Face transformers agent. See
     https://huggingface.co/docs/transformers/transformers_agents"""
 
     remote = param.Boolean(default=True, readonly=True)
 
     is_running = param.Boolean()
```

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/config.py` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/config.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/custom_run.py` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/custom_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from transformers.tools.agents import (
     clean_code_for_run,
     get_tool_creation_code,
     resolve_tools,
 )
 from transformers.tools.python_interpreter import InterpretorError, evaluate_ast
 
-from transformers_agent_ui.domain.run_output import RunOutput
+from transformers_agent_ui.domain.run import RunOutput
 
 
 # Source: transformers/tools/python_interpreter.py
 def evaluate(code: str, tools: Dict[str, Callable], state=None):
     """
     Evaluate a python expression using the content of the variables stored in a state and only
     evaluating a given set of functions.
```

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/store.py` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/store.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui/domain/token.py` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui/domain/token.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/config.py` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/config.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/token_manager.py` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/token_manager.py`

 * *Files identical despite different names*

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui/ui/transformers_agent_ui.py` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui/ui/transformers_agent_ui.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Provides the TransformersAgentUI"""
 import numpy as np
 import panel as pn
 import param
 from torch import Tensor
 
 from transformers_agent_ui.domain.agent import TransformersAgent
-from transformers_agent_ui.ui.asset_editor import AssetEditor
+from transformers_agent_ui.ui.components import (
+    KwargsEditor,
+    get_example_selection_widget,
+)
 from transformers_agent_ui.ui.config import (
     CONFIG,
     STYLES,
     TransformersAgentUIConfig,
     TransformersAgentUIStyles,
 )
 from transformers_agent_ui.ui.token_manager import TokenManagerUI
@@ -87,31 +90,33 @@
     def _create_editor(self):
         agent_input = pn.widgets.RadioButtonGroup.from_param(
             self.param.agent, margin=(5, 0), button_style="outline"
         )
         model_input = pn.widgets.RadioButtonGroup.from_param(
             self.param.model, button_style="outline"
         )
+        example_input = get_example_selection_widget(task=self)
         task_input = pn.widgets.TextAreaInput.from_param(
             self.param.task,
             sizing_mode="stretch_width",
             name="Task",
             stylesheets=["textarea { font-size: 2em; }"],
+            description="A short text describing the task to run",
         )
         submit_input = pn.widgets.Button.from_param(
             self.param.submit,
             button_type="primary",
             sizing_mode="stretch_width",
             disabled=self.param.is_running,
             loading=self.param.is_running,
             stylesheets=[self.styles.submit_button_style_sheet],
             name="RUN",
         )
         task_input = pn.Column(task_input, submit_input)
-        assets_input = AssetEditor(self.kwargs)
+        assets_input = KwargsEditor(kwargs=self.param.kwargs)
 
         inputs = pn.Column(
             pn.Row(
                 pn.pane.HTML(
                     "Agent",
                     styles={
                         "padding-top": "0.5em",
@@ -126,14 +131,15 @@
                     },
                 ),
                 model_input,
                 align="start",
             ),
             pn.Row(self.param.use_cache, self.param.remote, margin=(15, 5)),
             pn.Column(
+                example_input,
                 task_input,
                 pn.pane.HTML("Arguments", margin=(0, 10)),
                 pn.pane.Alert(
                     """You can refer to *arguments* in your task by their names. For example \
                         'image'. You can  also refer to the output value on the right via the name \
                         'value'.""",
                     alert_type="warning",
```

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/PKG-INFO` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-agent-ui
-Version: 0.3.0
+Version: 0.4.0
 Summary: This package makes it super simple to do exploratory data analysis and develop high-quality Panel data apps ...
 Author: awesome-panel
 Project-URL: repository, https://github.com/awesome-panel/transformers-agent-ui
 Keywords: python,huggingface,transformers,deeplearning,ai,agent,holoviz,panel
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -168,22 +168,26 @@
 - [ ] Support enabled `remote` parameter setting. Currently we only support `remote`.
 - [ ] Don't save asset if from cache. Instead reuse.
 - [ ] Make the Cache/ Store useful by providing an interface
 - [ ] Multi user support
   - [ ] Restrict logs to user session
     - See also [hf #23354](https://github.com/huggingface/transformers/issues/23354)
   - [ ] Restrict store to user session
-- [ ] Deploy to Hugging Face
+  - [ ] Make application non-blocking when used by multiple users
+- [ ] Deploy to Hugging Face. I probably wont be able to as the app needs a lot of power when
+running locally.
 - [ ] Build a sample store and collect data on runs
 - [ ] Enable downloading the output value
 - [ ] Help the app and/ or Panel display the outputs. For example when a tensor is returned Panel
 - [ ] Specifically test that the output of each tool is supported
 does not know how to display that. And the agent fails if we ask it to return the value wrapped in
 a HoloViz Panel Audio Pane. See [Panel #4836](https://github.com/holoviz/panel/issues/4836)
 - [ ] Profile the `run` and figure out if for example agents should be reused/ cached
+- [ ] Prompt seems to be cut of when displayed in the UI. Fix this
 
-## Maybe list
+## Maybe later list
 
 - [ ] Make the project more specific by calling it hfagent-ui and providing HFAgentUI,
 - [ ] Make the project more general as in agent-ui. We could provide HFAgentUI,
 LangChainAgentUI etc. Or maybe even just AgentUI. Much of the code would be reusable.
 - [ ] Run inference async to make app more performant if possible
+- [ ] Support chat mode.
```

### Comparing `transformers-agent-ui-0.3.0/src/transformers_agent_ui.egg-info/SOURCES.txt` & `transformers-agent-ui-0.4.0/src/transformers_agent_ui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 src/transformers_agent_ui/py.typed
 src/transformers_agent_ui.egg-info/PKG-INFO
 src/transformers_agent_ui.egg-info/SOURCES.txt
 src/transformers_agent_ui.egg-info/dependency_links.txt
 src/transformers_agent_ui.egg-info/requires.txt
 src/transformers_agent_ui.egg-info/top_level.txt
 src/transformers_agent_ui/assets/__init__.py
-src/transformers_agent_ui/assets/image.png
+src/transformers_agent_ui/assets/boat-in-water.png
+src/transformers_agent_ui/assets/capybara.png
 src/transformers_agent_ui/domain/__init__.py
 src/transformers_agent_ui/domain/agent.py
 src/transformers_agent_ui/domain/config.py
 src/transformers_agent_ui/domain/custom_run.py
-src/transformers_agent_ui/domain/run_input.py
-src/transformers_agent_ui/domain/run_output.py
+src/transformers_agent_ui/domain/examples.py
+src/transformers_agent_ui/domain/run.py
 src/transformers_agent_ui/domain/store.py
 src/transformers_agent_ui/domain/token.py
 src/transformers_agent_ui/ui/__init__.py
-src/transformers_agent_ui/ui/asset_editor.py
+src/transformers_agent_ui/ui/components.py
 src/transformers_agent_ui/ui/config.py
 src/transformers_agent_ui/ui/token_manager.py
 src/transformers_agent_ui/ui/transformers_agent_ui.py
```

