# Comparing `tmp/pancho-1.0.0.tar.gz` & `tmp/pancho-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pancho-1.0.0.tar", max compression
+gzip compressed data, was "pancho-1.0.1.tar", max compression
```

## Comparing `pancho-1.0.0.tar` & `pancho-1.0.1.tar`

### file list

```diff
@@ -1,43 +1,11 @@
--rw-r--r--   0        0        0       57 2023-01-04 14:20:51.437782 pancho-1.0.0/pancho/__init__.py
--rw-r--r--   0        0        0       93 2023-01-04 14:20:51.438102 pancho-1.0.0/pancho/bootstraping/__init__.py
--rw-r--r--   0        0        0     5721 2023-01-04 14:20:51.438392 pancho-1.0.0/pancho/bootstraping/registering.py
--rw-r--r--   0        0        0       40 2023-01-04 14:20:51.438657 pancho-1.0.0/pancho/context/__init__.py
--rw-r--r--   0        0        0     1743 2023-01-04 14:20:51.438840 pancho-1.0.0/pancho/context/collecting.py
--rw-r--r--   0        0        0        0 2022-10-08 12:17:19.416000 pancho-1.0.0/pancho/definitions/__init__.py
--rw-r--r--   0        0        0     1179 2023-01-04 14:20:51.439109 pancho-1.0.0/pancho/definitions/contracts/__init__.py
--rw-r--r--   0        0        0      552 2023-01-04 14:20:51.439296 pancho-1.0.0/pancho/definitions/contracts/context.py
--rw-r--r--   0        0        0      308 2022-10-20 08:34:36.004000 pancho-1.0.0/pancho/definitions/contracts/identity.py
--rw-r--r--   0        0        0     2000 2023-01-04 14:20:51.439548 pancho-1.0.0/pancho/definitions/contracts/interaction.py
--rw-r--r--   0        0        0      462 2022-11-21 07:40:58.324775 pancho-1.0.0/pancho/definitions/contracts/markup.py
--rw-r--r--   0        0        0      768 2022-11-24 06:56:58.034880 pancho-1.0.0/pancho/definitions/contracts/obtaining.py
--rw-r--r--   0        0        0      742 2023-01-04 14:20:51.439801 pancho-1.0.0/pancho/definitions/contracts/operations.py
--rw-r--r--   0        0        0     1005 2023-01-04 14:20:51.440057 pancho-1.0.0/pancho/definitions/contracts/processing.py
--rw-r--r--   0        0        0     3431 2023-01-04 14:20:51.440245 pancho-1.0.0/pancho/definitions/contracts/registering.py
--rw-r--r--   0        0        0      605 2023-01-04 14:20:51.440412 pancho-1.0.0/pancho/definitions/contracts/state.py
--rw-r--r--   0        0        0     1578 2022-11-22 07:31:22.189849 pancho-1.0.0/pancho/definitions/contracts/vendoring.py
--rw-r--r--   0        0        0      259 2023-01-04 14:20:51.440688 pancho-1.0.0/pancho/definitions/exceptions/__init__.py
--rw-r--r--   0        0        0      834 2023-01-04 14:20:51.440968 pancho-1.0.0/pancho/definitions/exceptions/definitions.py
--rw-r--r--   0        0        0       37 2023-01-04 14:20:51.441141 pancho-1.0.0/pancho/exploration/__init__.py
--rw-r--r--   0        0        0      398 2023-01-04 14:20:51.441301 pancho-1.0.0/pancho/exploration/types.py
--rw-r--r--   0        0        0        1 2022-10-15 17:26:35.639000 pancho-1.0.0/pancho/identity/__init__.py
--rw-r--r--   0        0        0      663 2022-10-20 08:34:36.009000 pancho-1.0.0/pancho/identity/factory.py
--rw-r--r--   0        0        0        1 2023-01-04 14:20:51.441615 pancho-1.0.0/pancho/interaction/__init__.py
--rw-r--r--   0        0        0     4116 2023-01-04 14:19:38.165013 pancho-1.0.0/pancho/interaction/factory.py
--rw-r--r--   0        0        0        0 2022-11-16 07:25:58.455883 pancho-1.0.0/pancho/markup/__init__.py
--rw-r--r--   0        0        0     4803 2023-01-02 15:27:24.286307 pancho-1.0.0/pancho/markup/schema.py
--rw-r--r--   0        0        0      110 2022-12-10 13:14:14.817501 pancho-1.0.0/pancho/obtaining/__init__.py
--rw-r--r--   0        0        0     1200 2022-12-06 07:33:04.012146 pancho-1.0.0/pancho/obtaining/factory.py
--rw-r--r--   0        0        0     2911 2022-11-22 07:31:22.182650 pancho-1.0.0/pancho/obtaining/view.py
--rw-r--r--   0        0        0       58 2023-01-04 14:20:51.441826 pancho-1.0.0/pancho/operations/__init__.py
--rw-r--r--   0        0        0     3242 2023-01-04 14:20:51.442067 pancho-1.0.0/pancho/operations/actor.py
--rw-r--r--   0        0        0     1413 2023-01-04 14:20:51.442273 pancho-1.0.0/pancho/operations/aux.py
--rw-r--r--   0        0        0        0 2022-12-10 15:56:21.286995 pancho-1.0.0/pancho/operations/handler.py
--rw-r--r--   0        0        0      132 2022-11-14 17:29:50.392233 pancho-1.0.0/pancho/processing/__init__.py
--rw-r--r--   0        0        0     2654 2023-01-04 14:20:51.442501 pancho-1.0.0/pancho/processing/factory.py
--rw-r--r--   0        0        0      847 2023-01-04 14:20:51.442732 pancho-1.0.0/pancho/processing/generic.py
--rw-r--r--   0        0        0     7037 2023-01-04 14:23:03.724207 pancho-1.0.0/pancho/processing/instance.py
--rw-r--r--   0        0        0       33 2023-01-04 14:20:51.443139 pancho-1.0.0/pancho/state/__init__.py
--rw-r--r--   0        0        0      578 2023-01-04 14:20:51.443322 pancho-1.0.0/pancho/state/handling.py
--rw-r--r--   0        0        0      555 2023-01-04 14:24:33.096328 pancho-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 pancho-1.0.0/setup.py
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pancho-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-04 14:53:25.782768 pancho-1.0.1/LICENSE
+-rw-r--r--   0        0        0      130 2024-04-02 15:23:42.891832 pancho-1.0.1/pancho/__init__.py
+-rw-r--r--   0        0        0       36 2023-10-20 11:24:28.509021 pancho-1.0.1/pancho/definition/__init__.py
+-rw-r--r--   0        0        0     2565 2024-04-12 13:04:05.932571 pancho-1.0.1/pancho/definition/contracts.py
+-rw-r--r--   0        0        0     1520 2024-04-02 15:23:42.892185 pancho-1.0.1/pancho/definition/exceptions.py
+-rw-r--r--   0        0        0      122 2024-04-02 15:23:42.892333 pancho-1.0.1/pancho/implementation/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-02 15:23:42.892474 pancho-1.0.1/pancho/implementation/factory.py
+-rw-r--r--   0        0        0     5573 2024-04-05 08:07:40.295161 pancho-1.0.1/pancho/implementation/processing.py
+-rw-r--r--   0        0        0     7615 2024-04-05 16:44:15.824108 pancho-1.0.1/pancho/implementation/registry.py
+-rw-r--r--   0        0        0      289 2024-04-13 11:47:45.279088 pancho-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 pancho-1.0.1/PKG-INFO
```

