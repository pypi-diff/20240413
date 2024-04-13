# Comparing `tmp/config-library-0.8.2.tar.gz` & `tmp/config-library-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config-library-0.8.2.tar", last modified: Thu Nov  2 12:56:52 2023, max compression
+gzip compressed data, was "config-library-0.9.0.tar", last modified: Mon Nov  6 16:27:58 2023, max compression
```

## Comparing `config-library-0.8.2.tar` & `config-library-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.015455 config-library-0.8.2/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1065 2022-11-09 07:43:43.000000 config-library-0.8.2/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     6857 2023-11-02 12:56:52.015455 config-library-0.8.2/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     5199 2023-11-02 12:56:40.000000 config-library-0.8.2/README.md
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2022-11-09 20:19:55.000000 config-library-0.8.2/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2023-11-02 12:56:52.015455 config-library-0.8.2/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2009 2023-10-31 13:51:51.000000 config-library-0.8.2/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.011455 config-library-0.8.2/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.011455 config-library-0.8.2/src/config_library.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     6857 2023-11-02 12:56:52.000000 config-library-0.8.2/src/config_library.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1472 2023-11-02 12:56:52.000000 config-library-0.8.2/src/config_library.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2023-11-02 12:56:52.000000 config-library-0.8.2/src/config_library.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      105 2023-11-02 12:56:52.000000 config-library-0.8.2/src/config_library.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       10 2023-11-02 12:56:52.000000 config-library-0.8.2/src/config_library.egg-info/top_level.txt
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.011455 config-library-0.8.2/src/configlib/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1916 2023-11-02 10:18:39.000000 config-library-0.8.2/src/configlib/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       86 2023-11-02 12:55:24.000000 config-library-0.8.2/src/configlib/__version__.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.011455 config-library-0.8.2/src/configlib/configurator/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       91 2023-09-18 06:21:38.000000 config-library-0.8.2/src/configlib/configurator/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      711 2023-09-23 16:48:11.000000 config-library-0.8.2/src/configlib/configurator/atrestart.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     4157 2023-11-02 10:18:39.000000 config-library-0.8.2/src/configlib/configurator/configurator.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      635 2023-09-23 16:52:31.000000 config-library-0.8.2/src/configlib/configurator/restarter.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      497 2023-10-30 09:30:57.000000 config-library-0.8.2/src/configlib/exceptions.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.011455 config-library-0.8.2/src/configlib/finder/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      112 2023-09-17 11:58:34.000000 config-library-0.8.2/src/configlib/finder/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      359 2023-10-31 08:14:05.000000 config-library-0.8.2/src/configlib/finder/default_places.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1563 2023-10-15 13:27:44.000000 config-library-0.8.2/src/configlib/finder/find.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1446 2023-10-31 08:14:05.000000 config-library-0.8.2/src/configlib/finder/places.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.011455 config-library-0.8.2/src/configlib/install/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      361 2023-09-18 08:54:22.000000 config-library-0.8.2/src/configlib/install/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1038 2023-09-18 08:54:22.000000 config-library-0.8.2/src/configlib/install/installer.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.015455 config-library-0.8.2/src/configlib/interface/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       79 2023-10-30 07:52:02.000000 config-library-0.8.2/src/configlib/interface/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     5031 2023-11-02 12:16:28.000000 config-library-0.8.2/src/configlib/interface/cls.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      158 2023-10-30 08:21:37.000000 config-library-0.8.2/src/configlib/interface/typing.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1910 2023-11-02 11:45:52.000000 config-library-0.8.2/src/configlib/interface/util.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.015455 config-library-0.8.2/src/configlib/loader/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1283 2023-11-02 10:18:39.000000 config-library-0.8.2/src/configlib/loader/__init__.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.015455 config-library-0.8.2/src/configlib/loader/environ/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      141 2023-10-31 09:28:08.000000 config-library-0.8.2/src/configlib/loader/environ/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1707 2023-10-31 09:32:36.000000 config-library-0.8.2/src/configlib/loader/environ/loader.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      458 2023-10-31 09:28:08.000000 config-library-0.8.2/src/configlib/loader/environ/util.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.015455 config-library-0.8.2/src/configlib/loader/loaders/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      645 2023-11-01 09:26:12.000000 config-library-0.8.2/src/configlib/loader/loaders/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1066 2023-11-01 08:36:20.000000 config-library-0.8.2/src/configlib/loader/loaders/conf_loader.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      857 2023-11-01 08:36:20.000000 config-library-0.8.2/src/configlib/loader/loaders/json5_loader.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      871 2023-11-01 08:36:20.000000 config-library-0.8.2/src/configlib/loader/loaders/json_loader.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1018 2023-11-01 08:36:20.000000 config-library-0.8.2/src/configlib/loader/loaders/jsonc_loader.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1065 2023-11-01 08:36:20.000000 config-library-0.8.2/src/configlib/loader/loaders/toml_loader.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1034 2023-11-01 09:22:34.000000 config-library-0.8.2/src/configlib/loader/loaders/xml_loader.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1225 2023-11-01 08:36:20.000000 config-library-0.8.2/src/configlib/loader/loaders/yaml_loader.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      818 2023-11-01 08:36:20.000000 config-library-0.8.2/src/configlib/loader/registry.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.015455 config-library-0.8.2/src/configlib/watcher/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       81 2023-09-18 05:32:32.000000 config-library-0.8.2/src/configlib/watcher/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1223 2023-09-22 12:34:47.000000 config-library-0.8.2/src/configlib/watcher/watcher.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-02 12:56:52.015455 config-library-0.8.2/tests/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      216 2023-09-20 18:59:36.000000 config-library-0.8.2/tests/test_import.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1830 2023-11-02 10:18:39.000000 config-library-0.8.2/tests/test_loaders.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.479316 config-library-0.9.0/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1065 2022-11-09 07:43:43.000000 config-library-0.9.0/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     8353 2023-11-06 16:27:58.479316 config-library-0.9.0/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     6695 2023-11-06 10:11:34.000000 config-library-0.9.0/README.md
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2022-11-09 20:19:55.000000 config-library-0.9.0/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2023-11-06 16:27:58.479316 config-library-0.9.0/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2009 2023-10-31 13:51:51.000000 config-library-0.9.0/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.475315 config-library-0.9.0/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.475315 config-library-0.9.0/src/config_library.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     8353 2023-11-06 16:27:58.000000 config-library-0.9.0/src/config_library.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1472 2023-11-06 16:27:58.000000 config-library-0.9.0/src/config_library.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2023-11-06 16:27:58.000000 config-library-0.9.0/src/config_library.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      105 2023-11-06 16:27:58.000000 config-library-0.9.0/src/config_library.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       10 2023-11-06 16:27:58.000000 config-library-0.9.0/src/config_library.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.475315 config-library-0.9.0/src/configlib/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1783 2023-11-06 09:24:54.000000 config-library-0.9.0/src/configlib/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       86 2023-11-06 16:24:00.000000 config-library-0.9.0/src/configlib/__version__.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.475315 config-library-0.9.0/src/configlib/configurator/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       91 2023-09-18 06:21:38.000000 config-library-0.9.0/src/configlib/configurator/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      711 2023-09-23 16:48:11.000000 config-library-0.9.0/src/configlib/configurator/atrestart.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     3724 2023-11-06 16:27:15.000000 config-library-0.9.0/src/configlib/configurator/configurator.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      635 2023-09-23 16:52:31.000000 config-library-0.9.0/src/configlib/configurator/restarter.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      497 2023-10-30 09:30:57.000000 config-library-0.9.0/src/configlib/exceptions.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.475315 config-library-0.9.0/src/configlib/finder/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      112 2023-09-17 11:58:34.000000 config-library-0.9.0/src/configlib/finder/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      359 2023-10-31 08:14:05.000000 config-library-0.9.0/src/configlib/finder/default_places.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1378 2023-11-06 10:11:34.000000 config-library-0.9.0/src/configlib/finder/find.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1446 2023-10-31 08:14:05.000000 config-library-0.9.0/src/configlib/finder/places.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.475315 config-library-0.9.0/src/configlib/install/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      361 2023-09-18 08:54:22.000000 config-library-0.9.0/src/configlib/install/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1153 2023-11-06 16:27:15.000000 config-library-0.9.0/src/configlib/install/installer.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.475315 config-library-0.9.0/src/configlib/interface/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       79 2023-10-30 07:52:02.000000 config-library-0.9.0/src/configlib/interface/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     5031 2023-11-02 12:16:28.000000 config-library-0.9.0/src/configlib/interface/cls.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      158 2023-10-30 08:21:37.000000 config-library-0.9.0/src/configlib/interface/typing.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1910 2023-11-02 11:45:52.000000 config-library-0.9.0/src/configlib/interface/util.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.479316 config-library-0.9.0/src/configlib/loader/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1283 2023-11-02 10:18:39.000000 config-library-0.9.0/src/configlib/loader/__init__.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.479316 config-library-0.9.0/src/configlib/loader/environ/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      141 2023-10-31 09:28:08.000000 config-library-0.9.0/src/configlib/loader/environ/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1707 2023-10-31 09:32:36.000000 config-library-0.9.0/src/configlib/loader/environ/loader.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      458 2023-10-31 09:28:08.000000 config-library-0.9.0/src/configlib/loader/environ/util.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.479316 config-library-0.9.0/src/configlib/loader/loaders/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      645 2023-11-01 09:26:12.000000 config-library-0.9.0/src/configlib/loader/loaders/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1066 2023-11-01 08:36:20.000000 config-library-0.9.0/src/configlib/loader/loaders/conf_loader.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      857 2023-11-01 08:36:20.000000 config-library-0.9.0/src/configlib/loader/loaders/json5_loader.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      871 2023-11-01 08:36:20.000000 config-library-0.9.0/src/configlib/loader/loaders/json_loader.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1018 2023-11-01 08:36:20.000000 config-library-0.9.0/src/configlib/loader/loaders/jsonc_loader.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1065 2023-11-01 08:36:20.000000 config-library-0.9.0/src/configlib/loader/loaders/toml_loader.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1034 2023-11-01 09:22:34.000000 config-library-0.9.0/src/configlib/loader/loaders/xml_loader.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1225 2023-11-01 08:36:20.000000 config-library-0.9.0/src/configlib/loader/loaders/yaml_loader.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      818 2023-11-01 08:36:20.000000 config-library-0.9.0/src/configlib/loader/registry.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.479316 config-library-0.9.0/src/configlib/watcher/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       81 2023-09-18 05:32:32.000000 config-library-0.9.0/src/configlib/watcher/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1223 2023-09-22 12:34:47.000000 config-library-0.9.0/src/configlib/watcher/watcher.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2023-11-06 16:27:58.479316 config-library-0.9.0/tests/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      216 2023-09-20 18:59:36.000000 config-library-0.9.0/tests/test_import.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1830 2023-11-02 10:18:39.000000 config-library-0.9.0/tests/test_loaders.py
```

### Comparing `config-library-0.8.2/LICENSE` & `config-library-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/PKG-INFO` & `config-library-0.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,27 @@
-Metadata-Version: 2.1
-Name: config-library
-Version: 0.8.2
-Summary: utility library to find and load configuration files
-Home-page: https://github.com/PlayerG9/configlib-py
-Author: PlayerG9
-License: MIT
-Project-URL: Author Github, https://github.com/PlayerG9
-Project-URL: Homepage, https://github.com/PlayerG9/configlib-py/
-Project-URL: Documentation, https://utility-libraries.github.io/configlib-py/
-Project-URL: Bug Tracker, https://github.com/PlayerG9/configlib-py/issues
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Classifier: Topic :: Utilities
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: yaml
-Requires-Dist: pyyaml; extra == "yaml"
-Provides-Extra: toml
-Requires-Dist: toml; extra == "toml"
-Provides-Extra: json5
-Requires-Dist: json-five; extra == "json5"
-Provides-Extra: watcher
-Requires-Dist: watchdog; extra == "watcher"
-Provides-Extra: all
-Requires-Dist: pyyaml; extra == "all"
-Requires-Dist: toml; extra == "all"
-Requires-Dist: json-five; extra == "all"
-Requires-Dist: watchdog; extra == "all"
-
 # config-library
 utility library to find and load configuration files
 
 > see the [documentation](https://utility-libraries.github.io/configlib-py/) for more information
 
-![configlib icon](https://github.com/utility-libraries/configlib-py/raw/main/README.assets/configlib.svg)
+<img style="height: 100px" src="https://github.com/utility-libraries/configlib-py/raw/main/README.assets/configlib.svg" alt="">
 
 <!-- TOC -->
 * [config-library](#config-library)
   * [Installation](#installation)
   * [Supported Config-Types](#supported-config-types)
   * [Install Variations](#install-variations)
-  * [More about `configlib`](#more-about-configlib)
-    * [Places to search for](#places-to-search-for)
   * [Usage Example](#usage-example)
     * [Basic Usage](#basic-usage)
     * [Loading specific file](#loading-specific-file)
     * [Specify/Customise search locations](#specifycustomise-search-locations)
   * [More in detail](#more-in-detail)
+    * [Searching](#searching)
+    * [Loading](#loading)
+    * [Accessing configuration](#accessing-configuration)
 <!-- TOC -->
 
 ## Installation
 
 [![PyPI - Version](https://img.shields.io/pypi/v/config-library)
 ](https://pypi.org/project/config-library/)
 
@@ -91,31 +50,14 @@
 |---------------------------|---------------------------------------------------|
 | `config-library[all]`     | adds all dependencies from the variations below   |
 | `config-library[watcher]` | adds support to watch the config-file for changes |
 | `config-library[json5]`   | adds support to load `.json5` files               |
 | `config-library[toml]`    | adds support to load `.toml` files                |
 | `config-library[yaml]`    | adds support to load `.yaml` files                |
 
-
-## More about `configlib`
-
-### Places to search for
-
-```
-/path/to/your/source/code/
-/path/to/your/git-repo/
-/home/<user>/.config/
-/home/<user>/
-/etc/
-```
-
-> Note: On Windows there are respective counterparts.
-
-And in these folders it searches for either directly the config file or a sub-folder that's named like your project.
-
 ## Usage Example
 
 ### Basic Usage
 
 ```python
 from configlib import find_and_load
 
@@ -130,51 +72,90 @@
 ```
 
 ### Loading specific file
 
 ```python
 import configlib
 
-
 config = configlib.load("./app.conf")
 ```
 
 ### Specify/Customise search locations
 
 ```python
 from configlib.finder import find, places
 
 config_file = find(
-    name="app.conf",  # name of config-file is 'app.conf'
+    "project-name.conf",  # variant of the config-file to search for is 'app.conf'
+    "project-name/settings.conf",  # alternate variant name to search for
     places=[places.local, places.user_conf],  # search in main.py folder and ~/.config/
-    namespace="myproject",
-    ns_only=True,  # only search for 'myproject/app.conf' in places
 )
 ```
 
 ## More in detail
 
+For the more detailed description we will use this code example.
+
 ```python
 import configlib
-config = configlib.find_and_load('app.conf', 'project')
+config = configlib.find_and_load('project.conf', 'project/app.conf')
 ```
+
+### Searching
+
+The `configlib.finder` subpackage has a few predefined paths it attempts to search in.
+In each of these places it attempts to find one of the passed variants (`project.conf`, `project/app.conf`).
+If it can't find one it goes to the next place and repeats this process.
+
 system file-structure
 ```
 /
 ├─ etc/
 ├─ home/user/
 │  ├─ path/to/repo/
 │  │  ├─ src/code/
 │  │  │  ├─ main.py
 │  ├─ .config/
 ```
 places where `config-library` searches for the config-file
-- /home/user/path/to/repo/src/code/app.conf
-- /home/user/path/to/repo/src/code/project/app.conf
-- /home/user/path/to/repo/app.conf
-- /home/user/path/to/repo/project/app.conf
-- /home/user/.config/app.conf
-- /home/user/.config/project/app.conf
-- /home/user/app.conf
-- /home/user/project/app.conf
-- /etc/app.conf
-- /etc/project/app.conf
+- `/home/user/path/to/repo/src/code/project.conf`
+- `/home/user/path/to/repo/src/code/project/app.conf`
+- `/home/user/path/to/repo/project.conf`
+- `/home/user/path/to/repo/project/app.conf`
+- `/home/user/.config/project.conf`
+- `/home/user/.config/project/app.conf`
+- `/home/user/project.conf`
+- `/home/user/project/app.conf`
+- `/etc/project.conf`
+- `/etc/project/app.conf`
+
+### Loading
+
+After the search return a filepath it is passed to the `load()` function.
+This function analyzes the file-extension and loads it with the correct loader.
+
+> The loader can be extended via the `configlib.loader.register_loader decorator`.
+> Important is that it should return native types to be compatible with the `ConfigInterface`
+> ```python
+> from configlib.loader import register_loader
+> 
+> @register_loader("env", "environ")  # support for *.env or *.environ files 
+> def custom_loader(fp) -> dict:
+>     ...
+> ```
+
+### Accessing configuration
+
+In the end you get an instance of the `ConfigInterface` with useful get-methods
+
+```python
+from configlib import ConfigInterface
+config: ConfigInterface
+config.get("database", "address", fallback="localhost")  # gets the value raw as parsed
+config.getstr("database", "address", fallback="localhost")  # gets as string
+config.getint("database", "port", fallback=5432)  # gets as integer
+config.getfloat("database", "timeout", fallback=10.0)  # gets as floating point number
+config.getboolean("database", "delayed-connect", fallback=False)  # gets as boolean
+config.getsplit("database", "tables")  # clean split by `,` or `;`
+config.getpaths("database", "client-paths", fallback=[])  # split by os.path.altsep (commonly `:`)
+config.getshlex("database", "additional-params", fallback=[])  # split like the command-line
+```
```

### Comparing `config-library-0.8.2/setup.py` & `config-library-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/config_library.egg-info/PKG-INFO` & `config-library-0.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-library
-Version: 0.8.2
+Version: 0.9.0
 Summary: utility library to find and load configuration files
 Home-page: https://github.com/PlayerG9/configlib-py
 Author: PlayerG9
 License: MIT
 Project-URL: Author Github, https://github.com/PlayerG9
 Project-URL: Homepage, https://github.com/PlayerG9/configlib-py/
 Project-URL: Documentation, https://utility-libraries.github.io/configlib-py/
@@ -41,28 +41,29 @@
 Requires-Dist: watchdog; extra == "all"
 
 # config-library
 utility library to find and load configuration files
 
 > see the [documentation](https://utility-libraries.github.io/configlib-py/) for more information
 
-![configlib icon](https://github.com/utility-libraries/configlib-py/raw/main/README.assets/configlib.svg)
+<img style="height: 100px" src="https://github.com/utility-libraries/configlib-py/raw/main/README.assets/configlib.svg" alt="">
 
 <!-- TOC -->
 * [config-library](#config-library)
   * [Installation](#installation)
   * [Supported Config-Types](#supported-config-types)
   * [Install Variations](#install-variations)
-  * [More about `configlib`](#more-about-configlib)
-    * [Places to search for](#places-to-search-for)
   * [Usage Example](#usage-example)
     * [Basic Usage](#basic-usage)
     * [Loading specific file](#loading-specific-file)
     * [Specify/Customise search locations](#specifycustomise-search-locations)
   * [More in detail](#more-in-detail)
+    * [Searching](#searching)
+    * [Loading](#loading)
+    * [Accessing configuration](#accessing-configuration)
 <!-- TOC -->
 
 ## Installation
 
 [![PyPI - Version](https://img.shields.io/pypi/v/config-library)
 ](https://pypi.org/project/config-library/)
 
@@ -91,31 +92,14 @@
 |---------------------------|---------------------------------------------------|
 | `config-library[all]`     | adds all dependencies from the variations below   |
 | `config-library[watcher]` | adds support to watch the config-file for changes |
 | `config-library[json5]`   | adds support to load `.json5` files               |
 | `config-library[toml]`    | adds support to load `.toml` files                |
 | `config-library[yaml]`    | adds support to load `.yaml` files                |
 
-
-## More about `configlib`
-
-### Places to search for
-
-```
-/path/to/your/source/code/
-/path/to/your/git-repo/
-/home/<user>/.config/
-/home/<user>/
-/etc/
-```
-
-> Note: On Windows there are respective counterparts.
-
-And in these folders it searches for either directly the config file or a sub-folder that's named like your project.
-
 ## Usage Example
 
 ### Basic Usage
 
 ```python
 from configlib import find_and_load
 
@@ -130,51 +114,90 @@
 ```
 
 ### Loading specific file
 
 ```python
 import configlib
 
-
 config = configlib.load("./app.conf")
 ```
 
 ### Specify/Customise search locations
 
 ```python
 from configlib.finder import find, places
 
 config_file = find(
-    name="app.conf",  # name of config-file is 'app.conf'
+    "project-name.conf",  # variant of the config-file to search for is 'app.conf'
+    "project-name/settings.conf",  # alternate variant name to search for
     places=[places.local, places.user_conf],  # search in main.py folder and ~/.config/
-    namespace="myproject",
-    ns_only=True,  # only search for 'myproject/app.conf' in places
 )
 ```
 
 ## More in detail
 
+For the more detailed description we will use this code example.
+
 ```python
 import configlib
-config = configlib.find_and_load('app.conf', 'project')
+config = configlib.find_and_load('project.conf', 'project/app.conf')
 ```
+
+### Searching
+
+The `configlib.finder` subpackage has a few predefined paths it attempts to search in.
+In each of these places it attempts to find one of the passed variants (`project.conf`, `project/app.conf`).
+If it can't find one it goes to the next place and repeats this process.
+
 system file-structure
 ```
 /
 ├─ etc/
 ├─ home/user/
 │  ├─ path/to/repo/
 │  │  ├─ src/code/
 │  │  │  ├─ main.py
 │  ├─ .config/
 ```
 places where `config-library` searches for the config-file
-- /home/user/path/to/repo/src/code/app.conf
-- /home/user/path/to/repo/src/code/project/app.conf
-- /home/user/path/to/repo/app.conf
-- /home/user/path/to/repo/project/app.conf
-- /home/user/.config/app.conf
-- /home/user/.config/project/app.conf
-- /home/user/app.conf
-- /home/user/project/app.conf
-- /etc/app.conf
-- /etc/project/app.conf
+- `/home/user/path/to/repo/src/code/project.conf`
+- `/home/user/path/to/repo/src/code/project/app.conf`
+- `/home/user/path/to/repo/project.conf`
+- `/home/user/path/to/repo/project/app.conf`
+- `/home/user/.config/project.conf`
+- `/home/user/.config/project/app.conf`
+- `/home/user/project.conf`
+- `/home/user/project/app.conf`
+- `/etc/project.conf`
+- `/etc/project/app.conf`
+
+### Loading
+
+After the search return a filepath it is passed to the `load()` function.
+This function analyzes the file-extension and loads it with the correct loader.
+
+> The loader can be extended via the `configlib.loader.register_loader decorator`.
+> Important is that it should return native types to be compatible with the `ConfigInterface`
+> ```python
+> from configlib.loader import register_loader
+> 
+> @register_loader("env", "environ")  # support for *.env or *.environ files 
+> def custom_loader(fp) -> dict:
+>     ...
+> ```
+
+### Accessing configuration
+
+In the end you get an instance of the `ConfigInterface` with useful get-methods
+
+```python
+from configlib import ConfigInterface
+config: ConfigInterface
+config.get("database", "address", fallback="localhost")  # gets the value raw as parsed
+config.getstr("database", "address", fallback="localhost")  # gets as string
+config.getint("database", "port", fallback=5432)  # gets as integer
+config.getfloat("database", "timeout", fallback=10.0)  # gets as floating point number
+config.getboolean("database", "delayed-connect", fallback=False)  # gets as boolean
+config.getsplit("database", "tables")  # clean split by `,` or `;`
+config.getpaths("database", "client-paths", fallback=[])  # split by os.path.altsep (commonly `:`)
+config.getshlex("database", "additional-params", fallback=[])  # split like the command-line
+```
```

### Comparing `config-library-0.8.2/src/config_library.egg-info/SOURCES.txt` & `config-library-0.9.0/src/config_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/__init__.py` & `config-library-0.9.0/src/configlib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,10 @@
 
 from .finder import find
 from .loader import load, get_supported_extensions, get_supported_loaders, loaders
 from .configurator import Configurator
 from .interface import ConfigInterface
 
 
-def find_and_load(name: str, namespace: str = None, ns_only: bool = None) -> ConfigInterface:
-    fp = find(
-        name=name,
-        namespace=namespace,
-        ns_only=ns_only if ns_only is not None else (namespace is not None),
-    )
+def find_and_load(*variants: str, places=None) -> ConfigInterface:
+    fp = find(*variants, places=places)
     return load(fp)
```

### Comparing `config-library-0.8.2/src/configlib/configurator/atrestart.py` & `config-library-0.9.0/src/configlib/configurator/atrestart.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/configurator/configurator.py` & `config-library-0.9.0/src/configlib/configurator/configurator.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,41 +13,31 @@
 
         from configlib import Configurator
         Configurator('app.conf').find().load().install().make_restart_on_change()
         ...
         from config import HOST
     """
 
-    def __init__(self, name: str, *, namespace: str = None, ns_only: bool = None, restart_on_change: bool = False):
+    def __init__(self, *variants: str, restart_on_change: bool = False):
         r"""
         :param name: name of the configuration file
         :param namespace: namespace of the project
         :param ns_only: only search for {namespace}/{name}
         :param restart_on_change: restart the whole application if the configuration file changes
         """
-        self._name = name
-        self._namespace = namespace
-        self._ns_only = ns_only
+        self._variants = variants
         self._fp = None
         self._config = None
         self._watcher = None
         self.restart_on_change = restart_on_change
         self.run_atexit = False
 
     @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def namespace(self) -> t.Optional[str]:
-        return self._namespace
-
-    @property
-    def search_namespace_only(self) -> bool:
-        return self._ns_only if self._ns_only is not None else (self._namespace is not None)
+    def variants(self) -> t.Tuple[str, ...]:
+        return self._variants
 
     @property
     def file(self) -> t.Optional[str]:
         return self._fp
 
     @property
     def config(self) -> t.Any:
@@ -64,19 +54,15 @@
         return self
 
     def find(self) -> 'Configurator':
         r"""
         find the configuration file
         """
         from ..finder import find
-        self._fp = find(
-            name=self.name,
-            namespace=self.namespace,
-            ns_only=self.search_namespace_only,
-        )
+        self._fp = find(*self.variants)
         return self
 
     def load(self) -> 'Configurator':
         r"""
         load the configuration file
         """
         from ..loader import load
```

### Comparing `config-library-0.8.2/src/configlib/configurator/restarter.py` & `config-library-0.9.0/src/configlib/configurator/restarter.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/finder/places.py` & `config-library-0.9.0/src/configlib/finder/places.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/install/installer.py` & `config-library-0.9.0/src/configlib/install/installer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 #!/usr/bin/python3
 # -*- coding=utf-8 -*-
 r"""
 
 """
 import sys
 import os.path as p
+from ..interface import ConfigInterface
 
 
 ModuleClass = type(sys)
 
 
 def install_config(config, *, fp: str = None):
     r"""
 
     :param config: the config-object to translate
     :param fp: set __file__ attribute
     :return:
     """
+
     if 'config' in sys.modules:
         raise ValueError("'config' module already exists")
 
     # note: sets __name__ and __doc__
     module = ModuleClass(name="config", doc="automatically generated module bases on one object")
 
     if fp:
         module.__file__ = p.abspath(fp)
 
+    if isinstance(config, ConfigInterface):
+        config = config.get()
     if isinstance(config, dict):
         for key in config:
             setattr(module, key, config[key])
     else:
         for key in dir(config):
             setattr(module, key, getattr(config, key))
```

### Comparing `config-library-0.8.2/src/configlib/interface/cls.py` & `config-library-0.9.0/src/configlib/interface/cls.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/interface/util.py` & `config-library-0.9.0/src/configlib/interface/util.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/__init__.py` & `config-library-0.9.0/src/configlib/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/environ/loader.py` & `config-library-0.9.0/src/configlib/loader/environ/loader.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/loaders/__init__.py` & `config-library-0.9.0/src/configlib/loader/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/loaders/conf_loader.py` & `config-library-0.9.0/src/configlib/loader/loaders/conf_loader.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/loaders/json5_loader.py` & `config-library-0.9.0/src/configlib/loader/loaders/json5_loader.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/loaders/json_loader.py` & `config-library-0.9.0/src/configlib/loader/loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/loaders/jsonc_loader.py` & `config-library-0.9.0/src/configlib/loader/loaders/jsonc_loader.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/loaders/toml_loader.py` & `config-library-0.9.0/src/configlib/loader/loaders/toml_loader.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/loaders/xml_loader.py` & `config-library-0.9.0/src/configlib/loader/loaders/xml_loader.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/loaders/yaml_loader.py` & `config-library-0.9.0/src/configlib/loader/loaders/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/loader/registry.py` & `config-library-0.9.0/src/configlib/loader/registry.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/src/configlib/watcher/watcher.py` & `config-library-0.9.0/src/configlib/watcher/watcher.py`

 * *Files identical despite different names*

### Comparing `config-library-0.8.2/tests/test_loaders.py` & `config-library-0.9.0/tests/test_loaders.py`

 * *Files identical despite different names*

