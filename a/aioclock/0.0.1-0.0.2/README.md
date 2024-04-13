# Comparing `tmp/aioclock-0.0.1.tar.gz` & `tmp/aioclock-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioclock-0.0.1.tar", max compression
+gzip compressed data, was "aioclock-0.0.2.tar", max compression
```

## Comparing `aioclock-0.0.1.tar` & `aioclock-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-03-31 12:43:56.933246 aioclock-0.0.1/LICENSE
--rw-r--r--   0        0        0     3674 2024-03-31 12:43:56.933246 aioclock-0.0.1/README.md
--rw-r--r--   0        0        0      299 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/__init__.py
--rw-r--r--   0        0        0     2495 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/app.py
--rw-r--r--   0        0        0     1182 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/group.py
--rw-r--r--   0        0        0       55 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/logger.py
--rw-r--r--   0        0        0      122 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/provider.py
--rw-r--r--   0        0        0      584 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/task.py
--rw-r--r--   0        0        0     5191 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/triggers.py
--rw-r--r--   0        0        0      972 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/types.py
--rw-r--r--   0        0        0      862 2024-03-31 12:43:56.933246 aioclock-0.0.1/aioclock/utils.py
--rw-r--r--   0        0        0     1956 2024-03-31 12:44:20.001277 aioclock-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4656 1970-01-01 00:00:00.000000 aioclock-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-12 16:32:46.825709 aioclock-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3674 2024-04-12 16:32:46.825709 aioclock-0.0.2/README.md
+-rw-r--r--   0        0        0      299 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/__init__.py
+-rw-r--r--   0        0        0     2495 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/app.py
+-rw-r--r--   0        0        0     1182 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/group.py
+-rw-r--r--   0        0        0       55 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/logger.py
+-rw-r--r--   0        0        0      122 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/provider.py
+-rw-r--r--   0        0        0      584 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/task.py
+-rw-r--r--   0        0        0     6408 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/triggers.py
+-rw-r--r--   0        0        0     1042 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/types.py
+-rw-r--r--   0        0        0      862 2024-04-12 16:32:46.825709 aioclock-0.0.2/aioclock/utils.py
+-rw-r--r--   0        0        0     1966 2024-04-12 16:33:09.645740 aioclock-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 aioclock-0.0.2/PKG-INFO
```

### Comparing `aioclock-0.0.1/LICENSE` & `aioclock-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.1/README.md` & `aioclock-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.1/aioclock/app.py` & `aioclock-0.0.2/aioclock/app.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.1/aioclock/group.py` & `aioclock-0.0.2/aioclock/group.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.1/aioclock/task.py` & `aioclock-0.0.2/aioclock/task.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.1/aioclock/triggers.py` & `aioclock-0.0.2/aioclock/triggers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,114 @@
 import asyncio
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from datetime import datetime, timedelta
 from typing import Literal, Union
 
-import pytz
-from pydantic import BaseModel, model_validator
+import zoneinfo
+from pydantic import BaseModel, PositiveInt, model_validator
 
-from aioclock.types import EveryT, HourT, MinuteT, SecondT, Triggers
+from aioclock.types import EveryT, HourT, MinuteT, PositiveNumber, SecondT, Triggers
 
 
 class BaseTrigger(BaseModel, ABC):
     type_: Triggers
 
     @abstractmethod
     async def trigger_next(self) -> None:
         """
         `trigger_next` keep waiting, until the event should be triggered.
         """
 
+    @abstractmethod
     def should_trigger(self) -> bool:
+        """
+        `should_trigger` checks if the event should be triggered or not.
+        """
         return True
 
 
 class Forever(BaseTrigger):
     type_: Literal[Triggers.FOREVER] = Triggers.FOREVER
 
+    def should_trigger(self) -> bool:
+        return True
+
     async def trigger_next(self) -> None:
         return None
 
 
-class Once(BaseTrigger):
+class LoopController(BaseTrigger, ABC):
+    _current_loop_count: int = 0
+    """
+    Current loop count, which is used to keep track of the number of times the event has been triggered.
+    Private attribute, should not be accessed directly.
+    """
+
+    max_loop_count: Union[PositiveInt, None] = None
+    """
+    The maximum number of times the event should be triggered.
+
+    If set to 3, then 4th time the event will not be triggered.
+    If set to None, it will keep running forever.
+    """
+
+    @model_validator(mode="after")
+    def validate_loop_controll(self):
+        if "_current_loop_count" in self.model_fields_set:
+            raise ValueError("_current_loop_count is a private attribute, should not be provided.")
+        return self
+
+    def increment_loop_counter(self) -> None:
+        if self._current_loop_count is not None:
+            self._current_loop_count += 1
+
+    def should_trigger(self) -> bool:
+        if self.max_loop_count is None:
+            return True
+        if self._current_loop_count < self.max_loop_count:
+            return True
+        return False
+
+
+class Once(LoopController):
     type_: Literal[Triggers.ONCE] = Triggers.ONCE
-    already_triggered: bool = False
+    max_loop_count: PositiveInt = 1
 
     async def trigger_next(self) -> None:
-        if self.already_triggered is False:
-            self.already_triggered = True
-            return None
-
-        await asyncio.Event().wait()  # waits for ever
+        self.increment_loop_counter()
+        return None
 
 
-class OnStartUp(Once):
+class OnStartUp(LoopController):
     type_: Literal[Triggers.ON_START_UP] = Triggers.ON_START_UP
+    max_loop_count: PositiveInt = 1
 
     async def trigger_next(self) -> None:
-        if self.already_triggered is False:
-            self.already_triggered = True
-            return None
-
-    def should_trigger(self) -> bool:
-        return not (self.already_triggered)
+        self.increment_loop_counter()
+        return None
 
 
-class OnShutDown(Once):
+class OnShutDown(LoopController):
     type_: Literal[Triggers.ON_SHUT_DOWN] = Triggers.ON_SHUT_DOWN
+    max_loop_count: PositiveInt = 1
 
     async def trigger_next(self) -> None:
-        if self.already_triggered is False:
-            self.already_triggered = True
-            return None
-
-    def should_trigger(self) -> bool:
-        return not (self.already_triggered)
+        self.increment_loop_counter()
+        return None
 
 
-class Every(BaseTrigger):
+class Every(LoopController):
     type_: Literal[Triggers.EVERY] = Triggers.EVERY
 
-    seconds: Union[int, float, None] = None
-    minutes: Union[int, float, None] = None
-    hours: Union[int, float, None] = None
-    days: Union[int, float, None] = None
-    weeks: Union[int, float, None] = None
+    seconds: Union[PositiveNumber, None] = None
+    minutes: Union[PositiveNumber, None] = None
+    hours: Union[PositiveNumber, None] = None
+    days: Union[PositiveNumber, None] = None
+    weeks: Union[PositiveNumber, None] = None
 
     @model_validator(mode="after")
     def validate_time_units(self):
         if (
             self.seconds is None
             and self.minutes is None
             and self.hours is None
@@ -99,38 +130,42 @@
             result += self.hours * 3600
         if self.minutes is not None:
             result += self.minutes * 60
 
         return result
 
     async def trigger_next(self) -> None:
+        self.increment_loop_counter()
+        if self.max_loop_count is not None:
+            self.max_loop_count += 1
         await asyncio.sleep(self.to_seconds)
         return
 
 
 WEEK_TO_SECOND = 604800
 
 
-class At(BaseTrigger):
+class At(LoopController):
     type_: Literal[Triggers.AT] = Triggers.AT
 
     second: SecondT = 0
     minute: MinuteT = 0
     hour: HourT = 0
     at: EveryT = "every day"
     tz: str
+    """Timzeon to use for the event."""
 
     @model_validator(mode="after")
     def validate_time_units(self):
         if self.second is None and self.minute is None and self.hour is None:
             raise ValueError("At least one time unit must be provided.")
 
         if self.tz is not None:
             try:
-                pytz.timezone(self.tz)
+                zoneinfo.ZoneInfo(self.tz)
             except Exception as error:
                 raise ValueError(f"Invalid timezone provided: {error}")
 
         return self
 
     def _shift_to_week(self, target_time: datetime, tz_aware_now: datetime):
         target_weekday: dict[EveryT, Union[int, None]] = {
@@ -155,24 +190,24 @@
 
         if self.at == "every day":
             target_time += timedelta(days=(1 if target_time < tz_aware_now else 0))
             return target_time
 
         # 1 second error
         error_margin = WEEK_TO_SECOND - 1
-        if days_ahead == 7 and target_time.timestamp() - tz_aware_now.timestamp() < (error_margin):
+        if days_ahead == 7 and target_time.timestamp() - tz_aware_now.timestamp() < error_margin:
             # date is today, and event is about to be triggered today. so no need to shift to 7 days.
             return target_time
 
         return target_time + timedelta(days_ahead)
 
     def _get_next_ts(self, now: datetime) -> float:
         target_time = deepcopy(now).replace(
             hour=self.hour, minute=self.minute, second=self.second, microsecond=0
         )
         target_time = self._shift_to_week(target_time, now)
         return (target_time - now).total_seconds()
 
     async def trigger_next(self) -> None:
-        now = datetime.now(pytz.timezone(self.tz))
+        now = datetime.now(tz=zoneinfo.ZoneInfo(self.tz))
         sleep_for = self._get_next_ts(now)
         await asyncio.sleep(sleep_for)
```

### Comparing `aioclock-0.0.1/aioclock/types.py` & `aioclock-0.0.2/aioclock/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import auto
-from typing import Annotated, Literal
+from typing import Annotated, Literal, Union
 
 from annotated_types import Interval
 
 from aioclock.utils import StrEnum
 
 EveryT = Literal[
     "every monday",
@@ -16,14 +16,16 @@
     "every day",
 ]
 
 SecondT = Annotated[int, Interval(ge=0, le=59)]
 MinuteT = Annotated[int, Interval(ge=0, le=59)]
 HourT = Annotated[int, Interval(ge=0, le=24)]
 
+PositiveNumber = Annotated[Union[int, float], Interval(ge=0)]
+
 
 class Triggers(StrEnum):
     # TODO: support cron job trigger
     # CRON = auto()
     # """Cron job trigger."""
     EVERY = auto()
     """Every (x) time units, it gets triggered."""
```

### Comparing `aioclock-0.0.1/aioclock/utils.py` & `aioclock-0.0.2/aioclock/utils.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.1/pyproject.toml` & `aioclock-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "aioclock"
-version = "0.0.1"
+version = "0.0.2"
 description = "An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management"
 authors = ["Mani Mozaffar <fmani.mozaffar@gmail.com>"]
 repository = "https://github.com/ManiMozaffar/aioclock"
 documentation = "https://ManiMozaffar.github.io/aioclock/"
 readme = "README.md"
 packages = [{ include = "aioclock" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pydantic = "^2.6.4"
-pytz = "^2024.1"
 fast-depends = "^2.4.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
+pytest-asyncio = "^0.23.6"
 tox = "^4.11.1"
 rich = "^13.7.1"
 pyright = "1.1.350"
 
 [tool.pyright]
 typeCheckingMode = "basic"
```

### Comparing `aioclock-0.0.1/PKG-INFO` & `aioclock-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: aioclock
-Version: 0.0.1
+Version: 0.0.2
 Summary: An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management
 Home-page: https://github.com/ManiMozaffar/aioclock
 Author: Mani Mozaffar
 Author-email: fmani.mozaffar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fast-depends (>=2.4.2,<3.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
-Requires-Dist: pytz (>=2024.1,<2025.0)
 Project-URL: Documentation, https://ManiMozaffar.github.io/aioclock/
 Project-URL: Repository, https://github.com/ManiMozaffar/aioclock
 Description-Content-Type: text/markdown
 
 # aioclock
 
 [![Release](https://img.shields.io/github/v/release/ManiMozaffar/aioclock)](https://img.shields.io/github/v/release/ManiMozaffar/aioclock)
```

