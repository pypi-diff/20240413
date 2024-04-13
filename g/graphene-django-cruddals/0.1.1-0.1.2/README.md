# Comparing `tmp/graphene_django_cruddals-0.1.1.tar.gz` & `tmp/graphene_django_cruddals-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_cruddals-0.1.1.tar", last modified: Sun Mar 31 01:56:38 2024, max compression
+gzip compressed data, was "graphene_django_cruddals-0.1.2.tar", last modified: Sat Apr 13 10:16:19 2024, max compression
```

## Comparing `graphene_django_cruddals-0.1.1.tar` & `graphene_django_cruddals-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-31 01:56:38.385375 graphene_django_cruddals-0.1.1/
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1093 2024-03-21 23:39:20.000000 graphene_django_cruddals-0.1.1/LICENSE
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       26 2024-03-28 10:52:13.000000 graphene_django_cruddals-0.1.1/MANIFEST.in
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     2439 2024-03-31 01:56:38.385375 graphene_django_cruddals-0.1.1/PKG-INFO
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1399 2024-03-28 12:17:14.000000 graphene_django_cruddals-0.1.1/README.md
-drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-31 01:56:38.381375 graphene_django_cruddals-0.1.1/graphene_django_cruddals/
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)      205 2024-03-31 01:55:04.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/__init__.py
-drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-31 01:56:38.381375 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/__init__.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     6441 2024-03-30 17:18:48.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/django_types.py
-drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-31 01:56:38.381375 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_entity/
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_entity/__init__.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     8086 2024-03-24 11:24:54.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_entity/main.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    11339 2024-03-24 13:17:53.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_entity/utils.py
-drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-31 01:56:38.385375 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/__init__.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)      724 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/compat.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    10612 2024-03-31 01:51:19.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/converter_filter_input.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    27898 2024-03-24 13:18:31.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/converter_input.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     5735 2024-03-21 23:30:04.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/converter_order_by_input.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    15519 2024-03-24 12:46:27.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/converter_output.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     3423 2024-03-24 12:58:48.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/main.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     6540 2024-03-31 01:21:28.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/utils.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    68415 2024-03-27 17:08:34.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/main.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     3879 2024-03-21 23:30:04.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/registry_global.py
-drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-31 01:56:38.385375 graphene_django_cruddals-0.1.1/graphene_django_cruddals/scalars_type/
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    10907 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/scalars_type/__init__.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     8515 2024-03-27 17:07:44.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/types.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     6610 2024-03-30 16:48:42.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/utils.py
-drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-31 01:56:38.385375 graphene_django_cruddals-0.1.1/graphene_django_cruddals/views/
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/views/__init__.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     2652 2024-03-21 23:30:04.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/views/cruddals_views.py
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     2822 2024-03-28 21:37:31.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals/views/file_upload_graphql_view.py
-drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-31 01:56:38.381375 graphene_django_cruddals-0.1.1/graphene_django_cruddals.egg-info/
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     2439 2024-03-31 01:56:38.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals.egg-info/PKG-INFO
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1485 2024-03-31 01:56:38.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals.egg-info/SOURCES.txt
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        1 2024-03-31 01:56:38.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals.egg-info/dependency_links.txt
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        1 2024-03-31 01:56:38.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals.egg-info/not-zip-safe
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       57 2024-03-31 01:56:38.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals.egg-info/requires.txt
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       25 2024-03-31 01:56:38.000000 graphene_django_cruddals-0.1.1/graphene_django_cruddals.egg-info/top_level.txt
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       38 2024-03-31 01:56:38.385375 graphene_django_cruddals-0.1.1/setup.cfg
--rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1789 2024-03-28 13:22:14.000000 graphene_django_cruddals-0.1.1/setup.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.585225 graphene_django_cruddals-0.1.2/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)      602 2024-04-13 10:09:26.000000 graphene_django_cruddals-0.1.2/LICENSE
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       26 2024-03-28 10:52:13.000000 graphene_django_cruddals-0.1.2/MANIFEST.in
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    18903 2024-04-13 10:16:19.581223 graphene_django_cruddals-0.1.2/PKG-INFO
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    17863 2024-04-08 15:16:49.000000 graphene_django_cruddals-0.1.2/README.md
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.577222 graphene_django_cruddals-0.1.2/graphene_django_cruddals/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)      205 2024-04-13 10:09:51.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/__init__.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.577222 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     6441 2024-03-30 17:18:48.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/django_types.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.581223 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_entity/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_entity/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     8086 2024-04-08 13:50:09.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_entity/main.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    11339 2024-03-24 13:17:53.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_entity/utils.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.581223 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)      724 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/compat.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    10612 2024-03-31 01:51:19.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/converter_filter_input.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    27898 2024-03-24 13:18:31.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/converter_input.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     5735 2024-03-21 23:30:04.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/converter_order_by_input.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    15519 2024-03-24 12:46:27.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/converter_output.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     3423 2024-03-24 12:58:48.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/main.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     6793 2024-04-08 13:50:09.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/utils.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    68493 2024-03-31 14:08:08.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/main.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.581223 graphene_django_cruddals-0.1.2/graphene_django_cruddals/operations_fields/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:07:50.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/operations_fields/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     9465 2024-03-30 17:12:56.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/operations_fields/default_resolvers.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     7974 2024-03-21 23:30:04.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/operations_fields/main.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    25094 2024-03-30 20:06:08.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/operations_fields/utils.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     3879 2024-03-21 23:30:04.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/registry_global.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.581223 graphene_django_cruddals-0.1.2/graphene_django_cruddals/scalars_type/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    10929 2024-03-31 10:29:18.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/scalars_type/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     8515 2024-03-27 17:07:44.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/types.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     6610 2024-03-30 16:48:42.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/utils.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.581223 graphene_django_cruddals-0.1.2/graphene_django_cruddals/utils_for_client/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:07:55.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/utils_for_client/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    26859 2024-03-30 17:16:06.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/utils_for_client/build_for_client.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.581223 graphene_django_cruddals-0.1.2/graphene_django_cruddals/views/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-03-18 15:02:24.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/views/__init__.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     2652 2024-03-21 23:30:04.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/views/cruddals_views.py
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     2822 2024-03-28 21:37:31.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals/views/file_upload_graphql_view.py
+drwxrwxr-x   0 juanjcardona13  (1000) juanjcardona13  (1000)        0 2024-04-13 10:16:19.577222 graphene_django_cruddals-0.1.2/graphene_django_cruddals.egg-info/
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)    18903 2024-04-13 10:16:19.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals.egg-info/PKG-INFO
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1823 2024-04-13 10:16:19.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        1 2024-04-13 10:16:19.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)        1 2024-04-13 10:16:19.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals.egg-info/not-zip-safe
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       57 2024-04-13 10:16:19.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals.egg-info/requires.txt
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       25 2024-04-13 10:16:19.000000 graphene_django_cruddals-0.1.2/graphene_django_cruddals.egg-info/top_level.txt
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)       38 2024-04-13 10:16:19.585225 graphene_django_cruddals-0.1.2/setup.cfg
+-rw-rw-r--   0 juanjcardona13  (1000) juanjcardona13  (1000)     1789 2024-03-28 13:22:14.000000 graphene_django_cruddals-0.1.2/setup.py
```

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/django_types.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/django_types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_entity/main.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_entity/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,21 +114,21 @@
 def convert_django_model_to_filter_input_object_type( model: DjangoModel, registry: RegistryGlobal, meta_attrs={}, extra_attrs={} ):
     names_of_model = get_name_of_model_in_different_case(model)
     singular_camel_case_name = names_of_model["camel_case"]
     if exists_conversion_for_model(model, registry, TypeRegistryForModelEnum.INPUT_OBJECT_TYPE_FOR_SEARCH.value):
         return get_converted_model(model, registry, TypeRegistryForModelEnum.INPUT_OBJECT_TYPE_FOR_SEARCH.value)
     attr_input_fields = get_input_fields_for_filter( model, registry, meta_attrs=meta_attrs )
     attr_input_fields.update( { "AND": graphene.Dynamic( lambda: graphene.InputField( graphene.List( convert_django_model_to_filter_input_object_type( model, registry ) ) ) ), "OR": graphene.Dynamic( lambda: graphene.InputField( graphene.List( convert_django_model_to_filter_input_object_type( model, registry ) ) ) ), "NOT": graphene.Dynamic( lambda: graphene.InputField( convert_django_model_to_filter_input_object_type(model, registry) ) ), } )
-    ModelInputObjectType = build_class( name=f"{singular_camel_case_name}FilterInput", bases=(graphene.InputObjectType,), attrs={**attr_input_fields, **extra_attrs}, )
+    ModelInputObjectType = build_class( name=f"Filter{singular_camel_case_name}Input", bases=(graphene.InputObjectType,), attrs={**attr_input_fields, **extra_attrs}, )
     registry.register_model(model, TypeRegistryForModelEnum.INPUT_OBJECT_TYPE_FOR_SEARCH.value, ModelInputObjectType)
     return ModelInputObjectType
 
 
 def convert_django_model_to_order_by_input_object_type( model: DjangoModel, registry: RegistryGlobal, meta_attrs={}, extra_attrs={} ):
     names_of_model = get_name_of_model_in_different_case(model)
     singular_camel_case_name = names_of_model["camel_case"]
     if exists_conversion_for_model(model, registry, TypeRegistryForModelEnum.INPUT_OBJECT_TYPE_FOR_ORDER_BY.value):
         return get_converted_model(model, registry, TypeRegistryForModelEnum.INPUT_OBJECT_TYPE_FOR_ORDER_BY.value)
     attr_input_fields = get_input_fields_for_order_by( model, registry, meta_attrs=meta_attrs )
-    ModelInputObjectType = build_class( name=f"{singular_camel_case_name}OrderByInput", bases=(graphene.InputObjectType,), attrs={**attr_input_fields, **extra_attrs}, )
+    ModelInputObjectType = build_class( name=f"OrderBy{singular_camel_case_name}Input", bases=(graphene.InputObjectType,), attrs={**attr_input_fields, **extra_attrs}, )
     registry.register_model( model, TypeRegistryForModelEnum.INPUT_OBJECT_TYPE_FOR_ORDER_BY.value, ModelInputObjectType )
     return ModelInputObjectType
```

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_entity/utils.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_entity/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/compat.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/compat.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/converter_filter_input.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/converter_filter_input.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/converter_input.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/converter_input.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/converter_order_by_input.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/converter_order_by_input.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/converter_output.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/converter_output.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/main.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/main.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/converters/for_fields/utils.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/converters/for_fields/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from graphql import Undefined
 from django.utils.functional import Promise
 from django.db import models
 from graphene_django_cruddals.registry_global import RegistryGlobal
 from graphene_django.settings import graphene_settings
 from django.db.models import Field as DjangoField
 from django.db.models.fields import NOT_PROVIDED
+from django.db.models.enums import ChoicesMeta
 
 from graphene_django_cruddals.types import TypeRegistryForField, TypesMutation, TypesMutationEnum
 
 
 # region === CONVERTER FOR FIELD WITH CHOICES
 class BlankValueField(graphene.Field):
     def wrap_resolve(self, parent_resolver):
@@ -58,14 +59,16 @@
     return name
 
 
 def get_choices(choices):
     converted_names = []
     if isinstance(choices, OrderedDict):
         choices = choices.items()
+    elif isinstance(choices, ChoicesMeta):
+        choices = choices.choices # This is for the case of a Django Enum
     for value, help_text in choices:
         if isinstance(help_text, (tuple, list)):
             yield from get_choices(help_text)
         else:
             name = convert_choice_name(value)
             while name in converted_names:
                 name += "_" + str(len(converted_names))
@@ -143,21 +146,24 @@
             default = getattr(field, "default", None)
             if default is None:
                 default = NOT_PROVIDED
             return not null and default == NOT_PROVIDED
         except AttributeError:
             return False
 
+
 def django_field_get_default(field: DjangoField):
     if field.default == models.fields.NOT_PROVIDED:
         return Undefined
     if callable(field.default):
         return Undefined
     if isinstance(field.default, Promise):
         return Undefined
+    if isinstance(type(field.default), ChoicesMeta):
+        return field.default.value
     return field.default
 
 
 def exists_conversion_for_field( field:DjangoField, registry: RegistryGlobal, type_of_registry: TypeRegistryForField ) -> bool:
     registries_for_field = registry.get_registry_for_field(field)
     if registries_for_field is not None and type_of_registry in registries_for_field:
         return True
```

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/main.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -995,17 +995,17 @@
     This class provides methods to dynamically create GraphQL schemas for Django models,
     along with query and mutation operation fields.
 
     Attributes:
         Query (Type[graphene.ObjectType]): The GraphQL Query object for the model.
         Mutation (Union[Type[graphene.ObjectType], None]): The GraphQL Mutation object for the model.
         schema (graphene.Schema): The GraphQL schema for the model.
-        query_operation_fields (Dict[str, Union[graphene.Field, DjangoReadField, DjangoListField, DjangoSearchField]]):
+        operation_fields_for_queries (Dict[str, Union[graphene.Field, DjangoReadField, DjangoListField, DjangoSearchField]]):
             The query operation fields for the model.
-        mutation_operation_fields (Union[Dict[str, Union[graphene.Field, DjangoCreateUpdateField, DjangoDeleteField,
+        operation_fields_for_mutations (Union[Dict[str, Union[graphene.Field, DjangoCreateUpdateField, DjangoDeleteField,
             DjangoDeactivateField, DjangoActivateField]], None]): The mutation operation fields for the model.
         meta (BuilderCruddalsModel): An instance of BuilderCruddalsModel containing metadata about the model.
 
     Methods:
         __init_subclass_with_meta__: Initialize the subclass with meta settings and dynamically create GraphQL schemas.
         _initialize_attributes: Initialize attributes to None.
         _build_cruddals_model: Build the CruddalsModel using BuilderCruddalsModel.
@@ -1013,16 +1013,16 @@
         _build_schema_query_mutation: Build the schema, Query, and Mutation objects.
 
     """
 
     Query:Type[graphene.ObjectType]
     Mutation:Union[Type[graphene.ObjectType], None] = None
     schema:graphene.Schema
-    query_operation_fields:Dict[str, graphene.Field | DjangoReadField | DjangoListField | DjangoSearchField]
-    mutation_operation_fields:Union[Dict[str, graphene.Field | DjangoCreateUpdateField | DjangoDeleteField | DjangoDeactivateField | DjangoActivateField ], None] = None
+    operation_fields_for_queries:Dict[str, graphene.Field | DjangoReadField | DjangoListField | DjangoSearchField]
+    operation_fields_for_mutations:Union[Dict[str, graphene.Field | DjangoCreateUpdateField | DjangoDeleteField | DjangoDeactivateField | DjangoActivateField ], None] = None
     meta:BuilderCruddalsModel
 
     @classmethod
     def __init_subclass_with_meta__(
         cls,
         model:Union[DjangoModel, None]=None,
         prefix:str="",
@@ -1064,15 +1064,15 @@
         super(CruddalsModel, cls).__init_subclass_with_meta__(**kwargs)
 
     @classmethod
     def _initialize_attributes(cls):
         """
         Initialize attributes to None for the child class.
         """
-        attrs_for_child = [ "Query", "Mutation", "schema", "query_operation_fields", "mutation_operation_fields", "meta", ]
+        attrs_for_child = [ "Query", "Mutation", "schema", "operation_fields_for_queries", "operation_fields_for_mutations", "meta", ]
         [setattr(cls, attr, None) for attr in attrs_for_child]
 
     @classmethod
     def _build_cruddals_model(cls, model, prefix, suffix, interfaces, exclude_interfaces, registry):
         """
         Build the CruddalsModel using BuilderCruddalsModel.
 
@@ -1109,46 +1109,46 @@
             "update",
             "activate",
             "deactivate",
             "delete",
         )
         final_functions = ( functions if functions else tuple( set(functions_type_query + functions_type_mutation) - set(exclude_functions) ) )
 
-        cls.query_operation_fields = {}
-        cls.mutation_operation_fields = {}
+        cls.operation_fields_for_queries = {}
+        cls.operation_fields_for_mutations = {}
 
         for function in final_functions:
             key = f"{function}_{cls.meta.model_name_in_different_case['plural_snake_case']}"
             if function == "read":
                 key = f"{function}_{cls.meta.model_name_in_different_case['snake_case']}"
             attr_field:Dict[str, graphene.Field] = {key: getattr(cls.meta, f"{function}_field")}
             if function in functions_type_query:
-                cls.query_operation_fields.update(attr_field)
+                cls.operation_fields_for_queries.update(attr_field)
             elif function in functions_type_mutation:
-                cls.mutation_operation_fields.update(attr_field)
+                cls.operation_fields_for_mutations.update(attr_field)
 
-        if not cls.query_operation_fields:
-            cls.query_operation_fields.update(
+        if not cls.operation_fields_for_queries:
+            cls.operation_fields_for_queries.update(
                 {
                     f"read_{cls.meta.model_name_in_different_case['snake_case']}": getattr(
                         cls.meta, "read_field"
                     )
                 }
             )
 
     @classmethod
     def _build_schema_query_mutation(cls):
         """
         Build the schema, Query, and Mutation objects.
         """
         cls.schema, cls.Query, cls.Mutation = get_schema_query_mutation( 
             (), 
-            cls.query_operation_fields, 
+            cls.operation_fields_for_queries, 
             (), 
-            cls.mutation_operation_fields 
+            cls.operation_fields_for_mutations 
         )
 
 
 class BuilderCruddalsApp:
     app_name = None
     app_config = None
     models = None
```

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/registry_global.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/registry_global.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/scalars_type/__init__.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/scalars_type/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,12 +311,12 @@
             raise Exception(f"Expected a timedelta object, but got {repr(dt)}")
 
     @staticmethod
     def parse_literal(node):
         if isinstance(node, graphene.IntValue):
             return timedelta(seconds=node.value)
         else:
-            raise Exception(f"Cannot represent {node} as timedelta.")
+            raise Exception(f"Cannot represent {node} as timedelta. Should be an integer.")
 
     @staticmethod
     def parse_value(value):
         return timedelta(seconds=value)
```

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/types.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/utils.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/views/cruddals_views.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/views/cruddals_views.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals/views/file_upload_graphql_view.py` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals/views/file_upload_graphql_view.py`

 * *Files identical despite different names*

### Comparing `graphene_django_cruddals-0.1.1/graphene_django_cruddals.egg-info/SOURCES.txt` & `graphene_django_cruddals-0.1.2/graphene_django_cruddals.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -22,11 +22,17 @@
 graphene_django_cruddals/converters/for_fields/compat.py
 graphene_django_cruddals/converters/for_fields/converter_filter_input.py
 graphene_django_cruddals/converters/for_fields/converter_input.py
 graphene_django_cruddals/converters/for_fields/converter_order_by_input.py
 graphene_django_cruddals/converters/for_fields/converter_output.py
 graphene_django_cruddals/converters/for_fields/main.py
 graphene_django_cruddals/converters/for_fields/utils.py
+graphene_django_cruddals/operations_fields/__init__.py
+graphene_django_cruddals/operations_fields/default_resolvers.py
+graphene_django_cruddals/operations_fields/main.py
+graphene_django_cruddals/operations_fields/utils.py
 graphene_django_cruddals/scalars_type/__init__.py
+graphene_django_cruddals/utils_for_client/__init__.py
+graphene_django_cruddals/utils_for_client/build_for_client.py
 graphene_django_cruddals/views/__init__.py
 graphene_django_cruddals/views/cruddals_views.py
 graphene_django_cruddals/views/file_upload_graphql_view.py
```

### Comparing `graphene_django_cruddals-0.1.1/setup.py` & `graphene_django_cruddals-0.1.2/setup.py`

 * *Files identical despite different names*

