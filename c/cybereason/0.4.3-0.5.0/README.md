# Comparing `tmp/cybereason-0.4.3.tar.gz` & `tmp/cybereason-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybereason-0.4.3.tar", last modified: Sat Mar  9 11:16:52 2024, max compression
+gzip compressed data, was "cybereason-0.5.0.tar", last modified: Sat Apr 13 10:46:23 2024, max compression
```

## Comparing `cybereason-0.4.3.tar` & `cybereason-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-03-09 11:16:52.439560 cybereason-0.4.3/
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1481 2023-07-28 13:38:20.000000 cybereason-0.4.3/LICENSE
--rw-rw-r--   0 nuno      (1000) nuno      (1000)     2895 2024-03-09 11:16:52.439560 cybereason-0.4.3/PKG-INFO
--rw-rw-r--   0 nuno      (1000) nuno      (1000)     1329 2024-03-09 11:12:55.000000 cybereason-0.4.3/pyproject.toml
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1668 2024-03-09 11:16:52.439560 cybereason-0.4.3/setup.cfg
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)       60 2023-07-28 13:38:20.000000 cybereason-0.4.3/setup.py
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-03-09 11:16:52.435560 cybereason-0.4.3/src/
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-03-09 11:16:52.435560 cybereason-0.4.3/src/cybereason/
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)      177 2024-03-09 11:14:53.000000 cybereason-0.4.3/src/cybereason/__init__.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1852 2024-03-08 18:54:10.000000 cybereason-0.4.3/src/cybereason/_typing.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)    15673 2024-03-08 18:52:54.000000 cybereason-0.4.3/src/cybereason/client.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4634 2024-03-08 13:40:36.000000 cybereason-0.4.3/src/cybereason/exceptions.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     3531 2023-11-26 16:25:11.000000 cybereason-0.4.3/src/cybereason/incident_response.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     6535 2024-03-09 03:05:31.000000 cybereason-0.4.3/src/cybereason/malops.py
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-03-09 11:16:52.439560 cybereason-0.4.3/src/cybereason/parse/
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)      147 2023-07-28 13:38:20.000000 cybereason-0.4.3/src/cybereason/parse/__init__.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2472 2023-07-28 13:38:20.000000 cybereason-0.4.3/src/cybereason/parse/cef.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2846 2023-07-28 13:38:20.000000 cybereason-0.4.3/src/cybereason/parse/server.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)        0 2023-07-28 13:38:20.000000 cybereason-0.4.3/src/cybereason/py.typed
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     5175 2023-07-28 13:38:20.000000 cybereason-0.4.3/src/cybereason/rules.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)    16835 2024-03-08 18:51:40.000000 cybereason-0.4.3/src/cybereason/sensors.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4503 2024-03-08 13:45:02.000000 cybereason-0.4.3/src/cybereason/system.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     7678 2024-03-08 13:36:46.000000 cybereason-0.4.3/src/cybereason/threat_intel.py
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-03-09 11:16:52.439560 cybereason-0.4.3/src/cybereason/utils/
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4515 2023-07-28 13:38:20.000000 cybereason-0.4.3/src/cybereason/utils/__init__.py
--rwxrwxrwx   0 nuno      (1000) nuno      (1000)      796 2023-07-28 13:38:20.000000 cybereason-0.4.3/src/cybereason/utils/guid.py
-drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-03-09 11:16:52.439560 cybereason-0.4.3/src/cybereason.egg-info/
--rw-rw-r--   0 nuno      (1000) nuno      (1000)     2895 2024-03-09 11:16:52.000000 cybereason-0.4.3/src/cybereason.egg-info/PKG-INFO
--rw-rw-r--   0 nuno      (1000) nuno      (1000)      719 2024-03-09 11:16:52.000000 cybereason-0.4.3/src/cybereason.egg-info/SOURCES.txt
--rw-rw-r--   0 nuno      (1000) nuno      (1000)        1 2024-03-09 11:16:52.000000 cybereason-0.4.3/src/cybereason.egg-info/dependency_links.txt
--rw-rw-r--   0 nuno      (1000) nuno      (1000)        1 2023-11-26 15:59:18.000000 cybereason-0.4.3/src/cybereason.egg-info/not-zip-safe
--rw-rw-r--   0 nuno      (1000) nuno      (1000)      229 2024-03-09 11:16:52.000000 cybereason-0.4.3/src/cybereason.egg-info/requires.txt
--rw-rw-r--   0 nuno      (1000) nuno      (1000)       11 2024-03-09 11:16:52.000000 cybereason-0.4.3/src/cybereason.egg-info/top_level.txt
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 10:46:23.334408 cybereason-0.5.0/
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1481 2023-07-28 13:38:20.000000 cybereason-0.5.0/LICENSE
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)     2935 2024-04-13 10:46:23.334408 cybereason-0.5.0/PKG-INFO
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)     1329 2024-03-09 11:12:55.000000 cybereason-0.5.0/pyproject.toml
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     1668 2024-04-13 10:46:23.334408 cybereason-0.5.0/setup.cfg
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)       60 2023-07-28 13:38:20.000000 cybereason-0.5.0/setup.py
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 10:46:23.330408 cybereason-0.5.0/src/
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 10:46:23.334408 cybereason-0.5.0/src/cybereason/
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)      177 2024-04-13 10:39:43.000000 cybereason-0.5.0/src/cybereason/__init__.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2019 2024-04-13 10:35:59.000000 cybereason-0.5.0/src/cybereason/_typing.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)    16290 2024-04-13 10:36:21.000000 cybereason-0.5.0/src/cybereason/client.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4620 2024-03-14 15:31:06.000000 cybereason-0.5.0/src/cybereason/exceptions.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     3531 2023-11-26 16:25:11.000000 cybereason-0.5.0/src/cybereason/incident_response.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     6528 2024-03-14 15:18:27.000000 cybereason-0.5.0/src/cybereason/malops.py
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 10:46:23.334408 cybereason-0.5.0/src/cybereason/parse/
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)      147 2023-07-28 13:38:20.000000 cybereason-0.5.0/src/cybereason/parse/__init__.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2472 2023-07-28 13:38:20.000000 cybereason-0.5.0/src/cybereason/parse/cef.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     2846 2023-07-28 13:38:20.000000 cybereason-0.5.0/src/cybereason/parse/server.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)        0 2023-07-28 13:38:20.000000 cybereason-0.5.0/src/cybereason/py.typed
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     5175 2023-07-28 13:38:20.000000 cybereason-0.5.0/src/cybereason/rules.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)    16945 2024-03-14 15:31:28.000000 cybereason-0.5.0/src/cybereason/sensors.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4774 2024-03-30 02:49:47.000000 cybereason-0.5.0/src/cybereason/system.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     7678 2024-03-08 13:36:46.000000 cybereason-0.5.0/src/cybereason/threat_intel.py
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 10:46:23.334408 cybereason-0.5.0/src/cybereason/utils/
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)     4515 2023-07-28 13:38:20.000000 cybereason-0.5.0/src/cybereason/utils/__init__.py
+-rwxrwxrwx   0 nuno      (1000) nuno      (1000)      796 2023-07-28 13:38:20.000000 cybereason-0.5.0/src/cybereason/utils/guid.py
+drwxrwxr-x   0 nuno      (1000) nuno      (1000)        0 2024-04-13 10:46:23.334408 cybereason-0.5.0/src/cybereason.egg-info/
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)     2935 2024-04-13 10:46:23.000000 cybereason-0.5.0/src/cybereason.egg-info/PKG-INFO
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)      719 2024-04-13 10:46:23.000000 cybereason-0.5.0/src/cybereason.egg-info/SOURCES.txt
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)        1 2024-04-13 10:46:23.000000 cybereason-0.5.0/src/cybereason.egg-info/dependency_links.txt
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)        1 2023-11-26 15:59:18.000000 cybereason-0.5.0/src/cybereason.egg-info/not-zip-safe
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)      229 2024-04-13 10:46:23.000000 cybereason-0.5.0/src/cybereason.egg-info/requires.txt
+-rw-rw-r--   0 nuno      (1000) nuno      (1000)       11 2024-04-13 10:46:23.000000 cybereason-0.5.0/src/cybereason.egg-info/top_level.txt
```

### Comparing `cybereason-0.4.3/LICENSE` & `cybereason-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/PKG-INFO` & `cybereason-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.4.3
+Version: 0.5.0
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
@@ -33,15 +33,15 @@
 Provides-Extra: zip
 License-File: LICENSE
 
 # Cybereason
 
 > Async Cybereason API client  
 >
-> ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cybereason)
+> [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cybereason)](https://pypi.org/project/cybereason/)
 
 
 
 ## Installation
 
 <a href="https://pypi.org/project/cybereason/"><pre>
 pip install cybereason
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.4.3 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.5.0 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
@@ -11,16 +11,17 @@
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Security Classifier: Typing :: Typed Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
 Extra: socks Provides-Extra: zip License-File: LICENSE # Cybereason > Async
-Cybereason API client > > ![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/cybereason) ## Installation
+Cybereason API client > > [![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/cybereason)](https://pypi.org/project/cybereason/) ##
+Installation
 _p_i_p_ _i_n_s_t_a_l_l_ _c_y_b_e_r_e_a_s_o_n
 Install _cybereason_ using: - `pip install cybereason[zip]` to enable on-the-
 fly extraction of files downloaded from sensors, - `pip install cybereason
 [socks]` to enable SOCKS proxy support, or - `pip install cybereason
 [zip,socks]` to enable both features. ## Examples ### Save metadata and config
 for every policy ```python from cybereason import Cybereason import asyncio
 import json async def dump_policies_config(): '''Save metadata and config for
```

### Comparing `cybereason-0.4.3/pyproject.toml` & `cybereason-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/setup.cfg` & `cybereason-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/src/cybereason/_typing.py` & `cybereason-0.5.0/src/cybereason/_typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,27 +14,32 @@
 unset = Unset()
 
 
 if TYPE_CHECKING:
     from typing import Any, AsyncIterator, Dict, Literal, NewType, Optional, Protocol, Union, Tuple, TypeVar
     from pathlib import Path
     from os import PathLike
-    from httpx import AsyncClient, URL
+    from httpx import AsyncClient, URL, Timeout
 
     T = TypeVar('T')
     Unforced = Union[Unset, T]
     Query = Optional[Dict[str, Any]]
     UrlPath = Union[URL, str]
 
     MalopId = NewType('MalopId', str)
     SensorId = NewType('SensorId', str)
 
     class CybereasonProtocol(Protocol):
+        tenant:       str
+        username:     str
+        password:     str
         proxy:        Optional[str]
         totp_code:    Optional[str]
+        timeout:      Union[float, Timeout]
+        new_password: Optional[str]
 
         @property
         def session(self) -> AsyncClient: ...
 
         def check_resp(self, resp: Dict[str, Any]) -> Any: ...
         async def get(self, path: UrlPath, query: Query=None, raw: bool=False) -> Any: ...
         async def post(self, path: UrlPath, data: Any, files: Query=None, raw_data: bool=False) -> Any: ...
```

### Comparing `cybereason-0.4.3/src/cybereason/client.py` & `cybereason-0.5.0/src/cybereason/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,27 +42,29 @@
     MalopsMixin,
     SensorsMixin,
     SystemMixin,
     ThreatIntelligenceMixin,
 ):
     def __init__(
         self,
-        tenant:    str,
-        username:  str,
-        password:  str,
-        proxy:     'Optional[str]' = None,
-        totp_code: 'Optional[str]' = None,
-        timeout:   'Union[float, Timeout]' = DEFAULT_TIMEOUT,
+        tenant:       str,
+        username:     str,
+        password:     str,
+        proxy:        'Optional[str]' = None,
+        totp_code:    'Optional[str]' = None,
+        timeout:      'Union[float, Timeout]' = DEFAULT_TIMEOUT,
+        new_password: 'Optional[str]' = None,
     ):
-        self.tenant = tenant.split('.')[0]
-        self.username = username
-        self.password = password
-        self.proxy = proxy
-        self.totp_code = totp_code
-        self.timeout = timeout
+        self.tenant       = tenant.split('.')[0]
+        self.username     = username
+        self.password     = password
+        self.proxy        = proxy
+        self.totp_code    = totp_code
+        self.timeout      = timeout
+        self.new_password = new_password
 
     @cached_property
     def session(self) -> AsyncClient:
         from . import __version__
 
         base_url = f'https://{self.tenant}.cybereason.net'
         headers  = {
@@ -119,16 +121,26 @@
         except ConnectError as e:
             raise ConnectionError(e) from None
 
         if 'error' in str(resp.url):
             await self.session.aclose()
             raise AuthenticationError('Invalid credentials')
         elif 'reset' in str(resp.url):
-            await self.session.aclose()
-            raise AuthenticationError('Expired password')
+            if not self.new_password:
+                await self.session.aclose()
+                raise AuthenticationError('Expired password')
+            else:
+                log.warning('Renewing expired password.')
+                data = {
+                    'oldPassword':        self.password,
+                    'newPassword':        self.new_password,
+                    'confirmNewPassword': self.new_password,
+                    'submit':             'Login',
+                }
+                await self.session.post('?originalurl=/current?', data=data, **options)
 
         if 'Two factor authentication' in resp.text:
             if not self.totp_code:
                 await self.session.aclose()
                 raise AuthenticationError('TOTP code (2FA) is required')
 
             totp = {'totpCode': self.totp_code, 'submit': 'Login'}
```

### Comparing `cybereason-0.4.3/src/cybereason/exceptions.py` & `cybereason-0.5.0/src/cybereason/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     ...
 
 
 class ResourceExistsError(CybereasonException):
     ...
 
 
-class FilterSyntaxError(CybereasonException, SyntaxError):
+class FilterSError(ClientError, ValueError):
     ...
 
 
 class AccessDenied(CybereasonException):
     ...
```

### Comparing `cybereason-0.4.3/src/cybereason/incident_response.py` & `cybereason-0.5.0/src/cybereason/incident_response.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/src/cybereason/malops.py` & `cybereason-0.5.0/src/cybereason/malops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, date, timezone
-from typing import TYPE_CHECKING, cast
+from typing import TYPE_CHECKING
 import logging
 
 from .exceptions import authz, min_version
 from .utils import parse_query_response
 from ._typing import CybereasonProtocol
 
 if TYPE_CHECKING:
@@ -28,15 +28,15 @@
         end = datetime.combine(end, datetime.max.time())
 
     if start.tzinfo is None:
         start = start.replace(tzinfo=timezone.utc)
     if end.tzinfo is None:
         end = end.replace(tzinfo=timezone.utc)
 
-    return  int(start.timestamp() * 1000), int(end.timestamp() * 1000)
+    return int(start.timestamp() * 1000), int(end.timestamp() * 1000)
 
 
 class MalopsMixin(CybereasonProtocol):
     async def get_malops(
         self,
         start: 'Union[datetime, date]',
         end:   'Union[datetime, date, None]' = None,
@@ -47,16 +47,16 @@
         data = {'startTime': _start, 'endTime': _end}
         return (await self.post('detection/inbox', data))['malops']
 
     async def get_malops_v2(
         self,
         start:   'Union[datetime, date]',
         end:     'Union[datetime, date, None]' = None,
-        search:  'Optional[dict[str, Any]]' = None,
-        filter_: 'Optional[dict[str, Any]]' = None,
+        search:  'Optional[Dict[str, Any]]' = None,
+        filter_: 'Optional[Dict[str, Any]]' = None,
     ) -> 'AsyncIterator[Dict[str, Any]]':
         _start, _end = _datetime_range(start, end)
         data = {
             'search':     search or {},
             'filter':     filter_ or {},
             'range':      {'from': _start, 'to': _end},
             'pagination': {'pageSize': 100, 'offset': 0},
```

### Comparing `cybereason-0.4.3/src/cybereason/parse/cef.py` & `cybereason-0.5.0/src/cybereason/parse/cef.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/src/cybereason/parse/server.py` & `cybereason-0.5.0/src/cybereason/parse/server.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/src/cybereason/rules.py` & `cybereason-0.5.0/src/cybereason/rules.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/src/cybereason/sensors.py` & `cybereason-0.5.0/src/cybereason/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING, cast
 from pathlib import Path
 import logging
 import asyncio
 
 from .utils import to_list, get_filename
 from .exceptions import (
-    AccessDenied, ServerError, ClientError,
+    AccessDenied, ServerError, ClientError, FilterSError,
     ResourceExistsError, ResourceNotFoundError,
     authz, min_version,
 )
 from ._typing import CybereasonProtocol, unset
 
 if TYPE_CHECKING:
     from typing import Any, AsyncIterator, Dict, List, Optional, Union
@@ -37,16 +37,19 @@
         if not archived:
             data['filters'].append({
                 'fieldName': 'status',
                 'operator':  'NotEquals',
                 'values':    ['Archived'],
             })
 
-        async for sensor in self.aiter_pages('sensors/query', data, 'sensors'):
-            yield sensor
+        try:
+            async for sensor in self.aiter_pages('sensors/query', data, 'sensors'):
+                yield sensor
+        except KeyError:
+            raise FilterSError(filters) from None
 
     @authz('System Admin')
     async def get_sensors_actions(self) -> 'Any':
         '''Returns a list of all the current or queued actions on sensors.
         '''
         return await self.get('sensors/allActions')
```

### Comparing `cybereason-0.4.3/src/cybereason/system.py` & `cybereason-0.5.0/src/cybereason/system.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,24 @@
         '''
         Args:
             username: If not specified, returns the client's logged user.
         '''
         username = username or 'current'
         return await self.get(f'users/{username}')
 
+    # TODO: check
+    async def update_password(self, new_password) -> str:
+        data = [self.password, new_password]
+        resp = await self.put('/users/reset', data)
+
+        if resp == 'incorrectPassword':
+            raise ValueError(resp)
+
+        return resp
+
     async def get_registration_servers(self):
         return await self.get('settings/get-registration-servers')
 
     async def get_detection_servers(self):
         return await self.get('settings/get-detection-servers')
 
     async def get_registration_config(self):
```

### Comparing `cybereason-0.4.3/src/cybereason/threat_intel.py` & `cybereason-0.5.0/src/cybereason/threat_intel.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/src/cybereason/utils/__init__.py` & `cybereason-0.5.0/src/cybereason/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/src/cybereason/utils/guid.py` & `cybereason-0.5.0/src/cybereason/utils/guid.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.4.3/src/cybereason.egg-info/PKG-INFO` & `cybereason-0.5.0/src/cybereason.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.4.3
+Version: 0.5.0
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
@@ -33,15 +33,15 @@
 Provides-Extra: zip
 License-File: LICENSE
 
 # Cybereason
 
 > Async Cybereason API client  
 >
-> ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cybereason)
+> [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cybereason)](https://pypi.org/project/cybereason/)
 
 
 
 ## Installation
 
 <a href="https://pypi.org/project/cybereason/"><pre>
 pip install cybereason
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.4.3 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.5.0 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
@@ -11,16 +11,17 @@
 Programming Language :: Python Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Security Classifier: Typing :: Typed Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
 Extra: socks Provides-Extra: zip License-File: LICENSE # Cybereason > Async
-Cybereason API client > > ![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/cybereason) ## Installation
+Cybereason API client > > [![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/cybereason)](https://pypi.org/project/cybereason/) ##
+Installation
 _p_i_p_ _i_n_s_t_a_l_l_ _c_y_b_e_r_e_a_s_o_n
 Install _cybereason_ using: - `pip install cybereason[zip]` to enable on-the-
 fly extraction of files downloaded from sensors, - `pip install cybereason
 [socks]` to enable SOCKS proxy support, or - `pip install cybereason
 [zip,socks]` to enable both features. ## Examples ### Save metadata and config
 for every policy ```python from cybereason import Cybereason import asyncio
 import json async def dump_policies_config(): '''Save metadata and config for
```

### Comparing `cybereason-0.4.3/src/cybereason.egg-info/SOURCES.txt` & `cybereason-0.5.0/src/cybereason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

