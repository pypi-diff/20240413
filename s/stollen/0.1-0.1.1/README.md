# Comparing `tmp/stollen-0.1.tar.gz` & `tmp/stollen-0.1.1.tar.gz`

## Comparing `stollen-0.1.tar` & `stollen-0.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 stollen-0.1/.editorconfig
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 stollen-0.1/.pre-commit.config.yaml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 stollen-0.1/Makefile
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 stollen-0.1/.github/workflows/pypi-release.yml
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 stollen-0.1/examples/coingecko.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/__init__.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/client.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/exceptions.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/signature_factory.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/methods/__init__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/methods/get_balance.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/types/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/types/balance.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptomus/types/balance_unit.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/__init__.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/client.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/exceptions.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/methods/__init__.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/methods/create_invoice.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/methods/get_me.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/types/__init__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/types/invoice.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 stollen-0.1/examples/cryptopay/types/profile.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 stollen-0.1/examples/xrocket/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 stollen-0.1/examples/xrocket/client.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 stollen-0.1/examples/xrocket/exceptions.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 stollen-0.1/examples/xrocket/methods/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 stollen-0.1/examples/xrocket/methods/get_app_info.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 stollen-0.1/examples/xrocket/types/__init__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 stollen-0.1/examples/xrocket/types/app_info.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 stollen-0.1/examples/xrocket/types/balance.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 stollen-0.1/stollen/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 stollen-0.1/stollen/__meta__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 stollen-0.1/stollen/exceptions.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 stollen-0.1/stollen/method.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 stollen-0.1/stollen/object.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stollen-0.1/stollen/py.typed
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 stollen-0.1/stollen/types.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 stollen-0.1/stollen/client/__init__.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 stollen-0.1/stollen/client/client.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 stollen-0.1/stollen/client/context_controller.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 stollen-0.1/stollen/client/api_access/__init__.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 stollen-0.1/stollen/client/api_access/factory.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 stollen-0.1/stollen/client/api_access/nodes.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 stollen-0.1/stollen/enums/__init__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 stollen-0.1/stollen/enums/access_node_type.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 stollen-0.1/stollen/enums/http_method.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stollen-0.1/stollen/session/__init__.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 stollen-0.1/stollen/session/aiohttp.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 stollen-0.1/stollen/session/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stollen-0.1/stollen/utils/__init__.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 stollen-0.1/stollen/utils/mapping.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stollen-0.1/stollen/utils/text.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 stollen-0.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 stollen-0.1/LICENSE
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 stollen-0.1/README.rst
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 stollen-0.1/pyproject.toml
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 stollen-0.1/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 stollen-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 stollen-0.1.1/.pre-commit.config.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 stollen-0.1.1/Makefile
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 stollen-0.1.1/.github/workflows/pypi-release.yml
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/coingecko.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/__init__.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/client.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/exceptions.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/signature_factory.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/methods/__init__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/methods/get_balance.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/types/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/types/balance.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptomus/types/balance_unit.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/__init__.py
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/client.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/exceptions.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/methods/__init__.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/methods/create_invoice.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/methods/get_me.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/types/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/types/invoice.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/cryptopay/types/profile.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/xrocket/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/xrocket/client.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/xrocket/exceptions.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/xrocket/methods/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/xrocket/methods/get_app_info.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/xrocket/types/__init__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/xrocket/types/app_info.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 stollen-0.1.1/examples/xrocket/types/balance.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/__meta__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/exceptions.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/method.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/object.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/py.typed
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/types.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/client/__init__.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/client/client.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/client/context_controller.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/client/api_access/__init__.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/client/api_access/factory.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/client/api_access/nodes.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/enums/__init__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/enums/access_node_type.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/enums/http_method.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/session/__init__.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/session/aiohttp.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/session/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/utils/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/utils/mapping.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 stollen-0.1.1/stollen/utils/text.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 stollen-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 stollen-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 stollen-0.1.1/README.rst
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 stollen-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 stollen-0.1.1/PKG-INFO
```

### Comparing `stollen-0.1/.pre-commit.config.yaml` & `stollen-0.1.1/.pre-commit.config.yaml`

 * *Files identical despite different names*

### Comparing `stollen-0.1/.github/workflows/pypi-release.yml` & `stollen-0.1.1/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `stollen-0.1/examples/coingecko.py` & `stollen-0.1.1/examples/coingecko.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/examples/cryptomus/client.py` & `stollen-0.1.1/examples/cryptomus/client.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/examples/cryptomus/signature_factory.py` & `stollen-0.1.1/examples/cryptomus/signature_factory.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/examples/cryptopay/client.py` & `stollen-0.1.1/examples/cryptopay/client.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/examples/cryptopay/methods/create_invoice.py` & `stollen-0.1.1/examples/cryptopay/methods/create_invoice.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/examples/cryptopay/types/invoice.py` & `stollen-0.1.1/examples/cryptopay/types/invoice.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/examples/xrocket/client.py` & `stollen-0.1.1/examples/xrocket/client.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/stollen/exceptions.py` & `stollen-0.1.1/stollen/exceptions.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/stollen/method.py` & `stollen-0.1.1/stollen/method.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from .types import StollenT
 
 if TYPE_CHECKING:
     from .types import HTTPMethodType
 
 
 class StollenMethod(
-    StollenContextController[StollenClientT], BaseModel, Generic[StollenT, StollenClientT]
+    StollenContextController[StollenClientT],
+    BaseModel,
+    Generic[StollenT, StollenClientT],
 ):
     http_method: ClassVar[HTTPMethodType]
     api_method: ClassVar[str]
     returning: ClassVar[type[Any]]
     type_adapter: ClassVar[TypeAdapter[Any]]
 
     async def emit(self, client: Stollen) -> StollenT:
```

### Comparing `stollen-0.1/stollen/object.py` & `stollen-0.1.1/stollen/object.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/stollen/client/client.py` & `stollen-0.1.1/stollen/client/client.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/stollen/client/context_controller.py` & `stollen-0.1.1/stollen/client/context_controller.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/stollen/client/api_access/factory.py` & `stollen-0.1.1/stollen/client/api_access/factory.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/stollen/session/aiohttp.py` & `stollen-0.1.1/stollen/session/aiohttp.py`

 * *Files identical despite different names*

### Comparing `stollen-0.1/stollen/session/base.py` & `stollen-0.1.1/stollen/session/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,17 @@
         cls,
         client: Stollen,
         method: StollenMethod[StollenT, StollenClientT],
         payload: dict[str, Any],
     ) -> str:
         if not client.use_method_placeholders:
             return method.api_method
-        return method.api_method.format(**{key: payload.pop(key) for key in payload.copy()})
+        return method.api_method.format(
+            **{key: payload.pop(key) for key in payload if f"{{{key}}}" in method.api_method}
+        )
 
     def _apply_access_nodes(
         self,
         nodes: Iterable[BaseAPIAccessNodeFactory | APIAccessNode],
         headers: dict[str, Any],
         placeholders: dict[str, Any],
         client: Stollen,
```

### Comparing `stollen-0.1/LICENSE` & `stollen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stollen-0.1/README.rst` & `stollen-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `stollen-0.1/pyproject.toml` & `stollen-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 )
 '''
 
 
 [tool.ruff]
 target-version = "py38"
 line-length = 99
-select = [
+lint.select = [
     "C",
     "DTZ",
     "E",
     "F",
     "I",
     "ICN",
     "ISC",
```

### Comparing `stollen-0.1/PKG-INFO` & `stollen-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: stollen
-Version: 0.1
+Version: 0.1.1
 Summary: An asynchronous framework to easily build a client-side API
 Project-URL: Repository, https://github.com/wakaree/stollen
 Author: nullmatawasoradesu
 Maintainer: nullmatawasoradesu
 License-Expression: MIT
 License-File: LICENSE
 Keywords: api,asyncio,client,framework,wrapper
```

