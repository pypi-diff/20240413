# Comparing `tmp/simo-zwave-1.0.6.tar.gz` & `tmp/simo_zwave-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simo-zwave-1.0.6.tar", last modified: Sun Jan 21 07:05:25 2024, max compression
+gzip compressed data, was "simo_zwave-1.0.7.tar", last modified: Sat Apr 13 15:10:11 2024, max compression
```

## Comparing `simo-zwave-1.0.6.tar` & `simo_zwave-1.0.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.066583 simo-zwave-1.0.6/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)    34916 2021-12-07 14:40:19.000000 simo-zwave-1.0.6/LICENSE.md
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       23 2023-12-22 10:09:15.000000 simo-zwave-1.0.6/MANIFEST.in
--rw-r--r--   0 simanas   (1000) simanas   (1000)      578 2024-01-21 07:05:25.062583 simo-zwave-1.0.6/PKG-INFO
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      760 2023-12-20 12:06:12.000000 simo-zwave-1.0.6/README.rst
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      677 2024-01-21 07:04:32.000000 simo-zwave-1.0.6/pyproject.toml
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       36 2024-01-18 10:26:29.000000 simo-zwave-1.0.6/requirements.txt
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       38 2024-01-21 07:05:25.066583 simo-zwave-1.0.6/setup.cfg
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.046583 simo-zwave-1.0.6/src/
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.054583 simo-zwave-1.0.6/src/simo_zwave/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)        0 2020-06-17 09:24:21.000000 simo-zwave-1.0.6/src/simo_zwave/__init__.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.058583 simo-zwave-1.0.6/src/simo_zwave/__pycache__/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      167 2021-11-04 11:46:52.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     6287 2024-01-18 09:53:40.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/admin.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      359 2022-01-17 14:17:30.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/auto_urls.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     2834 2024-01-18 14:40:17.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/controllers.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1578 2022-07-07 13:29:13.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/dynamic_settings.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     6610 2024-01-18 10:02:27.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/forms.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     6994 2024-01-21 07:04:23.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/gateways.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     4234 2024-01-21 07:03:12.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/models.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     2376 2022-01-25 13:33:11.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/utils.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      893 2021-12-02 13:47:22.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/views.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1374 2021-12-22 13:40:24.000000 simo-zwave-1.0.6/src/simo_zwave/__pycache__/widgets.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     8041 2024-01-18 08:28:46.000000 simo-zwave-1.0.6/src/simo_zwave/admin.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      205 2022-01-17 14:17:27.000000 simo-zwave-1.0.6/src/simo_zwave/auto_urls.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     2239 2024-01-18 11:24:03.000000 simo-zwave-1.0.6/src/simo_zwave/controllers.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1064 2022-07-07 13:29:11.000000 simo-zwave-1.0.6/src/simo_zwave/dynamic_settings.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     6898 2024-01-18 10:02:26.000000 simo-zwave-1.0.6/src/simo_zwave/forms.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     8889 2024-01-21 07:04:20.000000 simo-zwave-1.0.6/src/simo_zwave/gateways.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.058583 simo-zwave-1.0.6/src/simo_zwave/migrations/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     2727 2023-12-20 10:21:16.000000 simo-zwave-1.0.6/src/simo_zwave/migrations/0001_initial.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      407 2023-12-20 10:12:17.000000 simo-zwave-1.0.6/src/simo_zwave/migrations/0002_alter_nodevalue_genre.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)        0 2021-09-24 11:57:43.000000 simo-zwave-1.0.6/src/simo_zwave/migrations/__init__.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.062583 simo-zwave-1.0.6/src/simo_zwave/migrations/__pycache__/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1981 2023-12-20 10:21:23.000000 simo-zwave-1.0.6/src/simo_zwave/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      633 2023-12-20 10:12:26.000000 simo-zwave-1.0.6/src/simo_zwave/migrations/__pycache__/0002_alter_nodevalue_genre.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      178 2021-11-04 11:46:55.000000 simo-zwave-1.0.6/src/simo_zwave/migrations/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     4037 2024-01-21 07:03:09.000000 simo-zwave-1.0.6/src/simo_zwave/models.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.062583 simo-zwave-1.0.6/src/simo_zwave/templates/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     2992 2020-11-15 10:06:42.000000 simo-zwave-1.0.6/src/simo_zwave/templates/add_zwave_node.html
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.046583 simo-zwave-1.0.6/src/simo_zwave/templates/admin/
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.062583 simo-zwave-1.0.6/src/simo_zwave/templates/admin/zwave/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       89 2022-01-17 14:17:27.000000 simo-zwave-1.0.6/src/simo_zwave/templates/admin/zwave/library_update_btn.html
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.062583 simo-zwave-1.0.6/src/simo_zwave/templates/admin/zwave/zwavenode/
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      499 2020-11-15 10:06:42.000000 simo-zwave-1.0.6/src/simo_zwave/templates/admin/zwave/zwavenode/change_list_object_tools.html
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     3005 2020-11-15 10:06:42.000000 simo-zwave-1.0.6/src/simo_zwave/templates/remove_zwave_node.html
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     2459 2020-11-15 10:06:42.000000 simo-zwave-1.0.6/src/simo_zwave/templates/zwave_node_choose_gateway.html
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      113 2020-11-15 10:06:42.000000 simo-zwave-1.0.6/src/simo_zwave/templates/zwave_nodes.html
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     2950 2022-01-25 13:33:08.000000 simo-zwave-1.0.6/src/simo_zwave/utils.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      782 2021-12-02 13:47:20.000000 simo-zwave-1.0.6/src/simo_zwave/views.py
--rw-rw-r--   0 simanas   (1000) simanas   (1000)      920 2020-11-15 10:06:42.000000 simo-zwave-1.0.6/src/simo_zwave/widgets.py
-drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-01-21 07:05:25.062583 simo-zwave-1.0.6/src/simo_zwave.egg-info/
--rw-r--r--   0 simanas   (1000) simanas   (1000)      578 2024-01-21 07:05:25.000000 simo-zwave-1.0.6/src/simo_zwave.egg-info/PKG-INFO
--rw-rw-r--   0 simanas   (1000) simanas   (1000)     1779 2024-01-21 07:05:25.000000 simo-zwave-1.0.6/src/simo_zwave.egg-info/SOURCES.txt
--rw-rw-r--   0 simanas   (1000) simanas   (1000)        1 2024-01-21 07:05:25.000000 simo-zwave-1.0.6/src/simo_zwave.egg-info/dependency_links.txt
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       37 2024-01-21 07:05:25.000000 simo-zwave-1.0.6/src/simo_zwave.egg-info/requires.txt
--rw-rw-r--   0 simanas   (1000) simanas   (1000)       11 2024-01-21 07:05:25.000000 simo-zwave-1.0.6/src/simo_zwave.egg-info/top_level.txt
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.487571 simo_zwave-1.0.7/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)    34916 2021-12-07 14:40:19.000000 simo_zwave-1.0.7/LICENSE.md
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       23 2023-12-22 10:09:15.000000 simo_zwave-1.0.7/MANIFEST.in
+-rw-r--r--   0 simanas   (1000) simanas   (1000)      578 2024-04-13 15:10:11.487571 simo_zwave-1.0.7/PKG-INFO
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      760 2023-12-20 12:06:12.000000 simo_zwave-1.0.7/README.rst
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      677 2024-04-13 15:09:05.000000 simo_zwave-1.0.7/pyproject.toml
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       36 2024-01-18 10:26:29.000000 simo_zwave-1.0.7/requirements.txt
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       38 2024-04-13 15:10:11.487571 simo_zwave-1.0.7/setup.cfg
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.467564 simo_zwave-1.0.7/src/
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.475567 simo_zwave-1.0.7/src/simo_zwave/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)        0 2020-06-17 09:24:21.000000 simo_zwave-1.0.7/src/simo_zwave/__init__.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.483569 simo_zwave-1.0.7/src/simo_zwave/__pycache__/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      167 2021-11-04 11:46:52.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     6287 2024-01-18 09:53:40.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/admin.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      354 2024-04-13 15:09:27.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/auto_urls.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2834 2024-01-18 14:40:17.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/controllers.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1578 2022-07-07 13:29:13.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/dynamic_settings.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     6610 2024-01-18 10:02:27.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/forms.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     6994 2024-01-21 07:04:23.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/gateways.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     4234 2024-01-21 07:03:12.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/models.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2376 2022-01-25 13:33:11.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/utils.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      893 2021-12-02 13:47:22.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/views.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1374 2021-12-22 13:40:24.000000 simo_zwave-1.0.7/src/simo_zwave/__pycache__/widgets.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     8041 2024-01-18 08:28:46.000000 simo_zwave-1.0.7/src/simo_zwave/admin.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      199 2024-04-13 15:09:25.000000 simo_zwave-1.0.7/src/simo_zwave/auto_urls.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2239 2024-01-18 11:24:03.000000 simo_zwave-1.0.7/src/simo_zwave/controllers.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1064 2022-07-07 13:29:11.000000 simo_zwave-1.0.7/src/simo_zwave/dynamic_settings.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     6898 2024-01-18 10:02:26.000000 simo_zwave-1.0.7/src/simo_zwave/forms.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     8889 2024-01-21 07:04:20.000000 simo_zwave-1.0.7/src/simo_zwave/gateways.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.483569 simo_zwave-1.0.7/src/simo_zwave/migrations/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2727 2023-12-20 10:21:16.000000 simo_zwave-1.0.7/src/simo_zwave/migrations/0001_initial.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      407 2023-12-20 10:12:17.000000 simo_zwave-1.0.7/src/simo_zwave/migrations/0002_alter_nodevalue_genre.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)        0 2021-09-24 11:57:43.000000 simo_zwave-1.0.7/src/simo_zwave/migrations/__init__.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.483569 simo_zwave-1.0.7/src/simo_zwave/migrations/__pycache__/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1981 2023-12-20 10:21:23.000000 simo_zwave-1.0.7/src/simo_zwave/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      633 2023-12-20 10:12:26.000000 simo_zwave-1.0.7/src/simo_zwave/migrations/__pycache__/0002_alter_nodevalue_genre.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      178 2021-11-04 11:46:55.000000 simo_zwave-1.0.7/src/simo_zwave/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     4037 2024-01-21 07:03:09.000000 simo_zwave-1.0.7/src/simo_zwave/models.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.483569 simo_zwave-1.0.7/src/simo_zwave/templates/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2992 2020-11-15 10:06:42.000000 simo_zwave-1.0.7/src/simo_zwave/templates/add_zwave_node.html
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.467564 simo_zwave-1.0.7/src/simo_zwave/templates/admin/
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.483569 simo_zwave-1.0.7/src/simo_zwave/templates/admin/zwave/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       89 2022-01-17 14:17:27.000000 simo_zwave-1.0.7/src/simo_zwave/templates/admin/zwave/library_update_btn.html
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.487571 simo_zwave-1.0.7/src/simo_zwave/templates/admin/zwave/zwavenode/
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      499 2020-11-15 10:06:42.000000 simo_zwave-1.0.7/src/simo_zwave/templates/admin/zwave/zwavenode/change_list_object_tools.html
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     3005 2020-11-15 10:06:42.000000 simo_zwave-1.0.7/src/simo_zwave/templates/remove_zwave_node.html
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2459 2020-11-15 10:06:42.000000 simo_zwave-1.0.7/src/simo_zwave/templates/zwave_node_choose_gateway.html
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      113 2020-11-15 10:06:42.000000 simo_zwave-1.0.7/src/simo_zwave/templates/zwave_nodes.html
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     2950 2022-01-25 13:33:08.000000 simo_zwave-1.0.7/src/simo_zwave/utils.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      782 2021-12-02 13:47:20.000000 simo_zwave-1.0.7/src/simo_zwave/views.py
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)      920 2020-11-15 10:06:42.000000 simo_zwave-1.0.7/src/simo_zwave/widgets.py
+drwxrwxr-x   0 simanas   (1000) simanas   (1000)        0 2024-04-13 15:10:11.487571 simo_zwave-1.0.7/src/simo_zwave.egg-info/
+-rw-r--r--   0 simanas   (1000) simanas   (1000)      578 2024-04-13 15:10:11.000000 simo_zwave-1.0.7/src/simo_zwave.egg-info/PKG-INFO
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)     1779 2024-04-13 15:10:11.000000 simo_zwave-1.0.7/src/simo_zwave.egg-info/SOURCES.txt
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)        1 2024-04-13 15:10:11.000000 simo_zwave-1.0.7/src/simo_zwave.egg-info/dependency_links.txt
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       37 2024-04-13 15:10:11.000000 simo_zwave-1.0.7/src/simo_zwave.egg-info/requires.txt
+-rw-rw-r--   0 simanas   (1000) simanas   (1000)       11 2024-04-13 15:10:11.000000 simo_zwave-1.0.7/src/simo_zwave.egg-info/top_level.txt
```

### Comparing `simo-zwave-1.0.6/LICENSE.md` & `simo_zwave-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/PKG-INFO` & `simo_zwave-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simo-zwave
-Version: 1.0.6
+Version: 1.0.7
 Summary: OpenZwave integration for SIMO.io
 Author-email: Simanas Venčkauskas <simanas@simo.io>
 Project-URL: Homepage, https://github.com/SIMO-io/simo-zwave
 Project-URL: Issues, https://github.com/SIMO-io/simo-zwave/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simo-zwave-1.0.6/README.rst` & `simo_zwave-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/pyproject.toml` & `simo_zwave-1.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simo-zwave"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Simanas Venčkauskas", email="simanas@simo.io" },
 ]
 description = "OpenZwave integration for SIMO.io"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/admin.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/admin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/controllers.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/controllers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/dynamic_settings.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/dynamic_settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/forms.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/forms.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/gateways.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/gateways.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/models.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/utils.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/views.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/__pycache__/widgets.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/__pycache__/widgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/admin.py` & `simo_zwave-1.0.7/src/simo_zwave/admin.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/controllers.py` & `simo_zwave-1.0.7/src/simo_zwave/controllers.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/dynamic_settings.py` & `simo_zwave-1.0.7/src/simo_zwave/dynamic_settings.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/forms.py` & `simo_zwave-1.0.7/src/simo_zwave/forms.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/gateways.py` & `simo_zwave-1.0.7/src/simo_zwave/gateways.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/migrations/0001_initial.py` & `simo_zwave-1.0.7/src/simo_zwave/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/migrations/__pycache__/0001_initial.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/migrations/__pycache__/0001_initial.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/migrations/__pycache__/0002_alter_nodevalue_genre.cpython-38.pyc` & `simo_zwave-1.0.7/src/simo_zwave/migrations/__pycache__/0002_alter_nodevalue_genre.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/models.py` & `simo_zwave-1.0.7/src/simo_zwave/models.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/templates/add_zwave_node.html` & `simo_zwave-1.0.7/src/simo_zwave/templates/add_zwave_node.html`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/templates/remove_zwave_node.html` & `simo_zwave-1.0.7/src/simo_zwave/templates/remove_zwave_node.html`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/templates/zwave_node_choose_gateway.html` & `simo_zwave-1.0.7/src/simo_zwave/templates/zwave_node_choose_gateway.html`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/utils.py` & `simo_zwave-1.0.7/src/simo_zwave/utils.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/views.py` & `simo_zwave-1.0.7/src/simo_zwave/views.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave/widgets.py` & `simo_zwave-1.0.7/src/simo_zwave/widgets.py`

 * *Files identical despite different names*

### Comparing `simo-zwave-1.0.6/src/simo_zwave.egg-info/PKG-INFO` & `simo_zwave-1.0.7/src/simo_zwave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simo-zwave
-Version: 1.0.6
+Version: 1.0.7
 Summary: OpenZwave integration for SIMO.io
 Author-email: Simanas Venčkauskas <simanas@simo.io>
 Project-URL: Homepage, https://github.com/SIMO-io/simo-zwave
 Project-URL: Issues, https://github.com/SIMO-io/simo-zwave/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simo-zwave-1.0.6/src/simo_zwave.egg-info/SOURCES.txt` & `simo_zwave-1.0.7/src/simo_zwave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

