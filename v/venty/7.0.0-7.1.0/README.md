# Comparing `tmp/venty-7.0.0.tar.gz` & `tmp/venty-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venty-7.0.0.tar", last modified: Fri Apr 12 13:48:48 2024, max compression
+gzip compressed data, was "venty-7.1.0.tar", last modified: Sat Apr 13 20:58:53 2024, max compression
```

## Comparing `venty-7.0.0.tar` & `venty-7.1.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:48:48.164651 venty-7.0.0/
--rw-rw-rw-   0        0        0    11558 2022-08-05 14:38:16.000000 venty-7.0.0/LICENSE
--rw-rw-rw-   0        0        0      167 2024-03-15 16:24:05.000000 venty-7.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2189 2024-04-12 13:48:48.164651 venty-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2024-04-08 17:56:19.000000 venty-7.0.0/README.md
--rw-rw-rw-   0        0        0       47 2024-03-26 20:12:48.000000 venty-7.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 13:48:48.164651 venty-7.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2017 2024-04-12 13:09:25.000000 venty-7.0.0/setup.py
--rw-rw-rw-   0        0        0      159 2024-03-16 16:56:05.000000 venty-7.0.0/test_requirements.txt
--rw-rw-rw-   0        0        0      665 2024-03-27 06:50:13.000000 venty-7.0.0/tox.ini
-drwxrwxrwx   0        0        0        0 2024-04-12 13:48:48.149651 venty-7.0.0/venty/
--rw-rw-rw-   0        0        0      257 2024-03-16 01:45:41.000000 venty-7.0.0/venty/__init__.py
--rw-rw-rw-   0        0        0      245 2024-03-15 20:16:30.000000 venty-7.0.0/venty/_dummy.py
--rw-rw-rw-   0        0        0     1858 2024-04-08 17:52:38.000000 venty-7.0.0/venty/aggregate_root.py
--rw-rw-rw-   0        0        0     1304 2024-04-05 08:47:53.000000 venty-7.0.0/venty/aggregate_store.py
--rw-rw-rw-   0        0        0     2123 2024-03-27 06:14:06.000000 venty-7.0.0/venty/aggregate_store_test.py
--rw-rw-rw-   0        0        0      999 2024-04-12 13:16:52.000000 venty-7.0.0/venty/auth_event_producer.py
--rw-rw-rw-   0        0        0      756 2024-04-12 13:43:22.000000 venty-7.0.0/venty/classification.py
--rw-rw-rw-   0        0        0     1277 2024-04-12 13:34:09.000000 venty-7.0.0/venty/classification_test.py
--rw-rw-rw-   0        0        0     1315 2024-03-16 17:12:53.000000 venty-7.0.0/venty/event_channel.py
--rw-rw-rw-   0        0        0      521 2024-03-16 16:58:05.000000 venty-7.0.0/venty/event_channel_test.py
--rw-rw-rw-   0        0        0     5036 2024-03-27 06:20:52.000000 venty-7.0.0/venty/event_logger.py
--rw-rw-rw-   0        0        0     3521 2024-04-12 13:16:52.000000 venty-7.0.0/venty/event_producer.py
--rw-rw-rw-   0        0        0     1773 2024-04-12 13:36:23.000000 venty-7.0.0/venty/event_producer_stack.py
--rw-rw-rw-   0        0        0     1584 2024-04-12 13:07:59.000000 venty-7.0.0/venty/event_producer_stack_test.py
--rw-rw-rw-   0        0        0     1537 2024-04-12 13:08:41.000000 venty-7.0.0/venty/event_producer_test.py
--rw-rw-rw-   0        0        0     6996 2024-03-16 15:40:44.000000 venty-7.0.0/venty/event_store.py
--rw-rw-rw-   0        0        0     1327 2024-03-16 17:12:15.000000 venty-7.0.0/venty/http_event_channel.py
--rw-rw-rw-   0        0        0     1850 2024-03-16 17:18:33.000000 venty-7.0.0/venty/http_event_channel_test.py
--rw-rw-rw-   0        0        0      604 2024-03-16 17:00:49.000000 venty-7.0.0/venty/in_memory_event_channel.py
--rw-rw-rw-   0        0        0      338 2024-03-16 17:01:54.000000 venty-7.0.0/venty/in_memory_event_channel_test.py
--rw-rw-rw-   0        0        0     4492 2024-03-16 17:02:22.000000 venty-7.0.0/venty/in_memory_event_store.py
--rw-rw-rw-   0        0        0     6706 2024-03-16 00:47:54.000000 venty-7.0.0/venty/in_memory_event_store_test.py
--rw-rw-rw-   0        0        0      781 2024-04-08 17:48:30.000000 venty-7.0.0/venty/object_storage.py
--rw-rw-rw-   0        0        0      301 2024-04-08 18:03:19.000000 venty-7.0.0/venty/optional.py
--rw-rw-rw-   0        0        0        0 2023-01-06 20:34:35.000000 venty-7.0.0/venty/py.typed
--rw-rw-rw-   0        0        0      294 2024-04-05 09:27:44.000000 venty-7.0.0/venty/settings.py
--rw-rw-rw-   0        0        0      589 2024-03-16 16:02:34.000000 venty-7.0.0/venty/settings_test.py
--rw-rw-rw-   0        0        0     8270 2024-04-12 13:45:12.000000 venty-7.0.0/venty/sql_event_store.py
--rw-rw-rw-   0        0        0     6821 2024-03-16 22:24:29.000000 venty-7.0.0/venty/sql_event_store_test.py
--rw-rw-rw-   0        0        0      399 2024-04-12 13:16:52.000000 venty-7.0.0/venty/strong_types.py
--rw-rw-rw-   0        0        0     1003 2024-03-15 19:20:28.000000 venty-7.0.0/venty/strong_types_test.py
--rw-rw-rw-   0        0        0      958 2024-03-16 16:40:05.000000 venty-7.0.0/venty/timing.py
--rw-rw-rw-   0        0        0      961 2024-03-15 18:40:30.000000 venty-7.0.0/venty/timing_test.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:48:48.163649 venty-7.0.0/venty.egg-info/
--rw-rw-rw-   0        0        0     2189 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 13:48:47.000000 venty-7.0.0/venty.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 20:58:53.252396 venty-7.1.0/
+-rw-rw-rw-   0        0        0    11558 2022-08-05 14:38:16.000000 venty-7.1.0/LICENSE
+-rw-rw-rw-   0        0        0      167 2024-03-15 16:24:05.000000 venty-7.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2189 2024-04-13 20:58:53.251354 venty-7.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2024-04-08 17:56:19.000000 venty-7.1.0/README.md
+-rw-rw-rw-   0        0        0       47 2024-03-26 20:12:48.000000 venty-7.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 20:58:53.252396 venty-7.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2017 2024-04-12 14:26:40.000000 venty-7.1.0/setup.py
+-rw-rw-rw-   0        0        0      159 2024-03-16 16:56:05.000000 venty-7.1.0/test_requirements.txt
+-rw-rw-rw-   0        0        0      665 2024-03-27 06:50:13.000000 venty-7.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-04-13 20:58:53.238346 venty-7.1.0/venty/
+-rw-rw-rw-   0        0        0      257 2024-03-16 01:45:41.000000 venty-7.1.0/venty/__init__.py
+-rw-rw-rw-   0        0        0      245 2024-03-15 20:16:30.000000 venty-7.1.0/venty/_dummy.py
+-rw-rw-rw-   0        0        0      439 2024-04-12 14:47:07.000000 venty-7.1.0/venty/aggregate_channel.py
+-rw-rw-rw-   0        0        0     1858 2024-04-08 17:52:38.000000 venty-7.1.0/venty/aggregate_root.py
+-rw-rw-rw-   0        0        0     1390 2024-04-13 12:03:00.000000 venty-7.1.0/venty/aggregate_store.py
+-rw-rw-rw-   0        0        0     2084 2024-04-12 14:22:50.000000 venty-7.1.0/venty/aggregate_store_test.py
+-rw-rw-rw-   0        0        0      999 2024-04-12 13:16:52.000000 venty-7.1.0/venty/auth_event_producer.py
+-rw-rw-rw-   0        0        0      886 2024-04-13 10:07:54.000000 venty-7.1.0/venty/classification.py
+-rw-rw-rw-   0        0        0     1478 2024-04-13 10:08:57.000000 venty-7.1.0/venty/classification_test.py
+-rw-rw-rw-   0        0        0     1234 2024-04-12 14:26:00.000000 venty-7.1.0/venty/cloudevent.py
+-rw-rw-rw-   0        0        0     1315 2024-03-16 17:12:53.000000 venty-7.1.0/venty/event_channel.py
+-rw-rw-rw-   0        0        0      517 2024-04-12 14:22:40.000000 venty-7.1.0/venty/event_channel_test.py
+-rw-rw-rw-   0        0        0     5032 2024-04-12 14:22:40.000000 venty-7.1.0/venty/event_logger.py
+-rw-rw-rw-   0        0        0     3521 2024-04-12 13:16:52.000000 venty-7.1.0/venty/event_producer.py
+-rw-rw-rw-   0        0        0     1724 2024-04-12 14:23:14.000000 venty-7.1.0/venty/event_producer_stack.py
+-rw-rw-rw-   0        0        0     1580 2024-04-12 14:22:40.000000 venty-7.1.0/venty/event_producer_stack_test.py
+-rw-rw-rw-   0        0        0     1533 2024-04-12 14:22:40.000000 venty-7.1.0/venty/event_producer_test.py
+-rw-rw-rw-   0        0        0     7087 2024-04-13 09:34:29.000000 venty-7.1.0/venty/event_store.py
+-rw-rw-rw-   0        0        0      713 2024-04-13 09:35:17.000000 venty-7.1.0/venty/event_stream_channel.py
+-rw-rw-rw-   0        0        0     1327 2024-03-16 17:12:15.000000 venty-7.1.0/venty/http_event_channel.py
+-rw-rw-rw-   0        0        0     1846 2024-04-12 14:22:40.000000 venty-7.1.0/venty/http_event_channel_test.py
+-rw-rw-rw-   0        0        0      604 2024-03-16 17:00:49.000000 venty-7.1.0/venty/in_memory_event_channel.py
+-rw-rw-rw-   0        0        0      338 2024-03-16 17:01:54.000000 venty-7.1.0/venty/in_memory_event_channel_test.py
+-rw-rw-rw-   0        0        0     4492 2024-03-16 17:02:22.000000 venty-7.1.0/venty/in_memory_event_store.py
+-rw-rw-rw-   0        0        0     6706 2024-03-16 00:47:54.000000 venty-7.1.0/venty/in_memory_event_store_test.py
+-rw-rw-rw-   0        0        0      277 2024-04-12 15:22:15.000000 venty-7.1.0/venty/null_event_channel.py
+-rw-rw-rw-   0        0        0      781 2024-04-08 17:48:30.000000 venty-7.1.0/venty/object_storage.py
+-rw-rw-rw-   0        0        0      301 2024-04-08 18:03:19.000000 venty-7.1.0/venty/optional.py
+-rw-rw-rw-   0        0        0        0 2023-01-06 20:34:35.000000 venty-7.1.0/venty/py.typed
+-rw-rw-rw-   0        0        0      294 2024-04-05 09:27:44.000000 venty-7.1.0/venty/settings.py
+-rw-rw-rw-   0        0        0      589 2024-03-16 16:02:34.000000 venty-7.1.0/venty/settings_test.py
+-rw-rw-rw-   0        0        0     8293 2024-04-12 14:25:34.000000 venty-7.1.0/venty/sql_event_store.py
+-rw-rw-rw-   0        0        0     6817 2024-04-12 14:22:40.000000 venty-7.1.0/venty/sql_event_store_test.py
+-rw-rw-rw-   0        0        0      395 2024-04-12 14:22:40.000000 venty-7.1.0/venty/strong_types.py
+-rw-rw-rw-   0        0        0      996 2024-04-12 14:23:35.000000 venty-7.1.0/venty/strong_types_test.py
+-rw-rw-rw-   0        0        0      958 2024-03-16 16:40:05.000000 venty-7.1.0/venty/timing.py
+-rw-rw-rw-   0        0        0      961 2024-03-15 18:40:30.000000 venty-7.1.0/venty/timing_test.py
+drwxrwxrwx   0        0        0        0 2024-04-13 20:58:53.251354 venty-7.1.0/venty.egg-info/
+-rw-rw-rw-   0        0        0     2189 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1179 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-13 20:58:52.000000 venty-7.1.0/venty.egg-info/top_level.txt
```

### Comparing `venty-7.0.0/LICENSE` & `venty-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/PKG-INFO` & `venty-7.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venty
-Version: 7.0.0
+Version: 7.1.0
 Summary: Venty
 Home-page: https://github.com/sasha-tkachev/venty
 Author: Sasha Tkachev
 Author-email: sasha64sasha@gmail.com
 License: UNKNOWN
 Keywords: cloudevents,cloudevents[pydantic],ce,cloud,events,event,rest
 Platform: UNKNOWN
```

### Comparing `venty-7.0.0/README.md` & `venty-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/setup.py` & `venty-7.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 here = Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 if __name__ == "__main__":
     setuptools.setup(
         name="venty",
-        version="7.0.0",
+        version="7.1.0",
         author="Sasha Tkachev",
         author_email="sasha64sasha@gmail.com",
         description="Venty",
         long_description_content_type="text/markdown",
         long_description=long_description,
         home_page="https://github.com/sasha-tkachev/venty",
         url="https://github.com/sasha-tkachev/venty",
```

### Comparing `venty-7.0.0/tox.ini` & `venty-7.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/aggregate_root.py` & `venty-7.1.0/venty/aggregate_root.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/aggregate_store.py` & `venty-7.1.0/venty/aggregate_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from typing import Type
+from uuid import UUID, uuid5
+
+from venty.cloudevent import CloudEvent
+from pydantic import Field
 
 from venty import EventStore
 from venty.event_store import append_events, read_stream_no_metadata
 from venty.aggregate_root import AggregateRoot, AggregateUUID, AggregateRootT
-from venty.strong_types import StreamName, StreamVersion
+from venty.strong_types import StreamName
 
 
 def _aggregate_stream(uuid: AggregateUUID) -> StreamName:
     return StreamName(str(uuid))
 
 
 class AggregateStore:
```

### Comparing `venty-7.0.0/venty/aggregate_store_test.py` & `venty-7.1.0/venty/aggregate_store_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from dataclasses import dataclass
 from typing import Optional
 from uuid import UUID, uuid5
 
-from cloudevents.pydantic import CloudEvent
+from venty.cloudevent import CloudEvent
 
 from venty.aggregate_store import AggregateStore
 from venty.aggregate_root import AggregateUUID, AggregateRoot
 from venty.in_memory_event_store import InMemoryEventStore
 
 _BOOKS_NAMESPACE = UUID("c3ec5a4e-5e4f-44bf-ac40-bfb6c52cbdf6")
```

### Comparing `venty-7.0.0/venty/auth_event_producer.py` & `venty-7.1.0/venty/auth_event_producer.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/classification.py` & `venty-7.1.0/venty/classification.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, TypeVar, Any, Type, List
 
-from cloudevents.pydantic import CloudEvent
+from venty.cloudevent import CloudEvent
 
 
 T = TypeVar("T")
 
 
 def may_be(type_: Type[T], value: Any) -> Optional[T]:
     if isinstance(value, type_):
@@ -20,7 +20,11 @@
     if result is None:
         raise ValueError(f"Expected {type_.__name__}, got {value.__class__.__name__}")
     return result
 
 
 def must_be_list_of(type_: Type[T], value: Any) -> List[T]:
     return [must_be(type_, item) for item in must_be(list, value)]
+
+
+def is_any_instance_of(type_: Type[T], values: List[Any]) -> bool:
+    return any(isinstance(value, type_) for value in values)
```

### Comparing `venty-7.0.0/venty/classification_test.py` & `venty-7.1.0/venty/classification_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal
 
 import pytest
-from cloudevents.pydantic import CloudEvent
+from venty.cloudevent import CloudEvent
 from pydantic import BaseModel
 
-from venty.classification import may_be, must_be, must_be_list_of
+from venty.classification import may_be, must_be, must_be_list_of, is_any_instance_of
 
 
 class MyData(BaseModel):
     x: int
 
 
 class MyEvent(CloudEvent):
@@ -40,7 +40,13 @@
         must_be(int, 42.0)
 
 
 def test_must_be_list_of():
     assert must_be_list_of(int, [1, 2, 3]) == [1, 2, 3]
     with pytest.raises(ValueError, match="Expected int, got str"):
         must_be_list_of(int, [1, 2, "3"])
+
+
+def test_is_any_instance_of():
+    assert is_any_instance_of(int, [1, 2, 3])
+    assert is_any_instance_of(int, [1, 2, "3"])
+    assert not is_any_instance_of(str, [1, 2, 3.0])
```

### Comparing `venty-7.0.0/venty/event_channel.py` & `venty-7.1.0/venty/event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/event_logger.py` & `venty-7.1.0/venty/event_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from contextlib import contextmanager
 from datetime import datetime, timezone
 from logging import Formatter, LogRecord, StreamHandler
 from typing import Any, Dict, TypeVar, Optional
 
-from cloudevents.pydantic import CloudEvent
+from venty.cloudevent import CloudEvent
 from pythonjsonlogger.jsonlogger import JsonFormatter
 import json
 from venty.event_producer import EventProducer
 
 # https://github.com/cloudevents/spec/blob/main/cloudevents/extensions/severity.md
 _FATAL_SEVERITY = 21
 _ERROR_SEVERITY = 17
```

### Comparing `venty-7.0.0/venty/event_producer.py` & `venty-7.1.0/venty/event_producer.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/event_producer_stack.py` & `venty-7.1.0/venty/event_producer_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 from typing import Dict, Any, Optional, ContextManager, Type
-
-from cloudevents.pydantic import CloudEvent
-
 from venty.event_producer import (
     EventProducer,
     EventProducerT,
     AttributeValue,
 )
 from venty.strong_types import CloudEventT
 from collections import OrderedDict
```

### Comparing `venty-7.0.0/venty/event_producer_stack_test.py` & `venty-7.1.0/venty/event_producer_stack_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Literal
 
 import pytest
-from cloudevents.pydantic import CloudEvent
+from venty.cloudevent import CloudEvent
 
 from venty.event_producer import SimpleEventProducer
 from venty.event_producer_stack import EventProducerStack
 from venty.strong_types import EventSource
 
 
 class MyType(CloudEvent):
```

### Comparing `venty-7.0.0/venty/event_producer_test.py` & `venty-7.1.0/venty/event_producer_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import Literal
 
 from cloudevents.conversion import to_dict
-from cloudevents.pydantic import CloudEvent
+from venty.cloudevent import CloudEvent
 
 from venty.event_producer import SimpleEventProducer, testing_event_producer
 from venty.strong_types import EventSource
 
 
 class MyType(CloudEvent):
     type: Literal["my-type"] = "my-type"
```

### Comparing `venty-7.0.0/venty/event_store.py` & `venty-7.1.0/venty/event_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,131 +106,131 @@
     def current_version(
         self, stream_name: StreamName, *, timeout: Optional[timedelta] = None
     ) -> Optional[Union[StreamVersion, Literal[StreamState.NO_STREAM]]]:
         raise NotImplementedError()
 
 
 def attempt_append_event(
-    repo: EventStore,
+    event_store: EventStore,
     stream_name: StreamName,
     *,
     expected_version: ExpectedVersion,
     event: CloudEvent,
     timeout: Optional[timedelta] = None,
 ) -> Optional[CommitPosition]:
     """
     Syntax sugar to append a single event to a stream.
     """
-    return repo.attempt_append_events(
+    return event_store.attempt_append_events(
         stream_name=stream_name,
         expected_version=expected_version,
         events=(event,),
         timeout=timeout,
     )
 
 
 def attempt_append_events(
-    repo: EventStore,
+    event_store: EventStore,
     stream_name: StreamName,
     *,
     expected_version: ExpectedVersion,
     events: Iterable[CloudEvent],
     timeout: Optional[timedelta] = None,
 ) -> Optional[CommitPosition]:
     """
     Syntax sugar to stay consistent with `append_event`
     """
-    return repo.attempt_append_events(
+    return event_store.attempt_append_events(
         stream_name=stream_name,
         expected_version=expected_version,
         events=events,
         timeout=timeout,
     )
 
 
 class WrongExpectedVersion(ValueError):
     pass
 
 
 def append_events(
-    repo: EventStore,
+    event_store: EventStore,
     stream_name: StreamName,
     *,
     expected_version: ExpectedVersion,
     events: Iterable[CloudEvent],
     timeout: Optional[timedelta] = None,
 ) -> CommitPosition:
     """
     Syntax sugar to stay consistent with `append_event`
     """
-    result = repo.attempt_append_events(
+    result = event_store.attempt_append_events(
         stream_name=stream_name,
         expected_version=expected_version,
         events=events,
         timeout=timeout,
     )
     if result is None:
         raise WrongExpectedVersion()
     return result
 
 
 def append_event(
-    repo: EventStore,
+    event_store: EventStore,
     stream_name: StreamName,
     *,
     expected_version: ExpectedVersion,
     event: CloudEvent,
     timeout: Optional[timedelta] = None,
 ) -> Optional[CommitPosition]:
     """
     Syntax sugar to append a single event to a stream.
     """
     return append_events(
-        repo=repo,
+        event_store=event_store,
         stream_name=stream_name,
         expected_version=expected_version,
         events=(event,),
         timeout=timeout,
     )
 
 
 def read_stream(
-    repo: EventStore,
+    event_store: EventStore,
     stream_name: StreamName,
     *,
     stream_position: Optional[StreamVersion],
     limit: int = sys.maxsize,
     backwards: bool = False,
     timeout: Optional[timedelta] = None,
 ) -> Iterable[RecordedEvent]:
-    return repo.read_streams(
+    return event_store.read_streams(
         {
             stream_name: ReadInstruction(
                 stream_position=stream_position,
                 limit=limit,
             )
         },
         backwards=backwards,
         timeout=timeout,
     )
 
 
 def read_stream_no_metadata(
-    repo: EventStore,
+    event_store: EventStore,
     stream_name: StreamName,
     *,
     stream_position: Optional[StreamVersion],
     limit: int = sys.maxsize,
     backwards: bool = False,
     timeout: Optional[timedelta] = None,
 ) -> Iterable[CloudEvent]:
     return (
         e.event
         for e in read_stream(
-            repo,
+            event_store,
             stream_name,
             stream_position=stream_position,
             limit=limit,
             backwards=backwards,
             timeout=timeout,
         )
     )
```

### Comparing `venty-7.0.0/venty/http_event_channel.py` & `venty-7.1.0/venty/http_event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/http_event_channel_test.py` & `venty-7.1.0/venty/http_event_channel_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cloudevents.pydantic import CloudEvent
+from venty.cloudevent import CloudEvent
 from mock import Mock
 
 from venty.event_channel import publish_event
 from venty.http_event_channel import HttpEventChannel, HttpChannelMode
 
 
 def test_http_channel_with_binary_mode_must_put_all_ce_attributes_in_header():
```

### Comparing `venty-7.0.0/venty/in_memory_event_channel.py` & `venty-7.1.0/venty/in_memory_event_channel.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/in_memory_event_store.py` & `venty-7.1.0/venty/in_memory_event_store.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/in_memory_event_store_test.py` & `venty-7.1.0/venty/in_memory_event_store_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/object_storage.py` & `venty-7.1.0/venty/object_storage.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/settings_test.py` & `venty-7.1.0/venty/settings_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/sql_event_store.py` & `venty-7.1.0/venty/sql_event_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import json
 from uuid import uuid5, UUID
 
+from pydantic import BaseModel
 from sqlalchemy.exc import IntegrityError
 
 from venty.settings import SQL_RECORDED_EVENTS_TABLE_NAME
 from venty.timing import assert_timeout_not_supported
 
 try:
     import sqlalchemy
@@ -23,25 +25,25 @@
     Callable,
     Sequence,
     Tuple,
     Dict,
     Type,
 )
 
-from cloudevents.abstract import CloudEvent, AnyCloudEvent
-from cloudevents.conversion import to_json, from_json
+from venty.cloudevent import CloudEvent
+from cloudevents.conversion import from_json, to_json
 from sqlalchemy import (
     Column,
     Integer,
     BINARY,
     Text,
     UniqueConstraint,
 )
 from sqlalchemy.orm import declarative_base
-from sqlalchemy.orm import Session, aliased
+from sqlalchemy.orm import Session
 
 from venty import EventStore
 from venty.event_store import (
     ExpectedVersion,
     is_stream_version_correct,
     StreamState,
     ReadInstruction,
@@ -108,24 +110,24 @@
     last_stream_position: Union[StreamVersion, Literal[StreamState.NO_STREAM]],
     stream_id: bytes,
 ) -> Sequence[RecordedEventRow]:
     return [
         RecordedEventRow(
             stream_id=stream_id,
             stream_position=last_stream_position + 1 + i,
-            event=to_json(event),
+            event=event.json(exclude_none=True),
         )
         for i, event in enumerate(events)
     ]
 
 
 def _row_to_recorded_event(
     event_row: RecordedEventRow,
     stream_name_map: Dict[bytes, StreamName],
-    event_type: Type[AnyCloudEvent],
+    event_type: Type[CloudEvent],
 ) -> RecordedEvent:
     return RecordedEvent(
         commit_position=CommitPosition(
             event_row.id,
         ),
         stream_position=StreamVersion(
             event_row.stream_position,
@@ -138,15 +140,15 @@
     )
 
 
 def _query_streams(
     session: Session,
     instructions: Dict[StreamName, ReadInstruction],
     backwards: bool,
-    event_type: Type[AnyCloudEvent],
+    event_type: Type[CloudEvent],
 ) -> Iterable[RecordedEvent]:
     or_conditions = [
         and_(
             RecordedEventRow.stream_id == _stream_id(stream_name),
             RecordedEventRow.stream_position >= instruction.stream_position_or_default,
             RecordedEventRow.stream_position
             <= instruction.stream_position_or_default + instruction.limit,
@@ -206,15 +208,15 @@
     session.commit()
     return _highest_commit_position(row_records)
 
 
 class SqlEventStore(EventStore):
 
     def __init__(
-        self, session_factory: Callable[[], Session], event_type: Type[AnyCloudEvent]
+        self, session_factory: Callable[[], Session], event_type: Type[CloudEvent]
     ):
         self._session_factory = session_factory
         self._event_type = event_type
 
     def attempt_append_events(
         self,
         stream_name: StreamName,
```

### Comparing `venty-7.0.0/venty/sql_event_store_test.py` & `venty-7.1.0/venty/sql_event_store_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable, Any
 from uuid import UUID
 
 import pytest
-from cloudevents.pydantic import CloudEvent
+from venty.cloudevent import CloudEvent
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker, Session
 
 from venty import attempt_append_events
 from venty.event_store import append_events, StreamState, read_stream_no_metadata
 from venty.sql_event_store import Base, SqlEventStore
 from venty.strong_types import NO_EVENT_VERSION, StreamVersion
```

### Comparing `venty-7.0.0/venty/strong_types_test.py` & `venty-7.1.0/venty/strong_types_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable
 from uuid import UUID, uuid5
 from datetime import timedelta, datetime, timezone
 from venty.strong_types import StreamName, EventType
-from cloudevents.pydantic.v2 import CloudEvent
+from venty.cloudevent import CloudEvent
 import time
 
 MY_STREAM_NAME = StreamName("my-stream")
 YOUR_STREAM_NAME = StreamName("your-stream")
 MY_EVENT_TYPE = EventType("my-type")
```

### Comparing `venty-7.0.0/venty/timing.py` & `venty-7.1.0/venty/timing.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty/timing_test.py` & `venty-7.1.0/venty/timing_test.py`

 * *Files identical despite different names*

### Comparing `venty-7.0.0/venty.egg-info/PKG-INFO` & `venty-7.1.0/venty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venty
-Version: 7.0.0
+Version: 7.1.0
 Summary: Venty
 Home-page: https://github.com/sasha-tkachev/venty
 Author: Sasha Tkachev
 Author-email: sasha64sasha@gmail.com
 License: UNKNOWN
 Keywords: cloudevents,cloudevents[pydantic],ce,cloud,events,event,rest
 Platform: UNKNOWN
```

### Comparing `venty-7.0.0/venty.egg-info/SOURCES.txt` & `venty-7.1.0/venty.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,38 @@
 README.md
 requirements.txt
 setup.py
 test_requirements.txt
 tox.ini
 venty/__init__.py
 venty/_dummy.py
+venty/aggregate_channel.py
 venty/aggregate_root.py
 venty/aggregate_store.py
 venty/aggregate_store_test.py
 venty/auth_event_producer.py
 venty/classification.py
 venty/classification_test.py
+venty/cloudevent.py
 venty/event_channel.py
 venty/event_channel_test.py
 venty/event_logger.py
 venty/event_producer.py
 venty/event_producer_stack.py
 venty/event_producer_stack_test.py
 venty/event_producer_test.py
 venty/event_store.py
+venty/event_stream_channel.py
 venty/http_event_channel.py
 venty/http_event_channel_test.py
 venty/in_memory_event_channel.py
 venty/in_memory_event_channel_test.py
 venty/in_memory_event_store.py
 venty/in_memory_event_store_test.py
+venty/null_event_channel.py
 venty/object_storage.py
 venty/optional.py
 venty/py.typed
 venty/settings.py
 venty/settings_test.py
 venty/sql_event_store.py
 venty/sql_event_store_test.py
```

