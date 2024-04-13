# Comparing `tmp/zorge-1.0.0.tar.gz` & `tmp/zorge-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zorge-1.0.0.tar", max compression
+gzip compressed data, was "zorge-1.1.0.tar", max compression
```

## Comparing `zorge-1.0.0.tar` & `zorge-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-01-04 14:56:28.854602 zorge-1.0.0/LICENSE
--rw-r--r--   0        0        0      317 2023-02-26 14:53:45.189968 zorge-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        2 2022-10-20 07:19:05.275000 zorge-1.0.0/zorge/__init__.py
--rw-r--r--   0        0        0     2602 2023-02-24 16:04:27.562857 zorge-1.0.0/zorge/contracts.py
--rw-r--r--   0        0        0       84 2022-10-20 07:19:05.278000 zorge-1.0.0/zorge/di/__init__.py
--rw-r--r--   0        0        0      249 2023-02-19 14:21:42.999270 zorge-1.0.0/zorge/di/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3792 2023-02-24 15:11:44.057128 zorge-1.0.0/zorge/di/__pycache__/container.cpython-310.pyc
--rw-r--r--   0        0        0     1592 2023-02-24 16:09:13.314085 zorge-1.0.0/zorge/di/__pycache__/generic.cpython-310.pyc
--rw-r--r--   0        0        0     4180 2023-02-24 16:07:58.056459 zorge-1.0.0/zorge/di/__pycache__/provider.cpython-310.pyc
--rw-r--r--   0        0        0     4422 2023-02-24 15:11:43.816750 zorge-1.0.0/zorge/di/container.py
--rw-r--r--   0        0        0     2073 2023-02-24 16:09:13.066168 zorge-1.0.0/zorge/di/generic.py
--rw-r--r--   0        0        0     4684 2023-02-24 16:07:57.805398 zorge-1.0.0/zorge/di/provider.py
--rw-r--r--   0        0        0     2755 2023-02-24 15:44:35.734330 zorge-1.0.0/zorge/exceptions.py
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 zorge-1.0.0/setup.py
--rw-r--r--   0        0        0      283 1970-01-01 00:00:00.000000 zorge-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-04 14:56:28.854602 zorge-1.1.0/LICENSE
+-rw-r--r--   0        0        0      286 2024-04-13 14:07:59.244876 zorge-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-02-19 15:31:10.223460 zorge-1.1.0/zorge/.DS_Store
+-rw-r--r--   0        0        0      130 2024-04-11 07:57:07.720615 zorge-1.1.0/zorge/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-11 07:57:07.720731 zorge-1.1.0/zorge/contracts/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-11 07:57:07.720842 zorge-1.1.0/zorge/contracts/domain.py
+-rw-r--r--   0        0        0     1309 2024-04-11 07:57:07.720917 zorge-1.1.0/zorge/contracts/internal.py
+-rw-r--r--   0        0        0       87 2024-04-11 07:57:07.720992 zorge-1.1.0/zorge/exceptions/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-11 07:57:07.721065 zorge-1.1.0/zorge/exceptions/di.py
+-rw-r--r--   0        0        0        1 2024-04-11 07:57:07.721285 zorge-1.1.0/zorge/implementation/__init__.py
+-rw-r--r--   0        0        0     6888 2024-04-11 07:57:07.721589 zorge-1.1.0/zorge/implementation/container.py
+-rw-r--r--   0        0        0     4647 2024-04-11 07:57:07.721881 zorge-1.1.0/zorge/implementation/resolver.py
+-rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 zorge-1.1.0/PKG-INFO
```

### Comparing `zorge-1.0.0/LICENSE` & `zorge-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zorge-1.0.0/zorge/di/provider.py` & `zorge-1.1.0/zorge/implementation/resolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,116 @@
-import inspect
-import typing
 import collections.abc
-import itertools
+import types
+import typing
 
-from .. import contracts, exceptions
-from .generic import shutdown, startup
+from .. import contracts
 
 
-class DependencyProvider(contracts.DependencyProvider):
+class Resolver:
     def __init__(
         self,
-        bindings: contracts.DependencyBingingRegistry,
-        callbacks: typing.Iterable[contracts.DependencyBindingRecord],
-        literals: typing.Mapping,
-        container_singleton_registry: contracts.SingletonRegistry
+        unit_registry: contracts.internal.ContainerUnitRegistry,
+        callback_registry: collections.abc.MutableSequence[contracts.internal.ContainerUnit],
+        global_cache: contracts.internal.InstanceCacheType | None = None
     ):
-        self._bindings = bindings
-        self._callbacks = callbacks
-        self._literals = literals
-        self._container_singleton_registry = container_singleton_registry
-        self._provider_singleton_registry: contracts.SingletonRegistry = {}
+        self._unit_registry = unit_registry
+        self._callback_registry = callback_registry
+        self._global_cache = global_cache or {}
+        self._local_cache: contracts.internal.InstanceCacheType = {}
+        self._context = None
 
-    async def get(
+    def add_context(
         self,
-        contract: contracts.DependencyBindingContract,
-        context: contracts.ContextType | None = None
+        contract: contracts.ContractType,
+        data: collections.abc.Mapping
     ):
-        result = await self._resolve(contract, context=context)
-        if result is contracts.NotDefined:
-            result = None
-        return result
+        self._context = self._context or {contract: data}
 
-    def __getitem__(self, contract: contracts.DependencyBindingContract):
-        return self._get_singleton(contract)
+    async def resolve(
+        self,
+        contract: contracts.ContractType,
+        execution_context: collections.abc.Mapping[str, typing.Any] | None = None,
+        initial_context: collections.abc.Mapping[str, typing.Any] | None = None
+    ):
+        return await self._resolve(
+            contract=contract,
+            execution_context=execution_context,
+            initial_context=initial_context
+        )
+
+    async def shutdown(self, exc_type, exc_val):
+        for callback_unit in self._callback_registry:
+            if callback_unit.cache_scope is contracts.CacheScope.RESOLVER:
+                instance = self._local_cache.get(callback_unit.contract)
+                if callback_unit.implementation_execution_type is contracts.internal.ImplementationExecutionType.ASYNC:
+                    await callback_unit.implementation(instance, {'exc_type': exc_type, 'exc_val': exc_val})
+                else:
+                    callback_unit.implementation(instance, {'exc_type': exc_type, 'exc_val': exc_val})
 
     async def __aenter__(self):
-        await self.startup()
         return self
 
-    async def __aexit__(self, exc_type, exc, tb):
-        await self.shutdown(exc_type)
-
-    def __iter__(self) -> typing.Generator[contracts.DependencyBindingRecord, None, None]:
-        for record in itertools.chain(self._bindings.values(), self._callbacks):
-            yield record
-
-    async def shutdown(self, exc_type: typing.Any):
-        await shutdown(self, exc_type, contracts.DependencyBindingScope.INSTANCE)
-
-    async def startup(self):
-        await startup(self)
-
-    def get_registry(
-        self
-    ) -> collections.abc.Mapping[
-        contracts.DependencyBindingContract,
-        contracts.DependencyBindingRecord
-    ]:
-        return self._provider_singleton_registry
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.shutdown(exc_type, exc_val)
 
     async def _resolve(
         self,
-        contract: contracts.DependencyBindingContract,
-        context: contracts.ContextType | None
+        contract: contracts.ContractType,
+        default: typing.Any | None = None,
+        execution_context: collections.abc.Mapping[str, typing.Any] | None = None,
+        initial_context: collections.abc.Mapping[str, typing.Any] | None = None
     ):
-        binding_record = self._bindings.get(contract)
-        if not binding_record:
-            return contracts.NotDefined
-
-        if (
-            binding_record.binding_type == contracts.DependencyBindingType.SINGLETON and
-            isinstance(context, collections.abc.Mapping) and
-            contract in context
-        ):
-            raise exceptions.CannotPassContextToSingleton(contract=contract)
-
-        if result := self._get_singleton(contract):
-            return result
-
-        instance = binding_record.instance
-
-        if inspect.iscoroutinefunction(instance):
-            result = await instance()
-        elif not inspect.isclass(instance):
-            result = instance
-        else:
-            init_spec = inspect.getfullargspec(getattr(instance, '__init__'))
-            params = {}
-            for param_name, param_type in init_spec.annotations.items():
-                value = contracts.NotDefined
-                if isinstance(context, collections.abc.Mapping) and contract in context:
-                    value = context[contract].get(param_name, contracts.NotDefined)
-                if value is contracts.NotDefined and self._literals:
-                    value = self._literals.get(param_name, contracts.NotDefined)
-                if value is contracts.NotDefined:
-                    value = await self._resolve(param_type, context=context)
-                if value is not contracts.NotDefined:
-                    params[param_name] = value
-            try:
-                result = instance(**params)
-            except TypeError as e:
-                raise exceptions.CannotResolveParams(contract=contract, message=str(e))
-
-        self._register_singleton(contract, result)
+        if self._context and contract in self._context:
+            return self._context.get(contract)
+        if contract in self._local_cache:
+            return self._local_cache.get(contract)
+        if contract in self._global_cache:
+            return self._global_cache.get(contract)
+        if (unit := self._unit_registry.get(contract)) is None:
+            return default
+
+        result = None
+        if unit.implementation_kind is contracts.internal.ImplementationKind.STATIC:
+            result = unit.implementation
+        elif unit.implementation_kind is contracts.internal.ImplementationKind.CLASS:
+            params = {
+                k: await self._apply_context_value(k, v, initial_context)
+                for k, v in unit.init_signature.parameters.items()
+                if k not in ('args', 'kwargs')
+            } if unit.init_signature else {}
+            result = unit.implementation(**params)
+        elif unit.implementation_kind is contracts.internal.ImplementationKind.CALLABLE:
+            params = {
+                k: await self._apply_context_value(k, v, execution_context)
+                for k, v in unit.execution_signature.parameters.items()
+            } if unit.execution_signature else {}
+            if unit.implementation_execution_type is contracts.internal.ImplementationExecutionType.ASYNC:
+                result = await unit.implementation(**params)
+            else:
+                result = unit.implementation(**params)
+
+        if result is not None:
+            if unit.cache_scope is contracts.CacheScope.RESOLVER:
+                self._local_cache[contract] = result
+            elif unit.cache_scope is contracts.CacheScope.CONTAINER:
+                self._global_cache[contract] = result
 
         return result
 
-    def _get_singleton(
-        self,
-        contract: contracts.DependencyBindingContract
-    ):
-        instance = self._provider_singleton_registry.get(contract)
-        if not instance:
-            instance = self._container_singleton_registry.get(contract)
-        return instance
-
-    def _register_singleton(
+    async def _apply_context_value(
         self,
-        contract: contracts.DependencyBindingContract,
-        instance: contracts.SingletonInstance
+        key: str,
+        value: contracts.internal.FunctionParameter,
+        context: collections.abc.Mapping[str, typing.Any]
     ):
-        binding_record = self._bindings.get(contract)
-        if not binding_record:
-            return
-        if binding_record.binding_type != contracts.DependencyBindingType.SINGLETON:
-            return
+        if context and key in context:
+            return context.get(key)
 
-        if binding_record.scope == contracts.DependencyBindingScope.INSTANCE:
-            self._provider_singleton_registry[contract] = instance
+        args = list(filter(lambda x: x is not types.NoneType, typing.get_args(value.type)))
+        if len(args) > 1:
+            raise Exception("Cannot resolve more than 1 contract")
+        elif len(args) == 1:
+            _type = args[0]
         else:
-            self._container_singleton_registry[contract] = instance
+            _type = value.type
+
+        return await self._resolve(_type, value.default)
```

