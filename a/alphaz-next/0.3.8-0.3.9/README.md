# Comparing `tmp/alphaz-next-0.3.8.tar.gz` & `tmp/alphaz-next-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphaz-next-0.3.8.tar", last modified: Wed Feb  7 09:59:06 2024, max compression
+gzip compressed data, was "alphaz-next-0.3.9.tar", last modified: Wed Feb  7 10:25:40 2024, max compression
```

## Comparing `alphaz-next-0.3.8.tar` & `alphaz-next-0.3.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.169696 alphaz-next-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-07 09:59:06.169696 alphaz-next-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/asyncio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/exception_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/core/responses/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/html_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/json_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/orjson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/plaintext_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/redirect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/streaming_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/responses/ujson_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/core/uvicorn_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/libs/file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/libs/httpx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/models/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/auth/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/models/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/models/config/_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/_base/internal_config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/alpha_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/api_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/apm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/config_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/database_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/models/config/openapi_config_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.169696 alphaz-next-0.3.8/alphaz_next/tests/utils/mocking/
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/tests/utils/mocking/mock_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/tests/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.169696 alphaz-next-0.3.8/alphaz_next/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-07 09:59:01.000000 alphaz-next-0.3.8/alphaz_next/utils/logging_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:59:06.165696 alphaz-next-0.3.8/alphaz_next.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-07 09:59:06.000000 alphaz-next-0.3.8/alphaz_next.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-07 09:59:06.000000 alphaz-next-0.3.8/alphaz_next.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 09:59:06.000000 alphaz-next-0.3.8/alphaz_next.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-07 09:59:06.000000 alphaz-next-0.3.8/alphaz_next.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-07 09:59:06.000000 alphaz-next-0.3.8/alphaz_next.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 09:59:06.169696 alphaz-next-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-07 09:59:04.000000 alphaz-next-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/asyncio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/exception_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/core/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/html_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/orjson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/plaintext_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/redirect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/streaming_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/responses/ujson_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/core/uvicorn_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/libs/file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/libs/httpx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/models/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/auth/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/models/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/models/config/_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/_base/internal_config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/alpha_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/api_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/apm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/config_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/database_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/models/config/openapi_config_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/tests/utils/mocking/
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/tests/utils/mocking/mock_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/tests/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/alphaz_next/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11706 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-07 10:25:35.000000 alphaz-next-0.3.9/alphaz_next/utils/logging_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:25:40.347790 alphaz-next-0.3.9/alphaz_next.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-07 10:25:40.000000 alphaz-next-0.3.9/alphaz_next.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 10:25:40.351790 alphaz-next-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-07 10:25:38.000000 alphaz-next-0.3.9/setup.py
```

### Comparing `alphaz-next-0.3.8/PKG-INFO` & `alphaz-next-0.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.3.8
+Version: 0.3.9
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.3.8.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.3.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,10 +24,10 @@
 ```
 
 ## How to import alphaz-next
 
 To access alphaz-next and its functions import it in your Python code like this:
 
 ```
-from alphaz-next import AlphaDatabase, AlphaLogger
+from alphaz-next import DataBase, Logger
 from alphaz-next.models.config.config_settings import create_config_settings
 ```
```

### Comparing `alphaz-next-0.3.8/README.md` & `alphaz-next-0.3.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 ```
 
 ## How to import alphaz-next
 
 To access alphaz-next and its functions import it in your Python code like this:
 
 ```
-from alphaz-next import AlphaDatabase, AlphaLogger
+from alphaz-next import DataBase, Logger
 from alphaz-next.models.config.config_settings import create_config_settings
 ```
```

### Comparing `alphaz-next-0.3.8/alphaz_next/auth/auth.py` & `alphaz-next-0.3.9/alphaz_next/auth/auth.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/_base.py` & `alphaz-next-0.3.9/alphaz_next/core/_base.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/application.py` & `alphaz-next-0.3.9/alphaz_next/core/application.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/exception_handlers.py` & `alphaz-next-0.3.9/alphaz_next/core/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/exceptions.py` & `alphaz-next-0.3.9/alphaz_next/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/middleware.py` & `alphaz-next-0.3.9/alphaz_next/core/middleware.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/__init__.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/file_response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/html_response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/html_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/json_response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/json_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/orjson_response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/orjson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/plaintext_response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/plaintext_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/redirect_response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/redirect_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/streaming_response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/streaming_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/core/responses/ujson_response.py` & `alphaz-next-0.3.9/alphaz_next/core/responses/ujson_response.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/libs/httpx.py` & `alphaz-next-0.3.9/alphaz_next/libs/httpx.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/auth/user.py` & `alphaz-next-0.3.9/alphaz_next/models/auth/user.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/_base/internal_config_settings.py` & `alphaz-next-0.3.9/alphaz_next/models/config/_base/internal_config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/_base/utils.py` & `alphaz-next-0.3.9/alphaz_next/models/config/_base/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/alpha_config.py` & `alphaz-next-0.3.9/alphaz_next/models/config/alpha_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/api_config.py` & `alphaz-next-0.3.9/alphaz_next/models/config/api_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/apm_config.py` & `alphaz-next-0.3.9/alphaz_next/models/config/apm_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/config_settings.py` & `alphaz-next-0.3.9/alphaz_next/models/config/config_settings.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/database_config.py` & `alphaz-next-0.3.9/alphaz_next/models/config/database_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/logging_config.py` & `alphaz-next-0.3.9/alphaz_next/models/config/logging_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/models/config/openapi_config_schema.py` & `alphaz-next-0.3.9/alphaz_next/models/config/openapi_config_schema.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/tests/utils/mocking/mock_user.py` & `alphaz-next-0.3.9/alphaz_next/tests/utils/mocking/mock_user.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/tests/utils/utils.py` & `alphaz-next-0.3.9/alphaz_next/tests/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/utils/format.py` & `alphaz-next-0.3.9/alphaz_next/utils/format.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/utils/logger.py` & `alphaz-next-0.3.9/alphaz_next/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next/utils/logging_filters.py` & `alphaz-next-0.3.9/alphaz_next/utils/logging_filters.py`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/alphaz_next.egg-info/PKG-INFO` & `alphaz-next-0.3.9/alphaz_next.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz-next
-Version: 0.3.8
+Version: 0.3.9
 Summary: A project to make a lib to start FASTAPI quickly
 Home-page: https://github.com/STDef200mm/alphaz-next
-Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.3.8.tar.gz
+Download-URL: https://github.com/STDef200mm/alphaz-next/archive/refs/tags/0.3.9.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -24,10 +24,10 @@
 ```
 
 ## How to import alphaz-next
 
 To access alphaz-next and its functions import it in your Python code like this:
 
 ```
-from alphaz-next import AlphaDatabase, AlphaLogger
+from alphaz-next import DataBase, Logger
 from alphaz-next.models.config.config_settings import create_config_settings
 ```
```

### Comparing `alphaz-next-0.3.8/alphaz_next.egg-info/SOURCES.txt` & `alphaz-next-0.3.9/alphaz_next.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-next-0.3.8/setup.py` & `alphaz-next-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.8"
+version = "0.3.9"
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="alphaz-next",
     version=version,
```

