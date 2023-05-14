# Comparing `tmp/ItsPrompt-1.2.tar.gz` & `tmp/ItsPrompt-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ItsPrompt-1.2.tar", last modified: Sun May  7 11:29:09 2023, max compression
+gzip compressed data, was "ItsPrompt-1.3.tar", last modified: Sun May 14 14:06:15 2023, max compression
```

## Comparing `ItsPrompt-1.2.tar` & `ItsPrompt-1.3.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.441138 ItsPrompt-1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.433138 ItsPrompt-1.2/ItsPrompt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.437138 ItsPrompt-1.2/ItsPrompt/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/keyboard_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.437138 ItsPrompt-1.2/ItsPrompt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/raw_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.437138 ItsPrompt-1.2/ItsPrompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 11:28:58.000000 ItsPrompt-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-05-07 11:29:09.441138 ItsPrompt-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-05-07 11:28:58.000000 ItsPrompt-1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-07 11:28:58.000000 ItsPrompt-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 11:29:09.441138 ItsPrompt-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.027732 ItsPrompt-1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.023732 ItsPrompt-1.3/ItsPrompt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.023732 ItsPrompt-1.3/ItsPrompt/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/keyboard_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.027732 ItsPrompt-1.3/ItsPrompt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/confirm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/raw_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.023732 ItsPrompt-1.3/ItsPrompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-14 14:06:02.000000 ItsPrompt-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-14 14:06:15.027732 ItsPrompt-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-05-14 14:06:02.000000 ItsPrompt-1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-14 14:06:02.000000 ItsPrompt-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:06:15.027732 ItsPrompt-1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.027732 ItsPrompt-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-14 14:06:02.000000 ItsPrompt-1.3/tests/test_prompt.py
```

### Comparing `ItsPrompt-1.2/ItsPrompt/data/checkbox.py` & `ItsPrompt-1.3/ItsPrompt/data/checkbox.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.2/ItsPrompt/data/expand.py` & `ItsPrompt-1.3/ItsPrompt/data/expand.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     :raises ValueError: If the keys are not ascii
     :raises ValueError: If the keys are using h
     :raises TypeError: If an option is not processable
     :return: A list of `ExpandOptions`
     :rtype: list[ExpandOption]
     '''
     # check if every key is unique, otherwise return error
-    if any([options.count(option[0]) > 1 for option in options]):
+    keys = [option[0] for option in options]
+    if len(set(keys)) < len(keys):
         raise ValueError('Keys must be unique!')
 
     # check that every key string is only one char long
     if any([len(option[0]) > 1 or len(option[0]) < 1 for option in options]):
         raise ValueError('Keys must be of length 1!')
 
     # check that every key is ascii
```

### Comparing `ItsPrompt-1.2/ItsPrompt/data/select.py` & `ItsPrompt-1.3/ItsPrompt/data/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,18 @@
     :rtype: list[SelectOption]
     '''
     processed_options: list[SelectOption] = []
 
     # process given options
     for option in options:
         if type(option) is str:
-            processed_options.append(
-                SelectOption(
-                    name=option,
-                    id=option,
-                ))
+            processed_options.append(SelectOption(
+                name=option,
+                id=option,
+            ))
         elif type(option) is tuple:
             processed_options.append(
                 SelectOption(
                     name=option[0],
                     id=option[1],
                 ))
         else:
```

### Comparing `ItsPrompt-1.2/ItsPrompt/data/style.py` & `ItsPrompt-1.3/ItsPrompt/data/style.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.2/ItsPrompt/data/table.py` & `ItsPrompt-1.3/ItsPrompt/data/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         # add headers
         for header in self.data.columns:
             table_out[
                 0] += '─' * self.cell_width + self._char_if_last_else_otherchar(
                     header, '┐', '┬')
 
             if len(str(header)) > self.cell_width:
-                # convert the header to str in case the user did not give a header, so it is an integer
+                #   /\ convert the header to str in case the user did not give a header, so it is an integer
                 header = header[:self.cell_width - 1] + '.'
 
             table_out[1] += f'{header:^{self.cell_width}}' + '│'
 
         # add values, iterate over each column
         for header, values in self.data.items():
             # iterate over each row
```

### Comparing `ItsPrompt-1.2/ItsPrompt/keyboard_handler.py` & `ItsPrompt-1.3/ItsPrompt/keyboard_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,26 +65,28 @@
         event.app.on_enter()  # type: ignore
 
     @kb.add('space', filter=hasattr(app, 'on_space'))
     def space(event: KeyPressEvent):
         event.app.on_space()  # type: ignore
 
     @kb.add('escape', 'enter', filter=hasattr(app, 'on_alt_enter'))
+    # Vt100 terminals convert "alt+key" to "escape,key"
     def alt_enter(event: KeyPressEvent):
         event.app.on_alt_enter()  # type: ignore
 
     # backspace is mapped to ctrl-h
     @kb.add('c-h', filter=hasattr(app, 'on_backspace'))
     def backspace(event: KeyPressEvent):
         event.app.on_backspace()  # type: ignore
 
-    # ctrl-backspace is mapped to ctrl-w
-    @kb.add('c-w', filter=hasattr(app, 'on_ctrl_backspace'))
-    def ctrl_backspace(event: KeyPressEvent):
-        event.app.on_ctrl_backspace()  # type: ignore
+    # This Method is used nowhere, so it is commented out. If there is ever a need to use it, it is still there.
+    # # ctrl-backspace is mapped to ctrl-w
+    # @kb.add('c-w', filter=hasattr(app, 'on_ctrl_backspace'))
+    # def ctrl_backspace(event: KeyPressEvent):
+    #     event.app.on_ctrl_backspace()  # type: ignore
 
     @kb.add('<any>', filter=hasattr(app, 'on_key'))
     def wildcard(event: KeyPressEvent):
         # wildcard function, used for prompts which need standard key presses like numbers or characters
         event.app.on_key(  # type: ignore
             [key.key for key in event.key_sequence], )
```

### Comparing `ItsPrompt-1.2/ItsPrompt/prompt.py` & `ItsPrompt-1.3/ItsPrompt/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 created by ItsNameless
 
 :copyright: (c) 2023-present ItsNameless
 :license: MIT, see LICENSE for more details.
 '''
 
+# mypy: disable-error-code=return-value
+
 from typing import Callable
 
 from pandas import DataFrame
 from prompt_toolkit import HTML
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.completion import Completer
 from prompt_toolkit.layout.containers import (Float, FloatContainer, HSplit,
@@ -458,15 +460,17 @@
         app = TablePrompt(
             question,
             data,
             layout=Layout(
                 HSplit([
                     Window(FormattedTextControl()),
                     Window(FormattedTextControl(
-                        HTML('Use UP, DOWN, LEFT, RIGHT to select a cell, TYPE to add char, BACKSPACE to delete char, ENTER to submit')),
+                        HTML(
+                            'Use UP, DOWN, LEFT, RIGHT to select a cell, TYPE to add char, BACKSPACE to delete char, ENTER to submit'
+                        )),
                            char=' ',
                            style='class:tooltip',
                            height=1)
                 ])),
             key_bindings=generate_key_bindings(TablePrompt),
             erase_when_done=True,
             style=convert_style(style)
```

### Comparing `ItsPrompt-1.2/ItsPrompt/prompts/checkbox.py` & `ItsPrompt-1.3/ItsPrompt/prompts/checkbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.prompt_content.text = HTML(content)
 
         # show error, if error should be shown, else show normal prompt
         if not self.is_error:
             # show normal prompt, change style to standard toolbar
             self.toolbar_content.text = self.toolbar_content_default_text
             self.toolbar_window.style = 'class:tooltip'
-        else:
+        else:  # pragma: no cover
             # show error prompt and error style
             # the only error that might occur is that not enough options are selected
             self.toolbar_content.text = f'ERROR: a minimum of {self.min_selections} options need to be selected!'
             self.toolbar_window.style = 'class:error'
 
     def prompt(self) -> list[str] | None:
         '''start the application, returns the return value'''
@@ -129,14 +129,14 @@
         selected_options: list[str] = []
 
         for option in self.options:
             if option.is_selected:
                 selected_options.append(option.id)
 
         # make sure that enough are selected
-        if len(selected_options) < self.min_selections:
+        if len(selected_options) < self.min_selections:  # pragma: no cover
             # show error
             self.is_error = True
             self.update()
             return
 
         self.exit(result=selected_options)
```

### Comparing `ItsPrompt-1.2/ItsPrompt/prompts/confirm.py` & `ItsPrompt-1.3/ItsPrompt/prompts/confirm.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         self.prompt_content.text = HTML(content)
 
         # show error, if error should be shown, else show normal prompt
         if not self.is_error:
             # show normal prompt, change style to standard toolbar
             self.toolbar_content.text = self.toolbar_content_default_text
             self.toolbar_window.style = 'class:tooltip'
-        else:
+        else:  # pragma: no cover
             # show error prompt and error style
             # the only error that might occur is that not enough options are selected
             self.toolbar_content.text = f'ERROR: a selection must be made!'
             self.toolbar_window.style = 'class:error'
 
     def prompt(self) -> bool | None:
         '''start the application, returns the return value'''
@@ -69,13 +69,13 @@
             return
 
         # exit with answer
         self.exit(result=key == 'y')
 
     def on_enter(self):
         # if no default is present, user is not able to just submit
-        if self.default is None:
+        if self.default is None:  # pragma: no cover
             self.is_error = True
             self.update()
             return
 
         self.exit(result=self.default)
```

### Comparing `ItsPrompt-1.2/ItsPrompt/prompts/expand.py` & `ItsPrompt-1.3/ItsPrompt/prompts/expand.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.2/ItsPrompt/prompts/input.py` & `ItsPrompt-1.3/ItsPrompt/prompts/input.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,45 +70,45 @@
                 PasswordProcessor(self.show_symbol)
             ]
 
         # save validator function
         self.validate = validate
 
         # save the completer
-        self.completer = None
+        self.completer: None | Completer = None
 
         if completions and completer:
             raise ValueError(
                 'completions and completer are mutually exclusive! Please use only one of them!'
             )
 
         if show_symbol and (completions or completer):
             # symbol and completer are mutually exclusive
             raise ValueError(
                 'Completions are not compatible with show_symbol!')
 
-        if completions:
+        if completions:  # pragma: no cover
             # a list or a dict of completions to use is given
             if type(completions) is list:
                 # we use FuzzyWordCompleter
                 self.completer = FuzzyWordCompleter(list(completions))
             elif type(completions) is dict:
                 # we use FuzzyCompleter with NestedCompleter
                 self.completer = FuzzyCompleter(
                     NestedCompleter.from_nested_dict(completions))
 
-        elif completer:
+        elif completer:  # pragma: no cover
             # a self-created completer is given
             self.completer = completer
 
         # assign the created completer to the buffer
-        if self.completer:
+        if self.completer:  # pragma: no cover
             self.buffer.completer = self.completer
 
-    def update(self):
+    def update(self):  # pragma: no cover
         '''update prompt content'''
         content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>: '
 
         if self.default and self.buffer.text == '':
             content += f'<grayout>{self.default}</grayout>'
 
         self.prompt_content.text = HTML(content)
@@ -145,15 +145,15 @@
         out: str | None = self.run()
 
         return out
 
     def _submit(self):
         '''method for submitting result, as this is done by two functions'''
         # if an error is currently shown, prevent submit
-        if self.is_error:
+        if self.is_error:  # pragma: no cover
             return
 
         # return buffer if given, else default if given, else empty string
         if self.buffer.text != '':
             self.exit(result=self.buffer.text)
         elif self.default:
             self.exit(result=self.default)
@@ -165,15 +165,16 @@
         if self.multiline:
             self._submit()
 
     def on_enter(self):
         '''either submit key or in multiline, append new line'''
         # run completion
         if (self.is_running) and self.buffer.complete_state and (
-                completion := self.buffer.complete_state.current_completion):
+                completion := self.buffer.complete_state.current_completion
+        ):  # pragma: no cover
             self.buffer.apply_completion(completion)
 
         if self.multiline:
             self.buffer.text += '\n'
             self.buffer.cursor_down()
             self.update()
             return
```

### Comparing `ItsPrompt-1.2/ItsPrompt/prompts/raw_select.py` & `ItsPrompt-1.3/ItsPrompt/prompts/raw_select.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,20 +88,20 @@
         '''when a index is pressed, which is available to select, select this index'''
         key = key_sequence[0]
 
         # return if key is not a number
         if not key.isnumeric():
             return
 
-        key = int(key)
+        id = int(key)
 
         # and return if key is not in the range of possible indices
-        if key <= 0 or key > len(self.options):
+        if id <= 0 or id > len(self.options):
             return
 
-        self.selection = key - 1
+        self.selection = id - 1
 
         self.update()
 
     def on_enter(self):
         # get selected id
         self.exit(result=self.options[self.selection].id)
```

### Comparing `ItsPrompt-1.2/ItsPrompt/prompts/select.py` & `ItsPrompt-1.3/ItsPrompt/prompts/select.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.2/ItsPrompt/prompts/table.py` & `ItsPrompt-1.3/ItsPrompt/prompts/table.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.2/ItsPrompt.egg-info/PKG-INFO` & `ItsPrompt-1.3/ItsPrompt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ItsPrompt
-Version: 1.2
+Version: 1.3
 Summary: Prompting - the fancy way
 Author: ItsNameless
 License: MIT License
         
         Copyright (c) 2023-present ItsNameless
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/ItsPrompt.svg)](https://badge.fury.io/py/ItsPrompt)
+[![linting](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/lint.yml/badge.svg)](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/lint.yml)
+[![Tests](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/tests.yml/badge.svg)](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/tests.yml)
+
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ItsPrompt)](https://pypi.org/project/ItsPrompt/)
 [![GitHub issues](https://img.shields.io/github/issues/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/issues)
 [![GitHub Repo stars](https://img.shields.io/github/stars/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/stargazers)
 [![GitHub](https://img.shields.io/github/license/TheitsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/1082381448624996514)](https://discord.gg/rP9Qke2jDs)
 
 ![Demonstration](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/ItsPrompt.gif)
```

### Comparing `ItsPrompt-1.2/ItsPrompt.egg-info/SOURCES.txt` & `ItsPrompt-1.3/ItsPrompt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 ItsPrompt/keyboard_handler.py
 ItsPrompt/prompt.py
 ItsPrompt.egg-info/PKG-INFO
 ItsPrompt.egg-info/SOURCES.txt
 ItsPrompt.egg-info/dependency_links.txt
 ItsPrompt.egg-info/requires.txt
 ItsPrompt.egg-info/top_level.txt
+ItsPrompt/data/__init__.py
 ItsPrompt/data/checkbox.py
 ItsPrompt/data/expand.py
 ItsPrompt/data/select.py
 ItsPrompt/data/style.py
 ItsPrompt/data/table.py
 ItsPrompt/data/type.py
+ItsPrompt/prompts/__init__.py
 ItsPrompt/prompts/checkbox.py
 ItsPrompt/prompts/confirm.py
 ItsPrompt/prompts/expand.py
 ItsPrompt/prompts/input.py
 ItsPrompt/prompts/raw_select.py
 ItsPrompt/prompts/select.py
-ItsPrompt/prompts/table.py
+ItsPrompt/prompts/table.py
+tests/test_prompt.py
```

### Comparing `ItsPrompt-1.2/LICENSE` & `ItsPrompt-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.2/PKG-INFO` & `ItsPrompt-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ItsPrompt
-Version: 1.2
+Version: 1.3
 Summary: Prompting - the fancy way
 Author: ItsNameless
 License: MIT License
         
         Copyright (c) 2023-present ItsNameless
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,14 +32,17 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/ItsPrompt.svg)](https://badge.fury.io/py/ItsPrompt)
+[![linting](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/lint.yml/badge.svg)](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/lint.yml)
+[![Tests](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/tests.yml/badge.svg)](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/tests.yml)
+
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ItsPrompt)](https://pypi.org/project/ItsPrompt/)
 [![GitHub issues](https://img.shields.io/github/issues/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/issues)
 [![GitHub Repo stars](https://img.shields.io/github/stars/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/stargazers)
 [![GitHub](https://img.shields.io/github/license/TheitsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/1082381448624996514)](https://discord.gg/rP9Qke2jDs)
 
 ![Demonstration](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/ItsPrompt.gif)
```

### Comparing `ItsPrompt-1.2/README.md` & `ItsPrompt-1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 [![PyPI version](https://badge.fury.io/py/ItsPrompt.svg)](https://badge.fury.io/py/ItsPrompt)
+[![linting](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/lint.yml/badge.svg)](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/lint.yml)
+[![Tests](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/tests.yml/badge.svg)](https://github.com/TheItsProjects/ItsPrompt/actions/workflows/tests.yml)
+
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ItsPrompt)](https://pypi.org/project/ItsPrompt/)
 [![GitHub issues](https://img.shields.io/github/issues/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/issues)
 [![GitHub Repo stars](https://img.shields.io/github/stars/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/stargazers)
 [![GitHub](https://img.shields.io/github/license/TheitsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/1082381448624996514)](https://discord.gg/rP9Qke2jDs)
 
 ![Demonstration](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/ItsPrompt.gif)
```

### Comparing `ItsPrompt-1.2/pyproject.toml` & `ItsPrompt-1.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ItsPrompt"
-version = "1.2"
+version = "1.3"
 authors = [
-    {name = "ItsNameless"}
+    {name = "ItsNameless"},
 ]
 description = "Prompting - the fancy way"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
-    "prompt-toolkit>=3.0.37,<4.0"
+    "prompt-toolkit>=3.0.37,<4.0",
+    "pandas>=1.5.3",
 ]
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent"
+        "Operating System :: OS Independent",
 ]
 license = {file = "LICENSE"}
 
 [project.urls]
 Homepage = "https://github.com/TheItsProjects/ItsPrompt"
 Repository = "https://github.com/TheItsProjects/ItsPrompt"
 "Issue Tracker" = "https://github.com/TheItsProjects/ItsPrompt/issues"
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = [
     "ItsPrompt",
-    "ItsPrompt.*"
+    "ItsPrompt.*",
 ]
+
+[tool.pytest.ini_options]
+addopts = "--cov=ItsPrompt --cov-report term-missing"
+testpaths = [
+    "tests",
+]
+filterwarnings = [
+    # ignore warning, see https://github.com/prompt-toolkit/python-prompt-toolkit/issues/1696
+    "ignore:There is no current event loop:DeprecationWarning",
+]
+
+[tool.mypy]
+packages = "ItsPrompt"
+explicit_package_bases = true
+check_untyped_defs = true
```

