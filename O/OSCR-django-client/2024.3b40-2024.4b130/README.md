# Comparing `tmp/OSCR-django-client-2024.3b40.tar.gz` & `tmp/OSCR-django-client-2024.4b130.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OSCR-django-client-2024.3b40.tar", last modified: Tue Mar  5 03:13:25 2024, max compression
+gzip compressed data, was "OSCR-django-client-2024.4b130.tar", last modified: Sat Apr 13 10:49:48 2024, max compression
```

## Comparing `OSCR-django-client-2024.3b40.tar` & `OSCR-django-client-2024.4b130.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-03-05 03:13:25.635414 OSCR-django-client-2024.3b40/
-drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-03-05 03:13:25.628414 OSCR-django-client-2024.3b40/OSCR_django_client/
--rw-r--r--   0 kraust    (1000) users      (100)     1635 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/__init__.py
-drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-03-05 03:13:25.630414 OSCR-django-client-2024.3b40/OSCR_django_client/api/
--rw-r--r--   0 kraust    (1000) users      (100)      237 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/api/__init__.py
--rw-r--r--   0 kraust    (1000) users      (100)    41955 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/api/combatlog_api.py
--rw-r--r--   0 kraust    (1000) users      (100)    25784 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/api/ladder_api.py
--rw-r--r--   0 kraust    (1000) users      (100)   193624 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/api/ladder_entries_api.py
--rw-r--r--   0 kraust    (1000) users      (100)    25721 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/api_client.py
--rw-r--r--   0 kraust    (1000) users      (100)      652 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/api_response.py
--rw-r--r--   0 kraust    (1000) users      (100)    15057 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/configuration.py
--rw-r--r--   0 kraust    (1000) users      (100)     5872 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/exceptions.py
-drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-03-05 03:13:25.632414 OSCR-django-client-2024.3b40/OSCR_django_client/models/
--rw-r--r--   0 kraust    (1000) users      (100)      860 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/__init__.py
--rw-r--r--   0 kraust    (1000) users      (100)     2792 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/combat_log.py
--rw-r--r--   0 kraust    (1000) users      (100)     2792 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/combat_log_upload_response.py
--rw-r--r--   0 kraust    (1000) users      (100)     3547 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/combatlog_list200_response.py
--rw-r--r--   0 kraust    (1000) users      (100)     2912 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/ladder.py
--rw-r--r--   0 kraust    (1000) users      (100)     3571 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/ladder_entries_list200_response.py
--rw-r--r--   0 kraust    (1000) users      (100)     3173 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/ladder_entry.py
--rw-r--r--   0 kraust    (1000) users      (100)     3522 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/ladder_list200_response.py
--rw-r--r--   0 kraust    (1000) users      (100)     3129 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/models/metadata.py
--rw-r--r--   0 kraust    (1000) users      (100)        0 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/py.typed
--rw-r--r--   0 kraust    (1000) users      (100)     9136 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/OSCR_django_client/rest.py
-drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-03-05 03:13:25.634414 OSCR-django-client-2024.3b40/OSCR_django_client.egg-info/
--rw-r--r--   0 kraust    (1000) users      (100)      408 2024-03-05 03:13:25.000000 OSCR-django-client-2024.3b40/OSCR_django_client.egg-info/PKG-INFO
--rw-r--r--   0 kraust    (1000) users      (100)     1389 2024-03-05 03:13:25.000000 OSCR-django-client-2024.3b40/OSCR_django_client.egg-info/SOURCES.txt
--rw-r--r--   0 kraust    (1000) users      (100)        1 2024-03-05 03:13:25.000000 OSCR-django-client-2024.3b40/OSCR_django_client.egg-info/dependency_links.txt
--rw-r--r--   0 kraust    (1000) users      (100)       76 2024-03-05 03:13:25.000000 OSCR-django-client-2024.3b40/OSCR_django_client.egg-info/requires.txt
--rw-r--r--   0 kraust    (1000) users      (100)       19 2024-03-05 03:13:25.000000 OSCR-django-client-2024.3b40/OSCR_django_client.egg-info/top_level.txt
--rw-r--r--   0 kraust    (1000) users      (100)      408 2024-03-05 03:13:25.635414 OSCR-django-client-2024.3b40/PKG-INFO
--rw-r--r--   0 kraust    (1000) users      (100)     4184 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/README.md
--rw-r--r--   0 kraust    (1000) users      (100)     1954 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/pyproject.toml
--rw-r--r--   0 kraust    (1000) users      (100)       69 2024-03-05 03:13:25.635414 OSCR-django-client-2024.3b40/setup.cfg
--rw-r--r--   0 kraust    (1000) users      (100)     1138 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/setup.py
-drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-03-05 03:13:25.634414 OSCR-django-client-2024.3b40/test/
--rw-r--r--   0 kraust    (1000) users      (100)     1945 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_combat_log.py
--rw-r--r--   0 kraust    (1000) users      (100)     1608 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_combat_log_upload_response.py
--rw-r--r--   0 kraust    (1000) users      (100)     1046 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_combatlog_api.py
--rw-r--r--   0 kraust    (1000) users      (100)     2621 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_combatlog_list200_response.py
--rw-r--r--   0 kraust    (1000) users      (100)     1400 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_ladder.py
--rw-r--r--   0 kraust    (1000) users      (100)      733 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_ladder_api.py
--rw-r--r--   0 kraust    (1000) users      (100)      801 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_ladder_entries_api.py
--rw-r--r--   0 kraust    (1000) users      (100)     2378 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_ladder_entries_list200_response.py
--rw-r--r--   0 kraust    (1000) users      (100)     1609 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_ladder_entry.py
--rw-r--r--   0 kraust    (1000) users      (100)     2069 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_ladder_list200_response.py
--rw-r--r--   0 kraust    (1000) users      (100)     1578 2024-03-05 03:12:40.000000 OSCR-django-client-2024.3b40/test/test_metadata.py
+drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-04-13 10:49:48.487840 OSCR-django-client-2024.4b130/
+drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-04-13 10:49:48.432839 OSCR-django-client-2024.4b130/OSCR_django_client/
+-rw-r--r--   0 kraust    (1000) users      (100)     1635 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/__init__.py
+drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-04-13 10:49:48.434838 OSCR-django-client-2024.4b130/OSCR_django_client/api/
+-rw-r--r--   0 kraust    (1000) users      (100)      237 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/api/__init__.py
+-rw-r--r--   0 kraust    (1000) users      (100)    41955 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/api/combatlog_api.py
+-rw-r--r--   0 kraust    (1000) users      (100)    27113 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/api/ladder_api.py
+-rw-r--r--   0 kraust    (1000) users      (100)    54400 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/api/ladder_entries_api.py
+-rw-r--r--   0 kraust    (1000) users      (100)    25721 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/api_client.py
+-rw-r--r--   0 kraust    (1000) users      (100)      652 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/api_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)    15057 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/configuration.py
+-rw-r--r--   0 kraust    (1000) users      (100)     5872 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/exceptions.py
+drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-04-13 10:49:48.436838 OSCR-django-client-2024.4b130/OSCR_django_client/models/
+-rw-r--r--   0 kraust    (1000) users      (100)      860 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/__init__.py
+-rw-r--r--   0 kraust    (1000) users      (100)     2805 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/combat_log.py
+-rw-r--r--   0 kraust    (1000) users      (100)     2805 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/combat_log_upload_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)     3560 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/combatlog_list200_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)     3544 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/ladder.py
+-rw-r--r--   0 kraust    (1000) users      (100)     3584 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/ladder_entries_list200_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)     3186 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/ladder_entry.py
+-rw-r--r--   0 kraust    (1000) users      (100)     3535 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/ladder_list200_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)     3382 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/models/metadata.py
+-rw-r--r--   0 kraust    (1000) users      (100)        0 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/py.typed
+-rw-r--r--   0 kraust    (1000) users      (100)     9136 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/OSCR_django_client/rest.py
+drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-04-13 10:49:48.486840 OSCR-django-client-2024.4b130/OSCR_django_client.egg-info/
+-rw-r--r--   0 kraust    (1000) users      (100)      409 2024-04-13 10:49:48.000000 OSCR-django-client-2024.4b130/OSCR_django_client.egg-info/PKG-INFO
+-rw-r--r--   0 kraust    (1000) users      (100)     1389 2024-04-13 10:49:48.000000 OSCR-django-client-2024.4b130/OSCR_django_client.egg-info/SOURCES.txt
+-rw-r--r--   0 kraust    (1000) users      (100)        1 2024-04-13 10:49:48.000000 OSCR-django-client-2024.4b130/OSCR_django_client.egg-info/dependency_links.txt
+-rw-r--r--   0 kraust    (1000) users      (100)       76 2024-04-13 10:49:48.000000 OSCR-django-client-2024.4b130/OSCR_django_client.egg-info/requires.txt
+-rw-r--r--   0 kraust    (1000) users      (100)       19 2024-04-13 10:49:48.000000 OSCR-django-client-2024.4b130/OSCR_django_client.egg-info/top_level.txt
+-rw-r--r--   0 kraust    (1000) users      (100)      409 2024-04-13 10:49:48.487840 OSCR-django-client-2024.4b130/PKG-INFO
+-rw-r--r--   0 kraust    (1000) users      (100)     4211 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/README.md
+-rw-r--r--   0 kraust    (1000) users      (100)     1954 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/pyproject.toml
+-rw-r--r--   0 kraust    (1000) users      (100)       69 2024-04-13 10:49:48.488840 OSCR-django-client-2024.4b130/setup.cfg
+-rw-r--r--   0 kraust    (1000) users      (100)     1138 2024-04-13 10:48:58.000000 OSCR-django-client-2024.4b130/setup.py
+drwxr-xr-x   0 kraust    (1000) users      (100)        0 2024-04-13 10:49:48.486840 OSCR-django-client-2024.4b130/test/
+-rw-r--r--   0 kraust    (1000) users      (100)     1945 2024-04-06 13:09:51.000000 OSCR-django-client-2024.4b130/test/test_combat_log.py
+-rw-r--r--   0 kraust    (1000) users      (100)     1608 2024-04-06 13:09:51.000000 OSCR-django-client-2024.4b130/test/test_combat_log_upload_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)     1046 2024-04-06 13:09:52.000000 OSCR-django-client-2024.4b130/test/test_combatlog_api.py
+-rw-r--r--   0 kraust    (1000) users      (100)     2621 2024-04-06 13:09:51.000000 OSCR-django-client-2024.4b130/test/test_combatlog_list200_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)     1528 2024-04-06 13:09:51.000000 OSCR-django-client-2024.4b130/test/test_ladder.py
+-rw-r--r--   0 kraust    (1000) users      (100)      733 2024-04-06 13:09:52.000000 OSCR-django-client-2024.4b130/test/test_ladder_api.py
+-rw-r--r--   0 kraust    (1000) users      (100)      801 2024-04-06 13:09:52.000000 OSCR-django-client-2024.4b130/test/test_ladder_entries_api.py
+-rw-r--r--   0 kraust    (1000) users      (100)     2378 2024-04-06 13:09:51.000000 OSCR-django-client-2024.4b130/test/test_ladder_entries_list200_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)     1609 2024-04-06 13:09:51.000000 OSCR-django-client-2024.4b130/test/test_ladder_entry.py
+-rw-r--r--   0 kraust    (1000) users      (100)     2319 2024-04-06 13:09:51.000000 OSCR-django-client-2024.4b130/test/test_ladder_list200_response.py
+-rw-r--r--   0 kraust    (1000) users      (100)     1578 2024-04-06 13:09:51.000000 OSCR-django-client-2024.4b130/test/test_metadata.py
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/__init__.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v1
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "v2024.3b040"
+__version__ = "v2024.4b130"
 
 # import apis into sdk package
 from OSCR_django_client.api.combatlog_api import CombatlogApi
 from OSCR_django_client.api.ladder_api import LadderApi
 from OSCR_django_client.api.ladder_entries_api import LadderEntriesApi
 
 # import ApiClient
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/api/combatlog_api.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/api/combatlog_api.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/api/ladder_api.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/api/ladder_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,18 @@
 
 
     @validate_call
     def ladder_list(
         self,
         name: Annotated[Optional[StrictStr], Field(description="name")] = None,
         difficulty: Annotated[Optional[StrictStr], Field(description="difficulty")] = None,
-        metric: Annotated[Optional[StrictStr], Field(description="metric")] = None,
+        variant: Annotated[Optional[StrictStr], Field(description="variant")] = None,
         is_solo: Annotated[Optional[StrictStr], Field(description="is_solo")] = None,
+        is_space: Annotated[Optional[StrictStr], Field(description="is_space")] = None,
+        metric: Annotated[Optional[StrictStr], Field(description="metric")] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
@@ -68,18 +70,22 @@
 
         Ladder API
 
         :param name: name
         :type name: str
         :param difficulty: difficulty
         :type difficulty: str
-        :param metric: metric
-        :type metric: str
+        :param variant: variant
+        :type variant: str
         :param is_solo: is_solo
         :type is_solo: str
+        :param is_space: is_space
+        :type is_space: str
+        :param metric: metric
+        :type metric: str
         :param ordering: Which field to use when ordering the results.
         :type ordering: str
         :param search: A search term.
         :type search: str
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
@@ -105,16 +111,18 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._ladder_list_serialize(
             name=name,
             difficulty=difficulty,
-            metric=metric,
+            variant=variant,
             is_solo=is_solo,
+            is_space=is_space,
+            metric=metric,
             ordering=ordering,
             search=search,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -136,16 +144,18 @@
 
 
     @validate_call
     def ladder_list_with_http_info(
         self,
         name: Annotated[Optional[StrictStr], Field(description="name")] = None,
         difficulty: Annotated[Optional[StrictStr], Field(description="difficulty")] = None,
-        metric: Annotated[Optional[StrictStr], Field(description="metric")] = None,
+        variant: Annotated[Optional[StrictStr], Field(description="variant")] = None,
         is_solo: Annotated[Optional[StrictStr], Field(description="is_solo")] = None,
+        is_space: Annotated[Optional[StrictStr], Field(description="is_space")] = None,
+        metric: Annotated[Optional[StrictStr], Field(description="metric")] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
@@ -163,18 +173,22 @@
 
         Ladder API
 
         :param name: name
         :type name: str
         :param difficulty: difficulty
         :type difficulty: str
-        :param metric: metric
-        :type metric: str
+        :param variant: variant
+        :type variant: str
         :param is_solo: is_solo
         :type is_solo: str
+        :param is_space: is_space
+        :type is_space: str
+        :param metric: metric
+        :type metric: str
         :param ordering: Which field to use when ordering the results.
         :type ordering: str
         :param search: A search term.
         :type search: str
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
@@ -200,16 +214,18 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._ladder_list_serialize(
             name=name,
             difficulty=difficulty,
-            metric=metric,
+            variant=variant,
             is_solo=is_solo,
+            is_space=is_space,
+            metric=metric,
             ordering=ordering,
             search=search,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -231,16 +247,18 @@
 
 
     @validate_call
     def ladder_list_without_preload_content(
         self,
         name: Annotated[Optional[StrictStr], Field(description="name")] = None,
         difficulty: Annotated[Optional[StrictStr], Field(description="difficulty")] = None,
-        metric: Annotated[Optional[StrictStr], Field(description="metric")] = None,
+        variant: Annotated[Optional[StrictStr], Field(description="variant")] = None,
         is_solo: Annotated[Optional[StrictStr], Field(description="is_solo")] = None,
+        is_space: Annotated[Optional[StrictStr], Field(description="is_space")] = None,
+        metric: Annotated[Optional[StrictStr], Field(description="metric")] = None,
         ordering: Annotated[Optional[StrictStr], Field(description="Which field to use when ordering the results.")] = None,
         search: Annotated[Optional[StrictStr], Field(description="A search term.")] = None,
         page: Annotated[Optional[StrictInt], Field(description="A page number within the paginated result set.")] = None,
         page_size: Annotated[Optional[StrictInt], Field(description="Number of results to return per page.")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
@@ -258,18 +276,22 @@
 
         Ladder API
 
         :param name: name
         :type name: str
         :param difficulty: difficulty
         :type difficulty: str
-        :param metric: metric
-        :type metric: str
+        :param variant: variant
+        :type variant: str
         :param is_solo: is_solo
         :type is_solo: str
+        :param is_space: is_space
+        :type is_space: str
+        :param metric: metric
+        :type metric: str
         :param ordering: Which field to use when ordering the results.
         :type ordering: str
         :param search: A search term.
         :type search: str
         :param page: A page number within the paginated result set.
         :type page: int
         :param page_size: Number of results to return per page.
@@ -295,16 +317,18 @@
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._ladder_list_serialize(
             name=name,
             difficulty=difficulty,
-            metric=metric,
+            variant=variant,
             is_solo=is_solo,
+            is_space=is_space,
+            metric=metric,
             ordering=ordering,
             search=search,
             page=page,
             page_size=page_size,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
@@ -321,16 +345,18 @@
         return response_data.response
 
 
     def _ladder_list_serialize(
         self,
         name,
         difficulty,
-        metric,
+        variant,
         is_solo,
+        is_space,
+        metric,
         ordering,
         search,
         page,
         page_size,
         _request_auth,
         _content_type,
         _headers,
@@ -355,22 +381,30 @@
             
             _query_params.append(('name', name))
             
         if difficulty is not None:
             
             _query_params.append(('difficulty', difficulty))
             
-        if metric is not None:
+        if variant is not None:
             
-            _query_params.append(('metric', metric))
+            _query_params.append(('variant', variant))
             
         if is_solo is not None:
             
             _query_params.append(('is_solo', is_solo))
             
+        if is_space is not None:
+            
+            _query_params.append(('is_space', is_space))
+            
+        if metric is not None:
+            
+            _query_params.append(('metric', metric))
+            
         if ordering is not None:
             
             _query_params.append(('ordering', ordering))
             
         if search is not None:
             
             _query_params.append(('search', search))
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/api_client.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/v2024.3b040/python'
+        self.user_agent = 'OpenAPI-Generator/v2024.4b130/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/api_response.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/api_response.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/configuration.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: v2024.3b040".\
+               "SDK Package Version: v2024.4b130".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/exceptions.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/models/__init__.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/models/combat_log.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/models/combat_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,33 +13,33 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
 from OSCR_django_client.models.metadata import Metadata
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CombatLog(BaseModel):
     """
     CombatLog
     """ # noqa: E501
     id: Optional[StrictInt] = None
     metadata: Metadata
     __properties: ClassVar[List[str]] = ["id", "metadata"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/models/combat_log_upload_response.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/models/combat_log_upload_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt
 from typing import Any, ClassVar, Dict, List, Union
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CombatLogUploadResponse(BaseModel):
     """
@@ -29,19 +29,19 @@
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True)]
     updated: StrictBool
     detail: Annotated[str, Field(min_length=1, strict=True)]
     value: Union[StrictFloat, StrictInt]
     __properties: ClassVar[List[str]] = ["name", "updated", "detail", "value"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/models/combatlog_list200_response.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/models/combatlog_list200_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from OSCR_django_client.models.combat_log import CombatLog
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CombatlogList200Response(BaseModel):
     """
@@ -29,19 +29,19 @@
     """ # noqa: E501
     count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
     results: List[CombatLog]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/models/ladder.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/models/ladder_entry.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,86 +13,94 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Ladder(BaseModel):
+class LadderEntry(BaseModel):
     """
-    Ladder
+    LadderEntry
     """ # noqa: E501
     id: Optional[StrictInt] = None
-    name: Annotated[str, Field(min_length=1, strict=True)]
-    difficulty: Annotated[str, Field(min_length=1, strict=True)]
-    metric: Annotated[str, Field(min_length=1, strict=True)]
-    is_solo: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["id", "name", "difficulty", "metric", "is_solo"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    var_date: Optional[StrictStr] = Field(default=None, alias="date")
+    rank: Optional[StrictInt] = None
+    player: Annotated[str, Field(min_length=1, strict=True)]
+    data: Dict[str, Any]
+    combatlog: StrictInt
+    ladder: StrictInt
+    __properties: ClassVar[List[str]] = ["id", "date", "rank", "player", "data", "combatlog", "ladder"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Ladder from a JSON string"""
+        """Create an instance of LadderEntry from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
             "id",
+            "var_date",
+            "rank",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Ladder from a dict"""
+        """Create an instance of LadderEntry from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "name": obj.get("name"),
-            "difficulty": obj.get("difficulty"),
-            "metric": obj.get("metric"),
-            "is_solo": obj.get("is_solo")
+            "date": obj.get("date"),
+            "rank": obj.get("rank"),
+            "player": obj.get("player"),
+            "data": obj.get("data"),
+            "combatlog": obj.get("combatlog"),
+            "ladder": obj.get("ladder")
         })
         return _obj
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/models/ladder_entries_list200_response.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/models/ladder_list200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,49 +13,49 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from OSCR_django_client.models.ladder_entry import LadderEntry
+from OSCR_django_client.models.ladder import Ladder
 from typing import Optional, Set
 from typing_extensions import Self
 
-class LadderEntriesList200Response(BaseModel):
+class LadderList200Response(BaseModel):
     """
-    LadderEntriesList200Response
+    LadderList200Response
     """ # noqa: E501
     count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: List[LadderEntry]
+    results: List[Ladder]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of LadderEntriesList200Response from a JSON string"""
+        """Create an instance of LadderList200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -89,23 +89,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of LadderEntriesList200Response from a dict"""
+        """Create an instance of LadderList200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [LadderEntry.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [Ladder.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/models/ladder_entry.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/models/metadata.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,94 +13,97 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from datetime import datetime
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class LadderEntry(BaseModel):
+class Metadata(BaseModel):
     """
-    LadderEntry
+    Metadata
     """ # noqa: E501
     id: Optional[StrictInt] = None
-    var_date: Optional[StrictStr] = Field(default=None, alias="date")
-    rank: Optional[StrictInt] = None
-    player: Annotated[str, Field(min_length=1, strict=True)]
-    data: Dict[str, Any]
-    combatlog: StrictInt
-    ladder: StrictInt
-    __properties: ClassVar[List[str]] = ["id", "date", "rank", "player", "data", "combatlog", "ladder"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    map: Annotated[str, Field(min_length=1, strict=True)]
+    difficulty: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
+    summary: Dict[str, Any]
+    date_time: Optional[datetime] = None
+    __properties: ClassVar[List[str]] = ["id", "map", "difficulty", "summary", "date_time"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of LadderEntry from a JSON string"""
+        """Create an instance of Metadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
             "id",
-            "var_date",
-            "rank",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # set to None if difficulty (nullable) is None
+        # and model_fields_set contains the field
+        if self.difficulty is None and "difficulty" in self.model_fields_set:
+            _dict['difficulty'] = None
+
+        # set to None if date_time (nullable) is None
+        # and model_fields_set contains the field
+        if self.date_time is None and "date_time" in self.model_fields_set:
+            _dict['date_time'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of LadderEntry from a dict"""
+        """Create an instance of Metadata from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "date": obj.get("date"),
-            "rank": obj.get("rank"),
-            "player": obj.get("player"),
-            "data": obj.get("data"),
-            "combatlog": obj.get("combatlog"),
-            "ladder": obj.get("ladder")
+            "map": obj.get("map"),
+            "difficulty": obj.get("difficulty"),
+            "summary": obj.get("summary"),
+            "date_time": obj.get("date_time")
         })
         return _obj
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/models/ladder_list200_response.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/models/ladder_entries_list200_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,49 +13,49 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from OSCR_django_client.models.ladder import Ladder
+from OSCR_django_client.models.ladder_entry import LadderEntry
 from typing import Optional, Set
 from typing_extensions import Self
 
-class LadderList200Response(BaseModel):
+class LadderEntriesList200Response(BaseModel):
     """
-    LadderList200Response
+    LadderEntriesList200Response
     """ # noqa: E501
     count: StrictInt
     next: Optional[StrictStr] = None
     previous: Optional[StrictStr] = None
-    results: List[Ladder]
+    results: List[LadderEntry]
     __properties: ClassVar[List[str]] = ["count", "next", "previous", "results"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of LadderList200Response from a JSON string"""
+        """Create an instance of LadderEntriesList200Response from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -89,23 +89,23 @@
         if self.previous is None and "previous" in self.model_fields_set:
             _dict['previous'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of LadderList200Response from a dict"""
+        """Create an instance of LadderEntriesList200Response from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "count": obj.get("count"),
             "next": obj.get("next"),
             "previous": obj.get("previous"),
-            "results": [Ladder.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [LadderEntry.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client/rest.py` & `OSCR-django-client-2024.4b130/OSCR_django_client/rest.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/OSCR_django_client.egg-info/SOURCES.txt` & `OSCR-django-client-2024.4b130/OSCR_django_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/README.md` & `OSCR-django-client-2024.4b130/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # OSCR-django-client
 OSCR API
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v1
-- Package version: v2024.3b040
+- Package version: v2024.4b130
+- Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `OSCR-django-client-2024.3b40/pyproject.toml` & `OSCR-django-client-2024.4b130/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OSCR_django_client"
-version = "v2024.3b040"
+version = "v2024.4b130"
 description = "OSCR API"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "OSCR API"]
 include = ["OSCR_django_client/py.typed"]
```

### Comparing `OSCR-django-client-2024.3b40/setup.py` & `OSCR-django-client-2024.4b130/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "OSCR-django-client"
-VERSION = "v2024.3b040"
+VERSION = "v2024.4b130"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `OSCR-django-client-2024.3b40/test/test_combat_log.py` & `OSCR-django-client-2024.4b130/test/test_combat_log.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/test/test_combat_log_upload_response.py` & `OSCR-django-client-2024.4b130/test/test_combat_log_upload_response.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/test/test_combatlog_api.py` & `OSCR-django-client-2024.4b130/test/test_combatlog_api.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/test/test_combatlog_list200_response.py` & `OSCR-django-client-2024.4b130/test/test_combatlog_list200_response.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/test/test_ladder.py` & `OSCR-django-client-2024.4b130/test/test_ladder.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,24 +32,28 @@
             optional params are included """
         # uncomment below to create an instance of `Ladder`
         """
         model = Ladder()
         if include_optional:
             return Ladder(
                 id = 56,
+                variant_name = '',
                 name = '0',
                 difficulty = '0',
+                is_solo = True,
+                is_space = True,
                 metric = '0',
-                is_solo = True
+                variant = ''
             )
         else:
             return Ladder(
                 name = '0',
                 difficulty = '0',
                 metric = '0',
+                variant = '',
         )
         """
 
     def testLadder(self):
         """Test Ladder"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `OSCR-django-client-2024.3b40/test/test_ladder_api.py` & `OSCR-django-client-2024.4b130/test/test_ladder_api.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/test/test_ladder_entries_api.py` & `OSCR-django-client-2024.4b130/test/test_ladder_entries_api.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/test/test_ladder_entries_list200_response.py` & `OSCR-django-client-2024.4b130/test/test_ladder_entries_list200_response.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/test/test_ladder_entry.py` & `OSCR-django-client-2024.4b130/test/test_ladder_entry.py`

 * *Files identical despite different names*

### Comparing `OSCR-django-client-2024.3b40/test/test_ladder_list200_response.py` & `OSCR-django-client-2024.4b130/test/test_ladder_list200_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,30 +37,36 @@
             return LadderList200Response(
                 count = 56,
                 next = '',
                 previous = '',
                 results = [
                     OSCR_django_client.models.ladder.Ladder(
                         id = 56, 
+                        variant_name = '', 
                         name = '0', 
                         difficulty = '0', 
+                        is_solo = True, 
+                        is_space = True, 
                         metric = '0', 
-                        is_solo = True, )
+                        variant = '', )
                     ]
             )
         else:
             return LadderList200Response(
                 count = 56,
                 results = [
                     OSCR_django_client.models.ladder.Ladder(
                         id = 56, 
+                        variant_name = '', 
                         name = '0', 
                         difficulty = '0', 
+                        is_solo = True, 
+                        is_space = True, 
                         metric = '0', 
-                        is_solo = True, )
+                        variant = '', )
                     ],
         )
         """
 
     def testLadderList200Response(self):
         """Test LadderList200Response"""
         # inst_req_only = self.make_instance(include_optional=False)
```

### Comparing `OSCR-django-client-2024.3b40/test/test_metadata.py` & `OSCR-django-client-2024.4b130/test/test_metadata.py`

 * *Files identical despite different names*

