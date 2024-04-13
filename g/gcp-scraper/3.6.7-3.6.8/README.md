# Comparing `tmp/gcp-scraper-3.6.7.tar.gz` & `tmp/gcp-scraper-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-scraper-3.6.7.tar", last modified: Sat Apr  6 13:57:23 2024, max compression
+gzip compressed data, was "gcp-scraper-3.6.8.tar", last modified: Sat Apr 13 00:18:37 2024, max compression
```

## Comparing `gcp-scraper-3.6.7.tar` & `gcp-scraper-3.6.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.441382 gcp-scraper-3.6.7/
--rw-r--r--   0 cuz        (501) staff       (20)    35149 2023-08-11 13:24:50.000000 gcp-scraper-3.6.7/LICENSE
--rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-06 13:57:23.441110 gcp-scraper-3.6.7/PKG-INFO
--rw-r--r--   0 cuz        (501) staff       (20)       45 2023-08-11 13:24:50.000000 gcp-scraper-3.6.7/README.md
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.440258 gcp-scraper-3.6.7/gcp_scraper.egg-info/
--rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/PKG-INFO
--rw-r--r--   0 cuz        (501) staff       (20)      497 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 cuz        (501) staff       (20)        1 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 cuz        (501) staff       (20)      198 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/requires.txt
--rw-r--r--   0 cuz        (501) staff       (20)        9 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.428288 gcp-scraper-3.6.7/gscraper/
--rwxr-xr-x   0 cuz        (501) staff       (20)      284 2024-04-06 13:56:55.000000 gcp-scraper-3.6.7/gscraper/__init__.py
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.434515 gcp-scraper-3.6.7/gscraper/base/
--rwxr-xr-x   0 cuz        (501) staff       (20)        0 2023-10-27 05:39:56.000000 gcp-scraper-3.6.7/gscraper/base/__init__.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    22802 2024-04-06 13:49:06.000000 gcp-scraper-3.6.7/gscraper/base/abstract.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    38670 2024-03-23 03:20:34.000000 gcp-scraper-3.6.7/gscraper/base/gcloud.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    91060 2024-04-06 13:51:19.000000 gcp-scraper-3.6.7/gscraper/base/session.py
--rwxr-xr-x   0 cuz        (501) staff       (20)   113809 2024-04-06 13:56:10.000000 gcp-scraper-3.6.7/gscraper/base/spider.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    19111 2024-03-23 03:20:19.000000 gcp-scraper-3.6.7/gscraper/base/types.py
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.438537 gcp-scraper-3.6.7/gscraper/utils/
--rwxr-xr-x   0 cuz        (501) staff       (20)      962 2023-12-05 12:25:11.000000 gcp-scraper-3.6.7/gscraper/utils/__init__.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    11448 2024-03-30 10:37:57.000000 gcp-scraper-3.6.7/gscraper/utils/cast.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    16069 2024-02-24 02:47:12.000000 gcp-scraper-3.6.7/gscraper/utils/date.py
--rwxr-xr-x   0 cuz        (501) staff       (20)     8113 2023-11-08 14:08:25.000000 gcp-scraper-3.6.7/gscraper/utils/logs.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    69526 2024-03-23 03:17:26.000000 gcp-scraper-3.6.7/gscraper/utils/map.py
--rw-r--r--   0 cuz        (501) staff       (20)       38 2024-04-06 13:57:23.442271 gcp-scraper-3.6.7/setup.cfg
--rw-r--r--   0 cuz        (501) staff       (20)      764 2023-09-10 13:21:42.000000 gcp-scraper-3.6.7/setup.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:18:37.143367 gcp-scraper-3.6.8/
+-rw-r--r--   0 cuz        (501) staff       (20)    35149 2023-08-11 13:24:50.000000 gcp-scraper-3.6.8/LICENSE
+-rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-13 00:18:37.143256 gcp-scraper-3.6.8/PKG-INFO
+-rw-r--r--   0 cuz        (501) staff       (20)       45 2023-08-11 13:24:50.000000 gcp-scraper-3.6.8/README.md
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:18:37.142821 gcp-scraper-3.6.8/gcp_scraper.egg-info/
+-rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-13 00:18:37.000000 gcp-scraper-3.6.8/gcp_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 cuz        (501) staff       (20)      497 2024-04-13 00:18:37.000000 gcp-scraper-3.6.8/gcp_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 cuz        (501) staff       (20)        1 2024-04-13 00:18:37.000000 gcp-scraper-3.6.8/gcp_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 cuz        (501) staff       (20)      198 2024-04-13 00:18:37.000000 gcp-scraper-3.6.8/gcp_scraper.egg-info/requires.txt
+-rw-r--r--   0 cuz        (501) staff       (20)        9 2024-04-13 00:18:37.000000 gcp-scraper-3.6.8/gcp_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:18:37.134477 gcp-scraper-3.6.8/gscraper/
+-rwxr-xr-x   0 cuz        (501) staff       (20)      284 2024-04-13 00:17:49.000000 gcp-scraper-3.6.8/gscraper/__init__.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:18:37.139208 gcp-scraper-3.6.8/gscraper/base/
+-rwxr-xr-x   0 cuz        (501) staff       (20)        0 2023-10-27 05:39:56.000000 gcp-scraper-3.6.8/gscraper/base/__init__.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    22802 2024-04-06 13:49:06.000000 gcp-scraper-3.6.8/gscraper/base/abstract.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    38670 2024-03-23 03:20:34.000000 gcp-scraper-3.6.8/gscraper/base/gcloud.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    88962 2024-04-13 00:13:03.000000 gcp-scraper-3.6.8/gscraper/base/session.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)   116500 2024-04-13 00:17:32.000000 gcp-scraper-3.6.8/gscraper/base/spider.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    19111 2024-03-23 03:20:19.000000 gcp-scraper-3.6.8/gscraper/base/types.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-13 00:18:37.142065 gcp-scraper-3.6.8/gscraper/utils/
+-rwxr-xr-x   0 cuz        (501) staff       (20)      962 2023-12-05 12:25:11.000000 gcp-scraper-3.6.8/gscraper/utils/__init__.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    11448 2024-03-30 10:37:57.000000 gcp-scraper-3.6.8/gscraper/utils/cast.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    16069 2024-02-24 02:47:12.000000 gcp-scraper-3.6.8/gscraper/utils/date.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)     8113 2023-11-08 14:08:25.000000 gcp-scraper-3.6.8/gscraper/utils/logs.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    69526 2024-03-23 03:17:26.000000 gcp-scraper-3.6.8/gscraper/utils/map.py
+-rw-r--r--   0 cuz        (501) staff       (20)       38 2024-04-13 00:18:37.143694 gcp-scraper-3.6.8/setup.cfg
+-rw-r--r--   0 cuz        (501) staff       (20)      764 2023-09-10 13:21:42.000000 gcp-scraper-3.6.8/setup.py
```

### Comparing `gcp-scraper-3.6.7/LICENSE` & `gcp-scraper-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/PKG-INFO` & `gcp-scraper-3.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-scraper
-Version: 3.6.7
+Version: 3.6.8
 Summary: Scraping utils with GCP functions
 Home-page: https://github.com/minyeamer/gscraper.git
 Author: minyeamer
 Author-email: minyeamer@gmail.com
 License: minyeamer
 Keywords: gcp-scraper,scraper,gcp
 Requires-Python: >=3.7
```

### Comparing `gcp-scraper-3.6.7/gcp_scraper.egg-info/PKG-INFO` & `gcp-scraper-3.6.8/gcp_scraper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-scraper
-Version: 3.6.7
+Version: 3.6.8
 Summary: Scraping utils with GCP functions
 Home-page: https://github.com/minyeamer/gscraper.git
 Author: minyeamer
 Author-email: minyeamer@gmail.com
 License: minyeamer
 Keywords: gcp-scraper,scraper,gcp
 Requires-Python: >=3.7
```

### Comparing `gcp-scraper-3.6.7/gscraper/base/abstract.py` & `gcp-scraper-3.6.8/gscraper/base/abstract.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/gscraper/base/gcloud.py` & `gcp-scraper-3.6.8/gscraper/base/gcloud.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/gscraper/base/session.py` & `gcp-scraper-3.6.8/gscraper/base/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 from gscraper.base.abstract import CustomDict, TypedDict, TypedRecords, OptionalDict, Value, ValueSet, Query
 from gscraper.base.abstract import INVALID_INSTANCE_MSG
 
 from gscraper.base.types import _KT, _VT, _PASS, Context, LogLevel, TypeHint, TypeList
-from gscraper.base.types import IndexLabel, Keyword, Pagination, Pages, Unit, Range, DateFormat, DateQuery, Timedelta, Timezone
+from gscraper.base.types import IndexLabel, Keyword, Pagination, Pages, Unit, DateFormat, DateQuery, Timedelta, Timezone
 from gscraper.base.types import RenameMap, TypeMap, Records, NestedDict, Data, ResponseData, PandasData, PANDAS_DATA
 from gscraper.base.types import ApplyFunction, MatchFunction, RegexFormat
 from gscraper.base.types import get_type, init_origin, is_type, is_bool_type, is_float_type, is_numeric_type
 from gscraper.base.types import is_numeric_or_date_type, is_dict_type, is_records_type, is_dataframe_type, is_tag_type
 from gscraper.base.types import is_array, allin_instance, is_str_array
 
 from gscraper.utils import isna, notna, exists
@@ -25,16 +25,14 @@
 from ast import literal_eval
 from math import ceil
 from itertools import product
 import copy
 import functools
 import logging
 import os
-import random
-import time
 
 from typing import Any, Dict, Callable, Iterable, List, Literal, Optional, Sequence, Tuple, Type, Union
 from bs4 import BeautifulSoup
 from bs4.element import Tag
 import datetime as dt
 import json
 import pandas as pd
@@ -466,28 +464,22 @@
 ###################################################################
 
 class BaseSession(CustomDict):
     __metaclass__ = ABCMeta
     operation = "session"
     tzinfo = TZINFO
     datetimeUnit = "second"
-    numRetries = 0
-    delay = 1.
-    interruptType = tuple()
-    errorType = tuple()
     errors = list()
     info = Info()
 
     def __init__(self, tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
-                debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
-                numRetries: Optional[int]=None, delay: Range=1., **context):
+                debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None, **context):
         self.set_init_time(tzinfo, datetimeUnit)
         self.set_logger(logName, logLevel, logFile, localSave, debug, extraSave, interrupt)
-        self.set_retries(numRetries, delay)
         super().__init__(context)
 
     def set_init_time(self, tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None):
         self.tzinfo = tzinfo if tzinfo else self.tzinfo
         self.datetimeUnit = datetimeUnit if datetimeUnit else self.datetimeUnit
         self.initTime = now(tzinfo=self.tzinfo, droptz=True)
 
@@ -499,19 +491,14 @@
         self.logJson = bool(logFile)
         self.logger = CustomLogger(name=logName, level=self.logLevel, file=self.logFile)
         self.localSave = localSave
         self.debug = cast_list(debug)
         self.extraSave = cast_list(extraSave)
         self.interrupt = cast_list(interrupt)
 
-    def set_retries(self, numRetries: Optional[int]=None, delay: Range=1.):
-        if isinstance(numRetries, int) and numRetries > 0:
-            self.numRetries = numRetries
-        self.delay = delay
-
     def from_locals(self, locals: Dict=dict(), drop: _KT=list(), **context) -> Context:
         drop_keys = cast_list(drop)
         if locals:
             if "context" in drop_keys:
                 locals.pop("context", None)
                 drop_keys.pop(drop_keys.index("context"))
             else: locals = dict(locals, **locals.pop("context", dict()))
@@ -689,66 +676,31 @@
     ###################################################################
     ########################### Log Managers ##########################
     ###################################################################
 
     def catch_exception(func):
         @functools.wraps(func)
         def wrapper(self: BaseSession, *args, **context):
-            for count in reversed(range(self.numRetries+1)):
-                try: return func(self, *args, **context)
-                except Exception as exception:
-                    if self.is_interrupt(exception): raise exception
-                    elif self.is_error(exception) or (count == 0):
-                        return self.pass_exception(exception, func=func, msg={"args":args, "context":context})
-                    else: self.sleep()
-        return wrapper
-
-    def ignore_exception(func):
-        @functools.wraps(func)
-        def wrapper(self: BaseSession, *args, **context):
             try: return func(self, *args, **context)
-            except: return init_origin(func)
+            except Exception as exception:
+                return self.pass_exception(exception, func=func, msg={"args":args, "context":context})
         return wrapper
 
-    def is_interrupt(self, exception: Exception) -> bool:
-        return isinstance(exception, UserInterrupt) or isinstance(exception, self.interruptType)
-
-    def is_error(self, exception: Exception) -> bool:
-        return isinstance(exception, ForbiddenError) or isinstance(exception, self.errorType)
-
     def pass_exception(self, exception: Exception, func: Callable, msg: Dict) -> Any:
         self.log_errors(func=func, msg=msg)
         if ("exception" in self.debug) or ("all" in self.debug):
             self.checkpoint("exception", where=func.__name__, msg=msg)
             raise exception
         return init_origin(func)
 
     def log_errors(self, func: Callable, msg: Dict):
         func_name = f"{func.__name__}({self.__class__.__name__})"
         self.logger.error(log_exception(func_name, json=self.logJson, **msg))
         self.errors.append(msg)
 
-    def sleep(self, delay: Optional[Range]=None):
-        delay = delay if delay is not None else self.get_delay(self.delay)
-        if delay: time.sleep(delay)
-
-    def get_delay(self, delay: Range) -> Union[float,int]:
-        if isinstance(delay, (float,int)): return delay
-        else: return self.get_random_delay(delay)
-
-    def get_random_delay(self, delay: Sequence) -> Union[float,int]:
-        if not (isinstance(delay, Sequence) and delay): return 0.
-        min_ts, max_ts = delay[0], (delay[1] if len(delay) > 1 else None)
-        is_float_ts = isinstance(min_ts, float) or isinstance(max_ts, float)
-        if is_float_ts:
-            min_ts = int(min_ts * 1000)
-            max_ts = int(max_ts * 1000) if isinstance(max_ts, (float,int)) else None
-        delay = random.randrange(min_ts, max_ts)
-        return delay/1000 if is_float_ts else delay
-
     ###################################################################
     ############################ Print Log ############################
     ###################################################################
 
     def print_log(self, log_string: str, func="checkpoint", path: Optional[_KT]=None, drop: Optional[_KT]=None,
                     indent=2, step=2, sep=' '):
         log_object = self._eval_log(log_string, func=func)
@@ -821,15 +773,15 @@
         iterateDate = (DATE_PARAMS if _params else DATE_ITERATOR) * int(bool(self.interval)) * int(_date)
         iterateProduct = self.iterateProduct * int(_product)
         index = [ITER_INDEX] if _index else []
         query = unique(*iterateArgs, *iteratePage, *iterateDate, *iterateProduct, *index)
         if keys_only: return query
         else: return kloc(context, query, if_null=if_null, values_only=values_only)
 
-    @BaseSession.ignore_exception
+    @BaseSession.catch_exception
     def set_iterator(self, *args: Sequence, iterateArgs: List[_KT]=list(), iterateProduct: List[_KT]=list(),
                     iterateUnit: Optional[int]=None, pagination: Pagination=False, interval: Timedelta=str(),
                     indexing=True, **context) -> Tuple[List[Context],Context]:
         arguments, periods, ranges = list(), list(), list()
         args_context = self._check_args(*args, iterateArgs=iterateArgs, pagination=pagination)
         if args_context:
             arguments, context = self._from_args(*args, **args_context, **context)
```

### Comparing `gcp-scraper-3.6.7/gscraper/base/spider.py` & `gcp-scraper-3.6.8/gscraper/base/spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from gscraper.base.session import ITER_INDEX, ITER_SUFFIX, ITER_MSG, PAGE_ITERATOR
 from gscraper.base.gcloud import GoogleQueryReader, GoogleUploader, GoogleQueryList, GoogleUploadList
 from gscraper.base.gcloud import Account, fetch_gcloud_authorization, read_gcloud
 
 from gscraper.base.types import _KT, _PASS, Arguments, Context, LogLevel, TypeHint, EncryptedKey, DecryptedKey
 from gscraper.base.types import IndexLabel, Keyword, Pagination, Status, Unit, Range, DateFormat, Timedelta, Timezone
 from gscraper.base.types import Records, Data, MappedData, JsonData, RedirectData
-from gscraper.base.types import is_datetime_type, is_date_type, is_array, is_int_array, init_origin
+from gscraper.base.types import is_datetime_type, is_date_type, is_array, is_int_array
 
 from gscraper.utils import notna
 from gscraper.utils.cast import cast_list, cast_tuple, cast_int, cast_datetime_format
 from gscraper.utils.date import get_date_pair, get_datetime_pair
 from gscraper.utils.logs import log_encrypt, log_messages, log_response, log_client, log_data
 from gscraper.utils.map import to_array, align_array, transpose_array, unit_array, get_scala, union, inter, diff
 from gscraper.utils.map import kloc, exists_dict, drop_dict, split_dict
@@ -30,14 +30,15 @@
 from requests.cookies import RequestsCookieJar
 from urllib.parse import quote, urlencode, urlparse
 import asyncio
 import aiohttp
 import copy
 import functools
 import inspect
+import random
 import requests
 import time
 
 from typing import Callable, Dict, Iterable, List, Literal, Optional, Sequence, Tuple, Union
 from numbers import Real
 from ast import literal_eval
 from bs4 import BeautifulSoup, Tag
@@ -318,14 +319,18 @@
 
 class RequestSession(UploadSession):
     __metaclass__ = ABCMeta
     asyncio = False
     operation = "session"
     fields = list()
     ranges = list()
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     returnType = None
     mappedReturn = False
     info = Info()
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
@@ -341,15 +346,17 @@
     def set_filter_variables(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None,
                             returnType: Optional[TypeHint]=None):
         self.fields = fields if fields else self.fields
         self.ranges = RangeFilter(*ranges) if isinstance(ranges, Sequence) and ranges else RangeFilter()
         self.returnType = returnType if returnType else self.returnType
 
     def set_request_variables(self, numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None):
-        self.set_retries(numRetries, delay)
+        if isinstance(numRetries, int) and numRetries > 0:
+            self.numRetries = numRetries
+        self.delay = delay
         self.cookies = cookies
 
     ###################################################################
     ######################### Request Managers ########################
     ###################################################################
 
     def init_context(self, args: Arguments, context: Context, self_var=True,
@@ -384,14 +391,54 @@
         def wrapper(self: RequestSession, *args, **context):
             response = func(self, *args, **context)
             self.sleep()
             return response
         return wrapper
 
     ###################################################################
+    ########################### Log Managers ##########################
+    ###################################################################
+
+    def retry_request(func):
+        @functools.wraps(func)
+        def wrapper(self: RequestSession, *args, **context):
+            for count in reversed(range(self.numRetries+1)):
+                try: return func(self, *args, **context)
+                except Exception as exception:
+                    if self.is_interrupt(exception): raise exception
+                    elif self.is_error(exception) or (count == 0):
+                        return self.pass_exception(exception, func=func, msg={"args":args, "context":context})
+                    else: self.sleep()
+        return wrapper
+
+    def is_interrupt(self, exception: Exception) -> bool:
+        return isinstance(exception, UserInterrupt) or isinstance(exception, self.interruptType)
+
+    def is_error(self, exception: Exception) -> bool:
+        return isinstance(exception, ForbiddenError) or isinstance(exception, self.errorType)
+
+    def sleep(self, delay: Optional[Range]=None):
+        delay = delay if delay is not None else self.get_delay(self.delay)
+        if delay: time.sleep(delay)
+
+    def get_delay(self, delay: Range) -> Union[float,int]:
+        if isinstance(delay, (float,int)): return delay
+        else: return self.get_random_delay(delay)
+
+    def get_random_delay(self, delay: Sequence) -> Union[float,int]:
+        if not (isinstance(delay, Sequence) and delay): return 0.
+        min_ts, max_ts = delay[0], (delay[1] if len(delay) > 1 else None)
+        is_float_ts = isinstance(min_ts, float) or isinstance(max_ts, float)
+        if is_float_ts:
+            min_ts = int(min_ts * 1000)
+            max_ts = int(max_ts * 1000) if isinstance(max_ts, (float,int)) else None
+        delay = random.randrange(min_ts, max_ts)
+        return delay/1000 if is_float_ts else delay
+
+    ###################################################################
     ########################## Validate Data ##########################
     ###################################################################
 
     def validate_data(func):
         @functools.wraps(func)
         def wrapper(self: RequestSession, *args, fields: IndexLabel=list(), returnType: Optional[TypeHint]=None, **params):
             data = func(self, *args, fields=fields, returnType=returnType, **params)
@@ -472,15 +519,15 @@
         if reset_index: data = data.reset_index(drop=True)
         return data
 
     ###################################################################
     ############################ With Data ############################
     ###################################################################
 
-    def with_data(self, data: Data, uploadList: Optional[GoogleUploadList]=list(), func=str(), **context):
+    def with_data(self, data: Data, uploadList: GoogleUploadList=list(), func=str(), **context):
         self.checkpoint("crawl", where=func, msg={"data":data}, save=data)
         self.save_result(data)
         self.upload_result(data, uploadList, **context)
 
     @BaseSession.catch_exception
     def save_result(self, data: Data):
         if not self.localSave: return
@@ -537,14 +584,18 @@
     pageFrom = 1
     offsetFrom = 1
     pageUnit = 0
     pageLimit = 0
     interval = str()
     fromNow = None
     ssl = None
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     responseType = "records"
     returnType = "records"
     mappedReturn = False
     root = list()
     groupby = list()
     groupSize = dict()
     countby = str()
@@ -553,15 +604,15 @@
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None,
                 fromNow: Optional[Unit]=None, discard=True, progress=True, where=str(), which=str(), by=str(), message=str(),
-                iterateUnit: Optional[int]=None, interval: Timedelta=None, apiRedirect=False, redirectUnit: Optional[int]=None,
+                iterateUnit: Optional[int]=None, interval: Optional[Timedelta]=None, apiRedirect=False, redirectUnit: Optional[int]=None,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None, **context):
         self.set_filter_variables(fields, ranges, returnType)
         self.set_init_time(tzinfo, datetimeUnit)
         self.set_logger(logName, logLevel, logFile, localSave, debug, extraSave, interrupt)
         self.set_request_variables(numRetries, delay, cookies)
         self.set_spider_variables(fromNow, discard, progress)
         self.set_gather_message(where, which, by, message)
@@ -770,15 +821,15 @@
         return iterator, context
 
     ###################################################################
     ########################## Fetch Request ##########################
     ###################################################################
 
     @abstractmethod
-    @RequestSession.catch_exception
+    @RequestSession.retry_request
     @RequestSession.limit_request
     def fetch(self, *args, **context) -> Data:
         ...
 
     def encode_messages(func):
         @functools.wraps(func)
         def wrapper(self: Spider, method: str, url: str, session: Optional[requests.Session]=None,
@@ -918,15 +969,15 @@
         data = self._redirect_data(iterator, redirectUnit, message=message, progress=progress, fields=fields, **context)
         self.checkpoint("gather", where="redirect", msg={"data":data}, save=data)
         return self.reduce(data, fields=fields, ranges=ranges, returnType=returnType, **context)
 
     def get_redirect_message(self, **context) -> str:
         return REDIRECT_MSG(self.operation)
 
-    @RequestSession.catch_exception
+    @RequestSession.retry_request
     @RequestSession.limit_request
     @gcloud_authorized
     def fetch_redirect(self, iterator: List[Context], redirectUrl: str, authorization: str,
                         account: Account=dict(), cookies=str(), **context) -> Data:
         data = self._get_redirect_data(iterator, redirectUrl, authorization, account, cookies=cookies, **context).encode("utf-8")
         response = self.request_json(POST, redirectUrl, data=data, headers=dict(Authorization=authorization), **context)
         return self._parse_redirect(response, **context)
@@ -975,14 +1026,18 @@
 class AsyncSession(RequestSession):
     __metaclass__ = ABCMeta
     asyncio = True
     operation = "session"
     fields = list()
     ranges = list()
     maxLimit = MAX_ASYNC_TASK_LIMIT
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     returnType = None
     mappedReturn = False
     info = Info()
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
@@ -1044,33 +1099,26 @@
         delay = delay if delay is not None else self.get_delay(self.delay)
         if delay: await asyncio.sleep(delay)
 
     ###################################################################
     ########################## Async Override #########################
     ###################################################################
 
-    def catch_exception(func):
+    def retry_request(func):
         @functools.wraps(func)
         async def wrapper(self: AsyncSession, *args, **context):
             for count in reversed(range(self.numRetries+1)):
                 try: return await func(self, *args, **context)
                 except Exception as exception:
                     if isinstance(exception, self.interruptType): raise exception
                     elif isinstance(exception, self.errorType) or (count == 0):
                         return self.pass_exception(exception, func=func, msg={"args":args, "context":context})
                     else: await self.async_sleep()
         return wrapper
 
-    def ignore_exception(func):
-        @functools.wraps(func)
-        async def wrapper(self: AsyncSession, *args, **context):
-            try: return await func(self, *args, **context)
-            except: return init_origin(func)
-        return wrapper
-
     def validate_data(func):
         @functools.wraps(func)
         async def wrapper(self: AsyncSession, *args, fields: IndexLabel=list(), returnType: Optional[TypeHint]=None, **params):
             data = await func(self, *args, fields=fields, returnType=returnType, **params)
             if self.mappedReturn and isinstance(data, Dict):
                 return self.filter_mapped_data(data, fields=fields, returnType=returnType)
             else: return self.filter_data(data, fields=fields, returnType=returnType)
@@ -1113,14 +1161,18 @@
     pageFrom = 1
     offsetFrom = 1
     pageUnit = 0
     pageLimit = 0
     interval = str()
     fromNow = None
     ssl = None
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     responseType = "records"
     returnType = "records"
     mappedReturn = False
     root = list()
     groupby = list()
     groupSize = dict()
     countby = str()
@@ -1129,15 +1181,15 @@
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None, numTasks=100,
                 fromNow: Optional[Unit]=None, discard=True, progress=True, where=str(), which=str(), by=str(), message=str(),
-                iterateUnit: Optional[int]=None, interval: Timedelta=None, apiRedirect=False, redirectUnit: Optional[int]=None,
+                iterateUnit: Optional[int]=None, interval: Optional[Timedelta]=None, apiRedirect=False, redirectUnit: Optional[int]=None,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None, **context):
         self.set_filter_variables(fields, ranges, returnType)
         self.set_init_time(tzinfo, datetimeUnit)
         self.set_logger(logName, logLevel, logFile, localSave, debug, extraSave, interrupt)
         self.set_async_variables(numRetries, delay, cookies, numTasks)
         self.set_max_limit(apiRedirect)
         self.set_spider_variables(fromNow, discard, progress)
@@ -1216,15 +1268,15 @@
         return data
 
     ###################################################################
     ########################## Async Requests #########################
     ###################################################################
 
     @abstractmethod
-    @AsyncSession.catch_exception
+    @AsyncSession.retry_request
     @AsyncSession.limit_request
     async def fetch(self, *args, **context) -> Data:
         ...
 
     def encode_messages(func):
         @functools.wraps(func)
         async def wrapper(self: AsyncSpider, method: str, url: str, session: Optional[aiohttp.ClientSession]=None,
@@ -1354,15 +1406,15 @@
                         fields: IndexLabel=list(), ranges: RangeFilter=list(), returnType: Optional[TypeHint]=None, **context) -> Data:
         message = self.get_redirect_message(**context)
         iterator, context = self._init_iterator(args, context, self.iterateArgs, self.iterateProduct, self.pagination)
         data = await self._redirect_data(iterator, redirectUnit, message=message, progress=progress, fields=fields, **context)
         self.checkpoint("gather", where="redirect", msg={"data":data}, save=data)
         return self.reduce(data, fields=fields, ranges=ranges, returnType=returnType, **context)
 
-    @AsyncSession.catch_exception
+    @AsyncSession.retry_request
     @AsyncSession.limit_request
     @gcloud_authorized
     async def fetch_redirect(self, iterator: List[Context], redirectUrl: str, authorization: str,
                             account: Account=dict(), cookies=str(), **context) -> Records:
         data = self._get_redirect_data(iterator, redirectUrl, authorization, account, cookies=cookies, **context).encode("utf-8")
         response = await self.request_json(POST, url=redirectUrl, data=data, headers=dict(Authorization=authorization), **context)
         return self._parse_redirect(response, **context)
@@ -1523,14 +1575,18 @@
 class EncryptedSession(RequestSession):
     __metaclass__ = ABCMeta
     asyncio = False
     operation = "session"
     where = WHERE
     fields = list()
     ranges = list()
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     returnType = None
     mappedReturn = False
     auth = LoginSpider
     authKey = list()
     decryptedKey = dict()
     sessionCookies = True
     info = Info()
@@ -1672,14 +1728,18 @@
     pageFrom = 1
     offsetFrom = 1
     pageUnit = 0
     pageLimit = 0
     interval = str()
     fromNow = None
     ssl = None
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     responseType = "records"
     returnType = "records"
     mappedReturn = False
     root = list()
     groupby = list()
     groupSize = dict()
     countby = str()
@@ -1691,15 +1751,15 @@
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None,
                 fromNow: Optional[Unit]=None, discard=True, progress=True, where=str(), which=str(), by=str(), message=str(),
-                iterateUnit: Optional[int]=None, interval: Timedelta=None, apiRedirect=False, redirectUnit: Optional[int]=None,
+                iterateUnit: Optional[int]=None, interval: Optional[Timedelta]=None, apiRedirect=False, redirectUnit: Optional[int]=None,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None,
                 encryptedKey: Optional[EncryptedKey]=None, decryptedKey: Optional[DecryptedKey]=None, **context):
         Spider.__init__(self, **self.from_locals(locals(), drop=ENCRYPTED_UNIQUE))
         self.set_secret(encryptedKey, decryptedKey)
 
     def is_interrupt(self, exception: Exception) -> bool:
         return isinstance(exception, ENCRYPTED_SPIDER_INTERRUPT) or isinstance(exception, self.interruptType)
@@ -1712,14 +1772,18 @@
 class EncryptedAsyncSession(AsyncSession, EncryptedSession):
     __metaclass__ = ABCMeta
     asyncio = True
     operation = "session"
     fields = list()
     ranges = list()
     maxLimit = MAX_ASYNC_TASK_LIMIT
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     returnType = None
     mappedReturn = False
     auth = LoginSpider
     decryptedKey = dict()
     sessionCookies = True
     info = Info()
 
@@ -1823,14 +1887,18 @@
     pageFrom = 1
     offsetFrom = 1
     pageUnit = 0
     pageLimit = 0
     interval = str()
     fromNow = None
     ssl = None
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     responseType = "records"
     returnType = "records"
     mappedReturn = False
     root = list()
     groupby = list()
     groupSize = dict()
     countby = str()
@@ -1842,15 +1910,15 @@
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None, numTasks=100,
                 fromNow: Optional[Unit]=None, discard=True, progress=True, where=str(), which=str(), by=str(), message=str(),
-                iterateUnit: Optional[int]=None, interval: Timedelta=None, apiRedirect=False, redirectUnit: Optional[int]=None,
+                iterateUnit: Optional[int]=None, interval: Optional[Timedelta]=None, apiRedirect=False, redirectUnit: Optional[int]=None,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None,
                 encryptedKey: Optional[EncryptedKey]=None, decryptedKey: Optional[DecryptedKey]=None, **context):
         AsyncSpider.__init__(self, **self.from_locals(locals(), drop=ENCRYPTED_UNIQUE))
         self.set_secret(encryptedKey, decryptedKey)
 
     def is_interrupt(self, exception: Exception) -> bool:
         return isinstance(exception, ENCRYPTED_SPIDER_INTERRUPT) or isinstance(exception, self.interruptType)
@@ -1934,14 +2002,18 @@
 class Pipeline(EncryptedSession):
     __metaclass__ = ABCMeta
     asyncio = False
     operation = "pipeline"
     fields = list()
     derivFields = list()
     ranges = list()
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     returnType = "dataframe"
     mappedReturn = False
     info = PipelineInfo()
     dags = Dag()
 
     @abstractmethod
     @EncryptedSession.init_task
@@ -2049,14 +2121,18 @@
 
 class AsyncPipeline(EncryptedAsyncSession, Pipeline):
     __metaclass__ = ABCMeta
     operation = "pipeline"
     fields = list()
     derivFields = list()
     ranges = list()
+    numRetries = 0
+    delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     returnType = "dataframe"
     mappedReturn = False
     info = PipelineInfo()
     dags = Dag()
 
     @abstractmethod
     @EncryptedAsyncSession.init_task
```

### Comparing `gcp-scraper-3.6.7/gscraper/base/types.py` & `gcp-scraper-3.6.8/gscraper/base/types.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/gscraper/utils/__init__.py` & `gcp-scraper-3.6.8/gscraper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/gscraper/utils/cast.py` & `gcp-scraper-3.6.8/gscraper/utils/cast.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/gscraper/utils/date.py` & `gcp-scraper-3.6.8/gscraper/utils/date.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/gscraper/utils/logs.py` & `gcp-scraper-3.6.8/gscraper/utils/logs.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/gscraper/utils/map.py` & `gcp-scraper-3.6.8/gscraper/utils/map.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.7/setup.py` & `gcp-scraper-3.6.8/setup.py`

 * *Files identical despite different names*

