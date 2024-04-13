# Comparing `tmp/postgrest-0.16.2.tar.gz` & `tmp/postgrest-0.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgrest-0.16.2.tar", max compression
+gzip compressed data, was "postgrest-0.16.3.tar", max compression
```

## Comparing `postgrest-0.16.2.tar` & `postgrest-0.16.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1077 2024-03-23 11:54:22.969316 postgrest-0.16.2/LICENSE
--rw-r--r--   0        0        0     4078 2024-03-23 11:54:22.969316 postgrest-0.16.2/README.md
--rw-r--r--   0        0        0      941 2024-03-23 11:54:23.733311 postgrest-0.16.2/postgrest/__init__.py
--rw-r--r--   0        0        0       35 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/_async/__init__.py
--rw-r--r--   0        0        0     3263 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/_async/client.py
--rw-r--r--   0        0        0    13486 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/_async/request_builder.py
--rw-r--r--   0        0        0       35 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/_sync/__init__.py
--rw-r--r--   0        0        0     3217 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/_sync/client.py
--rw-r--r--   0        0        0    13410 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/_sync/request_builder.py
--rw-r--r--   0        0        0     1918 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/base_client.py
--rw-r--r--   0        0        0    21704 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/base_request_builder.py
--rw-r--r--   0        0        0      151 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/constants.py
--rw-r--r--   0        0        0      409 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/deprecated_client.py
--rw-r--r--   0        0        0      422 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/deprecated_get_request_builder.py
--rw-r--r--   0        0        0     1510 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/py.typed
--rw-r--r--   0        0        0      986 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/types.py
--rw-r--r--   0        0        0     1152 2024-03-23 11:54:22.973316 postgrest-0.16.2/postgrest/utils.py
--rw-r--r--   0        0        0     1915 2024-03-23 11:54:23.729311 postgrest-0.16.2/pyproject.toml
--rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 postgrest-0.16.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-13 09:57:42.465729 postgrest-0.16.3/LICENSE
+-rw-r--r--   0        0        0     4078 2024-04-13 09:57:42.465729 postgrest-0.16.3/README.md
+-rw-r--r--   0        0        0      941 2024-04-13 09:57:44.333740 postgrest-0.16.3/postgrest/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_async/__init__.py
+-rw-r--r--   0        0        0     3263 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_async/client.py
+-rw-r--r--   0        0        0    14157 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_async/request_builder.py
+-rw-r--r--   0        0        0       35 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_sync/__init__.py
+-rw-r--r--   0        0        0     3217 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_sync/client.py
+-rw-r--r--   0        0        0    14089 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/_sync/request_builder.py
+-rw-r--r--   0        0        0     1918 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/base_client.py
+-rw-r--r--   0        0        0    22420 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/base_request_builder.py
+-rw-r--r--   0        0        0      151 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/constants.py
+-rw-r--r--   0        0        0      409 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/deprecated_client.py
+-rw-r--r--   0        0        0      422 2024-04-13 09:57:42.465729 postgrest-0.16.3/postgrest/deprecated_get_request_builder.py
+-rw-r--r--   0        0        0     1510 2024-04-13 09:57:42.469729 postgrest-0.16.3/postgrest/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-13 09:57:42.469729 postgrest-0.16.3/postgrest/py.typed
+-rw-r--r--   0        0        0      986 2024-04-13 09:57:42.469729 postgrest-0.16.3/postgrest/types.py
+-rw-r--r--   0        0        0     1152 2024-04-13 09:57:42.469729 postgrest-0.16.3/postgrest/utils.py
+-rw-r--r--   0        0        0     1915 2024-04-13 09:57:44.333740 postgrest-0.16.3/pyproject.toml
+-rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 postgrest-0.16.3/PKG-INFO
```

### Comparing `postgrest-0.16.2/LICENSE` & `postgrest-0.16.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.2/README.md` & `postgrest-0.16.3/README.md`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.2/postgrest/__init__.py` & `postgrest-0.16.3/postgrest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "0.16.2"
+__version__ = "0.16.3"
 
 from httpx import Timeout
 
 from ._async.client import AsyncPostgrestClient
 from ._async.request_builder import (
     AsyncFilterRequestBuilder,
     AsyncMaybeSingleRequestBuilder,
```

### Comparing `postgrest-0.16.2/postgrest/_async/client.py` & `postgrest-0.16.3/postgrest/_async/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.2/postgrest/_async/request_builder.py` & `postgrest-0.16.3/postgrest/_sync/request_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,49 +17,49 @@
     pre_insert,
     pre_select,
     pre_update,
     pre_upsert,
 )
 from ..exceptions import APIError, generate_default_error_message
 from ..types import ReturnMethod
-from ..utils import AsyncClient, get_origin_and_cast
+from ..utils import SyncClient, get_origin_and_cast
 
 _ReturnT = TypeVar("_ReturnT")
 
 
-class AsyncQueryRequestBuilder(Generic[_ReturnT]):
+class SyncQueryRequestBuilder(Generic[_ReturnT]):
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
-        json: dict,
+        json: Union[dict, list],
     ) -> None:
         self.session = session
         self.path = path
         self.http_method = http_method
         self.headers = headers
         self.params = params
         self.json = json
 
-    async def execute(self) -> APIResponse[_ReturnT]:
+    def execute(self) -> APIResponse[_ReturnT]:
         """Execute the query.
 
         .. tip::
             This is the last method called, after the query is built.
 
         Returns:
             :class:`APIResponse`
 
         Raises:
             :class:`APIError` If the API raised an error.
         """
-        r = await self.session.request(
+        r = self.session.request(
             self.http_method,
             self.path,
             json=self.json,
             params=self.params,
             headers=self.headers,
         )
         try:
@@ -78,44 +78,44 @@
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
         except JSONDecodeError as e:
             raise APIError(generate_default_error_message(r))
 
 
-class AsyncSingleRequestBuilder(Generic[_ReturnT]):
+class SyncSingleRequestBuilder(Generic[_ReturnT]):
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         self.session = session
         self.path = path
         self.http_method = http_method
         self.headers = headers
         self.params = params
         self.json = json
 
-    async def execute(self) -> SingleAPIResponse[_ReturnT]:
+    def execute(self) -> SingleAPIResponse[_ReturnT]:
         """Execute the query.
 
         .. tip::
             This is the last method called, after the query is built.
 
         Returns:
             :class:`SingleAPIResponse`
 
         Raises:
             :class:`APIError` If the API raised an error.
         """
-        r = await self.session.request(
+        r = self.session.request(
             self.http_method,
             self.path,
             json=self.json,
             params=self.params,
             headers=self.headers,
         )
         try:
@@ -127,19 +127,19 @@
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
         except JSONDecodeError as e:
             raise APIError(generate_default_error_message(r))
 
 
-class AsyncMaybeSingleRequestBuilder(AsyncSingleRequestBuilder[_ReturnT]):
-    async def execute(self) -> Optional[SingleAPIResponse[_ReturnT]]:
+class SyncMaybeSingleRequestBuilder(SyncSingleRequestBuilder[_ReturnT]):
+    def execute(self) -> Optional[SingleAPIResponse[_ReturnT]]:
         r = None
         try:
-            r = await AsyncSingleRequestBuilder[_ReturnT].execute(self)
+            r = SyncSingleRequestBuilder[_ReturnT].execute(self)
         except APIError as e:
             if e.details and "The result contains 0 rows" in e.details:
                 return None
         if not r:
             raise APIError(
                 {
                     "message": "Missing response",
@@ -148,256 +148,267 @@
                     "details": "Postgrest couldn't retrieve response, please check traceback of the code. Please create an issue in `supabase-community/postgrest-py` if needed.",
                 }
             )
         return r
 
 
 # ignoring type checking as a workaround for https://github.com/python/mypy/issues/9319
-class AsyncFilterRequestBuilder(BaseFilterRequestBuilder[_ReturnT], AsyncQueryRequestBuilder[_ReturnT]):  # type: ignore
+class SyncFilterRequestBuilder(BaseFilterRequestBuilder[_ReturnT], SyncQueryRequestBuilder[_ReturnT]):  # type: ignore
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         get_origin_and_cast(BaseFilterRequestBuilder[_ReturnT]).__init__(
             self, session, headers, params
         )
-        get_origin_and_cast(AsyncQueryRequestBuilder[_ReturnT]).__init__(
+        get_origin_and_cast(SyncQueryRequestBuilder[_ReturnT]).__init__(
             self, session, path, http_method, headers, params, json
         )
 
 
 # this exists for type-safety. see https://gist.github.com/anand2312/93d3abf401335fd3310d9e30112303bf
-class AsyncRPCFilterRequestBuilder(
-    BaseRPCRequestBuilder[_ReturnT], AsyncSingleRequestBuilder[_ReturnT]
+class SyncRPCFilterRequestBuilder(
+    BaseRPCRequestBuilder[_ReturnT], SyncSingleRequestBuilder[_ReturnT]
 ):
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         get_origin_and_cast(BaseFilterRequestBuilder[_ReturnT]).__init__(
             self, session, headers, params
         )
-        get_origin_and_cast(AsyncSingleRequestBuilder[_ReturnT]).__init__(
+        get_origin_and_cast(SyncSingleRequestBuilder[_ReturnT]).__init__(
             self, session, path, http_method, headers, params, json
         )
 
 
 # ignoring type checking as a workaround for https://github.com/python/mypy/issues/9319
-class AsyncSelectRequestBuilder(BaseSelectRequestBuilder[_ReturnT], AsyncQueryRequestBuilder[_ReturnT]):  # type: ignore
+class SyncSelectRequestBuilder(BaseSelectRequestBuilder[_ReturnT], SyncQueryRequestBuilder[_ReturnT]):  # type: ignore
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         get_origin_and_cast(BaseSelectRequestBuilder[_ReturnT]).__init__(
             self, session, headers, params
         )
-        get_origin_and_cast(AsyncQueryRequestBuilder[_ReturnT]).__init__(
+        get_origin_and_cast(SyncQueryRequestBuilder[_ReturnT]).__init__(
             self, session, path, http_method, headers, params, json
         )
 
-    def single(self) -> AsyncSingleRequestBuilder[_ReturnT]:
+    def single(self) -> SyncSingleRequestBuilder[_ReturnT]:
         """Specify that the query will only return a single row in response.
 
         .. caution::
             The API will raise an error if the query returned more than one row.
         """
         self.headers["Accept"] = "application/vnd.pgrst.object+json"
-        return AsyncSingleRequestBuilder[_ReturnT](
+        return SyncSingleRequestBuilder[_ReturnT](
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
-    def maybe_single(self) -> AsyncMaybeSingleRequestBuilder[_ReturnT]:
+    def maybe_single(self) -> SyncMaybeSingleRequestBuilder[_ReturnT]:
         """Retrieves at most one row from the result. Result must be at most one row (e.g. using `eq` on a UNIQUE column), otherwise this will result in an error."""
         self.headers["Accept"] = "application/vnd.pgrst.object+json"
-        return AsyncMaybeSingleRequestBuilder[_ReturnT](
+        return SyncMaybeSingleRequestBuilder[_ReturnT](
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
     def text_search(
         self, column: str, query: str, options: dict[str, Any] = {}
-    ) -> AsyncFilterRequestBuilder[_ReturnT]:
+    ) -> SyncFilterRequestBuilder[_ReturnT]:
         type_ = options.get("type")
         type_part = ""
         if type_ == "plain":
             type_part = "pl"
         elif type_ == "phrase":
             type_part = "ph"
         elif type_ == "web_search":
             type_part = "w"
         config_part = f"({options.get('config')})" if options.get("config") else ""
         self.params = self.params.add(column, f"{type_part}fts{config_part}.{query}")
 
-        return AsyncQueryRequestBuilder[_ReturnT](
+        return SyncQueryRequestBuilder[_ReturnT](
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
-    def csv(self) -> AsyncSingleRequestBuilder[str]:
+    def csv(self) -> SyncSingleRequestBuilder[str]:
         """Specify that the query must retrieve data as a single CSV string."""
         self.headers["Accept"] = "text/csv"
-        return AsyncSingleRequestBuilder[str](
+        return SyncSingleRequestBuilder[str](
             session=self.session,  # type: ignore
             path=self.path,
             http_method=self.http_method,
             headers=self.headers,
             params=self.params,
             json=self.json,
         )
 
 
-class AsyncRequestBuilder(Generic[_ReturnT]):
-    def __init__(self, session: AsyncClient, path: str) -> None:
+class SyncRequestBuilder(Generic[_ReturnT]):
+    def __init__(self, session: SyncClient, path: str) -> None:
         self.session = session
         self.path = path
 
     def select(
         self,
         *columns: str,
         count: Optional[CountMethod] = None,
-    ) -> AsyncSelectRequestBuilder[_ReturnT]:
+    ) -> SyncSelectRequestBuilder[_ReturnT]:
         """Run a SELECT query.
 
         Args:
             *columns: The names of the columns to fetch.
             count: The method to use to get the count of rows returned.
         Returns:
-            :class:`AsyncSelectRequestBuilder`
+            :class:`SyncSelectRequestBuilder`
         """
         method, params, headers, json = pre_select(*columns, count=count)
-        return AsyncSelectRequestBuilder[_ReturnT](
+        return SyncSelectRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
 
     def insert(
         self,
         json: Union[dict, list],
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
         upsert: bool = False,
-    ) -> AsyncQueryRequestBuilder[_ReturnT]:
+        default_to_null: bool = True,
+    ) -> SyncQueryRequestBuilder[_ReturnT]:
         """Run an INSERT query.
 
         Args:
             json: The row to be inserted.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
             upsert: Whether the query should be an upsert.
+            default_to_null: Make missing fields default to `null`.
+                Otherwise, use the default value for the column.
+                Only applies for bulk inserts.
         Returns:
-            :class:`AsyncQueryRequestBuilder`
+            :class:`SyncQueryRequestBuilder`
         """
         method, params, headers, json = pre_insert(
             json,
             count=count,
             returning=returning,
             upsert=upsert,
+            default_to_null=default_to_null,
         )
-        return AsyncQueryRequestBuilder[_ReturnT](
+        return SyncQueryRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
 
     def upsert(
         self,
         json: Union[dict, list],
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
         ignore_duplicates: bool = False,
         on_conflict: str = "",
-    ) -> AsyncQueryRequestBuilder[_ReturnT]:
+        default_to_null: bool = True,
+    ) -> SyncQueryRequestBuilder[_ReturnT]:
         """Run an upsert (INSERT ... ON CONFLICT DO UPDATE) query.
 
         Args:
             json: The row to be inserted.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
             ignore_duplicates: Whether duplicate rows should be ignored.
             on_conflict: Specified columns to be made to work with UNIQUE constraint.
+            default_to_null: Make missing fields default to `null`. Otherwise, use the
+                default value for the column. This only applies when inserting new rows,
+                not when merging with existing rows under `ignoreDuplicates: false`.
+                This also only applies when doing bulk upserts.
         Returns:
-            :class:`AsyncQueryRequestBuilder`
+            :class:`SyncQueryRequestBuilder`
         """
         method, params, headers, json = pre_upsert(
             json,
             count=count,
             returning=returning,
             ignore_duplicates=ignore_duplicates,
             on_conflict=on_conflict,
+            default_to_null=default_to_null,
         )
-        return AsyncQueryRequestBuilder[_ReturnT](
+        return SyncQueryRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
 
     def update(
         self,
         json: dict,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
-    ) -> AsyncFilterRequestBuilder[_ReturnT]:
+    ) -> SyncFilterRequestBuilder[_ReturnT]:
         """Run an UPDATE query.
 
         Args:
             json: The updated fields.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
         Returns:
-            :class:`AsyncFilterRequestBuilder`
+            :class:`SyncFilterRequestBuilder`
         """
         method, params, headers, json = pre_update(
             json,
             count=count,
             returning=returning,
         )
-        return AsyncFilterRequestBuilder[_ReturnT](
+        return SyncFilterRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
 
     def delete(
         self,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
-    ) -> AsyncFilterRequestBuilder[_ReturnT]:
+    ) -> SyncFilterRequestBuilder[_ReturnT]:
         """Run a DELETE query.
 
         Args:
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
         Returns:
-            :class:`AsyncFilterRequestBuilder`
+            :class:`SyncFilterRequestBuilder`
         """
         method, params, headers, json = pre_delete(
             count=count,
             returning=returning,
         )
-        return AsyncFilterRequestBuilder[_ReturnT](
+        return SyncFilterRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
```

### Comparing `postgrest-0.16.2/postgrest/_sync/client.py` & `postgrest-0.16.3/postgrest/_sync/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.2/postgrest/_sync/request_builder.py` & `postgrest-0.16.3/postgrest/_async/request_builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,49 +17,49 @@
     pre_insert,
     pre_select,
     pre_update,
     pre_upsert,
 )
 from ..exceptions import APIError, generate_default_error_message
 from ..types import ReturnMethod
-from ..utils import SyncClient, get_origin_and_cast
+from ..utils import AsyncClient, get_origin_and_cast
 
 _ReturnT = TypeVar("_ReturnT")
 
 
-class SyncQueryRequestBuilder(Generic[_ReturnT]):
+class AsyncQueryRequestBuilder(Generic[_ReturnT]):
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         self.session = session
         self.path = path
         self.http_method = http_method
         self.headers = headers
         self.params = params
         self.json = json
 
-    def execute(self) -> APIResponse[_ReturnT]:
+    async def execute(self) -> APIResponse[_ReturnT]:
         """Execute the query.
 
         .. tip::
             This is the last method called, after the query is built.
 
         Returns:
             :class:`APIResponse`
 
         Raises:
             :class:`APIError` If the API raised an error.
         """
-        r = self.session.request(
+        r = await self.session.request(
             self.http_method,
             self.path,
             json=self.json,
             params=self.params,
             headers=self.headers,
         )
         try:
@@ -78,44 +78,44 @@
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
         except JSONDecodeError as e:
             raise APIError(generate_default_error_message(r))
 
 
-class SyncSingleRequestBuilder(Generic[_ReturnT]):
+class AsyncSingleRequestBuilder(Generic[_ReturnT]):
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         self.session = session
         self.path = path
         self.http_method = http_method
         self.headers = headers
         self.params = params
         self.json = json
 
-    def execute(self) -> SingleAPIResponse[_ReturnT]:
+    async def execute(self) -> SingleAPIResponse[_ReturnT]:
         """Execute the query.
 
         .. tip::
             This is the last method called, after the query is built.
 
         Returns:
             :class:`SingleAPIResponse`
 
         Raises:
             :class:`APIError` If the API raised an error.
         """
-        r = self.session.request(
+        r = await self.session.request(
             self.http_method,
             self.path,
             json=self.json,
             params=self.params,
             headers=self.headers,
         )
         try:
@@ -127,19 +127,19 @@
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
         except JSONDecodeError as e:
             raise APIError(generate_default_error_message(r))
 
 
-class SyncMaybeSingleRequestBuilder(SyncSingleRequestBuilder[_ReturnT]):
-    def execute(self) -> Optional[SingleAPIResponse[_ReturnT]]:
+class AsyncMaybeSingleRequestBuilder(AsyncSingleRequestBuilder[_ReturnT]):
+    async def execute(self) -> Optional[SingleAPIResponse[_ReturnT]]:
         r = None
         try:
-            r = SyncSingleRequestBuilder[_ReturnT].execute(self)
+            r = await AsyncSingleRequestBuilder[_ReturnT].execute(self)
         except APIError as e:
             if e.details and "The result contains 0 rows" in e.details:
                 return None
         if not r:
             raise APIError(
                 {
                     "message": "Missing response",
@@ -148,256 +148,267 @@
                     "details": "Postgrest couldn't retrieve response, please check traceback of the code. Please create an issue in `supabase-community/postgrest-py` if needed.",
                 }
             )
         return r
 
 
 # ignoring type checking as a workaround for https://github.com/python/mypy/issues/9319
-class SyncFilterRequestBuilder(BaseFilterRequestBuilder[_ReturnT], SyncQueryRequestBuilder[_ReturnT]):  # type: ignore
+class AsyncFilterRequestBuilder(BaseFilterRequestBuilder[_ReturnT], AsyncQueryRequestBuilder[_ReturnT]):  # type: ignore
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         get_origin_and_cast(BaseFilterRequestBuilder[_ReturnT]).__init__(
             self, session, headers, params
         )
-        get_origin_and_cast(SyncQueryRequestBuilder[_ReturnT]).__init__(
+        get_origin_and_cast(AsyncQueryRequestBuilder[_ReturnT]).__init__(
             self, session, path, http_method, headers, params, json
         )
 
 
 # this exists for type-safety. see https://gist.github.com/anand2312/93d3abf401335fd3310d9e30112303bf
-class SyncRPCFilterRequestBuilder(
-    BaseRPCRequestBuilder[_ReturnT], SyncSingleRequestBuilder[_ReturnT]
+class AsyncRPCFilterRequestBuilder(
+    BaseRPCRequestBuilder[_ReturnT], AsyncSingleRequestBuilder[_ReturnT]
 ):
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         get_origin_and_cast(BaseFilterRequestBuilder[_ReturnT]).__init__(
             self, session, headers, params
         )
-        get_origin_and_cast(SyncSingleRequestBuilder[_ReturnT]).__init__(
+        get_origin_and_cast(AsyncSingleRequestBuilder[_ReturnT]).__init__(
             self, session, path, http_method, headers, params, json
         )
 
 
 # ignoring type checking as a workaround for https://github.com/python/mypy/issues/9319
-class SyncSelectRequestBuilder(BaseSelectRequestBuilder[_ReturnT], SyncQueryRequestBuilder[_ReturnT]):  # type: ignore
+class AsyncSelectRequestBuilder(BaseSelectRequestBuilder[_ReturnT], AsyncQueryRequestBuilder[_ReturnT]):  # type: ignore
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         get_origin_and_cast(BaseSelectRequestBuilder[_ReturnT]).__init__(
             self, session, headers, params
         )
-        get_origin_and_cast(SyncQueryRequestBuilder[_ReturnT]).__init__(
+        get_origin_and_cast(AsyncQueryRequestBuilder[_ReturnT]).__init__(
             self, session, path, http_method, headers, params, json
         )
 
-    def single(self) -> SyncSingleRequestBuilder[_ReturnT]:
+    def single(self) -> AsyncSingleRequestBuilder[_ReturnT]:
         """Specify that the query will only return a single row in response.
 
         .. caution::
             The API will raise an error if the query returned more than one row.
         """
         self.headers["Accept"] = "application/vnd.pgrst.object+json"
-        return SyncSingleRequestBuilder[_ReturnT](
+        return AsyncSingleRequestBuilder[_ReturnT](
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
-    def maybe_single(self) -> SyncMaybeSingleRequestBuilder[_ReturnT]:
+    def maybe_single(self) -> AsyncMaybeSingleRequestBuilder[_ReturnT]:
         """Retrieves at most one row from the result. Result must be at most one row (e.g. using `eq` on a UNIQUE column), otherwise this will result in an error."""
         self.headers["Accept"] = "application/vnd.pgrst.object+json"
-        return SyncMaybeSingleRequestBuilder[_ReturnT](
+        return AsyncMaybeSingleRequestBuilder[_ReturnT](
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
     def text_search(
         self, column: str, query: str, options: dict[str, Any] = {}
-    ) -> SyncFilterRequestBuilder[_ReturnT]:
+    ) -> AsyncFilterRequestBuilder[_ReturnT]:
         type_ = options.get("type")
         type_part = ""
         if type_ == "plain":
             type_part = "pl"
         elif type_ == "phrase":
             type_part = "ph"
         elif type_ == "web_search":
             type_part = "w"
         config_part = f"({options.get('config')})" if options.get("config") else ""
         self.params = self.params.add(column, f"{type_part}fts{config_part}.{query}")
 
-        return SyncQueryRequestBuilder[_ReturnT](
+        return AsyncQueryRequestBuilder[_ReturnT](
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
-    def csv(self) -> SyncSingleRequestBuilder[str]:
+    def csv(self) -> AsyncSingleRequestBuilder[str]:
         """Specify that the query must retrieve data as a single CSV string."""
         self.headers["Accept"] = "text/csv"
-        return SyncSingleRequestBuilder[str](
+        return AsyncSingleRequestBuilder[str](
             session=self.session,  # type: ignore
             path=self.path,
             http_method=self.http_method,
             headers=self.headers,
             params=self.params,
             json=self.json,
         )
 
 
-class SyncRequestBuilder(Generic[_ReturnT]):
-    def __init__(self, session: SyncClient, path: str) -> None:
+class AsyncRequestBuilder(Generic[_ReturnT]):
+    def __init__(self, session: AsyncClient, path: str) -> None:
         self.session = session
         self.path = path
 
     def select(
         self,
         *columns: str,
         count: Optional[CountMethod] = None,
-    ) -> SyncSelectRequestBuilder[_ReturnT]:
+    ) -> AsyncSelectRequestBuilder[_ReturnT]:
         """Run a SELECT query.
 
         Args:
             *columns: The names of the columns to fetch.
             count: The method to use to get the count of rows returned.
         Returns:
             :class:`AsyncSelectRequestBuilder`
         """
         method, params, headers, json = pre_select(*columns, count=count)
-        return SyncSelectRequestBuilder[_ReturnT](
+        return AsyncSelectRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
 
     def insert(
         self,
         json: Union[dict, list],
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
         upsert: bool = False,
-    ) -> SyncQueryRequestBuilder[_ReturnT]:
+        default_to_null: bool = True,
+    ) -> AsyncQueryRequestBuilder[_ReturnT]:
         """Run an INSERT query.
 
         Args:
             json: The row to be inserted.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
             upsert: Whether the query should be an upsert.
+            default_to_null: Make missing fields default to `null`.
+                Otherwise, use the default value for the column.
+                Only applies for bulk inserts.
         Returns:
             :class:`AsyncQueryRequestBuilder`
         """
         method, params, headers, json = pre_insert(
             json,
             count=count,
             returning=returning,
             upsert=upsert,
+            default_to_null=default_to_null,
         )
-        return SyncQueryRequestBuilder[_ReturnT](
+        return AsyncQueryRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
 
     def upsert(
         self,
         json: Union[dict, list],
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
         ignore_duplicates: bool = False,
         on_conflict: str = "",
-    ) -> SyncQueryRequestBuilder[_ReturnT]:
+        default_to_null: bool = True,
+    ) -> AsyncQueryRequestBuilder[_ReturnT]:
         """Run an upsert (INSERT ... ON CONFLICT DO UPDATE) query.
 
         Args:
             json: The row to be inserted.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
             ignore_duplicates: Whether duplicate rows should be ignored.
             on_conflict: Specified columns to be made to work with UNIQUE constraint.
+            default_to_null: Make missing fields default to `null`. Otherwise, use the
+                default value for the column. This only applies when inserting new rows,
+                not when merging with existing rows under `ignoreDuplicates: false`.
+                This also only applies when doing bulk upserts.
         Returns:
             :class:`AsyncQueryRequestBuilder`
         """
         method, params, headers, json = pre_upsert(
             json,
             count=count,
             returning=returning,
             ignore_duplicates=ignore_duplicates,
             on_conflict=on_conflict,
+            default_to_null=default_to_null,
         )
-        return SyncQueryRequestBuilder[_ReturnT](
+        return AsyncQueryRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
 
     def update(
         self,
         json: dict,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
-    ) -> SyncFilterRequestBuilder[_ReturnT]:
+    ) -> AsyncFilterRequestBuilder[_ReturnT]:
         """Run an UPDATE query.
 
         Args:
             json: The updated fields.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
         Returns:
             :class:`AsyncFilterRequestBuilder`
         """
         method, params, headers, json = pre_update(
             json,
             count=count,
             returning=returning,
         )
-        return SyncFilterRequestBuilder[_ReturnT](
+        return AsyncFilterRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
 
     def delete(
         self,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
-    ) -> SyncFilterRequestBuilder[_ReturnT]:
+    ) -> AsyncFilterRequestBuilder[_ReturnT]:
         """Run a DELETE query.
 
         Args:
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
         Returns:
             :class:`AsyncFilterRequestBuilder`
         """
         method, params, headers, json = pre_delete(
             count=count,
             returning=returning,
         )
-        return SyncFilterRequestBuilder[_ReturnT](
+        return AsyncFilterRequestBuilder[_ReturnT](
             self.session, self.path, method, headers, params, json
         )
```

### Comparing `postgrest-0.16.2/postgrest/base_client.py` & `postgrest-0.16.3/postgrest/base_client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.2/postgrest/base_request_builder.py` & `postgrest-0.16.3/postgrest/base_request_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     # groups the method, json, headers and params for a query in a single object
     method: RequestMethod
     params: QueryParams
     headers: Headers
     json: Dict[Any, Any]
 
 
+def _unique_columns(json: List[Dict]):
+    unique_keys = {key for row in json for key in row.keys()}
+    columns = ",".join([f'"{k}"' for k in unique_keys])
+    return columns
+
+
 def pre_select(
     *columns: str,
     count: Optional[CountMethod] = None,
 ) -> QueryArgs:
     if columns:
         method = RequestMethod.GET
         params = QueryParams({"select": ",".join(columns)})
@@ -57,46 +63,59 @@
         method = RequestMethod.HEAD
         params = QueryParams()
     headers = Headers({"Prefer": f"count={count}"}) if count else Headers()
     return QueryArgs(method, params, headers, {})
 
 
 def pre_insert(
-    json: dict,
+    json: Union[dict, list],
     *,
     count: Optional[CountMethod],
     returning: ReturnMethod,
     upsert: bool,
+    default_to_null: bool = True,
 ) -> QueryArgs:
     prefer_headers = [f"return={returning}"]
     if count:
         prefer_headers.append(f"count={count}")
     if upsert:
         prefer_headers.append("resolution=merge-duplicates")
+    if not default_to_null:
+        prefer_headers.append("missing=default")
     headers = Headers({"Prefer": ",".join(prefer_headers)})
-    return QueryArgs(RequestMethod.POST, QueryParams(), headers, json)
+    # Adding 'columns' query parameters
+    query_params = {}
+    if isinstance(json, list):
+        query_params = {"columns": _unique_columns(json)}
+    return QueryArgs(RequestMethod.POST, QueryParams(query_params), headers, json)
 
 
 def pre_upsert(
-    json: dict,
+    json: Union[dict, list],
     *,
     count: Optional[CountMethod],
     returning: ReturnMethod,
     ignore_duplicates: bool,
     on_conflict: str = "",
+    default_to_null: bool = True,
 ) -> QueryArgs:
     query_params = {}
     prefer_headers = [f"return={returning}"]
     if count:
         prefer_headers.append(f"count={count}")
     resolution = "ignore" if ignore_duplicates else "merge"
     prefer_headers.append(f"resolution={resolution}-duplicates")
+    if not default_to_null:
+        prefer_headers.append("missing=default")
     headers = Headers({"Prefer": ",".join(prefer_headers)})
     if on_conflict:
         query_params["on_conflict"] = on_conflict
+    # Adding 'columns' query parameters
+    if isinstance(json, list):
+        query_params["columns"] = _unique_columns(json)
     return QueryArgs(RequestMethod.POST, QueryParams(query_params), headers, json)
 
 
 def pre_update(
     json: dict,
     *,
     count: Optional[CountMethod],
```

### Comparing `postgrest-0.16.2/postgrest/exceptions.py` & `postgrest-0.16.3/postgrest/exceptions.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.2/postgrest/types.py` & `postgrest-0.16.3/postgrest/types.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.2/postgrest/utils.py` & `postgrest-0.16.3/postgrest/utils.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.2/pyproject.toml` & `postgrest-0.16.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgrest"
-version = "0.16.2"
+version = "0.16.3"
 description = "PostgREST client for Python. This library provides an ORM interface to PostgREST."
 authors = ["Lương Quang Mạnh <luongquangmanh85@gmail.com>", "Joel Lee <joel@joellee.org>", "Anand", "Oliver Rice", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/postgrest-py"
 repository = "https://github.com/supabase-community/postgrest-py"
 documentation = "https://postgrest-py.rtfd.io"
 readme = "README.md"
 license = "MIT"
```

### Comparing `postgrest-0.16.2/PKG-INFO` & `postgrest-0.16.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgrest
-Version: 0.16.2
+Version: 0.16.3
 Summary: PostgREST client for Python. This library provides an ORM interface to PostgREST.
 Home-page: https://github.com/supabase-community/postgrest-py
 License: MIT
 Author: Lương Quang Mạnh
 Author-email: luongquangmanh85@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

