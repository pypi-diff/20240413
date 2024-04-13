# Comparing `tmp/panther-4.1.3.tar.gz` & `tmp/panther-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-4.1.3.tar", last modified: Thu Apr 11 01:05:43 2024, max compression
+gzip compressed data, was "panther-4.2.0.tar", last modified: Sat Apr 13 16:21:00 2024, max compression
```

## Comparing `panther-4.1.3.tar` & `panther-4.2.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.828752 panther-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-11 01:05:31.000000 panther-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-11 01:05:43.828752 panther-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-11 01:05:31.000000 panther-4.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.816752 panther-4.1.3/panther/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-11 01:05:31.000000 panther-4.1.3/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-11 01:05:31.000000 panther-4.1.3/panther/_load_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-11 01:05:31.000000 panther-4.1.3/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-11 01:05:31.000000 panther-4.1.3/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-11 01:05:31.000000 panther-4.1.3/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-11 01:05:31.000000 panther-4.1.3/panther/background_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-11 01:05:31.000000 panther-4.1.3/panther/base_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-11 01:05:31.000000 panther-4.1.3/panther/base_websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-11 01:05:31.000000 panther-4.1.3/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.820752 panther-4.1.3/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-11 01:05:31.000000 panther-4.1.3/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-11 01:05:31.000000 panther-4.1.3/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.820752 panther-4.1.3/panther/db/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.820752 panther-4.1.3/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/base_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-11 01:05:31.000000 panther-4.1.3/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-11 01:05:31.000000 panther-4.1.3/panther/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-11 01:05:31.000000 panther-4.1.3/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-11 01:05:31.000000 panther-4.1.3/panther/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-11 01:05:31.000000 panther-4.1.3/panther/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-11 01:05:31.000000 panther-4.1.3/panther/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-11 01:05:31.000000 panther-4.1.3/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.824752 panther-4.1.3/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 01:05:31.000000 panther-4.1.3/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-11 01:05:31.000000 panther-4.1.3/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-11 01:05:31.000000 panther-4.1.3/panther/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-11 01:05:31.000000 panther-4.1.3/panther/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.824752 panther-4.1.3/panther/panel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:31.000000 panther-4.1.3/panther/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-11 01:05:31.000000 panther-4.1.3/panther/panel/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-11 01:05:31.000000 panther-4.1.3/panther/panel/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 01:05:31.000000 panther-4.1.3/panther/panel/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-11 01:05:31.000000 panther-4.1.3/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-11 01:05:31.000000 panther-4.1.3/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-11 01:05:31.000000 panther-4.1.3/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-11 01:05:31.000000 panther-4.1.3/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9096 2024-04-11 01:05:31.000000 panther-4.1.3/panther/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-11 01:05:31.000000 panther-4.1.3/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-11 01:05:31.000000 panther-4.1.3/panther/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-11 01:05:31.000000 panther-4.1.3/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-11 01:05:31.000000 panther-4.1.3/panther/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-11 01:05:31.000000 panther-4.1.3/panther/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.828752 panther-4.1.3/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 01:05:43.000000 panther-4.1.3/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 01:05:31.000000 panther-4.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:05:43.828752 panther-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-11 01:05:31.000000 panther-4.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:05:43.824752 panther-4.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_background_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15572 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_multipart.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_panel_apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_throttling.py
--rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-11 01:05:31.000000 panther-4.1.3/tests/test_websockets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.673551 panther-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-13 16:20:52.000000 panther-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-13 16:21:00.673551 panther-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-13 16:20:52.000000 panther-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.665551 panther-4.2.0/panther/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-13 16:20:52.000000 panther-4.2.0/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-13 16:20:52.000000 panther-4.2.0/panther/_load_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-13 16:20:52.000000 panther-4.2.0/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-13 16:20:52.000000 panther-4.2.0/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-13 16:20:52.000000 panther-4.2.0/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-13 16:20:52.000000 panther-4.2.0/panther/background_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-13 16:20:52.000000 panther-4.2.0/panther/base_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-13 16:20:52.000000 panther-4.2.0/panther/base_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-04-13 16:20:52.000000 panther-4.2.0/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.665551 panther-4.2.0/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-13 16:20:52.000000 panther-4.2.0/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-13 16:20:52.000000 panther-4.2.0/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.665551 panther-4.2.0/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.669551 panther-4.2.0/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/base_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-13 16:20:52.000000 panther-4.2.0/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-13 16:20:52.000000 panther-4.2.0/panther/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-13 16:20:52.000000 panther-4.2.0/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-13 16:20:52.000000 panther-4.2.0/panther/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-04-13 16:20:52.000000 panther-4.2.0/panther/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-13 16:20:52.000000 panther-4.2.0/panther/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-13 16:20:52.000000 panther-4.2.0/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.669551 panther-4.2.0/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-13 16:20:52.000000 panther-4.2.0/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-13 16:20:52.000000 panther-4.2.0/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-13 16:20:52.000000 panther-4.2.0/panther/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-13 16:20:52.000000 panther-4.2.0/panther/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.669551 panther-4.2.0/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:20:52.000000 panther-4.2.0/panther/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-13 16:20:52.000000 panther-4.2.0/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-13 16:20:52.000000 panther-4.2.0/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 16:20:52.000000 panther-4.2.0/panther/panel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-13 16:20:52.000000 panther-4.2.0/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-13 16:20:52.000000 panther-4.2.0/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-13 16:20:52.000000 panther-4.2.0/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-13 16:20:52.000000 panther-4.2.0/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9096 2024-04-13 16:20:52.000000 panther-4.2.0/panther/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-13 16:20:52.000000 panther-4.2.0/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-13 16:20:52.000000 panther-4.2.0/panther/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 16:20:52.000000 panther-4.2.0/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-13 16:20:52.000000 panther-4.2.0/panther/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-13 16:20:52.000000 panther-4.2.0/panther/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.673551 panther-4.2.0/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 16:21:00.000000 panther-4.2.0/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 16:20:52.000000 panther-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:21:00.673551 panther-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-13 16:20:52.000000 panther-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:21:00.673551 panther-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_background_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16071 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_panel_apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17425 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30959 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13457 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_throttling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-13 16:20:52.000000 panther-4.2.0/tests/test_websockets.py
```

### Comparing `panther-4.1.3/LICENSE` & `panther-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/PKG-INFO` & `panther-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 4.1.3
+Version: 4.2.0
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: BSD-3-Clause license
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `panther-4.1.3/README.md` & `panther-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/_load_configs.py` & `panther-4.2.0/panther/_load_configs.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/_utils.py` & `panther-4.2.0/panther/_utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/app.py` & `panther-4.2.0/panther/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,18 @@
         self.request: Request | None = None
 
     def __call__(self, func):
         @functools.wraps(func)
         async def wrapper(request: Request) -> Response:
             self.request = request
 
+            # 0. Preflight
+            if self.request.method == 'OPTIONS':
+                return self.options()
+
             # 1. Check Method
             if self.methods and self.request.method not in self.methods:
                 raise MethodNotAllowedAPIError
 
             # 2. Authentication
             await self.handle_authentication()
 
@@ -138,14 +142,22 @@
                 raise AuthorizationAPIError
 
     def handle_input_validation(self):
         if self.input_model:
             self.request.validated_data = self.validate_input(model=self.input_model, request=self.request)
 
     @classmethod
+    def options(cls):
+        headers = {
+            'Access-Control-Allow-Methods': 'DELETE, GET, PATCH, POST, PUT, OPTIONS',
+            'Access-Control-Allow-Headers': 'Accept, Authorization, User-Agent, Content-Type',
+        }
+        return Response(headers=headers)
+
+    @classmethod
     def validate_input(cls, model, request: Request):
         if isinstance(request.data, bytes):
             raise BadRequestAPIError(detail='Content-Type is not valid')
         if request.data is None:
             raise BadRequestAPIError(detail='Request body is required')
         try:
             # `request` will be ignored in regular `BaseModel`
@@ -195,14 +207,16 @@
                 func = self.post
             case 'PUT':
                 func = self.put
             case 'PATCH':
                 func = self.patch
             case 'DELETE':
                 func = self.delete
+            case 'OPTIONS':
+                func = API.options
             case _:
                 raise MethodNotAllowedAPIError
 
         return await API(
             input_model=self.input_model or await self.get_input_model(request=request),
             output_model=self.output_model or await self.get_output_model(request=request),
             auth=self.auth,
```

### Comparing `panther-4.1.3/panther/authentications.py` & `panther-4.2.0/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/background_tasks.py` & `panther-4.2.0/panther/background_tasks.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/base_request.py` & `panther-4.2.0/panther/base_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import namedtuple
 from collections.abc import Callable
+from urllib.parse import parse_qsl
 
 from panther.db import Model
 from panther.exceptions import InvalidPathVariableAPIError
 
 
 class Headers:
     accept: str
@@ -70,19 +71,15 @@
         if self._headers is None:
             self._headers = Headers(self.scope['headers'])
         return self._headers
 
     @property
     def query_params(self) -> dict:
         if self._params is None:
-            self._params = {}
-            if (query_string := self.scope['query_string']) != b'':
-                for param in query_string.decode('utf-8').split('&'):
-                    k, *_, v = param.split('=')
-                    self._params[k] = v
+            self._params = {k: v for k, v in parse_qsl(self.scope['query_string'].decode('utf-8'))}
         return self._params
 
     @property
     def path(self) -> str:
         return self.scope['path']
 
     @property
```

### Comparing `panther-4.1.3/panther/base_websocket.py` & `panther-4.2.0/panther/base_websocket.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/caching.py` & `panther-4.2.0/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/cli/create_command.py` & `panther-4.2.0/panther/cli/create_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             {
                 'field': 'single_file',
                 'message': 'Do You Want To Work With Single File Structure',
                 'is_boolean': True,
             },
             {
                 'field': 'database',
-                'message': '    0: PantherDB (File-Base, No Requirements)\n    1: MongoDB (Required `pymongo`)\n    2: No Database\nChoose Your Database (default is 0)',
+                'message': '    0: PantherDB (File-Base, No Requirements)\n    1: MongoDB (Required `motor`)\n    2: No Database\nChoose Your Database (default is 0)',
                 'validation_func': lambda x: x in ['0', '1', '2'],
                 'error_message': "Invalid Choice, '{}' not in ['0', '1', '2']",
             },
             {
                 'field': 'database_encryption',
                 'message': 'Do You Want Encryption For Your Database (Required `cryptography`)',
                 'is_boolean': True,
```

### Comparing `panther-4.1.3/panther/cli/main.py` & `panther-4.2.0/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/cli/monitor_command.py` & `panther-4.2.0/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/cli/run_command.py` & `panther-4.2.0/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/cli/template.py` & `panther-4.2.0/panther/cli/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 
 SECRET_KEY = env['SECRET_KEY']{DATABASE}{REDIS}{USER_MODEL}{AUTHENTICATION}{MONITORING}{LOG_QUERIES}{AUTO_REFORMAT}
 
 InfoThrottling = Throttling(rate=5, duration=timedelta(minutes=1))
 
 TIMEZONE = 'UTC'
 
+
 @API()
 async def hello_world_api():
     return {'detail': 'Hello World'}
 
 
 @API(cache=True, throttling=InfoThrottling)
 async def info_api(request: Request):
```

### Comparing `panther-4.1.3/panther/cli/utils.py` & `panther-4.2.0/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/configs.py` & `panther-4.2.0/panther/configs.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/db/connections.py` & `panther-4.2.0/panther/db/connections.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/db/cursor.py` & `panther-4.2.0/panther/db/cursor.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/db/models.py` & `panther-4.2.0/panther/db/models.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/db/queries/base_queries.py` & `panther-4.2.0/panther/db/queries/base_queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/db/queries/mongodb_queries.py` & `panther-4.2.0/panther/db/queries/mongodb_queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         cursor = await cls.find(_filter, **kwargs)
         for result in cursor.sort('_id', -1).limit(-1):
             return result
         return None
 
     @classmethod
     async def aggregate(cls, pipeline: Sequence[dict]) -> Iterable[dict]:
-        return await db.session[cls.__name__].aggregate(pipeline)
+        return await db.session[cls.__name__].aggregate(pipeline).to_list(None)
 
     # # # # # Count # # # # #
     @classmethod
     async def count(cls, _filter: dict | None = None, /, **kwargs) -> int:
         return await db.session[cls.__name__].count_documents(cls._merge(_filter, kwargs))
 
     # # # # # Insert # # # # #
```

### Comparing `panther-4.1.3/panther/db/queries/pantherdb_queries.py` & `panther-4.2.0/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/db/queries/queries.py` & `panther-4.2.0/panther/db/queries/queries.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/db/utils.py` & `panther-4.2.0/panther/db/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,9 +50,9 @@
 
 def _convert_to_object_id(_id):
     if isinstance(_id, bson.ObjectId):
         return _id
     try:
         return bson.ObjectId(_id)
     except bson.objectid.InvalidId:
-        msg = f'id={_id} is invalid bson.ObjectId'
-        raise bson.errors.InvalidId(msg)
+        logger.warning(f'id={_id} is not a valid bson.ObjectId')
+        return None
```

### Comparing `panther-4.1.3/panther/events.py` & `panther-4.2.0/panther/events.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/exceptions.py` & `panther-4.2.0/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/file_handler.py` & `panther-4.2.0/panther/file_handler.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/generics.py` & `panther-4.2.0/panther/generics.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/logging.py` & `panther-4.2.0/panther/logging.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/main.py` & `panther-4.2.0/panther/main.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/middlewares/base.py` & `panther-4.2.0/panther/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/monitoring.py` & `panther-4.2.0/panther/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/pagination.py` & `panther-4.2.0/panther/pagination.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/panel/apis.py` & `panther-4.2.0/panther/panel/apis.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/request.py` & `panther-4.2.0/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/response.py` & `panther-4.2.0/panther/response.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/routings.py` & `panther-4.2.0/panther/routings.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/serializer.py` & `panther-4.2.0/panther/serializer.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/status.py` & `panther-4.2.0/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/test.py` & `panther-4.2.0/panther/test.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/utils.py` & `panther-4.2.0/panther/utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther/websocket.py` & `panther-4.2.0/panther/websocket.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/panther.egg-info/PKG-INFO` & `panther-4.2.0/panther.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 4.1.3
+Version: 4.2.0
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: BSD-3-Clause license
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `panther-4.1.3/panther.egg-info/SOURCES.txt` & `panther-4.2.0/panther.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/setup.py` & `panther-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_authentication.py` & `panther-4.2.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_background_tasks.py` & `panther-4.2.0/tests/test_background_tasks.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_caching.py` & `panther-4.2.0/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_cli.py` & `panther-4.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_database.py` & `panther-4.2.0/tests/test_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,29 @@
         else:
             assert isinstance(books, PantherDBCursor)
 
         assert _len == insert_count
         for book in books:
             assert isinstance(book, Book)
 
+    async def test_aggregation(self):
+        # Insert Many
+        insert_count = await self._insert_many()
+
+        # Find All with aggregate
+        books = await Book.aggregate([])
+        _len = sum(1 for _ in books)
+
+        assert isinstance(books, list)
+
+        assert _len == insert_count
+        for book in books:
+            assert isinstance(book, dict)
+            assert {*book.keys()} == {'_id', 'name', 'author', 'pages_count'}
+
     # # # Count
     async def test_count_all(self):
         # Insert Many
         insert_count = await self._insert_many()
 
         # Count All
         books_count = await Book.count()
@@ -498,14 +513,17 @@
             },
         }
         Panther(__name__, configs=__name__, urls={})
 
     def tearDown(self) -> None:
         Path(self.DB_PATH).unlink()
 
+    async def test_aggregation(self):
+        pass
+
 
 @pytest.mark.mongodb
 class TestMongoDB(_BaseDatabaseTestCase, IsolatedAsyncioTestCase):
     DB_NAME = 'test.pdb'
 
     @classmethod
     def setUpClass(cls) -> None:
```

### Comparing `panther-4.1.3/tests/test_events.py` & `panther-4.2.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_generics.py` & `panther-4.2.0/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_multipart.py` & `panther-4.2.0/tests/test_multipart.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_panel_apis.py` & `panther-4.2.0/tests/test_panel_apis.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_request.py` & `panther-4.2.0/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_response.py` & `panther-4.2.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_routing.py` & `panther-4.2.0/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_run.py` & `panther-4.2.0/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_serializer.py` & `panther-4.2.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_status.py` & `panther-4.2.0/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_throttling.py` & `panther-4.2.0/tests/test_throttling.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_utils.py` & `panther-4.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `panther-4.1.3/tests/test_websockets.py` & `panther-4.2.0/tests/test_websockets.py`

 * *Files identical despite different names*

