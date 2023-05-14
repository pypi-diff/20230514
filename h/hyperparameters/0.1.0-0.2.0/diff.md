# Comparing `tmp/hyperparameters-0.1.0.tar.gz` & `tmp/hyperparameters-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparameters-0.1.0.tar", max compression
+gzip compressed data, was "hyperparameters-0.2.0.tar", max compression
```

## Comparing `hyperparameters-0.1.0.tar` & `hyperparameters-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-05-11 14:57:17.769287 hyperparameters-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     6350 2023-05-12 11:15:03.716611 hyperparameters-0.1.0/README.md
--rw-r--r--   0        0        0      618 2023-05-12 11:00:52.633313 hyperparameters-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       99 2023-05-12 11:00:20.488095 hyperparameters-0.1.0/src/hyperparameters/__init__.py
--rw-r--r--   0        0        0     8132 2023-05-11 12:34:42.327686 hyperparameters-0.1.0/src/hyperparameters/hyperparams.py
--rw-r--r--   0        0        0      849 2023-05-12 11:00:20.489614 hyperparameters-0.1.0/src/hyperparameters/ray_tune_hyperparams.py
--rw-r--r--   0        0        0     6948 1970-01-01 00:00:00.000000 hyperparameters-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7491 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/README.md
+-rw-r--r--   0        0        0      768 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/src/hyperparameters/__init__.py
+-rw-r--r--   0        0        0     9343 2023-05-14 10:27:43.299402 hyperparameters-0.2.0/src/hyperparameters/hyperparams.py
+-rw-r--r--   0        0        0      849 2023-05-13 17:20:06.420558 hyperparameters-0.2.0/src/hyperparameters/ray_tune_hyperparams.py
+-rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 hyperparameters-0.2.0/PKG-INFO
```

### Comparing `hyperparameters-0.1.0/LICENSE.md` & `hyperparameters-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.1.0/README.md` & `hyperparameters-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 # Hyperparameters
 
 Are you tired of repeating hyperparameters in code, `argparse` definitions, and hyperparameter tunning libraries?
 
 `Hyperparameters` lets you define your hyperparameters once and use everywhere! Moreover, you get type linting and spelling checks for free!
 
+## Quickstart
+
+Install `Hyperparameters`:
+```bash
+pip install hyperparameters
+```
+
+You need to install the `ray.tune` package separately if you want to use the `ray.tune` hypertunning integration:
+```bash
+pip install -U "ray[tune]"
+```
+
 Define your parameters once using the `Hyperparams` class:
 
 ```python
 from argparse import ArgumentParser
+from typing import Optional
 
 from hyperparameters import HP, Hyperparams
 
 
 class MyHyperparams(Hyperparams):
     epochs: int = HP(
-        description="Number of epochs to train for",
+        "Number of epochs to train for",
         default=5,
     )
     lr: float = HP(
-        description="Learning rate",
+        "Learning rate",
         default=1e-3,
     )
     tokenizer: str = HP(
-        description="HF tokenizer to use",
+        "HF tokenizer to use",
         default="BPE",
         choices=["BPE", "WordPiece"],
     )
     train_data_path: str = HP(
-        description="Path to the training dataset",
+        "Path to the training dataset",
     )
     use_dropout: bool = HP(
-        description="Whether the dropout layers should be activated",
+        "Whether the dropout layers should be activated",
         default=True,
     )
+    pretrained_weights: Optional[str] = HP(
+        "Path to the pretrained model weights, if any",
+        default=None,
+    )
 
 
 parser = ArgumentParser()
 MyHyperparams.add_arguments(parser)
 params = MyHyperparams.from_arguments(parser.parse_args())
 
 # access parameters as typed attributes
@@ -44,36 +61,47 @@
 
 # convert to a dictionary
 print(params.dict())
 ```
 
 Let's see the registered arguments by running the code above with `--help`:
 ```
-usage: example.py [-h] [--epochs EPOCHS] [--lr LR] [--tokenizer {BPE,WordPiece}]
-                  --train-data-path TRAIN_DATA_PATH
-                  [--use-dropout | --no-use-dropout]
+usage: example.py [-h] [--epochs EPOCHS] [--lr LR] [--tokenizer {BPE,WordPiece}] --train-data-path TRAIN_DATA_PATH [--use-dropout | --no-use-dropout]
+                  [--pretrained-weights PRETRAINED_WEIGHTS]
 
 options:
   -h, --help            show this help message and exit
   --epochs EPOCHS       Number of epochs to train for
   --lr LR               Learning rate
   --tokenizer {BPE,WordPiece}
                         HF tokenizer to use
   --train-data-path TRAIN_DATA_PATH
                         Path to the training dataset
   --use-dropout         Whether the dropout layers should be activated
   --no-use-dropout      Disable: Whether the dropout layers should be activated
+  --pretrained-weights PRETRAINED_WEIGHTS
+                        Path to the pretrained model weights, if any
 ```
 As can be seen from the above, `Hyperparameters` takes care of low level details for you:
 
 1. The `--train-data-path` parameter is required because we didn't provide a default value for it. All other parameters are optional.
-2. You can provide the `--use-dropout` or the `--no-use-dropout` flag, but not both at the same time. Neither flag is required, as the `use_dropout` parameter has a default value.
-3. The `--tokenizer` parameter can only be `BPE` or `WordPiece`. Providing any other value results in an error.
-4. The data types of the parameters are parsed from strings and validated according to the type hints in the `MyHyperparams` class. 
-5. The default values are used whenever an argument is ommitted. Let's check that by running with `--train-data-path mydata/`: the script prints: `{'epochs': 5, 'lr': 0.001, 'tokenizer': 'BPE', 'train_data_path': 'mydata/', 'use_dropout': True}`.
+2. Even though the default value for `--pretrained-weights` is `None`, this parameter is optional. However, we had to use the `Optional[str]` type hint.
+3. You can provide the `--use-dropout` or the `--no-use-dropout` flag, but not both at the same time. Neither flag is required, as the `use_dropout` parameter has a default value.
+4. The `--tokenizer` parameter can only be `BPE` or `WordPiece`. Providing any other value results in an error.
+5. The data types of the parameters are parsed from strings and validated according to the type hints in the `MyHyperparams` class. 
+6. The default values are used whenever an argument is ommitted. Let's check that by running with `--train-data-path mydata/`: the script prints: `{'epochs': 5, 'lr': 0.001, 'tokenizer': 'BPE', 'train_data_path': 'mydata/', 'use_dropout': True, 'pretrained_weights': None}`.
+
+
+### Default values and required parameters
+
+1. If a default value is omitted completely, the parameter will be required.
+2. Otherwise, if any default value is specified, even `None`, the parameter will be optional.
+3. You must use the `Optional` type hint if the default value is `None`.
+4. You can't have `bool` parameters with `None` as default. Flags that can be `None` just don't make any sense.
+5. You can't have choice parameters with `None` as default. If you need this, just add a "null" value to the list of choices.
 
 
 ## Hypertunning
 Different hypertunning libraries provide different APIs for defining search spaces. `Hyperparameters` can be easily extended to support any hypertunning library. You can do it yourself following the steps discussed below - it's easy! The `ray.tune` library is supported out of the box.
 
 When defining hypertunable parameters with `Hyperparameters`, make sure to inherit from both the `Hyperparams` class and the mixin class specific to your hypertunning library. Here is an example for `ray.tune`:
 ```python
@@ -104,26 +132,26 @@
 
 from hyperparameters import HP, Hyperparams
 from hyperparameters.ray_tune_hyperparams import RayTuneHyperparamsMixin
 
 
 class MyHyperparams(Hyperparams, RayTuneHyperparamsMixin):
     lr: float = HP(
-        description="Learning rate",
+        "Learning rate",
         default=1e-3,
         search_space=tune.loguniform(1e-5, 1e-2),
     )
     layers_num: int = HP(
-        description="Number of model layers",
+        "Number of model layers",
         default=8,
         tunable=True,
         choices=[4, 8, 16, 24],
     )
     use_dropout: bool = HP(
-        description="Whether the dropout layers should be activated",
+        "Whether the dropout layers should be activated",
         default=True,
         tunable=True,
     )
 
 # Search space config that ray.tune understands
 MyHyperparams.ray_tune_param_space()
```

### Comparing `hyperparameters-0.1.0/pyproject.toml` & `hyperparameters-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [tool.poetry]
 name = "Hyperparameters"
-version = "0.1.0"
+version = "0.2.0"
 description = "Define your Hyperparameters once and use in argparse, hypertunning libraries, and as strongly-typed attributes in code!"
 authors = ["Oleh Lokshyn <olokshyn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
+[tool.poetry.urls]
+"Repository" = "https://github.com/olokshyn/Hyperparameters"
+"Bug Tracker" = "https://github.com/olokshyn/Hyperparameters/issues"
+
 [tool.poetry.dependencies]
 python = "~3.10"
 pydantic = "^1.10.7"
 ray = {extras = ["tune"], version = "^2.4.0", optional = true}
 
 [tool.poetry.extras]
 ray = ["ray"]
```

### Comparing `hyperparameters-0.1.0/src/hyperparameters/hyperparams.py` & `hyperparameters-0.2.0/src/hyperparameters/hyperparams.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,79 +7,108 @@
 
 
 class HyperparamInfo(BaseModel):
     class Config:
         validation = False
         arbitrary_types_allowed = True
 
+    description: str
+    default: Any = None
     tunable: bool = False
     search_space: Any = None
-    default: Any = None
     choices: list[Any] | None = None
 
+    annotation: Any = None
+    type_: Any = None
+    required: bool = False
 
-def Hyperparam(
-    *,
+    def can_be_none(self) -> bool:
+        return getattr(self.annotation, "_name", None) == "Optional"
+
+
+def HP(
     description: str,
+    *,
     default: Any = Undefined,
     tunable: bool | None = None,
     search_space: Any = None,
     choices: list[Any] | None = None,
 ):
     field = Field(
         default=default,
         description=description,
     )
-    default = default if default is not Undefined else None
     field.extra["info"] = HyperparamInfo(
+        description=description,
+        default=default if default is not Undefined else None,
         tunable=tunable if tunable is not None else search_space is not None,
         search_space=search_space,
-        default=default,
         choices=choices,
     )
     return field
 
 
 def _choices_validator(value: Any, *, field_name: str, choices: list[Any]) -> None:
     if value not in choices:
         raise ValueError(
             f"Param {field_name} is {value} but must be one of [{', '.join(choices)}]"
         )
     return value
 
 
+def _load_info(field_name: str, field: ModelField) -> HyperparamInfo:
+    info: HyperparamInfo | None = field.field_info.extra.get("info")
+    if info is None:
+        raise ValueError(f"Field {field_name} was not defined correctly, use HP().")
+    assert isinstance(info, HyperparamInfo)
+    return info
+
+
 class HyperparamsMeta(ModelMetaclass, _ProtocolMeta):
     def __new__(mcs, name, bases, namespace, **kwargs) -> type[BaseModel]:
         cls: type[BaseModel] = super().__new__(mcs, name, bases, namespace, **kwargs)
         field: ModelField
         for field_name, field in cls.__fields__.items():
-            if field.default is not None and not isinstance(field.default, field.type_):
-                raise TypeError(
-                    f"Field {field_name} is of type {field.type_} but has "
-                    f"default value '{field.default}' of type {type(field.default)}"
-                )
+            info = _load_info(field_name, field)
 
-            info: HyperparamInfo | None = field.field_info.extra.get("info")
-            assert info is None or isinstance(info, HyperparamInfo)
-            if field.type_ is bool and info is not None:
+            info.type_ = field.type_
+            info.annotation = field.annotation
+            info.required = field.required is True
+
+            if not info.required:
+                if info.default is None and not info.can_be_none():
+                    raise ValueError(
+                        f"Field {field_name} is of type {info.annotation} but is None by default. Use Optional."
+                    )
+
+                if info.default is not None and not isinstance(
+                    info.default, info.type_
+                ):
+                    raise ValueError(
+                        f"Field {field_name} is of type {info.annotation} but has "
+                        f"default value '{info.default}' of type {type(info.default)}"
+                    )
+
+            if info.type_ is bool:
                 if info.choices is not None:
                     raise ValueError(
-                        f"Field {field_name} is bool and cannot have choices set"
+                        f"Field {field_name} is bool and cannot have choices set. "
+                        "False and True are the only possible choices."
                     )
                 info.choices = [False, True]
-            if info is not None and info.choices is not None:
+            if info.choices is not None:
                 for choice in info.choices:
-                    if not isinstance(choice, field.type_):
-                        raise TypeError(
-                            f"Field {field_name} is of type {field.type_} but contains "
+                    if not isinstance(choice, info.type_):
+                        raise ValueError(
+                            f"Field {field_name} is of type {info.annotation} but contains "
                             f"choice '{choice}' of type {type(choice)}"
                         )
-                if field.default is not None and field.default not in info.choices:
+                if not info.required and info.default not in info.choices:
                     raise ValueError(
-                        f"Field {field_name} has invalid default '{field.default}' "
+                        f"Field {field_name} has invalid default '{info.default}' "
                         "that is not one of the choices"
                     )
 
                 validator = Validator(
                     func=partial(
                         _choices_validator, field_name=field_name, choices=info.choices
                     ),
@@ -96,14 +125,18 @@
 SelfHyperparamsProtocol = TypeVar(
     "SelfHyperparamsProtocol", bound="HyperparamsProtocol"
 )
 
 
 class HyperparamsProtocol(Protocol):
     @classmethod
+    def parameters(cls: type[SelfHyperparamsProtocol]) -> dict[str, HyperparamInfo]:
+        ...
+
+    @classmethod
     def add_arguments(
         cls: type[SelfHyperparamsProtocol], parser: argparse.ArgumentParser
     ) -> None:
         ...
 
     @classmethod
     def from_arguments(
@@ -123,48 +156,53 @@
 
 class Hyperparams(BaseModel, HyperparamsProtocol, metaclass=HyperparamsMeta):
     class Config:
         validate_assignment = True
         arbitrary_types_allowed = True
 
     @classmethod
+    def parameters(cls: type[SelfHyperparams]) -> dict[str, HyperparamInfo]:
+        return {
+            field_name: _load_info(field_name, field)
+            for field_name, field in cls.__fields__.items()
+        }
+
+    # TODO: add nargs support
+    @classmethod
     def add_arguments(
         cls: type[SelfHyperparams], parser: argparse.ArgumentParser
     ) -> None:
         for field_name, field in cls.__fields__.items():
-            info: HyperparamInfo | None = field.field_info.extra.get("info")
-            assert info is None or isinstance(info, HyperparamInfo)
+            info = _load_info(field_name, field)
             option_name = "--" + field_name.replace("_", "-")
-            help = field.field_info.description
-            required = field.required is True or field.default is None
 
-            if field.type_ is bool:
-                group = parser.add_mutually_exclusive_group(required=required)
+            if info.type_ is bool:
+                group = parser.add_mutually_exclusive_group(required=info.required)
                 group.add_argument(
                     option_name,
                     action="store_true",
                     dest=field_name,
-                    help=help,
+                    help=info.description,
                 )
                 group.add_argument(
                     "--no-" + field_name.replace("_", "-"),
                     action="store_false",
                     dest=field_name,
-                    help="Disable: " + help,
+                    help="Disable: " + info.description,
                 )
-                if field.default is not None:
-                    parser.set_defaults(**{field_name: bool(field.default)})
+                if info.default is not None:
+                    parser.set_defaults(**{field_name: bool(info.default)})
             else:
                 parser.add_argument(
                     option_name,
-                    help=help,
-                    type=field.type_,
-                    default=field.default,
-                    required=required,
-                    choices=getattr(info, "choices", None),
+                    help=info.description,
+                    type=info.type_,
+                    default=info.default,
+                    required=info.required,
+                    choices=info.choices,
                 )
 
     @classmethod
     def from_arguments(
         cls: type[SelfHyperparams],
         args: argparse.Namespace,
         **overrides,
@@ -174,17 +212,16 @@
             **overrides,
         }
         return cls(**fields)
 
     @classmethod
     def _tunable_params(cls) -> Iterator[tuple[str, HyperparamInfo]]:
         for field_name, field in cls.__fields__.items():
-            info: HyperparamInfo | None = field.field_info.extra.get("info")
-            assert info is None or isinstance(info, HyperparamInfo)
-            if info is not None and info.tunable:
+            info = _load_info(field_name, field)
+            if info.tunable:
                 if (
                     info.search_space is None
                     and info.choices is None
                     and info.default is None
                 ):
                     raise ValueError(
                         f"Tunable parameter {field_name} must have "
@@ -214,14 +251,19 @@
         self: SelfHyperparams,
         data: dict[str, Any],
         *,
         inplace: bool = False,
         validate: bool = False,
     ) -> SelfHyperparams:
         if validate:
+            unknown_keys = data.keys() - self.__dict__.keys()
+            if unknown_keys:
+                raise ValueError(
+                    f"Update data contains unknown keys: {' '.join(unknown_keys)}"
+                )
             target = self
             if not inplace:
                 target = self.copy()
             for name in data:
                 if name in target.__dict__:
                     setattr(target, name, data[name])
             return target
```

### Comparing `hyperparameters-0.1.0/src/hyperparameters/ray_tune_hyperparams.py` & `hyperparameters-0.2.0/src/hyperparameters/ray_tune_hyperparams.py`

 * *Files identical despite different names*

### Comparing `hyperparameters-0.1.0/PKG-INFO` & `hyperparameters-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,77 @@
 Metadata-Version: 2.1
 Name: hyperparameters
-Version: 0.1.0
+Version: 0.2.0
 Summary: Define your Hyperparameters once and use in argparse, hypertunning libraries, and as strongly-typed attributes in code!
 License: MIT
 Author: Oleh Lokshyn
 Author-email: olokshyn@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: ray
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: ray[tune] (>=2.4.0,<3.0.0) ; extra == "ray"
+Project-URL: Bug Tracker, https://github.com/olokshyn/Hyperparameters/issues
+Project-URL: Repository, https://github.com/olokshyn/Hyperparameters
 Description-Content-Type: text/markdown
 
 # Hyperparameters
 
 Are you tired of repeating hyperparameters in code, `argparse` definitions, and hyperparameter tunning libraries?
 
 `Hyperparameters` lets you define your hyperparameters once and use everywhere! Moreover, you get type linting and spelling checks for free!
 
+## Quickstart
+
+Install `Hyperparameters`:
+```bash
+pip install hyperparameters
+```
+
+You need to install the `ray.tune` package separately if you want to use the `ray.tune` hypertunning integration:
+```bash
+pip install -U "ray[tune]"
+```
+
 Define your parameters once using the `Hyperparams` class:
 
 ```python
 from argparse import ArgumentParser
+from typing import Optional
 
 from hyperparameters import HP, Hyperparams
 
 
 class MyHyperparams(Hyperparams):
     epochs: int = HP(
-        description="Number of epochs to train for",
+        "Number of epochs to train for",
         default=5,
     )
     lr: float = HP(
-        description="Learning rate",
+        "Learning rate",
         default=1e-3,
     )
     tokenizer: str = HP(
-        description="HF tokenizer to use",
+        "HF tokenizer to use",
         default="BPE",
         choices=["BPE", "WordPiece"],
     )
     train_data_path: str = HP(
-        description="Path to the training dataset",
+        "Path to the training dataset",
     )
     use_dropout: bool = HP(
-        description="Whether the dropout layers should be activated",
+        "Whether the dropout layers should be activated",
         default=True,
     )
+    pretrained_weights: Optional[str] = HP(
+        "Path to the pretrained model weights, if any",
+        default=None,
+    )
 
 
 parser = ArgumentParser()
 MyHyperparams.add_arguments(parser)
 params = MyHyperparams.from_arguments(parser.parse_args())
 
 # access parameters as typed attributes
@@ -60,36 +79,47 @@
 
 # convert to a dictionary
 print(params.dict())
 ```
 
 Let's see the registered arguments by running the code above with `--help`:
 ```
-usage: example.py [-h] [--epochs EPOCHS] [--lr LR] [--tokenizer {BPE,WordPiece}]
-                  --train-data-path TRAIN_DATA_PATH
-                  [--use-dropout | --no-use-dropout]
+usage: example.py [-h] [--epochs EPOCHS] [--lr LR] [--tokenizer {BPE,WordPiece}] --train-data-path TRAIN_DATA_PATH [--use-dropout | --no-use-dropout]
+                  [--pretrained-weights PRETRAINED_WEIGHTS]
 
 options:
   -h, --help            show this help message and exit
   --epochs EPOCHS       Number of epochs to train for
   --lr LR               Learning rate
   --tokenizer {BPE,WordPiece}
                         HF tokenizer to use
   --train-data-path TRAIN_DATA_PATH
                         Path to the training dataset
   --use-dropout         Whether the dropout layers should be activated
   --no-use-dropout      Disable: Whether the dropout layers should be activated
+  --pretrained-weights PRETRAINED_WEIGHTS
+                        Path to the pretrained model weights, if any
 ```
 As can be seen from the above, `Hyperparameters` takes care of low level details for you:
 
 1. The `--train-data-path` parameter is required because we didn't provide a default value for it. All other parameters are optional.
-2. You can provide the `--use-dropout` or the `--no-use-dropout` flag, but not both at the same time. Neither flag is required, as the `use_dropout` parameter has a default value.
-3. The `--tokenizer` parameter can only be `BPE` or `WordPiece`. Providing any other value results in an error.
-4. The data types of the parameters are parsed from strings and validated according to the type hints in the `MyHyperparams` class. 
-5. The default values are used whenever an argument is ommitted. Let's check that by running with `--train-data-path mydata/`: the script prints: `{'epochs': 5, 'lr': 0.001, 'tokenizer': 'BPE', 'train_data_path': 'mydata/', 'use_dropout': True}`.
+2. Even though the default value for `--pretrained-weights` is `None`, this parameter is optional. However, we had to use the `Optional[str]` type hint.
+3. You can provide the `--use-dropout` or the `--no-use-dropout` flag, but not both at the same time. Neither flag is required, as the `use_dropout` parameter has a default value.
+4. The `--tokenizer` parameter can only be `BPE` or `WordPiece`. Providing any other value results in an error.
+5. The data types of the parameters are parsed from strings and validated according to the type hints in the `MyHyperparams` class. 
+6. The default values are used whenever an argument is ommitted. Let's check that by running with `--train-data-path mydata/`: the script prints: `{'epochs': 5, 'lr': 0.001, 'tokenizer': 'BPE', 'train_data_path': 'mydata/', 'use_dropout': True, 'pretrained_weights': None}`.
+
+
+### Default values and required parameters
+
+1. If a default value is omitted completely, the parameter will be required.
+2. Otherwise, if any default value is specified, even `None`, the parameter will be optional.
+3. You must use the `Optional` type hint if the default value is `None`.
+4. You can't have `bool` parameters with `None` as default. Flags that can be `None` just don't make any sense.
+5. You can't have choice parameters with `None` as default. If you need this, just add a "null" value to the list of choices.
 
 
 ## Hypertunning
 Different hypertunning libraries provide different APIs for defining search spaces. `Hyperparameters` can be easily extended to support any hypertunning library. You can do it yourself following the steps discussed below - it's easy! The `ray.tune` library is supported out of the box.
 
 When defining hypertunable parameters with `Hyperparameters`, make sure to inherit from both the `Hyperparams` class and the mixin class specific to your hypertunning library. Here is an example for `ray.tune`:
 ```python
@@ -120,26 +150,26 @@
 
 from hyperparameters import HP, Hyperparams
 from hyperparameters.ray_tune_hyperparams import RayTuneHyperparamsMixin
 
 
 class MyHyperparams(Hyperparams, RayTuneHyperparamsMixin):
     lr: float = HP(
-        description="Learning rate",
+        "Learning rate",
         default=1e-3,
         search_space=tune.loguniform(1e-5, 1e-2),
     )
     layers_num: int = HP(
-        description="Number of model layers",
+        "Number of model layers",
         default=8,
         tunable=True,
         choices=[4, 8, 16, 24],
     )
     use_dropout: bool = HP(
-        description="Whether the dropout layers should be activated",
+        "Whether the dropout layers should be activated",
         default=True,
         tunable=True,
     )
 
 # Search space config that ray.tune understands
 MyHyperparams.ray_tune_param_space()
```

