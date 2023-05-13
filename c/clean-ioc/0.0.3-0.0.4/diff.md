# Comparing `tmp/clean_ioc-0.0.3.tar.gz` & `tmp/clean_ioc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-0.0.3.tar", max compression
+gzip compressed data, was "clean_ioc-0.0.4.tar", max compression
```

## Comparing `clean_ioc-0.0.3.tar` & `clean_ioc-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/LICENSE
--rw-r--r--   0        0        0    13354 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/README.md
--rw-r--r--   0        0        0    21083 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/clean_ioc/__init__.py
--rw-r--r--   0        0        0      285 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/clean_ioc/factories.py
--rw-r--r--   0        0        0     1320 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0     1763 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      587 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     5390 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1112 2023-02-17 23:53:01.798722 clean_ioc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    14505 1970-01-01 00:00:00.000000 clean_ioc-0.0.3/setup.py
--rw-r--r--   0        0        0    13981 1970-01-01 00:00:00.000000 clean_ioc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/LICENSE
+-rw-r--r--   0        0        0    14851 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/README.md
+-rw-r--r--   0        0        0    24809 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/clean_ioc/__init__.py
+-rw-r--r--   0        0        0      674 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/clean_ioc/factories.py
+-rw-r--r--   0        0        0     1320 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0     1811 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      587 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6537 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1112 2023-05-13 22:10:45.991560 clean_ioc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    16063 1970-01-01 00:00:00.000000 clean_ioc-0.0.4/setup.py
+-rw-r--r--   0        0        0    15478 1970-01-01 00:00:00.000000 clean_ioc-0.0.4/PKG-INFO
```

### Comparing `clean_ioc-0.0.3/LICENSE` & `clean_ioc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.3/README.md` & `clean_ioc-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -186,14 +186,44 @@
 container.register(int, instance=10)
 
 client = container.resolve(Client)
 
 client.get_number() # returns 20
 ```
 
+
+Decorators are resolved in order of when first registered. So the first registered decorator is the deepest in the class tree
+
+
+```python
+    class Concrete:
+        pass
+
+    class DecoratorOne(Concrete):
+        def __init__(self, child: Concrete):
+            self.child = child
+
+    class DecoratorTwo(Concrete):
+        def __init__(self, child: Concrete):
+            self.child = child
+
+    container = Container()
+
+    container.register(Concrete)
+    container.register_decorator(Concrete, DecoratorOne)
+    container.register_decorator(Concrete, DecoratorTwo)
+
+    root = container.resolve(Concrete)
+
+    type(root) # returns DecoratorTwo
+    type(root.child) # returns DecoratorOne
+    type(root.child.child) # returns Concrete
+```
+
+
 ## Subclasses registration
 
 This feature allows registartion of all subclasses of a giveb type
 
 ```python
 class Client(abc.ABC)
     @abc.abstractmethod
@@ -220,45 +250,45 @@
 twenty_client.get_number() # returns 20
 
 # Resolve all subsclasses of Client
 client = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]
 ```
 
 
-## Lifestyles
-Lifestyles configure how long and resolved object says alive for
-There are 4 lifestyle types
+## Lifespans
+Lifespans configure how long and resolved object says alive for
+There are 4 lifespan types
 
 ### transient
 Always create a new instance
 
 ```python
-container.register(Client, lifestyle=LifestyleType.transient)
+container.register(Client, lifespan=Lifespan.transient)
 ```
 
 
 ### once_per_graph (Default behaviour)
 Only create one instance throughout the resolve call
 
 ```python
-container.register(Client, lifestyle=LifestyleType.once_per_graph)
+container.register(Client, lifespan=Lifespan.once_per_graph)
 ```
 
 ### scoped
 Only create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**
 
 ```python
-container.register(Client, lifestyle=LifestyleType.scoped)
+container.register(Client, lifespan=Lifespan.scoped)
 ```
 
 ### singleton
 Only one instance of the object is created throughout the lifespan of the container
 
 ```python
-container.register(Client, lifestyle=LifestyleType.singleton)
+container.register(Client, lifespan=Lifespan.singleton)
 ```
 
 *Note:*
 When registering an instance, then the behaviour is always singleton
 
 ```python
 container.register(int, instance=10)
@@ -343,15 +373,15 @@
 h1.handle(HelloCommand()) # prints 'A VERY BIG\nHELLO'
 h2.handle(GoodbyeCommand()) # prints 'A VERY BIG\nGOODBYE'
 
 ```
 
 ## Scopes
 
-Scopes are a way to create a sub container that will live for a certain lifestyle.
+Scopes are a way to create a sub container that will live for a certain lifespan.
 Some good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system
 
 
 ```python
 class Client
     def __init__(self, number: int)
         return number
@@ -559,17 +589,48 @@
     def __init__(self, dep: ClientDependency)
         self.dep = dep
 
     def get_number(self):
         return self.dep.get_int()
 
 def client_module(c: Container):
-    container = Container()
-    container.register(ClientDependency)
-    container.register(Client)
+    c.register(ClientDependency)
+    c.register(Client)
 
 container.apply_module(client_module)
 
 client = container.resolve(Client)
 
 client.get_number() # returns 10
 ```
+
+
+
+## DependencyContext (BETA feature)
+
+You can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing
+One example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context
+
+```python
+class Logger
+    def __init__(self, module):
+        self.module = module
+
+class Client
+    def __init__(self, logger: Logger)
+        self.logger = logger
+
+def logger_fac(context: DependencyContext):
+    module = context.parent.__module__
+    return Logger(module)
+
+
+container = Container()
+container.register(Client)
+container.register(Logger, factory=logger_fac)
+
+container.apply_module(client_module)
+
+client = container.resolve(Client)
+
+
+```
```

### Comparing `clean_ioc-0.0.3/clean_ioc/__init__.py` & `clean_ioc-0.0.4/clean_ioc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Simple IOC container.
 """
 from __future__ import annotations
 import abc
 from collections import defaultdict, deque
 from dataclasses import dataclass
-import sys
 import types
 from enum import IntEnum
-from typing import Any, ForwardRef, Type, get_type_hints
+from typing import Any, Type, get_type_hints
 from collections.abc import Callable
 from typing import _GenericAlias  # type: ignore
 from uuid import uuid4
 from .functional_utils import constant, fn_and, fn_not
 from .type_filters import is_abstract
 from .typing_utils import (
     get_generic_bases,
     get_generic_types,
     get_subclasses,
     get_typevar_to_type_mapping,
+    is_open_generic_type,
     try_to_complete_generic,
 )
 import inspect
 
 
 class _empty:
     def __bool__(self):
@@ -33,34 +33,80 @@
         self.name = name
         self.arg_type = arg_type
         self.default_value = (
             _empty if default_value == inspect._empty else default_value
         )
 
 
-def get_arg_info(subject: Callable) -> dict[str, ArgInfo]:
+def get_arg_info(
+    subject: Callable, local_ns: dict = {}, global_ns: dict | None = None
+) -> dict[str, ArgInfo]:
     arg_spec_fn = subject if inspect.isfunction(subject) else subject.__init__
-    args = get_type_hints(arg_spec_fn, None, {})
+    args = get_type_hints(arg_spec_fn, global_ns, local_ns)
     signature = inspect.signature(subject)
     d: dict[str, ArgInfo] = {}
     for name, param in signature.parameters.items():
         d[name] = ArgInfo(name=name, arg_type=args[name], default_value=param.default)
     return d
 
 
 _all_registartions = constant(True)
 
 
-class LifestyleType(IntEnum):
+class Lifespan(IntEnum):
     transient = 0
     once_per_graph = 1
     scoped = 2
     singleton = 3
 
 
+class DependencyNode(abc.ABC):
+    service_type: type
+    implementation: type | Callable
+    parent: DependencyNode
+    decorated: DependencyNode
+
+    @property
+    def bottom_decorated(self):
+        bottom = self.implementation
+        decorated = self.decorated
+        while decorated:
+            bottom = decorated.implementation
+            decorated = decorated.decorated
+        return bottom
+
+
+class EmptyDependencyNode(DependencyNode):
+    def __init__(self):
+        self.service_type = _empty
+        self.implementation = _empty
+        self.parent = self
+        self.decorated = self
+
+    def __bool__(self):
+        return False
+
+
+@dataclass
+class FullDependencyNode(DependencyNode):
+    service_type: type
+    implementation: type | Callable
+    parent: DependencyNode = EmptyDependencyNode()
+    decorated: DependencyNode = EmptyDependencyNode()
+
+
+class DependencyContext:
+    def __init__(self, name: str, dependency_node: DependencyNode):
+        self.name = name
+        self.service_type = dependency_node.service_type
+        self.implementation = dependency_node.implementation
+        self.parent = dependency_node.parent
+        self.decorated = dependency_node.decorated
+
+
 class CannotResolveException(Exception):
     def __init__(self):
         self.stack = deque()
 
     def append(self, d: Dependency):
         self.stack.appendleft(d)
 
@@ -103,33 +149,36 @@
         if isinstance(parent_implementation, type):
             self.service_type = try_to_complete_generic(
                 service_type, parent_implementation
             )
         else:
             self.service_type = service_type
         self.settings = settings
+        self.is_dependency_context = service_type == DependencyContext
         self.is_generic_list = getattr(self.service_type, "__origin__", None) == list
         self.default_value = default_value
 
-    def resolve(self, context: ResolvingContext):
+    def resolve(self, context: ResolvingContext, depedency_node: DependencyNode):
         if not self.settings.value == _empty:
             return self.settings.value
 
         if not self.default_value == _empty and self.settings.use_default_paramater:
             return self.default_value
 
+        if self.is_dependency_context:
+            return DependencyContext(name=self.name, dependency_node=depedency_node)
+
         if self.is_generic_list:
             regs = context.find_registrations(self.service_type.__args__[0], self.settings.filter)  # type: ignore
-            return [s.build(context) for s in regs]
+            return [s.build(context, depedency_node) for s in regs]
         else:
             try:
                 reg = context.find_registration(self.service_type, self.settings.filter)
-                return reg.build(context)
+                return reg.build(context, depedency_node)
             except CannotResolveException as ex:
-                print(self.name)
                 ex.append(self)
                 raise ex
 
 
 class RootDependency(Dependency):
     @staticmethod
     def __PARENT_ROOT__():
@@ -166,114 +215,145 @@
 
     @classmethod
     def _get_dependencies(
         cls,
         creator_function: Callable,
         dependency_config: dict[str, DependencySettings],
     ) -> dict[str, Dependency]:
-        # signature = inspect.signature(creator_function)
         args_infos = get_arg_info(creator_function)
         return {
             name: Dependency(
                 name=name,
                 parent_implementation=creator_function,
                 service_type=arg_info.arg_type,
                 settings=dependency_config[name],
                 default_value=arg_info.default_value,
             )
             for name, arg_info in args_infos.items()
         }
 
-    def create(self, context: ResolvingContext, **kwargs):
+    def create(
+        self,
+        context: ResolvingContext,
+        dependency_node: DependencyNode,
+        **kwargs,
+    ):
         for arg_name, arg_dep in self.dependencies.items():
-            kwargs[arg_name] = arg_dep.resolve(context)
+            kwargs[arg_name] = arg_dep.resolve(context, dependency_node)
         built_instance = self.creator_function(**kwargs)
         return built_instance
 
 
 class DecoratorCreator(ImplementationCreator):
-    def __init__(self, service_type: type, decorator_type: type):
+    def __init__(
+        self, service_type: type, decorator_type: type, decorated_arg: str | None
+    ):
         self.service_type = service_type
         super().__init__(creator_function=decorator_type)
-        self.decorated_arg = next(
+
+        self.decorated_arg = decorated_arg or next(
             name
             for name, dep in self.dependencies.items()
             if dep.service_type == service_type
         )
         self.dependencies = {
             name: dep
             for name, dep in self.dependencies.items()
             if name != self.decorated_arg
         }
 
 
 class Decorator:
     def __init__(
-        self, service_type: type, decorator_type: type, filter: RegistartionFilter
+        self,
+        service_type: type,
+        decorator_type: type,
+        filter: RegistartionFilter,
+        decorated_arg: str | None,
     ):
         self.service_type = service_type
         self.decorator_type = decorator_type
         self.creator = DecoratorCreator(
-            service_type=service_type, decorator_type=decorator_type
+            service_type=service_type,
+            decorator_type=decorator_type,
+            decorated_arg=decorated_arg,
         )
         self.registartion_filter = filter
 
-    def decorate(self, instance: Any, context: ResolvingContext):
+    def decorate(
+        self,
+        instance: Any,
+        context: ResolvingContext,
+        dependency_node: DependencyNode,
+    ):
         kwargs = {}
         kwargs[self.creator.decorated_arg] = instance
-        return self.creator.create(context, **kwargs)
+        return self.creator.create(context, dependency_node, **kwargs)
 
 
 class Registration:
     def __init__(
         self,
         service_type: type,
         implementation: Callable,
-        lifestyle: LifestyleType,
+        lifespan: Lifespan,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
     ):
         self.service_type = service_type
         self.implementation = implementation
         self.creator = ImplementationCreator(
             creator_function=implementation, dependency_config=dependency_config
         )
-        self.lifestyle = lifestyle
+        self.lifespan = lifespan
         self.name = name
         self._id = str(uuid4())
         self.generic_mapping = get_typevar_to_type_mapping(self.service_type)
 
     @property
     def is_named(self):
         return self.name is not None
 
-    def build(self, context: ResolvingContext):
+    def build(self, context: ResolvingContext, dependency_node: DependencyNode):
+        next_node = FullDependencyNode(
+            service_type=self.service_type,
+            implementation=self.implementation,
+            parent=dependency_node,
+        )
+
         cached_instance = context.get_cached(self._id)
         if not cached_instance == _empty:
             return cached_instance
-        built_instance = self.creator.create(context)
-
+        built_instance = self.creator.create(context, next_node)
+        decorated_node = next_node
         for dec in context.find_decorators_that_apply(self):
-            built_instance = dec.decorate(built_instance, context)
+            next_dec_node = FullDependencyNode(
+                service_type=self.service_type,
+                implementation=dec.decorator_type,
+                parent=dependency_node,
+                decorated=decorated_node,
+            )
+            built_instance = dec.decorate(built_instance, context, next_dec_node)
+            decorated_node = next_dec_node
 
-        context.new_instance_created(self._id, built_instance, self.lifestyle)
+        context.new_instance_created(self._id, built_instance, self.lifespan)
         return built_instance
 
 
 class Registry:
     def __init__(self):
         self._registrations: dict[type, deque[Registration]] = defaultdict(deque)
         self._decorators: dict[type, deque[Decorator]] = defaultdict(deque)
         self._singletons: dict[str, Any] = {}
 
     def add_registration(self, registartion: Registration):
         self._registrations[registartion.service_type].appendleft(registartion)
 
     def add_decorator(self, decorator: Decorator):
-        self._decorators[decorator.service_type].appendleft(decorator)
+        self._decorators[decorator.service_type].append(decorator)
 
     def add_singleton_instance(self, registartion_id: str, instance: Any):
         self._singletons[registartion_id] = instance
 
     def get_registartions(self, service_type: type):
         return self._registrations[service_type]
 
@@ -336,23 +416,21 @@
             for d in self.registry.get_decorators(registration.service_type)
             if d.registartion_filter(registration)
         ]
 
     def get_cached(self, reg_id: str):
         return self._cache.get(reg_id, _empty)
 
-    def new_instance_created(
-        self, reg_id: str, instance: Any, lifestyle: LifestyleType
-    ):
-        if lifestyle == LifestyleType.singleton:
+    def new_instance_created(self, reg_id: str, instance: Any, lifespan: Lifespan):
+        if lifespan == Lifespan.singleton:
             self.registry.add_singleton_instance(reg_id, instance)
-        elif lifestyle == LifestyleType.scoped:
+        elif lifespan == Lifespan.scoped:
             self.scope.add_scoped_instance(reg_id, instance)
 
-        if lifestyle >= LifestyleType.once_per_graph:
+        if lifespan >= Lifespan.once_per_graph:
             self._cache[reg_id] = instance
 
 
 class Resolver(abc.ABC):
     @abc.abstractmethod
     def resolve(
         self,
@@ -412,44 +490,44 @@
         dependency_config: dict[str, DependencySettings] = {},
     ):
         if instance is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=lambda: instance,
-                    lifestyle=LifestyleType.scoped,
+                    lifespan=Lifespan.scoped,
                     name=name,
                 )
             )
         elif factory is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=factory,
-                    lifestyle=LifestyleType.scoped,
+                    lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
                 )
             )
         elif impl_type is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=impl_type,
-                    lifestyle=LifestyleType.scoped,
+                    lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
                 )
             )
         else:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=service_type,
-                    lifestyle=LifestyleType.scoped,
+                    lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
                 )
             )
 
     def _before_start(self):
         pass
@@ -490,94 +568,113 @@
     def register(self, *args):
         pass
 
     def resolve(self, *args):
         pass
 
 
+class NeedsScopedRegistrationError(Exception):
+    def __init__(self, service_type, name):
+        self.service_type = service_type
+        self.name = name
+
+    def __str__(self):
+        with_name = f" with {self.name}" if self.name else ""
+        return f"{self.service_type}{with_name} is expected to be used within a scope"
+
+
+def type_expected_to_be_scoped(service_type: type, name: str | None):
+    def raise_error():
+        raise NeedsScopedRegistrationError(service_type, name)
+
+    return raise_error
+
+
 class Container(Resolver):
     def __init__(self):
         self.registry = Registry()
         self.register(Container, instance=self)
         self.register(Resolver, instance=self)
 
     def register(
         self,
         service_type: type,
         impl_type: type | None = None,
         factory: Callable | None = None,
         instance: Any | None = None,
-        lifestyle: LifestyleType = LifestyleType.once_per_graph,
+        lifespan: Lifespan = Lifespan.once_per_graph,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
     ):
         if instance is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=lambda: instance,
                     dependency_config=dependency_config,
-                    lifestyle=LifestyleType.singleton,
+                    lifespan=Lifespan.singleton,
                     name=name,
                 )
             )
         elif factory is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=factory,
                     dependency_config=dependency_config,
-                    lifestyle=lifestyle,
+                    lifespan=lifespan,
                     name=name,
                 )
             )
         elif impl_type is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=impl_type,
                     dependency_config=dependency_config,
-                    lifestyle=lifestyle,
+                    lifespan=lifespan,
                     name=name,
                 )
             )
         else:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=service_type,
                     dependency_config=dependency_config,
-                    lifestyle=lifestyle,
+                    lifespan=lifespan,
                     name=name,
                 )
             )
 
     def register_subclasses(
         self,
         base_type: type,
-        lifestyle: LifestyleType = LifestyleType.once_per_graph,
+        lifespan: Lifespan = Lifespan.once_per_graph,
         type_filter: Callable[[type], bool] = constant(True),
     ):
         sub_classes = get_subclasses(base_type, type_filter)
 
         for sc in sub_classes:
-            self.register(base_type, sc, lifestyle=lifestyle)
-            self.register(sc, lifestyle=lifestyle)
+            self.register(base_type, sc, lifespan=lifespan)
+            self.register(sc, lifespan=lifespan)
 
     def register_decorator(
         self,
         service_type: type,
         decorator_type: type,
         registration_filter: Callable[[Registration], bool] = _all_registartions,
+        decorated_arg: str | None = None,
     ):
         self.registry.add_decorator(
             Decorator(
                 service_type=service_type,
                 decorator_type=decorator_type,
                 filter=registration_filter,
+                decorated_arg=decorated_arg,
             )
         )
 
     @staticmethod
     def _get_target_generic_base(generic_service_type: type, subclass: type):
         return next(
             (
@@ -590,75 +687,99 @@
             None,
         )
 
     def register_open_generic(
         self,
         generic_service_type: type,
         fallback_type: type | None = None,
-        lifestyle: LifestyleType = LifestyleType.once_per_graph,
+        lifespan: Lifespan = Lifespan.once_per_graph,
         name: str | None = None,
         type_filter: Callable[[type], bool] = constant(True),
     ):
         full_type_filter = fn_and(fn_not(is_abstract), type_filter)
         subclasses = get_subclasses(generic_service_type, full_type_filter)
         for subclass in subclasses:
             target_generic_base = self._get_target_generic_base(
                 generic_service_type, subclass
             )
             if target_generic_base:
-                self.register(target_generic_base, subclass, lifestyle=lifestyle)
+                self.register(target_generic_base, subclass, lifespan=lifespan)
 
         if fallback_type:
             self.register(
-                generic_service_type, fallback_type, lifestyle=lifestyle, name=name
+                generic_service_type, fallback_type, lifespan=lifespan, name=name
             )
 
     def register_open_generic_decorator(
         self,
         generic_service_type: type,
         generic_decorator_type: type,
         type_filter: Callable[[type], bool] = constant(True),
+        decorated_arg: str | None = None,
     ):
         full_type_filter = fn_and(fn_not(is_abstract), type_filter)
         subclasses = get_subclasses(generic_service_type, full_type_filter)
+        decorator_is_open_generic = is_open_generic_type(generic_decorator_type)
+
         for subclass in subclasses:
+
             target_generic_base = self._get_target_generic_base(
                 generic_service_type, subclass
             )
             if target_generic_base:
-                generic_values = get_generic_types(target_generic_base)
-                concrete_decorator = generic_decorator_type[generic_values]  # type: ignore
-                DecoratedType = types.new_class(
-                    f"DecoratedGeneric_{concrete_decorator.__name__}",
-                    (concrete_decorator,),
-                    {},
-                )
-
-                self.register_decorator(target_generic_base, DecoratedType)
+                if decorator_is_open_generic:
+                    generic_values = get_generic_types(target_generic_base)
+                    concrete_decorator = generic_decorator_type[generic_values]  # type: ignore
+                    DecoratedType = types.new_class(
+                        f"DecoratedGeneric_{concrete_decorator.__name__}",
+                        (concrete_decorator,),
+                        {},
+                    )
+
+                    self.register_decorator(
+                        target_generic_base, DecoratedType, decorated_arg=decorated_arg
+                    )
+                else:
+                    self.register_decorator(
+                        target_generic_base,
+                        generic_decorator_type,
+                        decorated_arg=decorated_arg,
+                    )
 
     def resolve(
         self,
         service_type,
         filter: RegistartionFilter = _all_registartions,
         scope: Scope = EmptyContainerScope(),
     ) -> Any:
         d = RootDependency(service_type, DependencySettings(filter=filter))
+        dependency_node = FullDependencyNode(
+            service_type=Container, implementation=Container
+        )
+
         context = ResolvingContext(self.registry, scope)
-        return d.resolve(context)
+        return d.resolve(context, dependency_node)
 
     def new_scope(
         self, ScopeClass: Type[ContainerScope] = ContainerScope, *args, **kwargs
     ) -> Scope:
         return ScopeClass(self, *args, **kwargs)
 
+    def expect_to_be_scoped(self, service_type: type, name: str | None = None):
+        self.register(
+            service_type=service_type,
+            factory=type_expected_to_be_scoped(service_type, name),
+            name=name,
+        )
+
     def apply_module(self, module_fn: Callable[[Container], None]):
         module_fn(self)
 
 
-@dataclass
+@dataclass(kw_only=True)
 class DependencySettings:
     value: Any = _empty
     use_default_paramater: bool = True
     filter: RegistartionFilter = _all_registartions
 
 
 RegistartionFilter = Callable[[Registration], bool]
```

### Comparing `clean_ioc-0.0.3/clean_ioc/functional_utils.py` & `clean_ioc-0.0.4/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.3/clean_ioc/registration_filters.py` & `clean_ioc-0.0.4/clean_ioc/registration_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from . import Registration
-from .functional_utils import constant
+from .functional_utils import constant, fn_not
 
 all_registrations = constant(True)
 
 
-def with_name(name: str):
+def with_name(name: str | None):
     """
     Filter registartions equal the name
     """
 
     def predicate(r: Registration):
         return r.name == name
 
@@ -44,14 +44,17 @@
 def is_named(r: Registration):
     """
     Filter registartions that have a name
     """
     return r.is_named
 
 
+is_not_named = with_name(None)
+
+
 def with_implementation(implementation: type):
     """
     Filter to registartions that have the implementation
     """
 
     def predicate(r: Registration):
         return r.implementation == implementation
```

### Comparing `clean_ioc-0.0.3/clean_ioc/type_filters.py` & `clean_ioc-0.0.4/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.0.3/clean_ioc/typing_utils.py` & `clean_ioc-0.0.4/clean_ioc/typing_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from typing import _GenericAlias  # type: ignore
+from typing import _GenericAlias, _SpecialGenericAlias  # type: ignore
 from typing import Generic, TypeVar
 from collections.abc import Callable
 from typing import get_type_hints
+import types
 from queue import Queue
 import inspect
 
+typingGenericAlias = (_GenericAlias, _SpecialGenericAlias, types.GenericAlias)
+
 
 def get_subclasses(cls: type, filter: Callable[[type], bool] = lambda t: True):
     queue = Queue()
     queue.put(cls)
     items = []
     while not queue.empty():
         t = queue.get_nowait()
@@ -48,17 +51,46 @@
     return True
 
 
 def get_type_args(cls: type):
     return getattr(cls, "__args__", ())
 
 
+def is_generic_type(tp: type):
+    """Test if the given type is a generic type. This includes Generic itself, but
+    excludes special typing constructs such as Union, Tuple, Callable, ClassVar.
+    Examples::
+
+        is_generic_type(int) == False
+        is_generic_type(Union[int, str]) == False
+        is_generic_type(Union[int, T]) == False
+        is_generic_type(ClassVar[List[int]]) == False
+        is_generic_type(Callable[..., T]) == False
+
+        is_generic_type(Generic) == True
+        is_generic_type(Generic[T]) == True
+        is_generic_type(Iterable[int]) == True
+        is_generic_type(Mapping) == True
+        is_generic_type(MutableMapping[T, List[int]]) == True
+        is_generic_type(Sequence[Union[str, bytes]]) == True
+    """
+
+    return (
+        isinstance(tp, type)
+        and issubclass(tp, Generic)
+        or isinstance(tp, typingGenericAlias)
+    )
+
+
 def is_open_generic_type(cls: type):
     type_args = get_type_args(cls)
-    return any([isinstance(t, TypeVar) for t in type_args])
+    if type_args:
+        return any([isinstance(t, TypeVar) for t in type_args])
+    else:
+        return is_generic_type(cls)
 
 
 def get_generic_type_args(type: type):
     queue = Queue()
     queue.put(type)
 
     while not queue.empty():
@@ -173,14 +205,16 @@
 
 def get_generic_types(cls: type):
     mapping = get_typevar_to_type_mapping(cls)
     return tuple(mapping.values())
 
 
 def try_to_complete_generic(open_type: _GenericAlias, closed_type: type) -> type:
+    if not getattr(open_type, "__args__", None):
+        return open_type
     if is_generic_type_closed(open_type):
         return open_type
 
     mapping = get_typevar_to_type_mapping(closed_type)
     new_args = tuple([mapping.get(a, a) for a in open_type.__args__])
     return open_type[new_args]
```

### Comparing `clean_ioc-0.0.3/pyproject.toml` & `clean_ioc-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "0.0.3"
+version = "0.0.4"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://github.com/peter-daly/clean_ioc"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://github.com/peter-daly/clean_ioc"
 readme = "README.md"
```

### Comparing `clean_ioc-0.0.3/setup.py` & `clean_ioc-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['clean_ioc']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'clean-ioc',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'An IOC Container for Python 3.10+',
-    'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n## Subclasses registration\n\nThis feature allows registartion of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifestyles\nLifestyles configure how long and resolved object says alive for\nThere are 4 lifestyle types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifestyle=LifestyleType.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifestyle=LifestyleType.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifestyle=LifestyleType.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifestyle=LifestyleType.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifestyle.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registartions & Registartion filters\n\nBy default the last registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.\n\nA registartion filter is simply function that receives a **Registartion** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registartion_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registartion and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistartionFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules (BETA feature)\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    container = Container()\n    container.register(ClientDependency)\n    container.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n',
+    'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the deepest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorTwo\n    type(root.child) # returns DecoratorOne\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registartion of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registartions & Registartion filters\n\nBy default the last registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registartion filter when we resolve.\n\nA registartion filter is simply function that receives a **Registartion** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registartion filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registartion_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registartion and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistartionFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistartionFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registartion using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules (BETA feature)\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\n\n```\n',
     'author': 'Peter Daly',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/peter-daly/clean_ioc',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `clean_ioc-0.0.3/PKG-INFO` & `clean_ioc-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-ioc
-Version: 0.0.3
+Version: 0.0.4
 Summary: An IOC Container for Python 3.10+
 Home-page: https://github.com/peter-daly/clean_ioc
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -203,14 +203,44 @@
 container.register(int, instance=10)
 
 client = container.resolve(Client)
 
 client.get_number() # returns 20
 ```
 
+
+Decorators are resolved in order of when first registered. So the first registered decorator is the deepest in the class tree
+
+
+```python
+    class Concrete:
+        pass
+
+    class DecoratorOne(Concrete):
+        def __init__(self, child: Concrete):
+            self.child = child
+
+    class DecoratorTwo(Concrete):
+        def __init__(self, child: Concrete):
+            self.child = child
+
+    container = Container()
+
+    container.register(Concrete)
+    container.register_decorator(Concrete, DecoratorOne)
+    container.register_decorator(Concrete, DecoratorTwo)
+
+    root = container.resolve(Concrete)
+
+    type(root) # returns DecoratorTwo
+    type(root.child) # returns DecoratorOne
+    type(root.child.child) # returns Concrete
+```
+
+
 ## Subclasses registration
 
 This feature allows registartion of all subclasses of a giveb type
 
 ```python
 class Client(abc.ABC)
     @abc.abstractmethod
@@ -237,45 +267,45 @@
 twenty_client.get_number() # returns 20
 
 # Resolve all subsclasses of Client
 client = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]
 ```
 
 
-## Lifestyles
-Lifestyles configure how long and resolved object says alive for
-There are 4 lifestyle types
+## Lifespans
+Lifespans configure how long and resolved object says alive for
+There are 4 lifespan types
 
 ### transient
 Always create a new instance
 
 ```python
-container.register(Client, lifestyle=LifestyleType.transient)
+container.register(Client, lifespan=Lifespan.transient)
 ```
 
 
 ### once_per_graph (Default behaviour)
 Only create one instance throughout the resolve call
 
 ```python
-container.register(Client, lifestyle=LifestyleType.once_per_graph)
+container.register(Client, lifespan=Lifespan.once_per_graph)
 ```
 
 ### scoped
 Only create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**
 
 ```python
-container.register(Client, lifestyle=LifestyleType.scoped)
+container.register(Client, lifespan=Lifespan.scoped)
 ```
 
 ### singleton
 Only one instance of the object is created throughout the lifespan of the container
 
 ```python
-container.register(Client, lifestyle=LifestyleType.singleton)
+container.register(Client, lifespan=Lifespan.singleton)
 ```
 
 *Note:*
 When registering an instance, then the behaviour is always singleton
 
 ```python
 container.register(int, instance=10)
@@ -360,15 +390,15 @@
 h1.handle(HelloCommand()) # prints 'A VERY BIG\nHELLO'
 h2.handle(GoodbyeCommand()) # prints 'A VERY BIG\nGOODBYE'
 
 ```
 
 ## Scopes
 
-Scopes are a way to create a sub container that will live for a certain lifestyle.
+Scopes are a way to create a sub container that will live for a certain lifespan.
 Some good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system
 
 
 ```python
 class Client
     def __init__(self, number: int)
         return number
@@ -576,18 +606,49 @@
     def __init__(self, dep: ClientDependency)
         self.dep = dep
 
     def get_number(self):
         return self.dep.get_int()
 
 def client_module(c: Container):
-    container = Container()
-    container.register(ClientDependency)
-    container.register(Client)
+    c.register(ClientDependency)
+    c.register(Client)
 
 container.apply_module(client_module)
 
 client = container.resolve(Client)
 
 client.get_number() # returns 10
 ```
 
+
+
+## DependencyContext (BETA feature)
+
+You can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing
+One example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context
+
+```python
+class Logger
+    def __init__(self, module):
+        self.module = module
+
+class Client
+    def __init__(self, logger: Logger)
+        self.logger = logger
+
+def logger_fac(context: DependencyContext):
+    module = context.parent.__module__
+    return Logger(module)
+
+
+container = Container()
+container.register(Client)
+container.register(Logger, factory=logger_fac)
+
+container.apply_module(client_module)
+
+client = container.resolve(Client)
+
+
+```
+
```

