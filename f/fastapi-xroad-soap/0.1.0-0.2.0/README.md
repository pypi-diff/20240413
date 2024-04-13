# Comparing `tmp/fastapi_xroad_soap-0.1.0.tar.gz` & `tmp/fastapi_xroad_soap-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_xroad_soap-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_xroad_soap-0.2.0.tar", max compression
```

## Comparing `fastapi_xroad_soap-0.1.0.tar` & `fastapi_xroad_soap-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,57 @@
--rw-r--r--   0        0        0     2571 2024-03-20 10:55:59.192771 fastapi_xroad_soap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       57 2024-03-20 08:45:35.826790 fastapi_xroad_soap-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-20 11:46:24.625007 fastapi_xroad_soap-0.1.0/src/main.py
--rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13749 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2813 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/README.md
+-rw-r--r--   0        0        0      524 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/__init__.py
+-rw-r--r--   0        0        0      567 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/elements.py
+-rw-r--r--   0        0        0      471 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/faults.py
+-rw-r--r--   0        0        0      340 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/__init__.py
+-rw-r--r--   0        0        0      579 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/__init__.py
+-rw-r--r--   0        0        0     4024 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/body.py
+-rw-r--r--   0        0        0     1181 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/meta.py
+-rw-r--r--   0        0        0     3024 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/base/spec.py
+-rw-r--r--   0        0        0      955 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/cid_gen.py
+-rw-r--r--   0        0        0     1119 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/constants.py
+-rw-r--r--   0        0        0     1031 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/boolean.py
+-rw-r--r--   0        0        0     2205 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/common.py
+-rw-r--r--   0        0        0     1146 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/date.py
+-rw-r--r--   0        0        0     1194 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/datetime.py
+-rw-r--r--   0        0        0     1131 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/float.py
+-rw-r--r--   0        0        0     1278 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/integer.py
+-rw-r--r--   0        0        0     1201 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/netres.py
+-rw-r--r--   0        0        0     1235 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/string.py
+-rw-r--r--   0        0        0     5104 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/swaref.py
+-rw-r--r--   0        0        0     1146 2024-04-13 20:11:22.967084 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/time.py
+-rw-r--r--   0        0        0     3157 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/elements/validators.py
+-rw-r--r--   0        0        0      679 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/__init__.py
+-rw-r--r--   0        0        0     2783 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/factory.py
+-rw-r--r--   0        0        0     1401 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/generics.py
+-rw-r--r--   0        0        0     1910 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/envelope/header.py
+-rw-r--r--   0        0        0     1910 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/file_size.py
+-rw-r--r--   0        0        0      732 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/__init__.py
+-rw-r--r--   0        0        0     2801 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/bodypart.py
+-rw-r--r--   0        0        0     2124 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/decoder.py
+-rw-r--r--   0        0        0     2502 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/encoder.py
+-rw-r--r--   0        0        0     1025 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/multipart/errors.py
+-rw-r--r--   0        0        0      901 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/__init__.py
+-rw-r--r--   0        0        0     4627 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/action.py
+-rw-r--r--   0        0        0     4064 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/faults.py
+-rw-r--r--   0        0        0     2517 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/response.py
+-rw-r--r--   0        0        0     4822 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/service.py
+-rw-r--r--   0        0        0     1938 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/soap/service.pyi
+-rw-r--r--   0        0        0     4957 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/storage.py
+-rw-r--r--   0        0        0      874 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1750 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/content_utils.py
+-rw-r--r--   0        0        0     2673 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/path_utils.py
+-rw-r--r--   0        0        0     2233 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/utils/route_utils.py
+-rw-r--r--   0        0        0     2487 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/binding.py
+-rw-r--r--   0        0        0     1558 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/conditions.py
+-rw-r--r--   0        0        0     1334 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/definitions.py
+-rw-r--r--   0        0        0      574 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/generator.py
+-rw-r--r--   0        0        0     1534 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/port_type.py
+-rw-r--r--   0        0        0     4947 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/restrictions.py
+-rw-r--r--   0        0        0     2264 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/schema.py
+-rw-r--r--   0        0        0     1335 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/internal/wsdl/service.py
+-rw-r--r--   0        0        0      506 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/fastapi_xroad_soap/utils.py
+-rw-r--r--   0        0        0     2579 2024-04-13 20:11:22.971083 fastapi_xroad_soap-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4534 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.2.0/PKG-INFO
```

