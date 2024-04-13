# Comparing `tmp/aioautomower-2024.4.0.tar.gz` & `tmp/aioautomower-2024.4.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2024.4.0.tar", last modified: Wed Apr  3 17:20:57 2024, max compression
+gzip compressed data, was "aioautomower-2024.4.1b0.tar", last modified: Sat Apr 13 18:55:05 2024, max compression
```

## Comparing `aioautomower-2024.4.0.tar` & `aioautomower-2024.4.1b0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/aioautomower/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/aioautomower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/aioautomower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:20:56.000000 aioautomower-2024.4.0/aioautomower.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 17:20:57.000000 aioautomower-2024.4.0/aioautomower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 17:20:53.000000 aioautomower-2024.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:20:57.028718 aioautomower-2024.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/tests/test_error_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/tests/test_high_feature_mower_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/tests/test_jwt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-03 17:20:48.000000 aioautomower-2024.4.0/tests/test_low_feature_mower_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:55:05.639852 aioautomower-2024.4.1b0/aioautomower/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/aioautomower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-13 18:55:03.000000 aioautomower-2024.4.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/tests/test_error_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/tests/test_high_feature_mower_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/tests/test_jwt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/tests/test_low_feature_mower_model.py
```

### Comparing `aioautomower-2024.4.0/PKG-INFO` & `aioautomower-2024.4.1b0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2024.4.0
+Version: 2024.4.1b0
 Summary: MPython module to talk to Husqvarna Automower.
 Author-email: Thomas Protzner <thomas.protzner@gmail.com>
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/Thomas55555/aioautomower
 Project-URL: Repository, https://github.com/Thomas55555/aioautomower
 Project-URL: Issues, https://github.com/Thomas55555/aioautomower/issues
 Platform: any
```

### Comparing `aioautomower-2024.4.0/README.md` & `aioautomower-2024.4.1b0/README.md`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.0/aioautomower/auth.py` & `aioautomower-2024.4.1b0/aioautomower/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     async def _async_get_access_token(self) -> str:
         """Request a new access token."""
         try:
             return await self.async_get_access_token()
         except ClientError as err:
             raise AuthException(f"Access token failure: {err}") from err
 
-    async def headers(self) -> dict:
+    async def headers(self) -> dict[str, str]:
         """Generate headers for ReST requests."""
         access_token = await self._async_get_access_token()
         if not self._client_id:
             token_structured = structure_token(access_token)
             self._client_id = token_structured.client_id
         return {
             "Authorization": f"Bearer {access_token}",
```

### Comparing `aioautomower-2024.4.0/aioautomower/const.py` & `aioautomower-2024.4.1b0/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.0/aioautomower/example.py` & `aioautomower-2024.4.1b0/aioautomower/example.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.0/aioautomower/exceptions.py` & `aioautomower-2024.4.1b0/aioautomower/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.0/aioautomower/model.py` & `aioautomower-2024.4.1b0/aioautomower/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 from re import sub
 
 from mashumaro import DataClassDictMixin, field_options
 
 from .const import ERRORCODES
 
 
-def snake_case(string) -> str:
+def snake_case(string: str | None) -> str:
     """Convert an error text to snake case"""
+    if string is None:
+        raise TypeError
     return "_".join(
         sub(
             "([A-Z][a-z][,]+)",
             r" \1",
             sub(
                 "([A-Z]+)",
                 r" \1",
@@ -30,28 +32,28 @@
 
 @dataclass
 class User(DataClassDictMixin):
     """The user details of the JWT."""
 
     first_name: str
     last_name: str
-    custom_attributes: dict
+    custom_attributes: dict[str, str]
     customer_id: str
 
 
 @dataclass
 class JWT(DataClassDictMixin):
     """The content of the JWT."""
 
     # pylint: disable=too-many-instance-attributes
     jti: str
     iss: str
-    roles: list
-    groups: list
-    scopes: list
+    roles: list[str]
+    groups: list[str]
+    scopes: list[str]
     scope: str
     client_id: str
     customer_id: str
     user: User
     iat: int
     exp: int
     sub: str
@@ -263,15 +265,15 @@
 class StayOutZones(DataClassDictMixin):
     """DataClass for StayOutZone values."""
 
     dirty: bool
     zones: dict[str, Zone] = field(
         metadata=field_options(
             deserialize=lambda zone_list: {
-                area.id: Zone(name=area.name or None, enabled=area.enabled)
+                area.id: Zone(name=area.name, enabled=area.enabled)
                 for area in map(_Zones.from_dict, zone_list)
             },
         ),
     )
 
 
 @dataclass
@@ -308,15 +310,15 @@
     headlight: Headlight
     cutting_height: int | None = field(
         metadata=field_options(alias="cuttingHeight"), default=None
     )
     stay_out_zones: StayOutZones | None = field(
         metadata=field_options(alias="stayOutZones"), default=None
     )
-    work_areas: dict[str, WorkArea] | None = field(
+    work_areas: dict[int, WorkArea] | None = field(
         metadata=field_options(
             deserialize=lambda workarea_list: {
                 area.work_area_id: WorkArea(
                     name=area.name or None, cutting_height=area.cutting_height
                 )
                 for area in map(_WorkAreas.from_dict, workarea_list)
             },
```

### Comparing `aioautomower-2024.4.0/aioautomower/session.py` & `aioautomower-2024.4.1b0/aioautomower/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,18 @@
 
     settings = "mowers/{mower_id}/settings"
     "Update the settings on the mower."
 
     stay_out_zones = "mowers/{mower_id}/stayOutZones/{stay_out_id}"
     "Enable or disable the stay-out zone."
 
-    work_area_calendar = "mowers/{mower_id}/workAreas{work_area_id}/calendar"
+    work_area_cutting_height = "mowers/{mower_id}/workAreas/{work_area_id}"
+    "This will update cutting height on the work area."
+
+    work_area_calendar = "mowers/{mower_id}/workAreas/{work_area_id}/calendar"
     "Update the calendar for a work area on the mower."
 
 
 class AutomowerSession:
     """Automower API to communicate with an Automower.
 
     The `AutomowerSession` is the primary API service for this library. It supports
@@ -54,48 +57,48 @@
         poll: bool = False,
     ) -> None:
         """Create a session.
 
         :param class auth: The AbstractAuth class from aioautomower.auth.
         :param bool poll: Poll data with rest if True.
         """
-        self._data: dict = {}
+        self._data: dict[str, str] = {}
         self.auth = auth
         self.data_update_cbs: list = []
         self.data: dict[str, MowerAttributes] = {}
         self.loop = asyncio.get_running_loop()
         self.poll = poll
-        self.rest_task = None
+        self.rest_task: asyncio.Task | None = None
         self.token = None
         self.token_task = None
         self.token_update_cbs: list = []
 
     def register_data_callback(self, callback):
         """Register a data update callback."""
         if callback not in self.data_update_cbs:
             self.data_update_cbs.append(callback)
 
     def _schedule_data_callback(self, cb):
         if self.poll and self.data is None:
             raise NoDataAvailableException
         self.loop.call_soon_threadsafe(cb, self.data)
 
-    def _schedule_data_callbacks(self):
+    def _schedule_data_callbacks(self) -> None:
         for cb in self.data_update_cbs:
             self._schedule_data_callback(cb)
 
     def unregister_data_callback(self, callback):
         """Unregister a data update callback.
 
         :param func callback: Takes one function, which should be unregistered.
         """
         if callback in self.data_update_cbs:
             self.data_update_cbs.remove(callback)
 
-    async def connect(self):
+    async def connect(self) -> None:
         """Connect to the API.
 
         This method handles the login and starts a task that keep the access
         token constantly fresh. Also a REST task will be started, which
         periodically polls the REST endpoint. This method works only, if the
         token is created with the Authorization Code Grant. Call this method
         before any other methods.
@@ -203,24 +206,40 @@
                 "attributes": {"duration": duration_in_min},
             }
         }
         url = AutomowerEndpoint.actions.format(mower_id=mower_id)
         await self.auth.post_json(url, json=body)
 
     async def set_cutting_height(self, mower_id: str, cutting_height: int):
-        """Start the mower for a period of minutes."""
+        """Set the cutting height for the mower."""
         body = {
             "data": {
                 "type": "settings",
                 "attributes": {"cuttingHeight": cutting_height},
             }
         }
         url = AutomowerEndpoint.settings.format(mower_id=mower_id)
         await self.auth.post_json(url, json=body)
 
+    async def set_cutting_height_workarea(
+        self, mower_id: str, cutting_height: int, work_area_id: int
+    ):
+        """Set the cutting height for a specific work area."""
+        body = {
+            "data": {
+                "type": "workArea",
+                "id": work_area_id,
+                "attributes": {"cuttingHeight": cutting_height},
+            }
+        }
+        url = AutomowerEndpoint.work_area_cutting_height.format(
+            mower_id=mower_id, work_area_id=work_area_id
+        )
+        await self.auth.patch_json(url, json=body)
+
     async def set_headlight_mode(
         self,
         mower_id: str,
         headlight_mode: Literal[
             HeadlightModes.ALWAYS_OFF,
             HeadlightModes.ALWAYS_ON,
             HeadlightModes.EVENING_AND_NIGHT,
@@ -236,15 +255,15 @@
         }
         url = AutomowerEndpoint.settings.format(mower_id=mower_id)
         await self.auth.post_json(url, json=body)
 
     async def set_calendar(
         self,
         mower_id: str,
-        task_list: list,
+        task_list: list[str],
     ):
         """Send calendar task to the mower."""
         body = {
             "data": {
                 "type": "calendar",
                 "attributes": {"tasks": task_list},
             }
@@ -288,21 +307,21 @@
                                     attrib
                                 ]
                         except KeyError:
                             datum["attributes"][attrib] = new_data["attributes"][attrib]
         self.data = mower_list_to_dictionary_dataclass(self._data)
         self._schedule_data_callbacks()
 
-    async def _rest_task(self):
+    async def _rest_task(self) -> None:
         """Poll data periodically via Rest."""
         while True:
             await self.get_status()
             self._schedule_data_callbacks()
             await asyncio.sleep(REST_POLL_CYCLE)
 
-    async def close(self):
+    async def close(self) -> None:
         """Close the session."""
         if self.rest_task:
             if not self.rest_task.cancelled():
                 self.rest_task.cancel()
             with contextlib.suppress(asyncio.CancelledError):
                 await asyncio.gather(self.rest_task)
```

### Comparing `aioautomower-2024.4.0/aioautomower/utils.py` & `aioautomower-2024.4.1b0/aioautomower/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Utils for Husqvarna Automower."""
 
 import logging
 import time
 from urllib.parse import quote_plus, urlencode
+from typing import cast, Mapping, Any
 import datetime
 import zoneinfo
 import aiohttp
 import jwt
 from .const import AUTH_API_REVOKE_URL, AUTH_API_TOKEN_URL, AUTH_HEADERS
 from .exceptions import ApiException
 from .model import JWT, MowerAttributes, MowerList, snake_case
 from .const import ERRORCODES
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def structure_token(access_token) -> JWT:
+def structure_token(access_token: str) -> JWT:
     """Decode JWT and convert to dataclass."""
     token_decoded = jwt.decode(access_token, options={"verify_signature": False})
     return JWT.from_dict(token_decoded)
 
 
-async def async_get_access_token(client_id, client_secret) -> dict:
+async def async_get_access_token(client_id: str, client_secret: str) -> dict[str, str]:
     """Get an access token from the Authentication API with client credentials.
 
     This grant type is intended only for you. If you want other
     users to use your application, then they should login using Authorization
     Code Grant.
     """
     auth_data = urlencode(
@@ -48,20 +49,20 @@
             result["expires_at"] = result["expires_in"] + time.time()
         if resp.status >= 400:
             raise ApiException(
                 f"""The token is invalid, response from
                     Husqvarna Automower API: {result}"""
             )
     result["status"] = resp.status
-    return result
+    return cast(dict[str, str], result)
 
 
 async def async_invalidate_access_token(
-    valid_access_token, access_token_to_invalidate
-) -> dict:
+    valid_access_token: str, access_token_to_invalidate: str
+) -> dict[str, str]:
     """Invalidate the token.
 
     :param str valid_access_token: A working access token to authorize this request.
     :param str access_token_to_delete: An access token to invalidate,
     can be th same like the first argument.
     """
     headers = {
@@ -76,19 +77,19 @@
         ) as resp,
     ):
         result = await resp.json(encoding="UTF-8")
         _LOGGER.debug("Resp.status delete token: %s", resp.status)
         if resp.status >= 400:
             resp.raise_for_status()
             _LOGGER.error("Response body delete token: %s", result)
-    return result
+    return cast(dict[str, str], result)
 
 
 def mower_list_to_dictionary_dataclass(
-    mower_list,
+    mower_list: Mapping[Any, Any],
 ) -> dict[str, MowerAttributes]:
     """Convert mower data to a dictionary DataClass."""
     mowers_list = MowerList.from_dict(mower_list)
     mowers_dict = {}
     for mower in mowers_list.data:
         mowers_dict[mower.id] = mower.attributes
     return mowers_dict
@@ -107,17 +108,18 @@
     codes = {}
     for error_text in ERRORCODES.values():
         codes[snake_case(error_text)] = error_text
     return codes
 
 
 def convert_timestamp_to_datetime_utc(
-    timestamp: int, time_zone: zoneinfo.ZoneInfo
+    timestamp: int | None, time_zone: zoneinfo.ZoneInfo
 ) -> datetime.datetime | None:
     """Create datetime object in the requested timezone."""
-
+    if timestamp is None:
+        raise TypeError
     if timestamp != 0:
-        local_datetime_unshifted = datetime.datetime.fromtimestamp(
+        local_unshifted = datetime.datetime.fromtimestamp(
             timestamp / 1000, tz=time_zone
         )
-        return local_datetime_unshifted - local_datetime_unshifted.utcoffset()
+        return local_unshifted - local_unshifted.utcoffset()  # type: ignore
     return None
```

### Comparing `aioautomower-2024.4.0/aioautomower.egg-info/PKG-INFO` & `aioautomower-2024.4.1b0/aioautomower.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2024.4.0
+Version: 2024.4.1b0
 Summary: MPython module to talk to Husqvarna Automower.
 Author-email: Thomas Protzner <thomas.protzner@gmail.com>
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/Thomas55555/aioautomower
 Project-URL: Repository, https://github.com/Thomas55555/aioautomower
 Project-URL: Issues, https://github.com/Thomas55555/aioautomower/issues
 Platform: any
```

### Comparing `aioautomower-2024.4.0/aioautomower.egg-info/SOURCES.txt` & `aioautomower-2024.4.1b0/aioautomower.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 aioautomower/__init__.py
 aioautomower/auth.py
 aioautomower/const.py
 aioautomower/example.py
 aioautomower/exceptions.py
 aioautomower/model.py
+aioautomower/py.typed
 aioautomower/session.py
 aioautomower/utils.py
 aioautomower.egg-info/PKG-INFO
 aioautomower.egg-info/SOURCES.txt
 aioautomower.egg-info/dependency_links.txt
 aioautomower.egg-info/not-zip-safe
 aioautomower.egg-info/requires.txt
```

### Comparing `aioautomower-2024.4.0/pyproject.toml` & `aioautomower-2024.4.1b0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=62.3",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioautomower"
-version = "2024.4.0"
+version = "2024.4.1b"
 description = "MPython module to talk to Husqvarna Automower."
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "Thomas Protzner", email = "thomas.protzner@gmail.com" },
 ]
 classifiers = [
@@ -47,20 +47,20 @@
 PyJWT = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
 mypy = "1.9.0"
 pre-commit = "3.7.0"
-pre-commit-hooks = "4.5.0"
+pre-commit-hooks = "4.6.0"
 pylint = "3.1.0"
 pytest = "8.1.1"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
-ruff = "0.3.5"
+ruff = "0.3.6"
 safety = "3.1.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
 freezegun = "^1.4.0"
 
 [tool.poetry.group.dev.dependencies.coverage]
@@ -123,29 +123,14 @@
 ]
 
 [tool.mypy]
 platform = "linux"
 python_version = "3.11"
 follow_imports = "normal"
 ignore_missing_imports = true
-check_untyped_defs = true
-disallow_any_generics = true
-disallow_incomplete_defs = true
-disallow_subclassing_any = true
-disallow_untyped_calls = true
-disallow_untyped_decorators = true
-disallow_untyped_defs = true
-no_implicit_optional = true
-strict_optional = true
-warn_incomplete_stub = true
-warn_no_return = true
-warn_redundant_casts = true
-warn_return_any = true
-warn_unused_configs = true
-warn_unused_ignores = true
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 30
 
 [tool.coverage.run]
 plugins = [
```

### Comparing `aioautomower-2024.4.0/tests/test_error_text.py` & `aioautomower-2024.4.1b0/tests/test_error_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Tests for asynchronous Python client for aioautomower."""
 
 import json
 
 
+from syrupy.assertion import SnapshotAssertion
 from aioautomower.utils import (
     mower_list_to_dictionary_dataclass,
     error_key_list,
     error_key_dict,
 )
 from tests import load_fixture
 
-
 MOWER_ID = "c7233734-b219-4287-a173-08e3643f89f0"
 
 
 async def test_error_key() -> None:
     """Test translating an error code to an error key."""
     mower_fixture = load_fixture("high_feature_mower.json")
     mower_python = json.loads(mower_fixture)
@@ -37,15 +37,15 @@
     mowers = mower_list_to_dictionary_dataclass(mower_python)
     assert (
         mowers[MOWER_ID].mower.error_key
         == "slipped_mower_has_slipped_situation_not_solved_with_moving_pattern"
     )
 
 
-async def test_error_keys_snapshot(snapshot) -> None:
+async def test_error_keys_snapshot(snapshot: SnapshotAssertion) -> None:
     """Make a snapshot of the error keys."""
     assert error_key_list() == snapshot
 
 
-async def test_error_key_dict_snapshot(snapshot) -> None:
+async def test_error_key_dict_snapshot(snapshot: SnapshotAssertion) -> None:
     """Make a snapshot of the error key dictionary."""
     assert error_key_dict() == snapshot
```

### Comparing `aioautomower-2024.4.0/tests/test_high_feature_mower_model.py` & `aioautomower-2024.4.1b0/tests/test_high_feature_mower_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """Tests for asynchronous Python client for aioautomower."""
 
 import json
 from dataclasses import fields
+from typing import cast
 from syrupy.assertion import SnapshotAssertion
 from freezegun import freeze_time
 from aioautomower.utils import mower_list_to_dictionary_dataclass
+from aioautomower.model import WorkArea
 from tests import load_fixture
 
+
 MOWER_ID = "c7233734-b219-4287-a173-08e3643f89f0"
 
 
 async def test_high_feature_mower() -> None:
     """Test converting a high feature mower."""
     mower_fixture = load_fixture("high_feature_mower.json")
     mower_python = json.loads(mower_fixture)
     mowers = mower_list_to_dictionary_dataclass(mower_python)
     assert mowers[MOWER_ID].battery.battery_percent == 100
-    assert mowers[MOWER_ID].stay_out_zones.dirty is False
-    print(mowers[MOWER_ID].stay_out_zones)
-    assert mowers[MOWER_ID].stay_out_zones.zones is not None
+    assert mowers[MOWER_ID].stay_out_zones.dirty is False  # type: ignore
+    assert mowers[MOWER_ID].stay_out_zones.zones is not None  # type: ignore
     assert (
-        mowers[MOWER_ID]
+        mowers[MOWER_ID]  # type: ignore
         .stay_out_zones.zones["81C6EEA2-D139-4FEA-B134-F22A6B3EA403"]
         .name
         == "Springflowers"
     )
     assert (
-        mowers[MOWER_ID]
+        mowers[MOWER_ID]  # type: ignore
         .stay_out_zones.zones["81C6EEA2-D139-4FEA-B134-F22A6B3EA403"]
         .enabled
         is True
     )
     assert mowers[MOWER_ID].work_areas is not None
-    assert mowers[MOWER_ID].work_areas[123456].name == "Front lawn"
-    assert mowers[MOWER_ID].work_areas[123456].cutting_height == 50
+    workarea = cast(dict[int, WorkArea], mowers[MOWER_ID].work_areas)
+    assert workarea[123456] is not None
+    assert workarea[123456].name == "Front lawn"
+    assert workarea[123456].cutting_height == 50
     assert mowers[MOWER_ID].statistics.cutting_blade_usage_time == 1234
-    assert len(mowers[MOWER_ID].positions) != 0
+    assert len(mowers[MOWER_ID].positions) != 0  # type: ignore
 
 
 @freeze_time(tz_offset=2)
 def test_mower_snapshot(snapshot: SnapshotAssertion):
     """Testing a snapshot of a high feature mower."""
     # pylint: disable=duplicate-code
     mower_fixture = load_fixture("high_feature_mower.json")
```

### Comparing `aioautomower-2024.4.0/tests/test_jwt_model.py` & `aioautomower-2024.4.1b0/tests/test_jwt_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests for asynchronous Python client for aioautomower."""
 
 from dataclasses import fields
 import json
-
+from syrupy.assertion import SnapshotAssertion
 from aioautomower.utils import structure_token
 from tests import load_fixture
 
 MOWER_ID = "c7233734-b219-4287-a173-08e3643f89f0"
 
 
 async def test_decode_token() -> None:
@@ -16,15 +16,15 @@
     token_structered = structure_token(token_python["data"])
     assert token_structered.scope == "iam:read amc:api"
     assert token_structered.client_id == "433e5fdf-5129-452c-xxxx-fadce3213042"
     assert token_structered.user.first_name == "Erika"
     assert token_structered.user.last_name == "Mustermann"
 
 
-async def test_jwt_snapshot(snapshot):
+async def test_jwt_snapshot(snapshot: SnapshotAssertion):
     """Testing a snapshot of a JWT."""
     token_fixture = load_fixture("jwt.json")
     token_python = json.loads(token_fixture)
     token_structered = structure_token(token_python["data"])
     for field in fields(token_structered):
         field_name = field.name
         field_value = getattr(token_structered, field_name)
```

### Comparing `aioautomower-2024.4.0/tests/test_low_feature_mower_model.py` & `aioautomower-2024.4.1b0/tests/test_low_feature_mower_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Tests for asynchronous Python client for aioautomower."""
 
 import json
 from dataclasses import fields
 from freezegun import freeze_time
 
+from syrupy.assertion import SnapshotAssertion
 from aioautomower.utils import mower_list_to_dictionary_dataclass
 from tests import load_fixture
 
 
 MOWER_ID = "c7233734-b219-4287-a173-08e3643f89f0"
 
 
 async def test_low_feature_mower() -> None:
     """Test converting a low feature mower."""
     mower_fixture = load_fixture("low_feature_mower.json")
     mower_python = json.loads(mower_fixture)
     mowers = mower_list_to_dictionary_dataclass(mower_python)
     assert mowers[MOWER_ID].headlight.mode is None
     assert mowers[MOWER_ID].cutting_height is None
-    assert len(mowers[MOWER_ID].positions) == 0
+    assert len(mowers[MOWER_ID].positions) == 0  # type: ignore
 
 
 @freeze_time(tz_offset=2)
-def test_mower_snapshot(snapshot):
+def test_mower_snapshot(snapshot: SnapshotAssertion) -> None:
     """Testing a snapshot of a high feature mower."""
     mower_fixture = load_fixture("low_feature_mower.json")
     mower_python = json.loads(mower_fixture)
     mowers = mower_list_to_dictionary_dataclass(mower_python)
     for field in fields(mowers[MOWER_ID]):
         field_name = field.name
         field_value = getattr(mowers[MOWER_ID], field_name)
```

