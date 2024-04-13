# Comparing `tmp/fastapi_sqlmodel_starter-1.0.0b0.tar.gz` & `tmp/fastapi_sqlmodel_starter-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sqlmodel_starter-1.0.0b0.tar", max compression
+gzip compressed data, was "fastapi_sqlmodel_starter-1.0.0b1.tar", max compression
```

## Comparing `fastapi_sqlmodel_starter-1.0.0b0.tar` & `fastapi_sqlmodel_starter-1.0.0b1.tar`

### file list

```diff
@@ -1,201 +1,264 @@
--rw-r--r--   0        0        0     1085 2024-04-08 03:12:27.583876 fastapi_sqlmodel_starter-1.0.0b0/LICENSE
--rw-r--r--   0        0        0     2261 2024-04-11 11:55:03.933846 fastapi_sqlmodel_starter-1.0.0b0/pyproject.toml
--rw-r--r--   0        0        0     2679 2024-04-11 11:41:34.689959 fastapi_sqlmodel_starter-1.0.0b0/README.md
--rw-r--r--   0        0        0      940 2024-04-09 04:17:12.813807 fastapi_sqlmodel_starter-1.0.0b0/src/.env.example
--rw-r--r--   0        0        0     3811 2024-04-09 04:17:12.813807 fastapi_sqlmodel_starter-1.0.0b0/src/alembic.ini
--rw-r--r--   0        0        0      736 2024-04-11 09:01:52.653623 fastapi_sqlmodel_starter-1.0.0b0/src/Dockerfile
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.592478 fastapi_sqlmodel_starter-1.0.0b0/src/fss/__init__.py
--rw-r--r--   0        0        0      178 2024-04-11 09:06:57.335502 fastapi_sqlmodel_starter-1.0.0b0/src/fss/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      109 2024-04-09 14:08:30.028788 fastapi_sqlmodel_starter-1.0.0b0/src/fss/apiserver.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.594467 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/__init__.py
--rw-r--r--   0        0        0      185 2024-04-11 09:06:57.356003 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4230 2024-04-11 09:08:34.765744 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.595464 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/__init__.py
--rw-r--r--   0        0        0      191 2024-04-11 09:08:35.245654 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2113 2024-04-11 11:07:51.352379 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/__pycache__/cache.cpython-311.pyc
--rw-r--r--   0        0        0     2237 2024-04-11 11:09:15.426621 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/__pycache__/page_cache.cpython-311.pyc
--rw-r--r--   0        0        0     1078 2024-04-11 10:49:23.532841 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/cache.py
--rw-r--r--   0        0        0      994 2024-04-11 10:49:23.563013 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/page_cache.py
--rw-r--r--   0        0        0     1682 2024-04-11 10:49:23.581507 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/redis_cache.py
--rw-r--r--   0        0        0     1926 2024-04-09 14:08:30.028788 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/config.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.601446 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/enum/__init__.py
--rw-r--r--   0        0        0      190 2024-04-11 09:08:35.245654 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/enum/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1316 2024-04-11 09:08:35.254202 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/enum/__pycache__/enum.cpython-311.pyc
--rw-r--r--   0        0        0      481 2024-04-09 14:08:30.028788 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/enum/enum.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.602445 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/exception/__init__.py
--rw-r--r--   0        0        0      195 2024-04-11 09:08:34.814177 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/exception/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1050 2024-04-11 09:08:34.814177 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/exception/__pycache__/exception.cpython-311.pyc
--rw-r--r--   0        0        0      428 2024-04-08 03:12:27.602445 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/exception/exception.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.603878 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__init__.py
--rw-r--r--   0        0        0      197 2024-04-11 09:06:57.356003 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4875 2024-04-11 11:07:51.370877 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__pycache__/base_mapper.cpython-311.pyc
--rw-r--r--   0        0        0     1732 2024-04-11 11:07:51.518920 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__pycache__/base_model.cpython-311.pyc
--rw-r--r--   0        0        0      510 2024-04-11 09:08:35.283993 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__pycache__/mapper.cpython-311.pyc
--rw-r--r--   0        0        0    13432 2024-04-11 11:07:51.458552 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-311.pyc
--rw-r--r--   0        0        0     2521 2024-04-11 10:49:23.599999 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/base_mapper.py
--rw-r--r--   0        0        0      814 2024-04-11 10:49:23.499749 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/base_model.py
--rw-r--r--   0        0        0       80 2024-04-08 03:12:27.605897 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/mapper.py
--rw-r--r--   0        0        0     6960 2024-04-11 10:49:23.617519 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/sqlmodel_impl.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.606872 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/result/__init__.py
--rw-r--r--   0        0        0      192 2024-04-11 09:08:35.435450 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/result/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3889 2024-04-11 09:08:35.435450 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/result/__pycache__/result.cpython-311.pyc
--rw-r--r--   0        0        0     2016 2024-04-09 14:08:30.033799 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/result/result.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.607873 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/schema/__init__.py
--rw-r--r--   0        0        0      192 2024-04-11 09:08:35.258216 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/schema/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1133 2024-04-11 09:08:35.263223 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/schema/__pycache__/schema.cpython-311.pyc
--rw-r--r--   0        0        0      315 2024-04-08 03:12:27.608863 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/schema/schema.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.608863 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/security/__init__.py
--rw-r--r--   0        0        0      194 2024-04-11 09:08:35.449274 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/security/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2156 2024-04-11 11:07:51.573400 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/security/__pycache__/security.cpython-311.pyc
--rw-r--r--   0        0        0     1305 2024-04-11 10:49:23.631146 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/security/security.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.609860 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/__init__.py
--rw-r--r--   0        0        0      193 2024-04-11 09:08:35.266847 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4490 2024-04-11 09:08:35.288520 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/__pycache__/service.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.609860 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/impl/__init__.py
--rw-r--r--   0        0        0      198 2024-04-11 09:08:35.273932 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/impl/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6568 2024-04-11 11:07:51.366085 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/impl/__pycache__/service_impl.cpython-311.pyc
--rw-r--r--   0        0        0     2802 2024-04-11 10:49:23.575666 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/impl/service_impl.py
--rw-r--r--   0        0        0     2052 2024-04-09 14:08:30.028788 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/service.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.611853 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/__init__.py
--rw-r--r--   0        0        0      190 2024-04-11 09:06:57.364030 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3072 2024-04-11 11:07:50.987856 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/__pycache__/security.cpython-311.pyc
--rw-r--r--   0        0        0     2450 2024-04-11 09:06:57.364030 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/__pycache__/snowflake.cpython-311.pyc
--rw-r--r--   0        0        0     1495 2024-04-11 10:49:23.558148 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/security.py
--rw-r--r--   0        0        0     1580 2024-04-08 03:12:27.612850 fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/snowflake.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.612850 fastapi_sqlmodel_starter-1.0.0b0/src/fss/middleware/__init__.py
--rw-r--r--   0        0        0      189 2024-04-11 09:08:35.135345 fastapi_sqlmodel_starter-1.0.0b0/src/fss/middleware/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8242 2024-04-11 09:08:35.143867 fastapi_sqlmodel_starter-1.0.0b0/src/fss/middleware/__pycache__/db_session_middleware.cpython-311.pyc
--rw-r--r--   0        0        0     4684 2024-04-09 14:08:30.028788 fastapi_sqlmodel_starter-1.0.0b0/src/fss/middleware/db_session_middleware.py
--rw-r--r--   0        0        0      221 2024-04-11 10:50:12.380955 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/__init__.py
--rw-r--r--   0        0        0      707 2024-04-11 11:07:50.714598 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8875 2024-04-11 11:07:50.719554 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/__pycache__/server.cpython-311.pyc
--rw-r--r--   0        0        0     5977 2024-04-11 10:49:23.526026 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/server.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.614844 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/__init__.py
--rw-r--r--   0        0        0      193 2024-04-11 09:06:57.344028 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.614844 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/__init__.py
--rw-r--r--   0        0        0      197 2024-04-11 09:08:35.225504 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.615861 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/v1/__init__.py
--rw-r--r--   0        0        0      200 2024-04-11 09:08:35.225504 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/v1/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1987 2024-04-11 11:07:51.340170 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/v1/__pycache__/probe_controller.cpython-311.pyc
--rw-r--r--   0        0        0     3135 2024-04-11 11:07:51.548106 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/v1/__pycache__/user_controller.cpython-311.pyc
--rw-r--r--   0        0        0      981 2024-04-11 10:49:23.551333 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/v1/probe_controller.py
--rw-r--r--   0        0        0     1695 2024-04-11 10:49:23.605841 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/v1/user_controller.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.616837 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/enum/__init__.py
--rw-r--r--   0        0        0      198 2024-04-11 09:08:35.233055 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/enum/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1281 2024-04-11 09:08:35.234081 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/enum/__pycache__/system.cpython-311.pyc
--rw-r--r--   0        0        0      501 2024-04-11 11:22:56.321257 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/enum/system.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.617833 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/exception/__init__.py
--rw-r--r--   0        0        0      203 2024-04-11 09:08:35.294119 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/exception/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1136 2024-04-11 11:07:51.378749 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/exception/__pycache__/system.cpython-311.pyc
--rw-r--r--   0        0        0      358 2024-04-11 10:49:23.519217 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/exception/system.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.618836 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/mapper/__init__.py
--rw-r--r--   0        0        0      200 2024-04-11 09:08:35.295679 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/mapper/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2005 2024-04-11 11:07:51.382556 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/mapper/__pycache__/user_mapper.cpython-311.pyc
--rw-r--r--   0        0        0     1045 2024-04-11 10:49:23.623360 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/mapper/user_mapper.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.619830 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/model/__init__.py
--rw-r--r--   0        0        0      199 2024-04-11 09:06:57.344028 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      400 2024-04-11 11:09:07.532939 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/model/__pycache__/migrate.cpython-311.pyc
--rw-r--r--   0        0        0     1772 2024-04-11 11:07:51.515967 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/model/__pycache__/user_do.cpython-311.pyc
--rw-r--r--   0        0        0      168 2024-04-11 11:06:34.663849 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/model/migrate.py
--rw-r--r--   0        0        0      728 2024-04-11 10:49:23.538680 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/model/user_do.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.621822 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/router/__init__.py
--rw-r--r--   0        0        0      200 2024-04-11 09:08:35.214039 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/router/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      751 2024-04-11 11:07:51.335306 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/router/__pycache__/system.cpython-311.pyc
--rw-r--r--   0        0        0      376 2024-04-11 10:49:23.569826 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/router/system.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.622819 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/schema/__init__.py
--rw-r--r--   0        0        0      200 2024-04-11 09:08:35.415488 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/schema/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1181 2024-04-11 09:08:35.424021 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/schema/__pycache__/user_schema.cpython-311.pyc
--rw-r--r--   0        0        0      342 2024-04-08 03:12:27.622819 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/schema/user_schema.py
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.623813 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/__init__.py
--rw-r--r--   0        0        0      201 2024-04-11 09:08:35.234081 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1413 2024-04-11 11:07:51.543231 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/__pycache__/user_service.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.623813 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/impl/__init__.py
--rw-r--r--   0        0        0      206 2024-04-11 09:08:35.234081 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/impl/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5080 2024-04-11 11:07:51.348587 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/impl/__pycache__/user_service_impl.cpython-311.pyc
--rw-r--r--   0        0        0     3012 2024-04-11 11:22:58.550000 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/impl/user_service_impl.py
--rw-r--r--   0        0        0      548 2024-04-11 10:49:23.513374 fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/user_service.py
--rw-r--r--   0        0        0       29 2024-04-11 11:09:28.119428 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/.gitignore
--rw-r--r--   0        0        0    22489 2024-04-11 11:09:28.113588 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     4536 2024-04-11 11:09:28.053241 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_07ed4fb7c74d9876___init___py.html
--rw-r--r--   0        0        0    12152 2024-04-11 11:09:28.058108 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_07ed4fb7c74d9876_user_do_py.html
--rw-r--r--   0        0        0     4524 2024-04-11 11:09:27.918934 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_0e53216603666de3___init___py.html
--rw-r--r--   0        0        0    26057 2024-04-11 11:09:27.925747 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_0e53216603666de3_result_py.html
--rw-r--r--   0        0        0     4508 2024-04-11 11:09:28.091205 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_160d2543108c5886___init___py.html
--rw-r--r--   0        0        0     4510 2024-04-11 11:09:27.849829 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_1e0a65662954c73a___init___py.html
--rw-r--r--   0        0        0    14792 2024-04-11 11:09:27.855654 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_1e0a65662954c73a_cache_py.html
--rw-r--r--   0        0        0    14113 2024-04-11 11:09:27.861505 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_1e0a65662954c73a_page_cache_py.html
--rw-r--r--   0        0        0     4528 2024-04-11 11:09:28.015282 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_204be9a6e4696b99___init___py.html
--rw-r--r--   0        0        0     4504 2024-04-11 11:09:27.847869 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_23127160240ab4f6___init___py.html
--rw-r--r--   0        0        0    25319 2024-04-11 11:09:27.871227 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_23127160240ab4f6_config_py.html
--rw-r--r--   0        0        0     4518 2024-04-11 11:09:27.879990 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2488d75dd8f8469d___init___py.html
--rw-r--r--   0        0        0     8329 2024-04-11 11:09:27.883892 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2488d75dd8f8469d_exception_py.html
--rw-r--r--   0        0        0     4518 2024-04-11 11:09:27.934507 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2a5f9cf02f67ac9f___init___py.html
--rw-r--r--   0        0        0    14975 2024-04-11 11:09:27.938388 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2a5f9cf02f67ac9f_security_py.html
--rw-r--r--   0        0        0     4518 2024-04-11 11:09:28.094124 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2ddb7f614afd77c0___init___py.html
--rw-r--r--   0        0        0     9732 2024-04-11 11:09:28.098014 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2ddb7f614afd77c0_probe_test_py.html
--rw-r--r--   0        0        0    15555 2024-04-11 11:09:28.102881 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2ddb7f614afd77c0_user_test_py.html
--rw-r--r--   0        0        0     4512 2024-04-11 11:09:27.963696 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_392b9405ba6460b0___init___py.html
--rw-r--r--   0        0        0    19152 2024-04-11 11:09:27.971481 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_392b9405ba6460b0_security_py.html
--rw-r--r--   0        0        0    20821 2024-04-11 11:09:27.978295 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_392b9405ba6460b0_snowflake_py.html
--rw-r--r--   0        0        0     4536 2024-04-11 11:09:28.044481 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_3be97aced3f710c9___init___py.html
--rw-r--r--   0        0        0    13167 2024-04-11 11:09:28.050321 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_3be97aced3f710c9_user_mapper_py.html
--rw-r--r--   0        0        0     7078 2024-04-11 11:09:27.994935 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_3c9f025fb530798e___init___py.html
--rw-r--r--   0        0        0    51456 2024-04-11 11:09:28.009456 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_3c9f025fb530798e_server_py.html
--rw-r--r--   0        0        0     4540 2024-04-11 11:09:28.031828 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_4c5c7dd0d2e26036___init___py.html
--rw-r--r--   0        0        0     9752 2024-04-11 11:09:28.035721 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_4c5c7dd0d2e26036_system_py.html
--rw-r--r--   0        0        0     4516 2024-04-11 11:09:28.012362 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_5d95fe6a529b7852___init___py.html
--rw-r--r--   0        0        0     4520 2024-04-11 11:09:27.941310 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_737f82a7e813f983___init___py.html
--rw-r--r--   0        0        0    25667 2024-04-11 11:09:27.960775 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_737f82a7e813f983_service_py.html
--rw-r--r--   0        0        0     4440 2024-04-11 11:09:27.843976 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_794d731f07d9e36c___init___py.html
--rw-r--r--   0        0        0     4502 2024-04-11 11:09:27.873179 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_8e9ea00a623205ec___init___py.html
--rw-r--r--   0        0        0    10386 2024-04-11 11:09:27.877073 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_8e9ea00a623205ec_enum_py.html
--rw-r--r--   0        0        0     4510 2024-04-11 11:09:27.928666 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_8efc05ae27a1a50a___init___py.html
--rw-r--r--   0        0        0     8101 2024-04-11 11:09:27.931575 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_8efc05ae27a1a50a_schema_py.html
--rw-r--r--   0        0        0     4538 2024-04-11 11:09:27.944227 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9373b28d605cd29a___init___py.html
--rw-r--r--   0        0        0    33198 2024-04-11 11:09:27.954054 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9373b28d605cd29a_service_impl_py.html
--rw-r--r--   0        0        0     4550 2024-04-11 11:09:28.017316 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9c41cf131237e8e8___init___py.html
--rw-r--r--   0        0        0    13961 2024-04-11 11:09:28.023069 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9c41cf131237e8e8_probe_controller_py.html
--rw-r--r--   0        0        0    19696 2024-04-11 11:09:28.028908 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9c41cf131237e8e8_user_controller_py.html
--rw-r--r--   0        0        0     4502 2024-04-11 11:09:28.088282 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0     4532 2024-04-11 11:09:28.038643 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_b6eeb7fba27ca014___init___py.html
--rw-r--r--   0        0        0     8287 2024-04-11 11:09:28.041562 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_b6eeb7fba27ca014_system_py.html
--rw-r--r--   0        0        0     4536 2024-04-11 11:09:27.885828 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695___init___py.html
--rw-r--r--   0        0        0    30040 2024-04-11 11:09:27.893627 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695_base_mapper_py.html
--rw-r--r--   0        0        0    12529 2024-04-11 11:09:27.897519 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695_base_model_py.html
--rw-r--r--   0        0        0     5790 2024-04-11 11:09:27.900429 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695_mapper_py.html
--rw-r--r--   0        0        0    71331 2024-04-11 11:09:27.916012 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695_sqlmodel_impl_py.html
--rw-r--r--   0        0        0     4536 2024-04-11 11:09:28.064923 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_dab9b2a1903716f2___init___py.html
--rw-r--r--   0        0        0     9034 2024-04-11 11:09:28.068816 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_dab9b2a1903716f2_user_schema_py.html
--rw-r--r--   0        0        0     4540 2024-04-11 11:09:27.981215 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_dcf1c620283c9c76___init___py.html
--rw-r--r--   0        0        0    39917 2024-04-11 11:09:27.991036 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_dcf1c620283c9c76_db_session_middleware_py.html
--rw-r--r--   0        0        0     4528 2024-04-11 11:09:28.060154 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_ebd618dd09682660___init___py.html
--rw-r--r--   0        0        0     7878 2024-04-11 11:09:28.062976 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_ebd618dd09682660_system_py.html
--rw-r--r--   0        0        0     4564 2024-04-11 11:09:28.074683 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_f83affef05b47916___init___py.html
--rw-r--r--   0        0        0    28794 2024-04-11 11:09:28.081554 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_f83affef05b47916_user_service_impl_py.html
--rw-r--r--   0        0        0     4542 2024-04-11 11:09:28.071735 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_fc0d8786bb154269___init___py.html
--rw-r--r--   0        0        0     9819 2024-04-11 11:09:28.085389 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_fc0d8786bb154269_user_service_py.html
--rw-r--r--   0        0        0     1732 2024-04-11 11:09:28.118464 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/favicon_32.png
--rw-r--r--   0        0        0    22046 2024-04-11 11:09:28.108721 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2024-04-11 11:09:28.115539 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2024-04-11 11:09:28.116514 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/keybd_open.png
--rw-r--r--   0        0        0    13435 2024-04-11 11:09:28.110764 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/status.json
--rw-r--r--   0        0        0    12703 2024-04-11 11:09:28.112622 fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/style.css
--rw-r--r--   0        0        0     4552 2024-04-11 11:09:07.337275 fastapi_sqlmodel_starter-1.0.0b0/src/migrations/__pycache__/env.cpython-311.pyc
--rw-r--r--   0        0        0    28672 2024-04-11 11:09:15.167818 fastapi_sqlmodel_starter-1.0.0b0/src/migrations/db/fss.db
--rw-r--r--   0        0        0       15 2024-04-09 04:17:12.829430 fastapi_sqlmodel_starter-1.0.0b0/src/migrations/db/README
--rw-r--r--   0        0        0     2714 2024-04-11 11:05:29.307806 fastapi_sqlmodel_starter-1.0.0b0/src/migrations/env.py
--rw-r--r--   0        0        0       39 2024-04-08 03:12:27.625809 fastapi_sqlmodel_starter-1.0.0b0/src/migrations/README
--rw-r--r--   0        0        0      577 2024-04-08 03:12:27.626804 fastapi_sqlmodel_starter-1.0.0b0/src/migrations/script.py.mako
--rw-r--r--   0        0        0     1516 2024-04-09 14:08:30.028788 fastapi_sqlmodel_starter-1.0.0b0/src/migrations/versions/947dad7dbfdb_init_project.py
--rw-r--r--   0        0        0     2495 2024-04-11 09:06:57.445602 fastapi_sqlmodel_starter-1.0.0b0/src/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-08 03:12:27.629793 fastapi_sqlmodel_starter-1.0.0b0/src/tests/__init__.py
--rw-r--r--   0        0        0      180 2024-04-11 09:17:42.924800 fastapi_sqlmodel_starter-1.0.0b0/src/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-09 14:06:33.727715 fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/__init__.py
--rw-r--r--   0        0        0      187 2024-04-11 09:17:42.934528 fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-04-09 14:06:33.727715 fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/v1/__init__.py
--rw-r--r--   0        0        0      190 2024-04-11 09:17:42.936359 fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/v1/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4373 2024-04-11 11:07:49.180778 fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/v1/__pycache__/probe_test.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0        0        0     6592 2024-04-11 11:07:51.674553 fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/v1/__pycache__/user_test.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0        0        0      527 2024-04-11 10:49:23.545492 fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/v1/probe_test.py
--rw-r--r--   0        0        0     1241 2024-04-11 10:49:23.505588 fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/v1/user_test.py
--rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 fastapi_sqlmodel_starter-1.0.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-04-12 11:51:13.244253 fastapi_sqlmodel_starter-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2196 2024-04-13 07:51:59.629874 fastapi_sqlmodel_starter-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2715 2024-04-13 07:58:31.878911 fastapi_sqlmodel_starter-1.0.0b1/README.md
+-rw-r--r--   0        0        0    69632 2024-04-13 07:26:42.863114 fastapi_sqlmodel_starter-1.0.0b1/src/.coverage
+-rw-r--r--   0        0        0      940 2024-04-13 06:18:35.281365 fastapi_sqlmodel_starter-1.0.0b1/src/.env.example
+-rw-r--r--   0        0        0     3811 2024-04-12 11:51:13.253984 fastapi_sqlmodel_starter-1.0.0b1/src/alembic.ini
+-rw-r--r--   0        0        0      736 2024-04-12 11:51:13.253984 fastapi_sqlmodel_starter-1.0.0b1/src/Dockerfile
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.254962 fastapi_sqlmodel_starter-1.0.0b1/src/fss/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-12 13:52:27.167753 fastapi_sqlmodel_starter-1.0.0b1/src/fss/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      108 2024-04-12 11:52:25.137476 fastapi_sqlmodel_starter-1.0.0b1/src/fss/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      109 2024-04-12 11:51:13.254962 fastapi_sqlmodel_starter-1.0.0b1/src/fss/apiserver.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.255934 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__init__.py
+-rw-r--r--   0        0        0      185 2024-04-12 13:52:27.168727 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      115 2024-04-12 11:52:25.150129 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4230 2024-04-12 13:52:27.169713 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     2468 2024-04-12 13:52:05.648727 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.256904 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-12 13:52:27.843248 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      173 2024-04-12 13:52:06.327106 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2113 2024-04-12 13:52:27.844221 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/cache.cpython-311.pyc
+-rw-r--r--   0        0        0     1583 2024-04-12 13:52:06.333920 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/cache.cpython-38.pyc
+-rw-r--r--   0        0        0     2237 2024-04-12 13:52:29.604173 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/page_cache.cpython-311.pyc
+-rw-r--r--   0        0        0     1528 2024-04-12 13:52:08.023657 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/page_cache.cpython-38.pyc
+-rw-r--r--   0        0        0     1078 2024-04-12 11:51:13.256904 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/cache.py
+-rw-r--r--   0        0        0      994 2024-04-12 11:51:13.257880 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/page_cache.py
+-rw-r--r--   0        0        0     1682 2024-04-12 11:51:13.258850 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/redis_cache.py
+-rw-r--r--   0        0        0     1926 2024-04-12 11:51:13.258850 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/config.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.259824 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-12 13:52:27.845194 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      172 2024-04-12 13:52:06.334904 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1316 2024-04-12 13:52:27.846168 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/enum.cpython-311.pyc
+-rw-r--r--   0        0        0     1012 2024-04-12 13:52:06.341709 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/enum.cpython-38.pyc
+-rw-r--r--   0        0        0      481 2024-04-12 11:51:13.259824 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/enum.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.260797 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-12 13:52:27.572672 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      177 2024-04-12 13:52:06.013718 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1050 2024-04-12 13:52:27.573635 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/exception.cpython-311.pyc
+-rw-r--r--   0        0        0      812 2024-04-12 13:52:06.020546 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/exception.cpython-38.pyc
+-rw-r--r--   0        0        0      428 2024-04-12 11:51:13.260797 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/exception.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.261771 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-12 13:52:27.855900 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      127 2024-04-12 11:52:25.152076 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4875 2024-04-12 13:52:27.856884 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_mapper.cpython-311.pyc
+-rw-r--r--   0        0        0     3541 2024-04-12 13:52:06.372865 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_mapper.cpython-38.pyc
+-rw-r--r--   0        0        0     1732 2024-04-12 13:52:27.960133 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_model.cpython-311.pyc
+-rw-r--r--   0        0        0     1184 2024-04-12 11:52:25.154022 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_model.cpython-38.pyc
+-rw-r--r--   0        0        0      510 2024-04-12 13:52:27.857847 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/mapper.cpython-311.pyc
+-rw-r--r--   0        0        0      402 2024-04-12 13:52:06.378696 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/mapper.cpython-38.pyc
+-rw-r--r--   0        0        0    13268 2024-04-13 06:05:45.222433 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-311.pyc
+-rw-r--r--   0        0        0     6828 2024-04-12 13:52:06.464346 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-38.pyc
+-rw-r--r--   0        0        0     2521 2024-04-12 11:51:13.262744 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/base_mapper.py
+-rw-r--r--   0        0        0      814 2024-04-12 11:51:13.263724 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/base_model.py
+-rw-r--r--   0        0        0       80 2024-04-12 11:51:13.264696 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/mapper.py
+-rw-r--r--   0        0        0     7039 2024-04-13 05:57:14.379609 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/sqlmodel_impl.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.265664 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-12 13:52:27.977642 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      174 2024-04-12 13:52:06.529601 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3889 2024-04-12 13:52:27.979614 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/result.cpython-311.pyc
+-rw-r--r--   0        0        0     2493 2024-04-12 13:52:06.539331 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/result.cpython-38.pyc
+-rw-r--r--   0        0        0     2016 2024-04-12 11:51:13.265664 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/result.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.265664 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-12 13:52:27.848126 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      174 2024-04-12 13:52:06.342681 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1133 2024-04-12 13:52:27.849098 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/schema.cpython-311.pyc
+-rw-r--r--   0        0        0      796 2024-04-12 13:52:06.349494 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/schema.cpython-38.pyc
+-rw-r--r--   0        0        0      315 2024-04-12 11:51:13.266637 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/schema.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.266637 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-12 13:52:27.989249 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      176 2024-04-12 13:52:06.549108 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2156 2024-04-12 13:52:27.990300 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/security.cpython-311.pyc
+-rw-r--r--   0        0        0     1482 2024-04-12 13:52:06.556889 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/security.cpython-38.pyc
+-rw-r--r--   0        0        0     1305 2024-04-12 11:51:13.267622 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/security.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.267622 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__init__.py
+-rw-r--r--   0        0        0      193 2024-04-12 13:52:27.852017 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      175 2024-04-12 13:52:06.354361 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4490 2024-04-12 13:52:27.859794 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/service.cpython-311.pyc
+-rw-r--r--   0        0        0     3214 2024-04-12 13:52:06.385508 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/service.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.268660 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__init__.py
+-rw-r--r--   0        0        0      198 2024-04-12 13:52:27.852981 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      180 2024-04-12 13:52:06.356306 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     6783 2024-04-12 13:52:27.854937 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/service_impl.cpython-311.pyc
+-rw-r--r--   0        0        0     4105 2024-04-12 13:52:06.365069 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/service_impl.cpython-38.pyc
+-rw-r--r--   0        0        0     2850 2024-04-12 13:07:40.882205 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/service_impl.py
+-rw-r--r--   0        0        0     2052 2024-04-12 11:51:13.269251 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/service.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.270148 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-12 13:52:27.574608 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      120 2024-04-12 11:52:25.156943 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3360 2024-04-12 14:08:26.649563 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/security.cpython-311.pyc
+-rw-r--r--   0        0        0     1889 2024-04-12 13:52:06.029300 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/security.cpython-38.pyc
+-rw-r--r--   0        0        0     2450 2024-04-12 13:52:27.961021 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/snowflake.cpython-311.pyc
+-rw-r--r--   0        0        0     1503 2024-04-12 11:52:25.159862 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/snowflake.cpython-38.pyc
+-rw-r--r--   0        0        0     1291 2024-04-13 07:46:45.486153 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/excel.py
+-rw-r--r--   0        0        0     1634 2024-04-12 14:08:19.414967 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/security.py
+-rw-r--r--   0        0        0     1580 2024-04-12 11:51:13.271119 fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/snowflake.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.271119 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__init__.py
+-rw-r--r--   0        0        0      189 2024-04-12 13:52:27.743976 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      171 2024-04-12 13:52:06.208653 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8242 2024-04-12 13:52:27.745923 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/db_session_middleware.cpython-311.pyc
+-rw-r--r--   0        0        0     5230 2024-04-12 13:52:06.216440 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/db_session_middleware.cpython-38.pyc
+-rw-r--r--   0        0        0     4684 2024-04-12 11:51:13.272093 fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/db_session_middleware.py
+-rw-r--r--   0        0        0      221 2024-04-12 11:51:13.273070 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-12 13:52:27.243673 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      361 2024-04-12 11:52:25.139422 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     8875 2024-04-12 13:52:27.245629 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/server.cpython-311.pyc
+-rw-r--r--   0        0        0     5191 2024-04-12 13:52:05.724720 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/server.cpython-38.pyc
+-rw-r--r--   0        0        0     5977 2024-04-12 11:51:13.273070 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/server.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.274042 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/__init__.py
+-rw-r--r--   0        0        0      193 2024-04-12 13:52:27.830596 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      123 2024-04-12 11:52:25.141368 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.274042 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-12 13:52:27.833516 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      179 2024-04-12 13:52:06.299854 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.275013 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-12 13:52:27.834489 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      182 2024-04-12 13:52:06.301799 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1987 2024-04-12 13:52:27.836467 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/probe_controller.cpython-311.pyc
+-rw-r--r--   0        0        0     1203 2024-04-12 13:52:06.308614 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/probe_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     6254 2024-04-13 06:38:33.855758 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/user_controller.cpython-311.pyc
+-rw-r--r--   0        0        0     2516 2024-04-12 13:52:06.528586 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/user_controller.cpython-38.pyc
+-rw-r--r--   0        0        0      981 2024-04-12 11:51:13.275013 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/probe_controller.py
+-rw-r--r--   0        0        0     3453 2024-04-13 06:38:25.879538 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/user_controller.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.275986 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__init__.py
+-rw-r--r--   0        0        0      198 2024-04-12 13:52:27.838380 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      180 2024-04-12 13:52:06.309586 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1331 2024-04-12 13:52:27.839432 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/system.cpython-311.pyc
+-rw-r--r--   0        0        0     1057 2024-04-12 13:52:06.315439 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/system.cpython-38.pyc
+-rw-r--r--   0        0        0      501 2024-04-12 11:51:13.276964 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/system.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.276964 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__init__.py
+-rw-r--r--   0        0        0      203 2024-04-12 13:52:27.860777 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      185 2024-04-12 13:52:06.386482 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1136 2024-04-12 13:52:27.861751 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/system.cpython-311.pyc
+-rw-r--r--   0        0        0      778 2024-04-12 13:52:06.393294 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/system.cpython-38.pyc
+-rw-r--r--   0        0        0      358 2024-04-12 11:51:13.277933 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/system.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.277933 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-12 13:52:27.862724 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      182 2024-04-12 13:52:06.394277 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2005 2024-04-12 13:52:27.863697 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/user_mapper.cpython-311.pyc
+-rw-r--r--   0        0        0     1419 2024-04-12 13:52:06.401081 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/user_mapper.cpython-38.pyc
+-rw-r--r--   0        0        0     1045 2024-04-12 11:51:13.278906 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/user_mapper.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.279881 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-12 13:52:27.947394 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2024-04-12 11:52:25.143317 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      400 2024-04-12 13:54:19.806764 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/migrate.cpython-311.pyc
+-rw-r--r--   0        0        0      311 2024-04-12 11:52:25.145262 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/migrate.cpython-38.pyc
+-rw-r--r--   0        0        0     1772 2024-04-12 13:52:27.954298 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/user_do.cpython-311.pyc
+-rw-r--r--   0        0        0     1127 2024-04-12 11:52:25.148187 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/user_do.cpython-38.pyc
+-rw-r--r--   0        0        0      168 2024-04-12 11:51:13.279881 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/migrate.py
+-rw-r--r--   0        0        0      728 2024-04-12 11:51:13.280857 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/user_do.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.280857 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-12 13:52:27.831568 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      182 2024-04-12 13:52:06.293040 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      751 2024-04-12 13:52:27.832542 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/system.cpython-311.pyc
+-rw-r--r--   0        0        0      542 2024-04-12 13:52:06.298881 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/system.cpython-38.pyc
+-rw-r--r--   0        0        0      376 2024-04-12 11:51:13.281826 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/system.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.281826 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-12 13:52:27.970761 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      182 2024-04-12 13:52:06.505301 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1845 2024-04-13 06:05:45.237824 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/user_schema.cpython-311.pyc
+-rw-r--r--   0        0        0     1160 2024-04-12 13:52:06.512086 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/__pycache__/user_schema.cpython-38.pyc
+-rw-r--r--   0        0        0      627 2024-04-13 07:46:45.274124 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/schema/user_schema.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.282800 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-12 13:52:27.840338 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      183 2024-04-12 13:52:06.316411 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2279 2024-04-13 06:05:45.242830 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/user_service.cpython-311.pyc
+-rw-r--r--   0        0        0     1083 2024-04-12 13:52:06.520875 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/user_service.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.283776 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__init__.py
+-rw-r--r--   0        0        0      206 2024-04-12 13:52:27.841301 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      188 2024-04-12 13:52:06.317373 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    11050 2024-04-13 06:34:47.200390 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/user_service_impl.cpython-311.pyc
+-rw-r--r--   0        0        0     3117 2024-04-12 13:52:06.325169 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/__pycache__/user_service_impl.cpython-38.pyc
+-rw-r--r--   0        0        0     4621 2024-04-13 07:46:45.486153 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/impl/user_service_impl.py
+-rw-r--r--   0        0        0     1017 2024-04-13 05:25:39.587003 fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/user_service.py
+-rw-r--r--   0        0        0       29 2024-04-12 14:20:41.845120 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/.gitignore
+-rw-r--r--   0        0        0    22489 2024-04-13 07:26:53.932618 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     4536 2024-04-12 14:20:41.761504 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_07ed4fb7c74d9876___init___py.html
+-rw-r--r--   0        0        0    12152 2024-04-12 14:20:41.764406 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_07ed4fb7c74d9876_user_do_py.html
+-rw-r--r--   0        0        0     4524 2024-04-12 14:20:41.672841 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_0e53216603666de3___init___py.html
+-rw-r--r--   0        0        0    26048 2024-04-12 14:20:41.678768 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_0e53216603666de3_result_py.html
+-rw-r--r--   0        0        0     4508 2024-04-12 14:20:41.786793 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_160d2543108c5886___init___py.html
+-rw-r--r--   0        0        0     4510 2024-04-12 14:20:41.625246 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a___init___py.html
+-rw-r--r--   0        0        0    14792 2024-04-12 14:20:41.628143 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a_cache_py.html
+-rw-r--r--   0        0        0    14113 2024-04-12 14:20:41.631060 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a_page_cache_py.html
+-rw-r--r--   0        0        0     4528 2024-04-12 14:20:41.736180 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_204be9a6e4696b99___init___py.html
+-rw-r--r--   0        0        0     4504 2024-04-12 14:20:41.622306 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_23127160240ab4f6___init___py.html
+-rw-r--r--   0        0        0    25319 2024-04-12 14:20:41.636902 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_23127160240ab4f6_config_py.html
+-rw-r--r--   0        0        0     4518 2024-04-12 14:20:41.642752 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2488d75dd8f8469d___init___py.html
+-rw-r--r--   0        0        0     8329 2024-04-12 14:20:41.644686 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2488d75dd8f8469d_exception_py.html
+-rw-r--r--   0        0        0     4518 2024-04-12 14:20:41.683621 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2a5f9cf02f67ac9f___init___py.html
+-rw-r--r--   0        0        0    14975 2024-04-12 14:20:41.686540 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2a5f9cf02f67ac9f_security_py.html
+-rw-r--r--   0        0        0     4518 2024-04-12 14:20:41.787787 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0___init___py.html
+-rw-r--r--   0        0        0     9732 2024-04-12 14:20:41.790689 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0_probe_test_py.html
+-rw-r--r--   0        0        0    39415 2024-04-13 07:26:53.922970 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0_user_test_py.html
+-rw-r--r--   0        0        0     4512 2024-04-12 14:20:41.703108 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0___init___py.html
+-rw-r--r--   0        0        0    20691 2024-04-12 14:20:41.707959 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0_security_py.html
+-rw-r--r--   0        0        0    20821 2024-04-12 14:20:41.712826 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0_snowflake_py.html
+-rw-r--r--   0        0        0     4536 2024-04-12 14:20:41.756622 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3be97aced3f710c9___init___py.html
+-rw-r--r--   0        0        0    13167 2024-04-12 14:20:41.759543 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3be97aced3f710c9_user_mapper_py.html
+-rw-r--r--   0        0        0     7078 2024-04-12 14:20:41.723529 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3c9f025fb530798e___init___py.html
+-rw-r--r--   0        0        0    51456 2024-04-12 14:20:41.733260 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3c9f025fb530798e_server_py.html
+-rw-r--r--   0        0        0     4540 2024-04-12 14:20:41.747861 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_4c5c7dd0d2e26036___init___py.html
+-rw-r--r--   0        0        0    10098 2024-04-12 14:20:41.750787 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_4c5c7dd0d2e26036_system_py.html
+-rw-r--r--   0        0        0     4516 2024-04-12 14:20:41.735209 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_5d95fe6a529b7852___init___py.html
+-rw-r--r--   0        0        0     4520 2024-04-12 14:20:41.688491 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_737f82a7e813f983___init___py.html
+-rw-r--r--   0        0        0    25667 2024-04-12 14:20:41.702121 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_737f82a7e813f983_service_py.html
+-rw-r--r--   0        0        0     4440 2024-04-12 14:20:41.620356 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_794d731f07d9e36c___init___py.html
+-rw-r--r--   0        0        0     4502 2024-04-12 14:20:41.638849 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8e9ea00a623205ec___init___py.html
+-rw-r--r--   0        0        0    10386 2024-04-12 14:20:41.640798 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8e9ea00a623205ec_enum_py.html
+-rw-r--r--   0        0        0     4510 2024-04-12 14:20:41.679727 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8efc05ae27a1a50a___init___py.html
+-rw-r--r--   0        0        0     8101 2024-04-12 14:20:41.681673 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8efc05ae27a1a50a_schema_py.html
+-rw-r--r--   0        0        0     4538 2024-04-12 14:20:41.689472 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9373b28d605cd29a___init___py.html
+-rw-r--r--   0        0        0    33428 2024-04-13 07:26:53.842997 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9373b28d605cd29a_service_impl_py.html
+-rw-r--r--   0        0        0     4550 2024-04-12 14:20:41.738132 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8___init___py.html
+-rw-r--r--   0        0        0    13961 2024-04-12 14:20:41.741050 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8_probe_controller_py.html
+-rw-r--r--   0        0        0    38279 2024-04-13 07:26:53.863012 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8_user_controller_py.html
+-rw-r--r--   0        0        0     4502 2024-04-12 14:20:41.784846 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0     4532 2024-04-12 14:20:41.752728 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_b6eeb7fba27ca014___init___py.html
+-rw-r--r--   0        0        0     8287 2024-04-12 14:20:41.754673 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_b6eeb7fba27ca014_system_py.html
+-rw-r--r--   0        0        0     4536 2024-04-12 14:20:41.645660 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695___init___py.html
+-rw-r--r--   0        0        0    30040 2024-04-12 14:20:41.651500 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_base_mapper_py.html
+-rw-r--r--   0        0        0    12529 2024-04-12 14:20:41.654432 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_base_model_py.html
+-rw-r--r--   0        0        0     5790 2024-04-12 14:20:41.656368 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_mapper_py.html
+-rw-r--r--   0        0        0    71690 2024-04-13 07:26:53.832931 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_sqlmodel_impl_py.html
+-rw-r--r--   0        0        0     4536 2024-04-12 14:20:41.769282 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dab9b2a1903716f2___init___py.html
+-rw-r--r--   0        0        0    13862 2024-04-13 07:26:53.888210 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dab9b2a1903716f2_user_schema_py.html
+-rw-r--r--   0        0        0     4540 2024-04-12 14:20:41.714770 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dcf1c620283c9c76___init___py.html
+-rw-r--r--   0        0        0    39917 2024-04-12 14:20:41.721582 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dcf1c620283c9c76_db_session_middleware_py.html
+-rw-r--r--   0        0        0     4528 2024-04-12 14:20:41.765384 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_ebd618dd09682660___init___py.html
+-rw-r--r--   0        0        0     7878 2024-04-12 14:20:41.768312 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_ebd618dd09682660_system_py.html
+-rw-r--r--   0        0        0     4564 2024-04-12 14:20:41.775113 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_f83affef05b47916___init___py.html
+-rw-r--r--   0        0        0    53392 2024-04-13 07:26:53.903255 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_f83affef05b47916_user_service_impl_py.html
+-rw-r--r--   0        0        0     4542 2024-04-12 14:20:41.773182 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_fc0d8786bb154269___init___py.html
+-rw-r--r--   0        0        0    13819 2024-04-13 07:26:53.905298 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_fc0d8786bb154269_user_service_py.html
+-rw-r--r--   0        0        0     1732 2024-04-13 07:26:53.932618 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0    22048 2024-04-13 07:26:53.922970 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2024-04-13 07:26:53.932618 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2024-04-13 07:26:53.932618 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0    13435 2024-04-13 07:26:53.922970 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/status.json
+-rw-r--r--   0        0        0    12703 2024-04-13 07:26:53.922970 fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/style.css
+-rw-r--r--   0        0        0     4552 2024-04-12 13:54:19.599443 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0        0        0     2408 2024-04-12 11:52:24.738430 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/__pycache__/env.cpython-38.pyc
+-rw-r--r--   0        0        0    28672 2024-04-13 07:42:12.020194 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/db/fss.db
+-rw-r--r--   0        0        0       15 2024-04-12 11:51:13.288642 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/db/README
+-rw-r--r--   0        0        0     2714 2024-04-12 11:51:13.288642 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/env.py
+-rw-r--r--   0        0        0       39 2024-04-12 11:51:13.286695 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/README
+-rw-r--r--   0        0        0      577 2024-04-12 11:51:13.289618 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/script.py.mako
+-rw-r--r--   0        0        0     1516 2024-04-12 11:51:13.291565 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/947dad7dbfdb_init_project.py
+-rw-r--r--   0        0        0     2495 2024-04-12 13:54:19.861271 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-311.pyc
+-rw-r--r--   0        0        0     1342 2024-04-12 11:52:25.233119 fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.291565 fastapi_sqlmodel_starter-1.0.0b1/src/tests/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-12 13:52:26.321928 fastapi_sqlmodel_starter-1.0.0b1/src/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      162 2024-04-12 13:52:04.950923 fastapi_sqlmodel_starter-1.0.0b1/src/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.292551 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-12 13:52:26.322901 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      169 2024-04-12 13:52:04.951811 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0        0 2024-04-12 11:51:13.292551 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__init__.py
+-rw-r--r--   0        0        0      190 2024-04-12 13:52:26.323873 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      172 2024-04-12 13:52:04.952785 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     4373 2024-04-12 13:52:26.327768 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/probe_test.cpython-311-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     2009 2024-04-12 13:52:04.962595 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/probe_test.cpython-38-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0    16631 2024-04-13 07:25:55.722716 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/user_test.cpython-311-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0     5051 2024-04-12 13:52:06.605481 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/user_test.cpython-38-pytest-8.1.1.pyc
+-rw-r--r--   0        0        0      527 2024-04-12 11:51:13.293506 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/probe_test.py
+-rw-r--r--   0        0        0     3833 2024-04-13 07:24:44.674018 fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/user_test.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 fastapi_sqlmodel_starter-1.0.0b1/PKG-INFO
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/LICENSE` & `fastapi_sqlmodel_starter-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/pyproject.toml` & `fastapi_sqlmodel_starter-1.0.0b1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,82 +1,84 @@
-[build-system]
-build-backend = "poetry.core.masonry.api"
-requires = [
-  "poetry-core",
-]
-
-[tool.poetry]
-name = "fastapi-sqlmodel-starter"
-version = "1.0.0-beta.0"
-description = "Fss aims to be one of top scaffold in PyWeb."
-license = "MIT"
-authors = [
-  "tyvekZhang <tyvekzhang@gmail.com>",
-]
-maintainers = [
-  "tyvekZhang <tyvekzhang@gmail.com>",
-]
-readme = "README.md"
-homepage = "https://github.com/tyvekzhang/fastapi-sqlmodel-starter"
-repository = "https://github.com/tyvekzhang/fastapi-sqlmodel-starter"
-documentation = "https://github.com/tyvekzhang/fastapi-sqlmodel-starter/wiki"
-keywords = ["fastapi", "sqlmodel", "tools", "web", "scaffold"]
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python",
-  "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3.12",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
-]
-packages = [
-  { include = "src"},
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-loguru = "^0.7.2"
-fastapi = "^0.110.0"
-fastapi-pagination = "^0.12.21"
-fastapi-async-sqlalchemy = "^0.6.1"
-fastapi-offline = "^1.7.1"
-uvicorn = "^0.29.0"
-sqlmodel = "^0.0.16"
-python-dotenv = "^1.0.1"
-python-multipart = "^0.0.9"
-bcrypt = "==4.0.1"
-python-jose = {extras = ["cryptography"], version = "^3.3.0"}
-passlib = "^1.7.4"
-alembic = "^1.13.1"
-sqlalchemy-utils = "^0.41.2"
-asyncpg = "^0.29.0"
-aiosqlite = "^0.20.0"
-aiomysql = "^0.2.0"
-redis = {extras = ["hiredis"], version = "^5.0.3"}
-eval-type-backport = "^0.1.3"
-diskcache = "^5.6.3"
-
-[tool.poetry.group.test.dependencies]
-pytest = "^8.1.1"
-httpx = "^0.27.0"
-coverage = "^7.4.4"
-
-[tool.poetry.group.docs.dependencies]
-mkdocs = "*"
-
-[tool.poetry.scripts]
-[[tool.poetry.source]]
-name = "tsinghua"
-url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
-priority = "primary"
-
-[tool.coverage.run]
-parallel = true
-branch = true
-source = ["src/fss", "src/tests"]
-
-[tool.coverage.report]
-show_missing = true
+[build-system]
+build-backend = "poetry.core.masonry.api"
+requires = [
+  "poetry-core",
+]
+
+[tool.poetry]
+name = "fastapi-sqlmodel-starter"
+version = "1.0.0-beta.1"
+description = "Fss aims to be one of top scaffold in PyWeb."
+license = "MIT"
+authors = [
+  "tyvekZhang <tyvekzhang@gmail.com>",
+]
+maintainers = [
+  "tyvekZhang <tyvekzhang@gmail.com>",
+]
+readme = "README.md"
+homepage = "https://github.com/tyvekzhang/fastapi-sqlmodel-starter"
+repository = "https://github.com/tyvekzhang/fastapi-sqlmodel-starter"
+documentation = "https://github.com/tyvekzhang/fastapi-sqlmodel-starter/wiki"
+keywords = ["fastapi", "sqlmodel", "tools", "web", "scaffold"]
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: Implementation :: CPython",
+  "Programming Language :: Python :: Implementation :: PyPy",
+]
+packages = [
+  { include = "src"},
+]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+loguru = "^0.7.2"
+fastapi = "^0.110.0"
+fastapi-pagination = "^0.12.21"
+fastapi-async-sqlalchemy = "^0.6.1"
+fastapi-offline = "^1.7.1"
+uvicorn = "^0.29.0"
+sqlmodel = "^0.0.16"
+python-dotenv = "^1.0.1"
+python-multipart = "^0.0.9"
+bcrypt = "==4.0.1"
+python-jose = {extras = ["cryptography"], version = "^3.3.0"}
+passlib = "^1.7.4"
+alembic = "^1.13.1"
+sqlalchemy-utils = "^0.41.2"
+asyncpg = "^0.29.0"
+aiosqlite = "^0.20.0"
+aiomysql = "^0.2.0"
+redis = {extras = ["hiredis"], version = "^5.0.3"}
+eval-type-backport = "^0.1.3"
+diskcache = "^5.6.3"
+pandas = "^2.2.2"
+xlsxwriter = "^3.2.0"
+openpyxl = "^3.1.2"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^8.1.1"
+httpx = "^0.27.0"
+coverage = "^7.4.4"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "*"
+
+[tool.poetry.scripts]
+[[tool.poetry.source]]
+name = "tsinghua"
+url = "https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple/"
+priority = "primary"
+
+[tool.coverage.run]
+parallel = true
+branch = true
+source = ["src/fss", "src/tests"]
+
+[tool.coverage.report]
+show_missing = true
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/README.md` & `fastapi_sqlmodel_starter-1.0.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    </h1>
    <p>
      <img src="https://raw.githubusercontent.com/tyvekzhang/fastapi-sqlmodel-starter/main/docs/img/logo.png" alt="logo" style="vertical-align:middle; margin: 0.5%"/>
    </p>
    <p>
      <img alt="GitHub License" src="https://img.shields.io/github/license/tyvekzhang/fastapi-sqlmodel-starter">
      <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/fastapi-sqlmodel-starter">
-     <img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/tyvekzhang/fastapi-sqlmodel-starter/ci.yaml">
+     <img alt="CI" src="https://github.com/tyvekzhang/fastapi-sqlmodel-starter/actions/workflows/ci.yaml/badge.svg">
      <img alt="Codecov" src="https://img.shields.io/codecov/c/github/tyvekzhang/fastapi-sqlmodel-starter">
      <img alt="Read the Docs" src="https://img.shields.io/readthedocs/fastapi-sqlmodel-starter">
    </p>
    <h4>
       <p>
         <b>简体中文</b> |
         <a href="https://github.com/tyvekzhang/fastapi-sqlmodel-starter/blob/main/docs/README_en.md">English</a>
@@ -27,15 +27,15 @@
 ## 特性
 
 - 开箱即用, 内置常见数据库、缓存([默认]Sqlite, PostgreSQL, MySQL, [默认]文件缓存, Redis)
 - 自带单表的几乎所有操作
 - 数据库迁移, 静态代码扫描, 接口文档等一众特性
 
 ## 快速开始
-1. 首先确保python的版本是3.8及以上的
+1. 首先确保python的版本是3.9及以上的
 2. 克隆代码
 ```shell
 git clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter
 cd fastapi-sqlmodel-starter/src
 ```
 3. [可选]创建虚拟环境, 本篇以venv为例, 类似的工具还有conda, virtualenv等
 ```shell
@@ -53,14 +53,15 @@
 ```shell
 alembic upgrade head
 ```
 7. 启动
    - Windows: python3 fss\apiserver.py
    - macOS 或 Linux: python3 fss/apiserver.py
 8. 访问: http://127.0.0.1:9010/docs
+9. 首先通过注册接口新建用户, 接着进行认证, 一切Ok.
 ## 文档
 - https://fastapi-sqlmodel-starter.readthedocs.io/en/latest/
 ## 贡献
 
 欢迎为 FastapiSqlmodelStarter 做出贡献！你可以通过以下方式参与：
 
 - 提交 Bug 或功能需求到 [Issue 追踪器](https://github.com/tyvekzhang/fastapi-sqlmodel-starter/issues)
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
                  ************ FFaassttAAPPII SSqqllmmooddeell SSttaarrtteerr ((FFssss)) ************
                                     [logo]
-    [GitHub License][PyPI - Python Version][GitHub Actions Workflow Status]
-                           [Codecov][Read the Docs]
+      [GitHub License][PyPI - Python Version][CI][Codecov][Read the Docs]
                         ****** ?ç?®??ä?½??ä?¸?­?æ?? || _EE_nn_gg_ll_ii_ss_hh ******
               ******** PPyyWWeebb?é?¢??å???æ???å?¥?½?ç??¨?ç???è???æ???æ??¶?ä?¹??ä?¸??ã?? ********
 ## ç¹æ§ - å¼ç®±å³ç¨, åç½®å¸¸è§æ°æ®åºãç¼å­([é»è®¤]Sqlite,
 PostgreSQL, MySQL, [é»è®¤]æä»¶ç¼å­, Redis) -
 èªå¸¦åè¡¨çå ä¹æææä½ - æ°æ®åºè¿ç§», éæä»£ç æ«æ,
 æ¥å£ææ¡£ç­ä¸ä¼ç¹æ§ ## å¿«éå¼å§ 1.
-é¦åç¡®ä¿pythonççæ¬æ¯3.8åä»¥ä¸ç 2. åéä»£ç  ```shell git
+é¦åç¡®ä¿pythonççæ¬æ¯3.9åä»¥ä¸ç 2. åéä»£ç  ```shell git
 clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter cd fastapi-
 sqlmodel-starter/src ``` 3. [å¯é]åå»ºèæç¯å¢, æ¬ç¯ä»¥venvä¸ºä¾,
 ç±»ä¼¼çå·¥å·è¿æconda, virtualenvç­ ```shell python3 -m venv .env_fss ```
 4. [å¯é]æ¿æ´»èæç¯å¢ - Windows: .env_fss\Scripts\activate - macOS æ
 Linux: source .env_fss/bin/activate 5. å®è£ Poetryå¹¶ä¸è½½ä¾èµ ```shell
 pip install poetry --trusted-host=mirrors.tuna.tsinghua.edu.cn --index-
 url=https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple poetry install ``` 6.
 æ°æ®åºè¿ç§» ```shell alembic upgrade head ``` 7. å¯å¨ - Windows: python3
 fss\apiserver.py - macOS æ Linux: python3 fss/apiserver.py 8. è®¿é®: http://
-127.0.0.1:9010/docs ## ææ¡£ - https://fastapi-sqlmodel-
+127.0.0.1:9010/docs 9. é¦åéè¿æ³¨åæ¥å£æ°å»ºç¨æ·,
+æ¥çè¿è¡è®¤è¯, ä¸åOk. ## ææ¡£ - https://fastapi-sqlmodel-
 starter.readthedocs.io/en/latest/ ## è´¡ç® æ¬¢è¿ä¸º FastapiSqlmodelStarter
 ååºè´¡ç®ï¼ä½ å¯ä»¥éè¿ä»¥ä¸æ¹å¼åä¸ï¼ - æäº¤ Bug
 æåè½éæ±å° [Issue è¿½è¸ªå¨](https://github.com/tyvekzhang/fastapi-
 sqlmodel-starter/issues) - æäº¤ä»£ç æ¹è¿ç Pull Request -
 ç¼ååæ¹è¿ææ¡£ - åäº«ä½ ä½¿ç¨ FastapiSqlmodelStarter
 çç»éªåæ³æ³ ## è®¸å¯è¯ FastapiSqlmodelStarter éç¨ [MIT è®¸å¯è¯]
 (https://opensource.org/licenses/MIT)å¼æºã
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/.env.example` & `fastapi_sqlmodel_starter-1.0.0b1/src/.env.example`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/alembic.ini` & `fastapi_sqlmodel_starter-1.0.0b1/src/alembic.ini`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/Dockerfile` & `fastapi_sqlmodel_starter-1.0.0b1/src/Dockerfile`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/__pycache__/config.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/__pycache__/config.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xde4b1566 (Tue Apr  9 14:08:30 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 1926
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/__pycache__/cache.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/cache.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 1078
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/__pycache__/page_cache.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/__pycache__/page_cache.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 994
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/cache.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/cache.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/page_cache.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/page_cache.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/cache/redis_cache.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/config.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/enum/__pycache__/enum.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/enum/__pycache__/enum.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xde4b1566 (Tue Apr  9 14:08:30 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 481
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/exception/__pycache__/exception.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/exception/__pycache__/exception.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9b601366 (Mon Apr  8 03:12:27 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 428
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__pycache__/base_mapper.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_mapper.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 2521
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__pycache__/base_model.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/base_model.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 814
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/__pycache__/sqlmodel_impl.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
-files sz: 6960
+moddate:  0xba1e1a66 (Sat Apr 13 05:57:14 2024 UTC)
+files sz: 7039
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a036d045a046d055a056d
@@ -190,21 +190,21 @@
             0f640e6405640f9c026410650d6506190000000000000000006411650b64
             0865066403650d6506190000000000000000006608641284065a10640564
             069c01640865066403650b6604641384065a1164146415640564169c0364
             17650b6418650b64196506640865066403650d6506190000000000000000
             00660a641a84065a1264146415640564169c036417650b6418650b641965
             06641b6506641c6506640865066403650d65061900000000000000000066
             0e641d84065a13640564069c01641e650664196506640865066403650d65
-            06190000000000000000006608641f84065a14640564069c01641e650664
-            196506641b6506641c6506640865066403650d6506190000000000000000
-            00660c642084065a15640564069c0164076506640865066403650b660664
-            2184065a16640564069c01640a650d650619000000000000000000640865
-            066403650b6606642284065a17640564069c01640c650664086506640365
-            0b6606642384065a18640564069c016410650d6506190000000000000000
-            00640865066403650b6606642484065a1964055300
+            06190000000000000000006608641f84065a14640564056405640564209c
+            04641e650664196506641b6506641c6506640865066403650d6506190000
+            00000000000000660c642184065a15640564069c01640765066408650664
+            03650b6606642284065a16640564069c01640a650d650619000000000000
+            000000640865066403650b6606642384065a17640564069c01640c650664
+            0865066403650b6606642484065a18640564069c016410650d6506190000
+            00000000000000640865066403650b6606642584065a1964055300
           21           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('SqlModelMapper')
                        8 STORE_NAME               2 (__qualname__)
          
           22          10 LOAD_CONST               1 ('model')
@@ -273,283 +273,289 @@
           42         144 LOAD_NAME               11 (int)
          
           40         146 BUILD_TUPLE              6
                      148 LOAD_CONST              11 (<code object insert_batch, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 40>)
                      150 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      152 STORE_NAME              14 (insert_batch)
          
-          54         154 LOAD_CONST               5 (None)
+          51         154 LOAD_CONST               5 (None)
                      156 LOAD_CONST               6 (('db_session',))
                      158 BUILD_CONST_KEY_MAP      1
                      160 LOAD_CONST              12 ('id')
                      162 LOAD_NAME                6 (Any)
                      164 LOAD_CONST               8 ('db_session')
                      166 LOAD_NAME                6 (Any)
                      168 LOAD_CONST               3 ('return')
                      170 LOAD_NAME                6 (Any)
                      172 BUILD_TUPLE              6
-                     174 LOAD_CONST              13 (<code object select_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 54>)
+                     174 LOAD_CONST              13 (<code object select_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 51>)
                      176 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      178 STORE_NAME              15 (select_by_id)
          
-          61         180 LOAD_CONST              14 (1000)
+          58         180 LOAD_CONST              14 (1000)
                      182 LOAD_CONST               5 (None)
          
-          60         184 LOAD_CONST              15 (('batch_size', 'db_session'))
+          57         184 LOAD_CONST              15 (('batch_size', 'db_session'))
                      186 BUILD_CONST_KEY_MAP      2
                      188 LOAD_CONST              16 ('ids')
          
-          61         190 LOAD_NAME               13 (List)
+          58         190 LOAD_NAME               13 (List)
                      192 LOAD_NAME                6 (Any)
                      194 BINARY_SUBSCR
          
-          60         204 LOAD_CONST              17 ('batch_size')
+          57         204 LOAD_CONST              17 ('batch_size')
          
-          61         206 LOAD_NAME               11 (int)
+          58         206 LOAD_NAME               11 (int)
          
-          60         208 LOAD_CONST               8 ('db_session')
+          57         208 LOAD_CONST               8 ('db_session')
          
-          61         210 LOAD_NAME                6 (Any)
+          58         210 LOAD_NAME                6 (Any)
          
-          60         212 LOAD_CONST               3 ('return')
+          57         212 LOAD_CONST               3 ('return')
          
-          62         214 LOAD_NAME               13 (List)
+          59         214 LOAD_NAME               13 (List)
                      216 LOAD_NAME                6 (Any)
                      218 BINARY_SUBSCR
          
-          60         228 BUILD_TUPLE              8
-                     230 LOAD_CONST              18 (<code object select_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 60>)
+          57         228 BUILD_TUPLE              8
+                     230 LOAD_CONST              18 (<code object select_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 57>)
                      232 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      234 STORE_NAME              16 (select_by_ids)
          
-          72         236 LOAD_CONST               5 (None)
+          69         236 LOAD_CONST               5 (None)
                      238 LOAD_CONST               6 (('db_session',))
                      240 BUILD_CONST_KEY_MAP      1
                      242 LOAD_CONST               8 ('db_session')
                      244 LOAD_NAME                6 (Any)
                      246 LOAD_CONST               3 ('return')
                      248 LOAD_NAME               11 (int)
                      250 BUILD_TUPLE              4
-                     252 LOAD_CONST              19 (<code object select_count, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 72>)
+                     252 LOAD_CONST              19 (<code object select_count, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 69>)
                      254 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      256 STORE_NAME              17 (select_count)
          
-          80         258 LOAD_CONST              20 (1)
+          77         258 LOAD_CONST              20 (1)
                      260 LOAD_CONST              21 (100)
                      262 LOAD_CONST               5 (None)
          
-          79         264 LOAD_CONST              22 (('page', 'size', 'db_session'))
+          76         264 LOAD_CONST              22 (('page', 'size', 'db_session'))
                      266 BUILD_CONST_KEY_MAP      3
                      268 LOAD_CONST              23 ('page')
          
-          80         270 LOAD_NAME               11 (int)
+          77         270 LOAD_NAME               11 (int)
          
-          79         272 LOAD_CONST              24 ('size')
+          76         272 LOAD_CONST              24 ('size')
          
-          80         274 LOAD_NAME               11 (int)
+          77         274 LOAD_NAME               11 (int)
          
-          79         276 LOAD_CONST              25 ('query')
+          76         276 LOAD_CONST              25 ('query')
          
-          80         278 LOAD_NAME                6 (Any)
+          77         278 LOAD_NAME                6 (Any)
          
-          79         280 LOAD_CONST               8 ('db_session')
+          76         280 LOAD_CONST               8 ('db_session')
          
-          80         282 LOAD_NAME                6 (Any)
+          77         282 LOAD_NAME                6 (Any)
          
-          79         284 LOAD_CONST               3 ('return')
+          76         284 LOAD_CONST               3 ('return')
          
-          81         286 LOAD_NAME               13 (List)
+          78         286 LOAD_NAME               13 (List)
                      288 LOAD_NAME                6 (Any)
                      290 BINARY_SUBSCR
          
-          79         300 BUILD_TUPLE             10
-                     302 LOAD_CONST              26 (<code object select_list, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 79>)
+          76         300 BUILD_TUPLE             10
+                     302 LOAD_CONST              26 (<code object select_list, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 76>)
                      304 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      306 STORE_NAME              18 (select_list)
          
-          96         308 LOAD_CONST              20 (1)
+          93         308 LOAD_CONST              20 (1)
          
-          97         310 LOAD_CONST              21 (100)
+          94         310 LOAD_CONST              21 (100)
          
-         101         312 LOAD_CONST               5 (None)
+          98         312 LOAD_CONST               5 (None)
          
-          93         314 LOAD_CONST              22 (('page', 'size', 'db_session'))
+          90         314 LOAD_CONST              22 (('page', 'size', 'db_session'))
                      316 BUILD_CONST_KEY_MAP      3
                      318 LOAD_CONST              23 ('page')
          
-          96         320 LOAD_NAME               11 (int)
+          93         320 LOAD_NAME               11 (int)
          
-          93         322 LOAD_CONST              24 ('size')
+          90         322 LOAD_CONST              24 ('size')
          
-          97         324 LOAD_NAME               11 (int)
+          94         324 LOAD_NAME               11 (int)
          
-          93         326 LOAD_CONST              25 ('query')
+          90         326 LOAD_CONST              25 ('query')
          
-          98         328 LOAD_NAME                6 (Any)
+          95         328 LOAD_NAME                6 (Any)
          
-          93         330 LOAD_CONST              27 ('order_by')
+          90         330 LOAD_CONST              27 ('order_by')
          
-          99         332 LOAD_NAME                6 (Any)
+          96         332 LOAD_NAME                6 (Any)
          
-          93         334 LOAD_CONST              28 ('sort_order')
+          90         334 LOAD_CONST              28 ('sort_order')
          
-         100         336 LOAD_NAME                6 (Any)
+          97         336 LOAD_NAME                6 (Any)
          
-          93         338 LOAD_CONST               8 ('db_session')
+          90         338 LOAD_CONST               8 ('db_session')
          
-         101         340 LOAD_NAME                6 (Any)
+          98         340 LOAD_NAME                6 (Any)
          
-          93         342 LOAD_CONST               3 ('return')
+          90         342 LOAD_CONST               3 ('return')
          
-         102         344 LOAD_NAME               13 (List)
+          99         344 LOAD_NAME               13 (List)
                      346 LOAD_NAME                6 (Any)
                      348 BINARY_SUBSCR
          
-          93         358 BUILD_TUPLE             14
-                     360 LOAD_CONST              29 (<code object select_list_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 93>)
+          90         358 BUILD_TUPLE             14
+                     360 LOAD_CONST              29 (<code object select_list_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 90>)
                      362 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      364 STORE_NAME              19 (select_list_ordered)
          
-         125         366 LOAD_CONST               5 (None)
+         122         366 LOAD_CONST               5 (None)
          
-         124         368 LOAD_CONST               6 (('db_session',))
+         121         368 LOAD_CONST               6 (('db_session',))
                      370 BUILD_CONST_KEY_MAP      1
                      372 LOAD_CONST              30 ('params')
          
-         125         374 LOAD_NAME                6 (Any)
+         122         374 LOAD_NAME                6 (Any)
          
-         124         376 LOAD_CONST              25 ('query')
+         121         376 LOAD_CONST              25 ('query')
          
-         125         378 LOAD_NAME                6 (Any)
+         122         378 LOAD_NAME                6 (Any)
          
-         124         380 LOAD_CONST               8 ('db_session')
+         121         380 LOAD_CONST               8 ('db_session')
          
-         125         382 LOAD_NAME                6 (Any)
+         122         382 LOAD_NAME                6 (Any)
          
-         124         384 LOAD_CONST               3 ('return')
+         121         384 LOAD_CONST               3 ('return')
          
-         126         386 LOAD_NAME               13 (List)
+         123         386 LOAD_NAME               13 (List)
                      388 LOAD_NAME                6 (Any)
                      390 BINARY_SUBSCR
          
-         124         400 BUILD_TUPLE              8
-                     402 LOAD_CONST              31 (<code object select_list_page, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 124>)
+         121         400 BUILD_TUPLE              8
+                     402 LOAD_CONST              31 (<code object select_list_page, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 121>)
                      404 MAKE_FUNCTION            6 (kwdefaults, annotations)
                      406 STORE_NAME              20 (select_list_page)
          
-         140         408 LOAD_CONST               5 (None)
+         134         408 LOAD_CONST               5 (None)
          
-         133         410 LOAD_CONST               6 (('db_session',))
-                     412 BUILD_CONST_KEY_MAP      1
-                     414 LOAD_CONST              30 ('params')
+         135         410 LOAD_CONST               5 (None)
          
-         136         416 LOAD_NAME                6 (Any)
+         136         412 LOAD_CONST               5 (None)
          
-         133         418 LOAD_CONST              25 ('query')
+         137         414 LOAD_CONST               5 (None)
          
-         137         420 LOAD_NAME                6 (Any)
+         130         416 LOAD_CONST              32 (('query', 'order_by', 'sort_order', 'db_session'))
+                     418 BUILD_CONST_KEY_MAP      4
+                     420 LOAD_CONST              30 ('params')
          
-         133         422 LOAD_CONST              27 ('order_by')
+         133         422 LOAD_NAME                6 (Any)
          
-         138         424 LOAD_NAME                6 (Any)
+         130         424 LOAD_CONST              25 ('query')
          
-         133         426 LOAD_CONST              28 ('sort_order')
+         134         426 LOAD_NAME                6 (Any)
          
-         139         428 LOAD_NAME                6 (Any)
+         130         428 LOAD_CONST              27 ('order_by')
          
-         133         430 LOAD_CONST               8 ('db_session')
+         135         430 LOAD_NAME                6 (Any)
          
-         140         432 LOAD_NAME                6 (Any)
+         130         432 LOAD_CONST              28 ('sort_order')
          
-         133         434 LOAD_CONST               3 ('return')
+         136         434 LOAD_NAME                6 (Any)
          
-         141         436 LOAD_NAME               13 (List)
-                     438 LOAD_NAME                6 (Any)
-                     440 BINARY_SUBSCR
+         130         436 LOAD_CONST               8 ('db_session')
          
-         133         450 BUILD_TUPLE             12
-                     452 LOAD_CONST              32 (<code object select_list_page_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 133>)
-                     454 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     456 STORE_NAME              21 (select_list_page_ordered)
+         137         438 LOAD_NAME                6 (Any)
          
-         153         458 LOAD_CONST               5 (None)
-                     460 LOAD_CONST               6 (('db_session',))
-                     462 BUILD_CONST_KEY_MAP      1
-                     464 LOAD_CONST               7 ('data')
-                     466 LOAD_NAME                6 (Any)
-                     468 LOAD_CONST               8 ('db_session')
-                     470 LOAD_NAME                6 (Any)
-                     472 LOAD_CONST               3 ('return')
-                     474 LOAD_NAME               11 (int)
-                     476 BUILD_TUPLE              6
-                     478 LOAD_CONST              33 (<code object update_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 153>)
-                     480 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     482 STORE_NAME              22 (update_by_id)
+         130         440 LOAD_CONST               3 ('return')
          
-         166         484 LOAD_CONST               5 (None)
+         138         442 LOAD_NAME               13 (List)
+                     444 LOAD_NAME                6 (Any)
+                     446 BINARY_SUBSCR
          
-         165         486 LOAD_CONST               6 (('db_session',))
-                     488 BUILD_CONST_KEY_MAP      1
-                     490 LOAD_CONST              10 ('data_list')
+         130         456 BUILD_TUPLE             12
+                     458 LOAD_CONST              33 (<code object select_list_page_ordered, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 130>)
+                     460 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     462 STORE_NAME              21 (select_list_page_ordered)
          
-         166         492 LOAD_NAME               13 (List)
-                     494 LOAD_NAME                6 (Any)
-                     496 BINARY_SUBSCR
+         150         464 LOAD_CONST               5 (None)
+                     466 LOAD_CONST               6 (('db_session',))
+                     468 BUILD_CONST_KEY_MAP      1
+                     470 LOAD_CONST               7 ('data')
+                     472 LOAD_NAME                6 (Any)
+                     474 LOAD_CONST               8 ('db_session')
+                     476 LOAD_NAME                6 (Any)
+                     478 LOAD_CONST               3 ('return')
+                     480 LOAD_NAME               11 (int)
+                     482 BUILD_TUPLE              6
+                     484 LOAD_CONST              34 (<code object update_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 150>)
+                     486 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     488 STORE_NAME              22 (update_by_id)
          
-         165         506 LOAD_CONST               8 ('db_session')
+         168         490 LOAD_CONST               5 (None)
          
-         166         508 LOAD_NAME                6 (Any)
+         167         492 LOAD_CONST               6 (('db_session',))
+                     494 BUILD_CONST_KEY_MAP      1
+                     496 LOAD_CONST              10 ('data_list')
          
-         165         510 LOAD_CONST               3 ('return')
+         168         498 LOAD_NAME               13 (List)
+                     500 LOAD_NAME                6 (Any)
+                     502 BINARY_SUBSCR
          
-         167         512 LOAD_NAME               11 (int)
+         167         512 LOAD_CONST               8 ('db_session')
          
-         165         514 BUILD_TUPLE              6
-                     516 LOAD_CONST              34 (<code object update_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 165>)
-                     518 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     520 STORE_NAME              23 (update_batch_by_ids)
+         168         514 LOAD_NAME                6 (Any)
          
-         179         522 LOAD_CONST               5 (None)
-                     524 LOAD_CONST               6 (('db_session',))
-                     526 BUILD_CONST_KEY_MAP      1
-                     528 LOAD_CONST              12 ('id')
-                     530 LOAD_NAME                6 (Any)
-                     532 LOAD_CONST               8 ('db_session')
-                     534 LOAD_NAME                6 (Any)
-                     536 LOAD_CONST               3 ('return')
-                     538 LOAD_NAME               11 (int)
-                     540 BUILD_TUPLE              6
-                     542 LOAD_CONST              35 (<code object delete_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 179>)
-                     544 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     546 STORE_NAME              24 (delete_by_id)
+         167         516 LOAD_CONST               3 ('return')
          
-         189         548 LOAD_CONST               5 (None)
+         169         518 LOAD_NAME               11 (int)
          
-         188         550 LOAD_CONST               6 (('db_session',))
-                     552 BUILD_CONST_KEY_MAP      1
-                     554 LOAD_CONST              16 ('ids')
+         167         520 BUILD_TUPLE              6
+                     522 LOAD_CONST              35 (<code object update_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 167>)
+                     524 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     526 STORE_NAME              23 (update_batch_by_ids)
          
-         189         556 LOAD_NAME               13 (List)
-                     558 LOAD_NAME                6 (Any)
-                     560 BINARY_SUBSCR
+         181         528 LOAD_CONST               5 (None)
+                     530 LOAD_CONST               6 (('db_session',))
+                     532 BUILD_CONST_KEY_MAP      1
+                     534 LOAD_CONST              12 ('id')
+                     536 LOAD_NAME                6 (Any)
+                     538 LOAD_CONST               8 ('db_session')
+                     540 LOAD_NAME                6 (Any)
+                     542 LOAD_CONST               3 ('return')
+                     544 LOAD_NAME               11 (int)
+                     546 BUILD_TUPLE              6
+                     548 LOAD_CONST              36 (<code object delete_by_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 181>)
+                     550 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     552 STORE_NAME              24 (delete_by_id)
          
-         188         570 LOAD_CONST               8 ('db_session')
+         189         554 LOAD_CONST               5 (None)
          
-         189         572 LOAD_NAME                6 (Any)
+         188         556 LOAD_CONST               6 (('db_session',))
+                     558 BUILD_CONST_KEY_MAP      1
+                     560 LOAD_CONST              16 ('ids')
          
-         188         574 LOAD_CONST               3 ('return')
+         189         562 LOAD_NAME               13 (List)
+                     564 LOAD_NAME                6 (Any)
+                     566 BINARY_SUBSCR
          
-         190         576 LOAD_NAME               11 (int)
+         188         576 LOAD_CONST               8 ('db_session')
          
-         188         578 BUILD_TUPLE              6
-                     580 LOAD_CONST              36 (<code object delete_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 188>)
-                     582 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     584 STORE_NAME              25 (delete_batch_by_ids)
-                     586 LOAD_CONST               5 (None)
-                     588 RETURN_VALUE
+         189         578 LOAD_NAME                6 (Any)
+         
+         188         580 LOAD_CONST               3 ('return')
+         
+         190         582 LOAD_NAME               11 (int)
+         
+         188         584 BUILD_TUPLE              6
+                     586 LOAD_CONST              37 (<code object delete_batch_by_ids, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 188>)
+                     588 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     590 STORE_NAME              25 (delete_batch_by_ids)
+                     592 LOAD_CONST               5 (None)
+                     594 RETURN_VALUE
          consts
             'SqlModelMapper'
             'model'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
@@ -652,146 +658,106 @@
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'insert'
                firstlineno 29
                lnotab 0x06061c0134012a01
             'data_list'
             code
                argcount  : 1
-               nlocals   : 5
-               stacksize : 4
+               nlocals   : 6
+               stacksize : 6
                flags     : 131
                code
-                  0x87004b00010097007c02700b89006a0000000000000000006a01000000
-                  00000000007d0288006601640184087c014400a6000000ab000000000000
-                  0000007d0374050000000000000000000089006a030000000000000000a6
-                  010000ab010000000000000000a004000000000000000000000000000000
-                  0000000000640284007c034400a6000000ab000000000000000000a60100
-                  00ab0100000000000000007d047c02a00500000000000000000000000000
-                  000000000000007c04a6010000ab010000000000000000830064007b0356
-                  00970386040100740d000000000000000000007c01a6010000ab01000000
-                  00000000005300
-                             0 MAKE_CELL                0 (self)
-               
-                40           2 RETURN_GENERATOR
-                             4 POP_TOP
-                             6 RESUME                   0
-               
-                43           8 LOAD_FAST                2 (db_session)
-                            10 JUMP_IF_TRUE_OR_POP     11 (to 34)
-                            12 LOAD_DEREF               0 (self)
-                            14 LOAD_ATTR                0 (db)
-                            24 LOAD_ATTR                1 (session)
-                       >>   34 STORE_FAST               2 (db_session)
-               
-                44          36 LOAD_CLOSURE             0 (self)
-                            38 BUILD_TUPLE              1
-                            40 LOAD_CONST               1 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 44>)
-                            42 MAKE_FUNCTION            8 (closure)
-               
-                48          44 LOAD_FAST                1 (data_list)
-               
-                44          46 GET_ITER
-                            48 PRECALL                  0
-                            52 CALL                     0
-                            62 STORE_FAST               3 (orm_datas)
-               
-                50          64 LOAD_GLOBAL              5 (NULL + insert)
-                            76 LOAD_DEREF               0 (self)
-                            78 LOAD_ATTR                3 (model)
-                            88 PRECALL                  1
-                            92 CALL                     1
-                           102 LOAD_METHOD              4 (values)
-                           124 LOAD_CONST               2 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 50>)
-                           126 MAKE_FUNCTION            0
-                           128 LOAD_FAST                3 (orm_datas)
-                           130 GET_ITER
-                           132 PRECALL                  0
-                           136 CALL                     0
-                           146 PRECALL                  1
-                           150 CALL                     1
-                           160 STORE_FAST               4 (statement)
-               
-                51         162 LOAD_FAST                2 (db_session)
-                           164 LOAD_METHOD              5 (execute)
-                           186 LOAD_FAST                4 (statement)
-                           188 PRECALL                  1
-                           192 CALL                     1
-                           202 GET_AWAITABLE            0
-                           204 LOAD_CONST               0 (None)
-                       >>  206 SEND                     3 (to 214)
-                           208 YIELD_VALUE
-                           210 RESUME                   3
-                           212 JUMP_BACKWARD_NO_INTERRUPT     4 (to 206)
-                       >>  214 POP_TOP
+                  0x4b00010097007c02700b7c006a0000000000000000006a010000000000
+                  0000007d0267007d037c0144005d2f7d047c03a002000000000000000000
+                  00000000000000000000007c006a030000000000000000a0040000000000
+                  0000000000000000000000000000007c04a6010000ab0100000000000000
+                  00a6010000ab01000000000000000001008c30740b000000000000000000
+                  007c006a030000000000000000a6010000ab010000000000000000a00600
+                  00000000000000000000000000000000000000640184007c034400a60000
+                  00ab000000000000000000a6010000ab0100000000000000007d057c02a0
+                  0700000000000000000000000000000000000000007c05a6010000ab0100
+                  00000000000000830064007b035600970386040100741100000000000000
+                  0000007c01a6010000ab0100000000000000005300
+                40           0 RETURN_GENERATOR
+                             2 POP_TOP
+                             4 RESUME                   0
                
-                52         216 LOAD_GLOBAL             13 (NULL + len)
-                           228 LOAD_FAST                1 (data_list)
-                           230 PRECALL                  1
-                           234 CALL                     1
-                           244 RETURN_VALUE
+                43           6 LOAD_FAST                2 (db_session)
+                             8 JUMP_IF_TRUE_OR_POP     11 (to 32)
+                            10 LOAD_FAST                0 (self)
+                            12 LOAD_ATTR                0 (db)
+                            22 LOAD_ATTR                1 (session)
+                       >>   32 STORE_FAST               2 (db_session)
+               
+                44          34 BUILD_LIST               0
+                            36 STORE_FAST               3 (orm_datas)
+               
+                45          38 LOAD_FAST                1 (data_list)
+                            40 GET_ITER
+                       >>   42 FOR_ITER                47 (to 138)
+                            44 STORE_FAST               4 (data)
+               
+                46          46 LOAD_FAST                3 (orm_datas)
+                            48 LOAD_METHOD              2 (append)
+                            70 LOAD_FAST                0 (self)
+                            72 LOAD_ATTR                3 (model)
+                            82 LOAD_METHOD              4 (model_validate)
+                           104 LOAD_FAST                4 (data)
+                           106 PRECALL                  1
+                           110 CALL                     1
+                           120 PRECALL                  1
+                           124 CALL                     1
+                           134 POP_TOP
+                           136 JUMP_BACKWARD           48 (to 42)
+               
+                47     >>  138 LOAD_GLOBAL             11 (NULL + insert)
+                           150 LOAD_FAST                0 (self)
+                           152 LOAD_ATTR                3 (model)
+                           162 PRECALL                  1
+                           166 CALL                     1
+                           176 LOAD_METHOD              6 (values)
+                           198 LOAD_CONST               1 (<code object <listcomp>, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\persistence\sqlmodel_impl.py", line 47>)
+                           200 MAKE_FUNCTION            0
+                           202 LOAD_FAST                3 (orm_datas)
+                           204 GET_ITER
+                           206 PRECALL                  0
+                           210 CALL                     0
+                           220 PRECALL                  1
+                           224 CALL                     1
+                           234 STORE_FAST               5 (statement)
+               
+                48         236 LOAD_FAST                2 (db_session)
+                           238 LOAD_METHOD              7 (execute)
+                           260 LOAD_FAST                5 (statement)
+                           262 PRECALL                  1
+                           266 CALL                     1
+                           276 GET_AWAITABLE            0
+                           278 LOAD_CONST               0 (None)
+                       >>  280 SEND                     3 (to 288)
+                           282 YIELD_VALUE
+                           284 RESUME                   3
+                           286 JUMP_BACKWARD_NO_INTERRUPT     4 (to 280)
+                       >>  288 POP_TOP
+               
+                49         290 LOAD_GLOBAL             17 (NULL + len)
+                           302 LOAD_FAST                1 (data_list)
+                           304 PRECALL                  1
+                           308 CALL                     1
+                           318 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
-                     stacksize : 6
-                     flags     : 19
-                     code
-                        0x9501970067007c005d337d017401000000000000000000007c0189026a
-                        010000000000000000a6020000ab020000000000000000731a89026a0100
-                        00000000000000a00200000000000000000000000000000000000000007c
-                        01a6010000ab0100000000000000006e017c0191028c345300
-                                   0 COPY_FREE_VARS           1
-                     
-                      44           2 RESUME                   0
-                                   4 BUILD_LIST               0
-                                   6 LOAD_FAST                0 (.0)
-                             >>    8 FOR_ITER                51 (to 112)
-                     
-                      48          10 STORE_FAST               1 (data)
-                     
-                      46          12 LOAD_GLOBAL              1 (NULL + isinstance)
-                                  24 LOAD_FAST                1 (data)
-                                  26 LOAD_DEREF               2 (self)
-                                  28 LOAD_ATTR                1 (model)
-                                  38 PRECALL                  2
-                                  42 CALL                     2
-                     
-                      45          52 POP_JUMP_FORWARD_IF_TRUE    26 (to 106)
-                                  54 LOAD_DEREF               2 (self)
-                                  56 LOAD_ATTR                1 (model)
-                                  66 LOAD_METHOD              2 (model_validate)
-                                  88 LOAD_FAST                1 (data)
-                                  90 PRECALL                  1
-                                  94 CALL                     1
-                                 104 JUMP_FORWARD             1 (to 108)
-                     
-                      47     >>  106 LOAD_FAST                1 (data)
-                     
-                      44     >>  108 LIST_APPEND              2
-                                 110 JUMP_BACKWARD           52 (to 8)
-                             >>  112 RETURN_VALUE
-                     consts
-                     names      ('isinstance', 'model', 'model_validate')
-                     varnames   ('.0', 'data')
-                     freevars   ('self',)
-                     cellvars   ()
-                     filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
-                     name       '<listcomp>'
-                     firstlineno 44
-                     lnotab 0x0a0402fe28ff360202fd
-                  code
-                     argcount  : 1
-                     nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d167d017c01a000000000000000000000000000000000
                         0000000000a6000000ab00000000000000000091028c175300
-                      50           0 RESUME                   0
+                      47           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                22 (to 52)
                                    8 STORE_FAST               1 (data)
                                   10 LOAD_FAST                1 (data)
                                   12 LOAD_METHOD              0 (model_dump)
                                   34 PRECALL                  0
@@ -802,24 +768,24 @@
                      consts
                      names      ('model_dump',)
                      varnames   ('.0', 'data')
                      freevars   ()
                      cellvars   ()
                      filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                      name       '<listcomp>'
-                     firstlineno 50
+                     firstlineno 47
                      lnotab 0x
-               names      ('db', 'session', 'insert', 'model', 'values', 'execute', 'len')
-               varnames   ('self', 'data_list', 'db_session', 'orm_datas', 'statement')
+               names      ('db', 'session', 'append', 'model', 'model_validate', 'insert', 'values', 'execute', 'len')
+               varnames   ('self', 'data_list', 'db_session', 'orm_datas', 'data', 'statement')
                freevars   ()
-               cellvars   ('self',)
+               cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'insert_batch'
                firstlineno 40
-               lnotab 0x08031c01080402fc120662013601
+               lnotab 0x06031c01040108015c0162013601
             'id'
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 4
                flags     : 131
                code
@@ -827,67 +793,67 @@
                   0000007d027405000000000000000000007c006a030000000000000000a6
                   010000ab010000000000000000a004000000000000000000000000000000
                   00000000007c006a0300000000000000006a0500000000000000007c016b
                   0200000000a6010000ab0100000000000000007d037c02a0060000000000
                   0000000000000000000000000000007c03a6010000ab0100000000000000
                   00830064007b035600970386047d047c04a0070000000000000000000000
                   000000000000000000a6000000ab0000000000000000005300
-                54           0 RETURN_GENERATOR
+                51           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                55           6 LOAD_FAST                2 (db_session)
+                52           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-                56          34 LOAD_GLOBAL              5 (NULL + select)
+                53          34 LOAD_GLOBAL              5 (NULL + select)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (model)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (where)
                             94 LOAD_FAST                0 (self)
                             96 LOAD_ATTR                3 (model)
                            106 LOAD_ATTR                5 (id)
                            116 LOAD_FAST                1 (id)
                            118 COMPARE_OP               2 (==)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 STORE_FAST               3 (statement)
                
-                57         140 LOAD_FAST                2 (db_session)
+                54         140 LOAD_FAST                2 (db_session)
                            142 LOAD_METHOD              6 (execute)
                            164 LOAD_FAST                3 (statement)
                            166 PRECALL                  1
                            170 CALL                     1
                            180 GET_AWAITABLE            0
                            182 LOAD_CONST               0 (None)
                        >>  184 SEND                     3 (to 192)
                            186 YIELD_VALUE
                            188 RESUME                   3
                            190 JUMP_BACKWARD_NO_INTERRUPT     4 (to 184)
                        >>  192 STORE_FAST               4 (response)
                
-                58         194 LOAD_FAST                4 (response)
+                55         194 LOAD_FAST                4 (response)
                            196 LOAD_METHOD              7 (scalar_one_or_none)
                            218 PRECALL                  0
                            222 CALL                     0
                            232 RETURN_VALUE
                consts
                   None
                names      ('db', 'session', 'select', 'model', 'where', 'id', 'execute', 'scalar_one_or_none')
                varnames   ('self', 'id', 'db_session', 'statement', 'response')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_by_id'
-               firstlineno 54
+               firstlineno 51
                lnotab 0x06011c016a013601
             1000
             ('batch_size', 'db_session')
             'ids'
             'batch_size'
             code
                argcount  : 1
@@ -905,51 +871,51 @@
                   00a00800000000000000000000000000000000000000007c06a6010000ab
                   010000000000000000a6010000ab0100000000000000007d077c03a00900
                   000000000000000000000000000000000000007c07a6010000ab01000000
                   0000000000a00a0000000000000000000000000000000000000000a60000
                   00ab000000000000000000830064007b035600970386047d087c04a00b00
                   000000000000000000000000000000000000007c08a6010000ab01000000
                   000000000001008c967c045300
-                60           0 RETURN_GENERATOR
+                57           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                63           6 LOAD_FAST                3 (db_session)
+                60           6 LOAD_FAST                3 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               3 (db_session)
                
-                64          34 BUILD_LIST               0
+                61          34 BUILD_LIST               0
                             36 STORE_FAST               4 (result_set)
                
-                65          38 LOAD_GLOBAL              5 (NULL + range)
+                62          38 LOAD_GLOBAL              5 (NULL + range)
                             50 LOAD_CONST               1 (0)
                             52 LOAD_GLOBAL              7 (NULL + len)
                             64 LOAD_FAST                1 (ids)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 LOAD_FAST                2 (batch_size)
                             82 PRECALL                  3
                             86 CALL                     3
                             96 GET_ITER
                        >>   98 FOR_ITER               149 (to 398)
                            100 STORE_FAST               5 (i)
                
-                66         102 LOAD_FAST                1 (ids)
+                63         102 LOAD_FAST                1 (ids)
                            104 LOAD_FAST                5 (i)
                            106 LOAD_FAST                5 (i)
                            108 LOAD_FAST                2 (batch_size)
                            110 BINARY_OP                0 (+)
                            114 BUILD_SLICE              2
                            116 BINARY_SUBSCR
                            126 STORE_FAST               6 (batch_ids)
                
-                67         128 LOAD_GLOBAL              9 (NULL + select)
+                64         128 LOAD_GLOBAL              9 (NULL + select)
                            140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                5 (model)
                            152 PRECALL                  1
                            156 CALL                     1
                            166 LOAD_METHOD              6 (where)
                            188 LOAD_FAST                0 (self)
                            190 LOAD_ATTR                5 (model)
@@ -958,15 +924,15 @@
                            232 LOAD_FAST                6 (batch_ids)
                            234 PRECALL                  1
                            238 CALL                     1
                            248 PRECALL                  1
                            252 CALL                     1
                            262 STORE_FAST               7 (statement)
                
-                68         264 LOAD_FAST                3 (db_session)
+                65         264 LOAD_FAST                3 (db_session)
                            266 LOAD_METHOD              9 (exec)
                            288 LOAD_FAST                7 (statement)
                            290 PRECALL                  1
                            294 CALL                     1
                            304 LOAD_METHOD             10 (all)
                            326 PRECALL                  0
                            330 CALL                     0
@@ -974,34 +940,34 @@
                            342 LOAD_CONST               0 (None)
                        >>  344 SEND                     3 (to 352)
                            346 YIELD_VALUE
                            348 RESUME                   3
                            350 JUMP_BACKWARD_NO_INTERRUPT     4 (to 344)
                        >>  352 STORE_FAST               8 (results)
                
-                69         354 LOAD_FAST                4 (result_set)
+                66         354 LOAD_FAST                4 (result_set)
                            356 LOAD_METHOD             11 (extend)
                            378 LOAD_FAST                8 (results)
                            380 PRECALL                  1
                            384 CALL                     1
                            394 POP_TOP
                            396 JUMP_BACKWARD          150 (to 98)
                
-                70     >>  398 LOAD_FAST                4 (result_set)
+                67     >>  398 LOAD_FAST                4 (result_set)
                            400 RETURN_VALUE
                consts
                   None
                   0
                names      ('db', 'session', 'range', 'len', 'select', 'model', 'where', 'id', 'in_', 'exec', 'all', 'extend')
                varnames   ('self', 'ids', 'batch_size', 'db_session', 'result_set', 'i', 'batch_ids', 'statement', 'results')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_by_ids'
-               firstlineno 60
+               firstlineno 57
                lnotab 0x06031c01040140011a0188015a012c01
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 7
                flags     : 131
                code
@@ -1011,29 +977,29 @@
                   000000a6000000ab000000000000000000a6010000ab0100000000000000
                   00a006000000000000000000000000000000000000000074070000000000
                   00000000007c006a070000000000000000a6010000ab0100000000000000
                   00a0080000000000000000000000000000000000000000a6000000ab0000
                   00000000000000a6010000ab010000000000000000a6010000ab01000000
                   0000000000830064007b035600970386047d027c02a00900000000000000
                   00000000000000000000000000a6000000ab0000000000000000005300
-                72           0 RETURN_GENERATOR
+                69           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                73           6 LOAD_FAST                1 (db_session)
+                70           6 LOAD_FAST                1 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               1 (db_session)
                
-                74          34 LOAD_FAST                1 (db_session)
+                71          34 LOAD_FAST                1 (db_session)
                             36 LOAD_METHOD              2 (execute)
                
-                75          58 LOAD_GLOBAL              7 (NULL + select)
+                72          58 LOAD_GLOBAL              7 (NULL + select)
                             70 LOAD_GLOBAL              9 (NULL + func)
                             82 LOAD_ATTR                5 (count)
                             92 PRECALL                  0
                             96 CALL                     0
                            106 PRECALL                  1
                            110 CALL                     1
                            120 LOAD_METHOD              6 (select_from)
@@ -1044,38 +1010,38 @@
                            170 CALL                     1
                            180 LOAD_METHOD              8 (subquery)
                            202 PRECALL                  0
                            206 CALL                     0
                            216 PRECALL                  1
                            220 CALL                     1
                
-                74         230 PRECALL                  1
+                71         230 PRECALL                  1
                            234 CALL                     1
                            244 GET_AWAITABLE            0
                            246 LOAD_CONST               0 (None)
                        >>  248 SEND                     3 (to 256)
                            250 YIELD_VALUE
                            252 RESUME                   3
                            254 JUMP_BACKWARD_NO_INTERRUPT     4 (to 248)
                        >>  256 STORE_FAST               2 (response)
                
-                77         258 LOAD_FAST                2 (response)
+                74         258 LOAD_FAST                2 (response)
                            260 LOAD_METHOD              9 (scalar_one)
                            282 PRECALL                  0
                            286 CALL                     0
                            296 RETURN_VALUE
                consts
                   None
                names      ('db', 'session', 'execute', 'select', 'func', 'count', 'select_from', 'model', 'subquery', 'scalar_one')
                varnames   ('self', 'db_session', 'response')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_count'
-               firstlineno 72
+               firstlineno 69
                lnotab 0x06011c011801acff1c03
             1
             100
             ('page', 'size', 'db_session')
             'page'
             'size'
             'query'
@@ -1093,71 +1059,71 @@
                   02a6010000ab010000000000000000a00600000000000000000000000000
                   000000000000007c006a0300000000000000006a070000000000000000a6
                   010000ab0100000000000000007d037c04a0080000000000000000000000
                   0000000000000000007c03a6010000ab010000000000000000830064007b
                   035600970386047d057c05a0090000000000000000000000000000000000
                   000000a6000000ab000000000000000000a00a0000000000000000000000
                   000000000000000000a6000000ab0000000000000000005300
-                79           0 RETURN_GENERATOR
+                76           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-                82           6 LOAD_FAST                4 (db_session)
+                79           6 LOAD_FAST                4 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               4 (db_session)
                
-                83          34 LOAD_FAST                3 (query)
+                80          34 LOAD_FAST                3 (query)
                             36 POP_JUMP_FORWARD_IF_NOT_NONE    93 (to 224)
                
-                85          38 LOAD_GLOBAL              5 (NULL + select)
+                82          38 LOAD_GLOBAL              5 (NULL + select)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                3 (model)
                             62 PRECALL                  1
                             66 CALL                     1
                
-                86          76 LOAD_METHOD              4 (offset)
+                83          76 LOAD_METHOD              4 (offset)
                             98 LOAD_FAST                1 (page)
                            100 LOAD_CONST               1 (1)
                            102 BINARY_OP               10 (-)
                            106 LOAD_FAST                2 (size)
                            108 BINARY_OP                5 (*)
                            112 PRECALL                  1
                            116 CALL                     1
                
-                87         126 LOAD_METHOD              5 (limit)
+                84         126 LOAD_METHOD              5 (limit)
                            148 LOAD_FAST                2 (size)
                            150 PRECALL                  1
                            154 CALL                     1
                
-                88         164 LOAD_METHOD              6 (order_by)
+                85         164 LOAD_METHOD              6 (order_by)
                            186 LOAD_FAST                0 (self)
                            188 LOAD_ATTR                3 (model)
                            198 LOAD_ATTR                7 (id)
                            208 PRECALL                  1
                            212 CALL                     1
                
-                84         222 STORE_FAST               3 (query)
+                81         222 STORE_FAST               3 (query)
                
-                90     >>  224 LOAD_FAST                4 (db_session)
+                87     >>  224 LOAD_FAST                4 (db_session)
                            226 LOAD_METHOD              8 (execute)
                            248 LOAD_FAST                3 (query)
                            250 PRECALL                  1
                            254 CALL                     1
                            264 GET_AWAITABLE            0
                            266 LOAD_CONST               0 (None)
                        >>  268 SEND                     3 (to 276)
                            270 YIELD_VALUE
                            272 RESUME                   3
                            274 JUMP_BACKWARD_NO_INTERRUPT     4 (to 268)
                        >>  276 STORE_FAST               5 (response)
                
-                91         278 LOAD_FAST                5 (response)
+                88         278 LOAD_FAST                5 (response)
                            280 LOAD_METHOD              9 (scalars)
                            302 PRECALL                  0
                            306 CALL                     0
                            316 LOAD_METHOD             10 (all)
                            338 PRECALL                  0
                            342 CALL                     0
                            352 RETURN_VALUE
@@ -1166,15 +1132,15 @@
                   1
                names      ('db', 'session', 'select', 'model', 'offset', 'limit', 'order_by', 'id', 'execute', 'scalars', 'all')
                varnames   ('self', 'page', 'size', 'query', 'db_session', 'response')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_list'
-               firstlineno 79
+               firstlineno 76
                lnotab 0x06031c0104022601320126013afc02063601
             'order_by'
             'sort_order'
             code
                argcount  : 1
                nlocals   : 9
                stacksize : 4
@@ -1199,126 +1165,126 @@
                   007c077c0419000000000000000000a00c00000000000000000000000000
                   00000000000000a6000000ab000000000000000000a6010000ab01000000
                   00000000007d037c06a00d00000000000000000000000000000000000000
                   007c03a6010000ab010000000000000000830064007b035600970386047d
                   087c08a00e0000000000000000000000000000000000000000a6000000ab
                   000000000000000000a00f00000000000000000000000000000000000000
                   00a6000000ab0000000000000000005300
-                93           0 RETURN_GENERATOR
+                90           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               103           6 LOAD_FAST                6 (db_session)
+               100           6 LOAD_FAST                6 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               6 (db_session)
                
-               104          34 LOAD_FAST                0 (self)
+               101          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (model)
                             46 LOAD_ATTR                3 (__table__)
                             56 LOAD_ATTR                4 (columns)
                             66 STORE_FAST               7 (columns)
                
-               105          68 LOAD_FAST                4 (order_by)
+               102          68 LOAD_FAST                4 (order_by)
                             70 POP_JUMP_FORWARD_IF_NONE     4 (to 80)
                             72 LOAD_FAST                4 (order_by)
                             74 LOAD_FAST                7 (columns)
                             76 CONTAINS_OP              1
                             78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
                
-               106     >>   80 LOAD_CONST               1 ('id')
+               103     >>   80 LOAD_CONST               1 ('id')
                             82 STORE_FAST               4 (order_by)
                
-               107     >>   84 LOAD_FAST                5 (sort_order)
+               104     >>   84 LOAD_FAST                5 (sort_order)
                             86 LOAD_GLOBAL             10 (SortEnum)
                             98 LOAD_ATTR                6 (ascending)
                            108 COMPARE_OP               2 (==)
                            114 POP_JUMP_FORWARD_IF_FALSE   108 (to 332)
                
-               109         116 LOAD_GLOBAL             15 (NULL + select)
+               106         116 LOAD_GLOBAL             15 (NULL + select)
                            128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                2 (model)
                            140 PRECALL                  1
                            144 CALL                     1
                
-               110         154 LOAD_METHOD              8 (offset)
+               107         154 LOAD_METHOD              8 (offset)
                            176 LOAD_FAST                1 (page)
                            178 LOAD_CONST               2 (1)
                            180 BINARY_OP               10 (-)
                            184 LOAD_FAST                2 (size)
                            186 BINARY_OP                5 (*)
                            190 PRECALL                  1
                            194 CALL                     1
                
-               111         204 LOAD_METHOD              9 (limit)
+               108         204 LOAD_METHOD              9 (limit)
                            226 LOAD_FAST                2 (size)
                            228 PRECALL                  1
                            232 CALL                     1
                
-               112         242 LOAD_METHOD             10 (order_by)
+               109         242 LOAD_METHOD             10 (order_by)
                            264 LOAD_FAST                7 (columns)
                            266 LOAD_FAST                4 (order_by)
                            268 BINARY_SUBSCR
                            278 LOAD_METHOD             11 (asc)
                            300 PRECALL                  0
                            304 CALL                     0
                            314 PRECALL                  1
                            318 CALL                     1
                
-               108         328 STORE_FAST               3 (query)
+               105         328 STORE_FAST               3 (query)
                            330 JUMP_FORWARD           107 (to 546)
                
-               116     >>  332 LOAD_GLOBAL             15 (NULL + select)
+               113     >>  332 LOAD_GLOBAL             15 (NULL + select)
                            344 LOAD_FAST                0 (self)
                            346 LOAD_ATTR                2 (model)
                            356 PRECALL                  1
                            360 CALL                     1
                
-               117         370 LOAD_METHOD              8 (offset)
+               114         370 LOAD_METHOD              8 (offset)
                            392 LOAD_FAST                1 (page)
                            394 LOAD_CONST               2 (1)
                            396 BINARY_OP               10 (-)
                            400 LOAD_FAST                2 (size)
                            402 BINARY_OP                5 (*)
                            406 PRECALL                  1
                            410 CALL                     1
                
-               118         420 LOAD_METHOD              9 (limit)
+               115         420 LOAD_METHOD              9 (limit)
                            442 LOAD_FAST                2 (size)
                            444 PRECALL                  1
                            448 CALL                     1
                
-               119         458 LOAD_METHOD             10 (order_by)
+               116         458 LOAD_METHOD             10 (order_by)
                            480 LOAD_FAST                7 (columns)
                            482 LOAD_FAST                4 (order_by)
                            484 BINARY_SUBSCR
                            494 LOAD_METHOD             12 (desc)
                            516 PRECALL                  0
                            520 CALL                     0
                            530 PRECALL                  1
                            534 CALL                     1
                
-               115         544 STORE_FAST               3 (query)
+               112         544 STORE_FAST               3 (query)
                
-               121     >>  546 LOAD_FAST                6 (db_session)
+               118     >>  546 LOAD_FAST                6 (db_session)
                            548 LOAD_METHOD             13 (execute)
                            570 LOAD_FAST                3 (query)
                            572 PRECALL                  1
                            576 CALL                     1
                            586 GET_AWAITABLE            0
                            588 LOAD_CONST               0 (None)
                        >>  590 SEND                     3 (to 598)
                            592 YIELD_VALUE
                            594 RESUME                   3
                            596 JUMP_BACKWARD_NO_INTERRUPT     4 (to 590)
                        >>  598 STORE_FAST               8 (response)
                
-               122         600 LOAD_FAST                8 (response)
+               119         600 LOAD_FAST                8 (response)
                            602 LOAD_METHOD             14 (scalars)
                            624 PRECALL                  0
                            628 CALL                     0
                            638 LOAD_METHOD             15 (all)
                            660 PRECALL                  0
                            664 CALL                     0
                            674 RETURN_VALUE
@@ -1328,15 +1294,15 @@
                   1
                names      ('db', 'session', 'model', '__table__', 'columns', 'SortEnum', 'ascending', 'select', 'offset', 'limit', 'order_by', 'asc', 'desc', 'execute', 'scalars', 'all')
                varnames   ('self', 'page', 'size', 'query', 'order_by', 'sort_order', 'db_session', 'columns', 'response')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_list_ordered'
-               firstlineno 93
+               firstlineno 90
                lnotab
                   0x060a1c0122010c010401200226013201260156fc040826013201260156
                   fc02063601
             'params'
             code
                argcount  : 1
                nlocals   : 5
@@ -1344,61 +1310,62 @@
                flags     : 131
                code
                   0x4b00010097007c03700b7c006a0000000000000000006a010000000000
                   0000007d037c0280147405000000000000000000007c006a030000000000
                   000000a6010000ab0100000000000000007d027409000000000000000000
                   007c037c027c01a6030000ab030000000000000000830064007b03560097
                   0386047d047c045300
-               124           0 RETURN_GENERATOR
+               121           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               127           6 LOAD_FAST                3 (db_session)
+               124           6 LOAD_FAST                3 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               3 (db_session)
                
-               128          34 LOAD_FAST                2 (query)
+               125          34 LOAD_FAST                2 (query)
                             36 POP_JUMP_FORWARD_IF_NOT_NONE    20 (to 78)
                
-               129          38 LOAD_GLOBAL              5 (NULL + select)
+               126          38 LOAD_GLOBAL              5 (NULL + select)
                             50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                3 (model)
                             62 PRECALL                  1
                             66 CALL                     1
                             76 STORE_FAST               2 (query)
                
-               130     >>   78 LOAD_GLOBAL              9 (NULL + paginate)
+               127     >>   78 LOAD_GLOBAL              9 (NULL + paginate)
                             90 LOAD_FAST                3 (db_session)
                             92 LOAD_FAST                2 (query)
                             94 LOAD_FAST                1 (params)
                             96 PRECALL                  3
                            100 CALL                     3
                            110 GET_AWAITABLE            0
                            112 LOAD_CONST               0 (None)
                        >>  114 SEND                     3 (to 122)
                            116 YIELD_VALUE
                            118 RESUME                   3
                            120 JUMP_BACKWARD_NO_INTERRUPT     4 (to 114)
                        >>  122 STORE_FAST               4 (response)
                
-               131         124 LOAD_FAST                4 (response)
+               128         124 LOAD_FAST                4 (response)
                            126 RETURN_VALUE
                consts
                   None
                names      ('db', 'session', 'select', 'model', 'paginate')
                varnames   ('self', 'params', 'query', 'db_session', 'response')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_list_page'
-               firstlineno 124
+               firstlineno 121
                lnotab 0x06031c01040128012e01
+            ('query', 'order_by', 'sort_order', 'db_session')
             code
                argcount  : 1
                nlocals   : 7
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c05700b7c006a0000000000000000006a010000000000
@@ -1412,51 +1379,51 @@
                   00000000007d026e3f740f000000000000000000007c006a020000000000
                   000000a6010000ab010000000000000000a0080000000000000000000000
                   0000000000000000007c067c0319000000000000000000a00a0000000000
                   000000000000000000000000000000a6000000ab000000000000000000a6
                   010000ab0100000000000000007d027417000000000000000000007c057c
                   027c01a6030000ab030000000000000000830064007b0356009703860453
                   00
-               133           0 RETURN_GENERATOR
+               130           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               142           6 LOAD_FAST                5 (db_session)
+               139           6 LOAD_FAST                5 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               5 (db_session)
                
-               143          34 LOAD_FAST                0 (self)
+               140          34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (model)
                             46 LOAD_ATTR                3 (__table__)
                             56 LOAD_ATTR                4 (columns)
                             66 STORE_FAST               6 (columns)
                
-               144          68 LOAD_FAST                3 (order_by)
+               141          68 LOAD_FAST                3 (order_by)
                             70 POP_JUMP_FORWARD_IF_NONE     4 (to 80)
                             72 LOAD_FAST                3 (order_by)
                             74 LOAD_FAST                6 (columns)
                             76 CONTAINS_OP              1
                             78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
                
-               145     >>   80 LOAD_CONST               1 ('id')
+               142     >>   80 LOAD_CONST               1 ('id')
                             82 STORE_FAST               3 (order_by)
                
-               146     >>   84 LOAD_FAST                2 (query)
+               143     >>   84 LOAD_FAST                2 (query)
                             86 POP_JUMP_FORWARD_IF_NOT_NONE   143 (to 374)
                
-               147          88 LOAD_FAST                4 (sort_order)
+               144          88 LOAD_FAST                4 (sort_order)
                             90 LOAD_GLOBAL             10 (SortEnum)
                            102 LOAD_ATTR                6 (ascending)
                            112 COMPARE_OP               2 (==)
                            118 POP_JUMP_FORWARD_IF_FALSE    64 (to 248)
                
-               148         120 LOAD_GLOBAL             15 (NULL + select)
+               145         120 LOAD_GLOBAL             15 (NULL + select)
                            132 LOAD_FAST                0 (self)
                            134 LOAD_ATTR                2 (model)
                            144 PRECALL                  1
                            148 CALL                     1
                            158 LOAD_METHOD              8 (order_by)
                            180 LOAD_FAST                6 (columns)
                            182 LOAD_FAST                3 (order_by)
@@ -1465,15 +1432,15 @@
                            216 PRECALL                  0
                            220 CALL                     0
                            230 PRECALL                  1
                            234 CALL                     1
                            244 STORE_FAST               2 (query)
                            246 JUMP_FORWARD            63 (to 374)
                
-               150     >>  248 LOAD_GLOBAL             15 (NULL + select)
+               147     >>  248 LOAD_GLOBAL             15 (NULL + select)
                            260 LOAD_FAST                0 (self)
                            262 LOAD_ATTR                2 (model)
                            272 PRECALL                  1
                            276 CALL                     1
                            286 LOAD_METHOD              8 (order_by)
                            308 LOAD_FAST                6 (columns)
                            310 LOAD_FAST                3 (order_by)
@@ -1481,15 +1448,15 @@
                            322 LOAD_METHOD             10 (desc)
                            344 PRECALL                  0
                            348 CALL                     0
                            358 PRECALL                  1
                            362 CALL                     1
                            372 STORE_FAST               2 (query)
                
-               151     >>  374 LOAD_GLOBAL             23 (NULL + paginate)
+               148     >>  374 LOAD_GLOBAL             23 (NULL + paginate)
                            386 LOAD_FAST                5 (db_session)
                            388 LOAD_FAST                2 (query)
                            390 LOAD_FAST                1 (params)
                            392 PRECALL                  3
                            396 CALL                     3
                            406 GET_AWAITABLE            0
                            408 LOAD_CONST               0 (None)
@@ -1503,49 +1470,49 @@
                   'id'
                names      ('db', 'session', 'model', '__table__', 'columns', 'SortEnum', 'ascending', 'select', 'order_by', 'asc', 'desc', 'paginate')
                varnames   ('self', 'params', 'query', 'order_by', 'sort_order', 'db_session', 'columns')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'select_list_page_ordered'
-               firstlineno 133
+               firstlineno 130
                lnotab 0x06091c0122010c0104010401200180027e01
             code
                argcount  : 1
                nlocals   : 8
-               stacksize : 6
+               stacksize : 7
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
                   0000007d027405000000000000000000007c006a030000000000000000a6
                   010000ab010000000000000000a004000000000000000000000000000000
                   00000000007c006a0300000000000000006a0500000000000000007c016a
                   0500000000000000006b0200000000a6010000ab0100000000000000007d
                   037c02a00600000000000000000000000000000000000000007c03a60100
                   00ab010000000000000000830064007b035600970386047d047c04800264
                   0153007c04a0070000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007d057c01a00800000000000000000000000000
-                  00000000000000a6000000ab00000000000000000044005d165c0200007d
-                  067d077413000000000000000000007c057c067c07a6030000ab03000000
-                  000000000001008c177c02a00a0000000000000000000000000000000000
-                  0000007c05a6010000ab01000000000000000001007c00a00b0000000000
-                  0000000000000000000000000000007c05a6010000ab0100000000000000
-                  005300
-               153           0 RETURN_GENERATOR
+                  00ab0000000000000000007d057411000000000000000000007c01741200
+                  000000000000000000a6020000ab02000000000000000072037c017d066e
+                  167c01a00a00000000000000000000000000000000000000006402ac03a6
+                  010000ab0100000000000000007d067c0644005d197d0774170000000000
+                  00000000007c057c077c067c0719000000000000000000a6030000ab0300
+                  0000000000000001008c1a7c02a00c000000000000000000000000000000
+                  00000000007c05a6010000ab01000000000000000001007c055300
+               150           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               154           6 LOAD_FAST                2 (db_session)
+               151           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-               155          34 LOAD_GLOBAL              5 (NULL + select)
+               152          34 LOAD_GLOBAL              5 (NULL + select)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (model)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 LOAD_METHOD              4 (where)
                             94 LOAD_FAST                0 (self)
                             96 LOAD_ATTR                3 (model)
@@ -1553,82 +1520,96 @@
                            116 LOAD_FAST                1 (data)
                            118 LOAD_ATTR                5 (id)
                            128 COMPARE_OP               2 (==)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 STORE_FAST               3 (query)
                
-               156         150 LOAD_FAST                2 (db_session)
+               153         150 LOAD_FAST                2 (db_session)
                            152 LOAD_METHOD              6 (execute)
                            174 LOAD_FAST                3 (query)
                            176 PRECALL                  1
                            180 CALL                     1
                            190 GET_AWAITABLE            0
                            192 LOAD_CONST               0 (None)
                        >>  194 SEND                     3 (to 202)
                            196 YIELD_VALUE
                            198 RESUME                   3
                            200 JUMP_BACKWARD_NO_INTERRUPT     4 (to 194)
                        >>  202 STORE_FAST               4 (result)
                
-               157         204 LOAD_FAST                4 (result)
+               154         204 LOAD_FAST                4 (result)
                            206 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 212)
                
-               158         208 LOAD_CONST               1 (0)
+               155         208 LOAD_CONST               1 (0)
                            210 RETURN_VALUE
                
-               159     >>  212 LOAD_FAST                4 (result)
+               156     >>  212 LOAD_FAST                4 (result)
                            214 LOAD_METHOD              7 (scalar_one)
                            236 PRECALL                  0
                            240 CALL                     0
                            250 STORE_FAST               5 (db_data)
                
-               160         252 LOAD_FAST                1 (data)
-                           254 LOAD_METHOD              8 (items)
-                           276 PRECALL                  0
-                           280 CALL                     0
-                           290 GET_ITER
-                       >>  292 FOR_ITER                22 (to 338)
-                           294 UNPACK_SEQUENCE          2
-                           298 STORE_FAST               6 (attr)
-                           300 STORE_FAST               7 (value)
-               
-               161         302 LOAD_GLOBAL             19 (NULL + setattr)
-                           314 LOAD_FAST                5 (db_data)
-                           316 LOAD_FAST                6 (attr)
-                           318 LOAD_FAST                7 (value)
-                           320 PRECALL                  3
-                           324 CALL                     3
-                           334 POP_TOP
-                           336 JUMP_BACKWARD           23 (to 292)
-               
-               162     >>  338 LOAD_FAST                2 (db_session)
-                           340 LOAD_METHOD             10 (add)
-                           362 LOAD_FAST                5 (db_data)
-                           364 PRECALL                  1
-                           368 CALL                     1
-                           378 POP_TOP
-               
-               163         380 LOAD_FAST                0 (self)
-                           382 LOAD_METHOD             11 (count_affected_rows)
-                           404 LOAD_FAST                5 (db_data)
-                           406 PRECALL                  1
-                           410 CALL                     1
-                           420 RETURN_VALUE
+               157         252 LOAD_GLOBAL             17 (NULL + isinstance)
+                           264 LOAD_FAST                1 (data)
+                           266 LOAD_GLOBAL             18 (dict)
+                           278 PRECALL                  2
+                           282 CALL                     2
+                           292 POP_JUMP_FORWARD_IF_FALSE     3 (to 300)
+               
+               158         294 LOAD_FAST                1 (data)
+                           296 STORE_FAST               6 (update_data)
+                           298 JUMP_FORWARD            22 (to 344)
+               
+               160     >>  300 LOAD_FAST                1 (data)
+                           302 LOAD_METHOD             10 (model_dump)
+                           324 LOAD_CONST               2 (True)
+                           326 KW_NAMES                 3
+                           328 PRECALL                  1
+                           332 CALL                     1
+                           342 STORE_FAST               6 (update_data)
+               
+               161     >>  344 LOAD_FAST                6 (update_data)
+                           346 GET_ITER
+                       >>  348 FOR_ITER                25 (to 400)
+                           350 STORE_FAST               7 (field)
+               
+               162         352 LOAD_GLOBAL             23 (NULL + setattr)
+                           364 LOAD_FAST                5 (db_data)
+                           366 LOAD_FAST                7 (field)
+                           368 LOAD_FAST                6 (update_data)
+                           370 LOAD_FAST                7 (field)
+                           372 BINARY_SUBSCR
+                           382 PRECALL                  3
+                           386 CALL                     3
+                           396 POP_TOP
+                           398 JUMP_BACKWARD           26 (to 348)
+               
+               164     >>  400 LOAD_FAST                2 (db_session)
+                           402 LOAD_METHOD             12 (add)
+                           424 LOAD_FAST                5 (db_data)
+                           426 PRECALL                  1
+                           430 CALL                     1
+                           440 POP_TOP
+               
+               165         442 LOAD_FAST                5 (db_data)
+                           444 RETURN_VALUE
                consts
                   None
                   0
-               names      ('db', 'session', 'select', 'model', 'where', 'id', 'execute', 'scalar_one', 'items', 'setattr', 'add', 'count_affected_rows')
-               varnames   ('self', 'data', 'db_session', 'query', 'result', 'db_data', 'attr', 'value')
+                  True
+                  ('exclude_unset',)
+               names      ('db', 'session', 'select', 'model', 'where', 'id', 'execute', 'scalar_one', 'isinstance', 'dict', 'model_dump', 'setattr', 'add')
+               varnames   ('self', 'data', 'db_session', 'query', 'result', 'db_data', 'update_data', 'field')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'update_by_id'
-               firstlineno 153
-               lnotab 0x06011c0174013601040104012801320124012a01
+               firstlineno 150
+               lnotab 0x06011c01740136010401040128012a0106022c01080130022a01
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 8
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
@@ -1639,86 +1620,86 @@
                   0600000000000000007c036a0600000000000000006b0200000000a60100
                   00ab0100000000000000006a070000000000000000640469007c03a00800
                   000000000000000000000000000000000000006402ac03a6010000ab0100
                   00000000000000a4018e017d047c02a00900000000000000000000000000
                   000000000000007c04a6010000ab010000000000000000830064007b0356
                   009703860401008c877415000000000000000000007c01a6010000ab0100
                   000000000000005300
-               165           0 RETURN_GENERATOR
+               167           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               168           6 LOAD_FAST                2 (db_session)
+               170           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-               169          34 LOAD_FAST                1 (data_list)
+               171          34 LOAD_FAST                1 (data_list)
                             36 GET_ITER
                        >>   38 FOR_ITER               134 (to 308)
                             40 STORE_FAST               3 (data)
                
-               170          42 LOAD_GLOBAL              5 (NULL + hasattr)
+               172          42 LOAD_GLOBAL              5 (NULL + hasattr)
                             54 LOAD_FAST                3 (data)
                             56 LOAD_CONST               1 ('id')
                             58 PRECALL                  2
                             62 CALL                     2
                             72 POP_JUMP_FORWARD_IF_FALSE   116 (to 306)
                
-               172          74 PUSH_NULL
+               174          74 PUSH_NULL
                             76 LOAD_GLOBAL              7 (NULL + update)
                             88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (model)
                            100 PRECALL                  1
                            104 CALL                     1
                
-               173         114 LOAD_METHOD              5 (where)
+               175         114 LOAD_METHOD              5 (where)
                            136 LOAD_FAST                0 (self)
                            138 LOAD_ATTR                4 (model)
                            148 LOAD_ATTR                6 (id)
                            158 LOAD_FAST                3 (data)
                            160 LOAD_ATTR                6 (id)
                            170 COMPARE_OP               2 (==)
                            176 PRECALL                  1
                            180 CALL                     1
                
-               174         190 LOAD_ATTR                7 (values)
+               176         190 LOAD_ATTR                7 (values)
                
-               172         200 LOAD_CONST               4 (())
+               174         200 LOAD_CONST               4 (())
                            202 BUILD_MAP                0
                
-               174         204 LOAD_FAST                3 (data)
+               176         204 LOAD_FAST                3 (data)
                            206 LOAD_METHOD              8 (dict)
                            228 LOAD_CONST               2 (True)
                            230 KW_NAMES                 3
                            232 PRECALL                  1
                            236 CALL                     1
                
-               172         246 DICT_MERGE               1
+               174         246 DICT_MERGE               1
                            248 CALL_FUNCTION_EX         1
                
-               171         250 STORE_FAST               4 (statement)
+               173         250 STORE_FAST               4 (statement)
                
-               176         252 LOAD_FAST                2 (db_session)
+               178         252 LOAD_FAST                2 (db_session)
                            254 LOAD_METHOD              9 (execute)
                            276 LOAD_FAST                4 (statement)
                            278 PRECALL                  1
                            282 CALL                     1
                            292 GET_AWAITABLE            0
                            294 LOAD_CONST               0 (None)
                        >>  296 SEND                     3 (to 304)
                            298 YIELD_VALUE
                            300 RESUME                   3
                            302 JUMP_BACKWARD_NO_INTERRUPT     4 (to 296)
                        >>  304 POP_TOP
                        >>  306 JUMP_BACKWARD          135 (to 38)
                
-               177     >>  308 LOAD_GLOBAL             21 (NULL + len)
+               179     >>  308 LOAD_GLOBAL             21 (NULL + len)
                            320 LOAD_FAST                1 (data_list)
                            322 PRECALL                  1
                            326 CALL                     1
                            336 RETURN_VALUE
                consts
                   None
                   'id'
@@ -1727,102 +1708,99 @@
                   ()
                names      ('db', 'session', 'hasattr', 'update', 'model', 'where', 'id', 'values', 'dict', 'execute', 'len')
                varnames   ('self', 'data_list', 'db_session', 'data', 'statement')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'update_batch_by_ids'
-               firstlineno 165
+               firstlineno 167
                lnotab 0x06031c010801200228014c010afe04022afe04ff02053801
             code
                argcount  : 1
-               nlocals   : 5
-               stacksize : 6
+               nlocals   : 6
+               stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
-                  0000007d027c02a002000000000000000000000000000000000000000074
-                  07000000000000000000007c006a040000000000000000a6010000ab0100
-                  00000000000000a00500000000000000000000000000000000000000007c
-                  006a0400000000000000006a0600000000000000007c016b0200000000a6
-                  010000ab010000000000000000a6010000ab010000000000000000830064
-                  007b035600970386047d037c03a007000000000000000000000000000000
-                  0000000000a6000000ab0000000000000000007d047c02a0080000000000
-                  0000000000000000000000000000007c04a6010000ab0100000000000000
-                  00830064007b03560097038604010064015300
-               179           0 RETURN_GENERATOR
+                  0000007d027405000000000000000000007c006a030000000000000000a6
+                  010000ab010000000000000000a004000000000000000000000000000000
+                  00000000007c006a0300000000000000006a0500000000000000007c016b
+                  0200000000a6010000ab0100000000000000007d037c02a0060000000000
+                  0000000000000000000000000000007c03a6010000ab0100000000000000
+                  00830064007b035600970386047d047c04a0070000000000000000000000
+                  000000000000000000a6000000ab0000000000000000007d057c02a00800
+                  000000000000000000000000000000000000007c05a6010000ab01000000
+                  0000000000830064007b035600970386045300
+               181           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               180           6 LOAD_FAST                2 (db_session)
+               182           6 LOAD_FAST                2 (db_session)
                              8 JUMP_IF_TRUE_OR_POP     11 (to 32)
                             10 LOAD_FAST                0 (self)
                             12 LOAD_ATTR                0 (db)
                             22 LOAD_ATTR                1 (session)
                        >>   32 STORE_FAST               2 (db_session)
                
-               181          34 LOAD_FAST                2 (db_session)
-                            36 LOAD_METHOD              2 (execute)
+               183          34 LOAD_GLOBAL              5 (NULL + select)
+                            46 LOAD_FAST                0 (self)
+                            48 LOAD_ATTR                3 (model)
+                            58 PRECALL                  1
+                            62 CALL                     1
+                            72 LOAD_METHOD              4 (where)
+                            94 LOAD_FAST                0 (self)
+                            96 LOAD_ATTR                3 (model)
+                           106 LOAD_ATTR                5 (id)
+                           116 LOAD_FAST                1 (id)
+                           118 COMPARE_OP               2 (==)
+                           124 PRECALL                  1
+                           128 CALL                     1
+                           138 STORE_FAST               3 (statement)
                
-               182          58 LOAD_GLOBAL              7 (NULL + select)
-                            70 LOAD_FAST                0 (self)
-                            72 LOAD_ATTR                4 (model)
-                            82 PRECALL                  1
-                            86 CALL                     1
-                            96 LOAD_METHOD              5 (where)
-                           118 LOAD_FAST                0 (self)
-                           120 LOAD_ATTR                4 (model)
-                           130 LOAD_ATTR                6 (id)
-                           140 LOAD_FAST                1 (id)
-                           142 COMPARE_OP               2 (==)
-                           148 PRECALL                  1
-                           152 CALL                     1
+               184         140 LOAD_FAST                2 (db_session)
+                           142 LOAD_METHOD              6 (execute)
+                           164 LOAD_FAST                3 (statement)
+                           166 PRECALL                  1
+                           170 CALL                     1
+                           180 GET_AWAITABLE            0
+                           182 LOAD_CONST               0 (None)
+                       >>  184 SEND                     3 (to 192)
+                           186 YIELD_VALUE
+                           188 RESUME                   3
+                           190 JUMP_BACKWARD_NO_INTERRUPT     4 (to 184)
+                       >>  192 STORE_FAST               4 (response)
                
-               181         162 PRECALL                  1
-                           166 CALL                     1
-                           176 GET_AWAITABLE            0
-                           178 LOAD_CONST               0 (None)
-                       >>  180 SEND                     3 (to 188)
-                           182 YIELD_VALUE
-                           184 RESUME                   3
-                           186 JUMP_BACKWARD_NO_INTERRUPT     4 (to 180)
-                       >>  188 STORE_FAST               3 (response)
-               
-               184         190 LOAD_FAST                3 (response)
-                           192 LOAD_METHOD              7 (scalar_one)
-                           214 PRECALL                  0
-                           218 CALL                     0
-                           228 STORE_FAST               4 (data)
-               
-               185         230 LOAD_FAST                2 (db_session)
-                           232 LOAD_METHOD              8 (delete)
-                           254 LOAD_FAST                4 (data)
-                           256 PRECALL                  1
-                           260 CALL                     1
-                           270 GET_AWAITABLE            0
-                           272 LOAD_CONST               0 (None)
-                       >>  274 SEND                     3 (to 282)
-                           276 YIELD_VALUE
-                           278 RESUME                   3
-                           280 JUMP_BACKWARD_NO_INTERRUPT     4 (to 274)
-                       >>  282 POP_TOP
+               185         194 LOAD_FAST                4 (response)
+                           196 LOAD_METHOD              7 (scalar_one)
+                           218 PRECALL                  0
+                           222 CALL                     0
+                           232 STORE_FAST               5 (data)
                
-               186         284 LOAD_CONST               1 (1)
-                           286 RETURN_VALUE
+               186         234 LOAD_FAST                2 (db_session)
+                           236 LOAD_METHOD              8 (delete)
+                           258 LOAD_FAST                5 (data)
+                           260 PRECALL                  1
+                           264 CALL                     1
+                           274 GET_AWAITABLE            0
+                           276 LOAD_CONST               0 (None)
+                       >>  278 SEND                     3 (to 286)
+                           280 YIELD_VALUE
+                           282 RESUME                   3
+                           284 JUMP_BACKWARD_NO_INTERRUPT     4 (to 278)
+                       >>  286 RETURN_VALUE
                consts
                   None
-                  1
-               names      ('db', 'session', 'execute', 'select', 'model', 'where', 'id', 'scalar_one', 'delete')
-               varnames   ('self', 'id', 'db_session', 'response', 'data')
+               names      ('db', 'session', 'select', 'model', 'where', 'id', 'execute', 'scalar_one', 'delete')
+               varnames   ('self', 'id', 'db_session', 'statement', 'response', 'data')
                freevars   ()
                cellvars   ()
                filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
                name       'delete_by_id'
-               firstlineno 179
-               lnotab 0x06011c01180168ff1c0328013601
+               firstlineno 181
+               lnotab 0x06011c016a0136012801
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c02700b7c006a0000000000000000006a010000000000
@@ -1892,20 +1870,21 @@
          freevars   ()
          cellvars   ()
          filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
          name       'SqlModelMapper'
          firstlineno 21
          lnotab
             0x0a011804180702fc060312fd020412fc020502fb080c02ff06010eff02
-            0102ff020202fe080e1a0704ff06010eff020102ff020102ff02020efe08
+            0102ff020202fe080b1a0704ff06010eff020102ff020102ff02020efe08
             0c160806ff060102ff020102ff020102ff020102ff02020efe0811020102
             0402f8060302fd020402fc020502fb020602fa020702f9020802f802090e
-            f7082002ff060102ff020102ff020102ff02020efe081002f9060302fd02
-            0402fc020502fb020602fa020702f902080ef808141a0d02ff06010eff02
-            0102ff020202fe080e1a0a02ff06010eff020102ff020202fe
+            f7082002ff060102ff020102ff020102ff02020efe080d02010201020102
+            f9060302fd020402fc020502fb020602fa020702f902080ef808141a1202
+            ff06010eff020102ff020202fe080e1a0802ff06010eff020102ff020202
+            fe
       'SqlModelMapper'
       None
    names      ('__doc__', 'typing', 'Generic', 'TypeVar', 'List', 'Any', 'Type', 'Union', 'fastapi_pagination.ext.sqlmodel', 'paginate', 'pydantic', 'BaseModel', 'sqlmodel', 'SQLModel', 'select', 'func', 'insert', 'update', 'delete', 'sqlmodel.ext.asyncio.session', 'AsyncSession', 'fss.common.enum.enum', 'SortEnum', 'fss.common.persistence.base_mapper', 'BaseMapper', 'fss.middleware.db_session_middleware', 'db', 'ModelType', 'CreateSchemaType', 'UpdateSchemaType', 'SchemaType', 'T', 'SqlModelMapper')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\persistence\\sqlmodel_impl.py'
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/base_mapper.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/base_mapper.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/base_model.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/base_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/persistence/sqlmodel_impl.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/persistence/sqlmodel_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,20 +37,17 @@
         db_session.add(orm_data)
         return orm_data
 
     async def insert_batch(
         self, *, data_list: List[Any], db_session: Any = None
     ) -> int:
         db_session = db_session or self.db.session
-        orm_datas = [
-            self.model.model_validate(data)
-            if not isinstance(data, self.model)
-            else data
-            for data in data_list
-        ]
+        orm_datas = []
+        for data in data_list:
+            orm_datas.append(self.model.model_validate(data))
         statement = insert(self.model).values([data.model_dump() for data in orm_datas])
         await db_session.execute(statement)
         return len(data_list)
 
     async def select_by_id(self, *, id: Any, db_session: Any = None) -> Any:
         db_session = db_session or self.db.session
         statement = select(self.model).where(self.model.id == id)
@@ -130,17 +127,17 @@
         response = await paginate(db_session, query, params)
         return response
 
     async def select_list_page_ordered(
         self,
         *,
         params: Any,
-        query: Any,
-        order_by: Any,
-        sort_order: Any,
+        query: Any = None,
+        order_by: Any = None,
+        sort_order: Any = None,
         db_session: Any = None,
     ) -> List[Any]:
         db_session = db_session or self.db.session
         columns = self.model.__table__.columns
         if order_by is None or order_by not in columns:
             order_by = "id"
         if query is None:
@@ -153,18 +150,23 @@
     async def update_by_id(self, *, data: Any, db_session: Any = None) -> int:
         db_session = db_session or self.db.session
         query = select(self.model).where(self.model.id == data.id)
         result = await db_session.execute(query)
         if result is None:
             return 0
         db_data = result.scalar_one()
-        for attr, value in data.items():
-            setattr(db_data, attr, value)
+        if isinstance(data, dict):
+            update_data = data
+        else:
+            update_data = data.model_dump(exclude_unset=True)
+        for field in update_data:
+            setattr(db_data, field, update_data[field])
+
         db_session.add(db_data)
-        return self.count_affected_rows(db_data)
+        return db_data
 
     async def update_batch_by_ids(
         self, *, data_list: List[Any], db_session: Any = None
     ) -> int:
         db_session = db_session or self.db.session
         for data in data_list:
             if hasattr(data, "id"):
@@ -174,20 +176,18 @@
                     .values(**data.dict(exclude_unset=True))
                 )
                 await db_session.execute(statement)
         return len(data_list)
 
     async def delete_by_id(self, *, id: Any, db_session: Any = None) -> int:
         db_session = db_session or self.db.session
-        response = await db_session.execute(
-            select(self.model).where(self.model.id == id)
-        )
+        statement = select(self.model).where(self.model.id == id)
+        response = await db_session.execute(statement)
         data = response.scalar_one()
-        await db_session.delete(data)
-        return 1
+        return await db_session.delete(data)
 
     async def delete_batch_by_ids(
         self, *, ids: List[Any], db_session: Any = None
     ) -> int:
         db_session = db_session or self.db.session
         statement = delete(self.model).where(self.model.id.in_(ids))
         result = await db_session.execute(statement)
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/result/__pycache__/result.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/__pycache__/result.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xde4b1566 (Tue Apr  9 14:08:30 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 2016
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/result/result.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/result/result.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/schema/__pycache__/schema.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/schema/__pycache__/schema.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9b601366 (Mon Apr  8 03:12:27 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 315
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/security/__pycache__/security.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/__pycache__/security.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 1305
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/security/security.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/security/security.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/__pycache__/service.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/__pycache__/service.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xde4b1566 (Tue Apr  9 14:08:30 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 2052
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/impl/__pycache__/service_impl.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/__pycache__/service_impl.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
-files sz: 2802
+moddate:  0x1c321966 (Fri Apr 12 13:07:40 2024 UTC)
+files sz: 2850
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d035a036d045a046d055a056d
@@ -694,29 +694,35 @@
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c017c027c03ac01a6030000ab030000000000
-                  0000005300
+                  000000830064007b035600970386045300
                 48           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 49           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (select_list)
                             40 LOAD_FAST                1 (page)
                             42 LOAD_FAST                2 (size)
                             44 LOAD_FAST                3 (query)
                             46 KW_NAMES                 1
                             48 PRECALL                  3
                             52 CALL                     3
-                            62 RETURN_VALUE
+                            62 GET_AWAITABLE            0
+                            64 LOAD_CONST               0 (None)
+                       >>   66 SEND                     3 (to 74)
+                            68 YIELD_VALUE
+                            70 RESUME                   3
+                            72 JUMP_BACKWARD_NO_INTERRUPT     4 (to 66)
+                       >>   74 RETURN_VALUE
                consts
                   None
                   ('page', 'size', 'query')
                names      ('mapper', 'select_list')
                varnames   ('self', 'page', 'size', 'query')
                freevars   ()
                cellvars   ()
@@ -730,15 +736,15 @@
                argcount  : 1
                nlocals   : 6
                stacksize : 7
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c017c027c037c047c05ac01a6050000ab0500
-                  000000000000005300
+                  00000000000000830064007b035600970386045300
                 51           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 54           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (select_list_ordered)
@@ -748,15 +754,21 @@
                             44 LOAD_FAST                3 (query)
                             46 LOAD_FAST                4 (order_by)
                             48 LOAD_FAST                5 (sort_order)
                
                 54          50 KW_NAMES                 1
                             52 PRECALL                  5
                             56 CALL                     5
-                            66 RETURN_VALUE
+                            66 GET_AWAITABLE            0
+                            68 LOAD_CONST               0 (None)
+                       >>   70 SEND                     3 (to 78)
+                            72 YIELD_VALUE
+                            74 RESUME                   3
+                            76 JUMP_BACKWARD_NO_INTERRUPT     4 (to 70)
+                       >>   78 RETURN_VALUE
                consts
                   None
                   ('page', 'size', 'query', 'order_by', 'sort_order')
                names      ('mapper', 'select_list_ordered')
                varnames   ('self', 'page', 'size', 'query', 'order_by', 'sort_order')
                freevars   ()
                cellvars   ()
@@ -769,28 +781,34 @@
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c017c02ac01a6020000ab0200000000000000
-                  005300
+                  00830064007b035600970386045300
                 58           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 59           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (select_list_page)
                             40 LOAD_FAST                1 (params)
                             42 LOAD_FAST                2 (query)
                             44 KW_NAMES                 1
                             46 PRECALL                  2
                             50 CALL                     2
-                            60 RETURN_VALUE
+                            60 GET_AWAITABLE            0
+                            62 LOAD_CONST               0 (None)
+                       >>   64 SEND                     3 (to 72)
+                            66 YIELD_VALUE
+                            68 RESUME                   3
+                            70 JUMP_BACKWARD_NO_INTERRUPT     4 (to 64)
+                       >>   72 RETURN_VALUE
                consts
                   None
                   ('params', 'query')
                names      ('mapper', 'select_list_page')
                varnames   ('self', 'params', 'query')
                freevars   ()
                cellvars   ()
@@ -802,15 +820,15 @@
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
                   00000000000000000000007c017c027c03ac01a6030000ab030000000000
-                  0000005300
+                  000000830064007b035600970386045300
                 61           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 62           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (select_list_page_ordered)
@@ -818,15 +836,21 @@
                 63          40 LOAD_FAST                1 (params)
                             42 LOAD_FAST                2 (query)
                             44 LOAD_FAST                3 (sort_order)
                
                 62          46 KW_NAMES                 1
                             48 PRECALL                  3
                             52 CALL                     3
-                            62 RETURN_VALUE
+                            62 GET_AWAITABLE            0
+                            64 LOAD_CONST               0 (None)
+                       >>   66 SEND                     3 (to 74)
+                            68 YIELD_VALUE
+                            70 RESUME                   3
+                            72 JUMP_BACKWARD_NO_INTERRUPT     4 (to 66)
+                       >>   74 RETURN_VALUE
                consts
                   None
                   ('params', 'query', 'sort_order')
                names      ('mapper', 'select_list_page_ordered')
                varnames   ('self', 'params', 'query', 'sort_order')
                freevars   ()
                cellvars   ()
@@ -837,28 +861,34 @@
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c01ac01a6010000ab01000000000000000053
-                  00
+                  00000000000000000000007c01ac01a6010000ab01000000000000000083
+                  0064007b035600970386045300
                 66           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 67           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (update_by_id)
                             40 LOAD_FAST                1 (data)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
-                            58 RETURN_VALUE
+                            58 GET_AWAITABLE            0
+                            60 LOAD_CONST               0 (None)
+                       >>   62 SEND                     3 (to 70)
+                            64 YIELD_VALUE
+                            66 RESUME                   3
+                            68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
+                       >>   70 RETURN_VALUE
                consts
                   None
                   ('data',)
                names      ('mapper', 'update_by_id')
                varnames   ('self', 'data')
                freevars   ()
                cellvars   ()
@@ -869,28 +899,34 @@
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c01ac01a6010000ab01000000000000000053
-                  00
+                  00000000000000000000007c01ac01a6010000ab01000000000000000083
+                  0064007b035600970386045300
                 69           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 70           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (update_batch_by_ids)
                             40 LOAD_FAST                1 (data_list)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
-                            58 RETURN_VALUE
+                            58 GET_AWAITABLE            0
+                            60 LOAD_CONST               0 (None)
+                       >>   62 SEND                     3 (to 70)
+                            64 YIELD_VALUE
+                            66 RESUME                   3
+                            68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
+                       >>   70 RETURN_VALUE
                consts
                   None
                   ('data_list',)
                names      ('mapper', 'update_batch_by_ids')
                varnames   ('self', 'data_list')
                freevars   ()
                cellvars   ()
@@ -901,28 +937,34 @@
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c01ac01a6010000ab01000000000000000053
-                  00
+                  00000000000000000000007c01ac01a6010000ab01000000000000000083
+                  0064007b035600970386045300
                 72           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 73           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (delete_by_id)
                             40 LOAD_FAST                1 (id)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
-                            58 RETURN_VALUE
+                            58 GET_AWAITABLE            0
+                            60 LOAD_CONST               0 (None)
+                       >>   62 SEND                     3 (to 70)
+                            64 YIELD_VALUE
+                            66 RESUME                   3
+                            68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
+                       >>   70 RETURN_VALUE
                consts
                   None
                   ('id',)
                names      ('mapper', 'delete_by_id')
                varnames   ('self', 'id')
                freevars   ()
                cellvars   ()
@@ -933,28 +975,34 @@
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 131
                code
                   0x4b00010097007c006a000000000000000000a001000000000000000000
-                  00000000000000000000007c01ac01a6010000ab01000000000000000053
-                  00
+                  00000000000000000000007c01ac01a6010000ab01000000000000000083
+                  0064007b035600970386045300
                 75           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
                 76           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (mapper)
                             18 LOAD_METHOD              1 (delete_batch_by_ids)
                             40 LOAD_FAST                1 (ids)
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
-                            58 RETURN_VALUE
+                            58 GET_AWAITABLE            0
+                            60 LOAD_CONST               0 (None)
+                       >>   62 SEND                     3 (to 70)
+                            64 YIELD_VALUE
+                            66 RESUME                   3
+                            68 JUMP_BACKWARD_NO_INTERRUPT     4 (to 62)
+                       >>   70 RETURN_VALUE
                consts
                   None
                   ('ids',)
                names      ('mapper', 'delete_batch_by_ids')
                varnames   ('self', 'ids')
                freevars   ()
                cellvars   ()
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/impl/service_impl.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/impl/service_impl.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,35 +42,35 @@
     async def get_by_ids(self, *, ids: List[T], batch_size: int = 1000) -> List[Any]:
         return await self.mapper.select_by_ids(ids=ids, batch_size=batch_size)
 
     async def count(self) -> int:
         return await self.mapper.select_count()
 
     async def list(self, *, page: int, size: int, query: T) -> List[T]:
-        return self.mapper.select_list(page=page, size=size, query=query)
+        return await self.mapper.select_list(page=page, size=size, query=query)
 
     async def list_ordered(
         self, *, page: int, size: int, query: T, order_by: T, sort_order: T
     ) -> List[T]:
-        return self.mapper.select_list_ordered(
+        return await self.mapper.select_list_ordered(
             page=page, size=size, query=query, order_by=order_by, sort_order=sort_order
         )
 
     async def list_page(self, *, params: T, query: T) -> List[T]:
-        return self.mapper.select_list_page(params=params, query=query)
+        return await self.mapper.select_list_page(params=params, query=query)
 
     async def list_page_ordered(self, *, params: T, query: T, sort_order: T) -> List[T]:
-        return self.mapper.select_list_page_ordered(
+        return await self.mapper.select_list_page_ordered(
             params=params, query=query, sort_order=sort_order
         )
 
     async def update_by_id(self, *, data: T) -> bool:
-        return self.mapper.update_by_id(data=data)
+        return await self.mapper.update_by_id(data=data)
 
     async def update_batch_by_ids(self, *, data_list: List[T]) -> bool:
-        return self.mapper.update_batch_by_ids(data_list=data_list)
+        return await self.mapper.update_batch_by_ids(data_list=data_list)
 
     async def remove_by_id(self, *, id: T) -> bool:
-        return self.mapper.delete_by_id(id=id)
+        return await self.mapper.delete_by_id(id=id)
 
     async def remove_batch_by_ids(self, *, ids: List[Any]) -> bool:
-        return self.mapper.delete_batch_by_ids(ids=ids)
+        return await self.mapper.delete_batch_by_ids(ids=ids)
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/service/service.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/service/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/__pycache__/security.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/security.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,24 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
-files sz: 1495
+moddate:  0x53401966 (Fri Apr 12 14:08:19 2024 UTC)
+files sz: 1634
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 9
    flags     : 0
    code
       0x970064005a00640164026c016d025a026d015a010100640164036c036d
       045a046d055a050100640164046c066d075a070100640164056c086d095a
       090100640164066c0a6d0b5a0b0100640164076c0c6d0d5a0d0100020065
       09640867016409ac0aa6020000ab0200000000000000005a0e640b5a0f09
-      00641a640d650565106504660219000000000000000000640e6502640f65
+      00641b640d650565106504660219000000000000000000640e6502640f65
       10641065106608641184055a116412651064136510641065126606641484
       045a1364156510641065106604641684045a14641765106602641884045a
-      15641765106602641984045a16640c5300
+      15641765106602641984045a16641765106602641a84045a17640c5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('Security util, such as encode decode and etc')
                  4 STORE_NAME               0 (__doc__)
    
      3           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (('timedelta', 'datetime'))
@@ -77,15 +77,15 @@
                112 STORE_NAME              14 (pwd_context)
    
     13         114 LOAD_CONST              11 (30)
                116 STORE_NAME              15 (DAYS_WITHOUT_LOGIN)
    
     17         118 NOP
    
-    16         120 LOAD_CONST              26 ((None, None))
+    16         120 LOAD_CONST              27 ((None, None))
                122 LOAD_CONST              13 ('subject')
    
     17         124 LOAD_NAME                5 (Union)
                126 LOAD_NAME               16 (str)
                128 LOAD_NAME                4 (Any)
                130 BUILD_TUPLE              2
                132 BINARY_SUBSCR
@@ -133,19 +133,26 @@
                204 LOAD_CONST              24 (<code object get_payload, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\util\security.py", line 37>)
                206 MAKE_FUNCTION            4 (annotations)
                208 STORE_NAME              21 (get_payload)
    
     41         210 LOAD_CONST              23 ('token')
                212 LOAD_NAME               16 (str)
                214 BUILD_TUPLE              2
-               216 LOAD_CONST              25 (<code object is_valid_token, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\util\security.py", line 41>)
+               216 LOAD_CONST              25 (<code object get_user_id, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\util\security.py", line 41>)
                218 MAKE_FUNCTION            4 (annotations)
-               220 STORE_NAME              22 (is_valid_token)
-               222 LOAD_CONST              12 (None)
-               224 RETURN_VALUE
+               220 STORE_NAME              22 (get_user_id)
+   
+    46         222 LOAD_CONST              23 ('token')
+               224 LOAD_NAME               16 (str)
+               226 BUILD_TUPLE              2
+               228 LOAD_CONST              26 (<code object is_valid_token, file "E:\user\train\production\fastapi-sqlmodel-starter\src\fss\common\util\security.py", line 46>)
+               230 MAKE_FUNCTION            4 (annotations)
+               232 STORE_NAME              23 (is_valid_token)
+               234 LOAD_CONST              12 (None)
+               236 RETURN_VALUE
    consts
       'Security util, such as encode decode and etc'
       0
       ('timedelta', 'datetime')
       ('Any', 'Union')
       ('jwt',)
       ('CryptContext',)
@@ -339,80 +346,120 @@
          cellvars   ()
          filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\util\\security.py'
          name       'get_payload'
          firstlineno 37
          lnotab 0x0601
       code
          argcount  : 1
+         nlocals   : 2
+         stacksize : 5
+         flags     : 3
+         code
+            0x97007401000000000000000000006a0100000000000000007c00740400
+            0000000000000000006a0300000000000000007404000000000000000000
+            006a040000000000000000ac01a6030000ab0300000000000000007d017c
+            016402190000000000000000005300
+          41           0 RESUME                   0
+         
+          42           2 LOAD_GLOBAL              1 (NULL + jwt)
+                      14 LOAD_ATTR                1 (decode)
+                      24 LOAD_FAST                0 (token)
+                      26 LOAD_GLOBAL              4 (configs)
+                      38 LOAD_ATTR                3 (secret_key)
+                      48 LOAD_GLOBAL              4 (configs)
+                      60 LOAD_ATTR                4 (algorithm)
+                      70 KW_NAMES                 1
+                      72 PRECALL                  3
+                      76 CALL                     3
+                      86 STORE_FAST               1 (payload)
+         
+          43          88 LOAD_FAST                1 (payload)
+                      90 LOAD_CONST               2 ('sub')
+                      92 BINARY_SUBSCR
+                     102 RETURN_VALUE
+         consts
+            None
+            ('algorithms',)
+            'sub'
+         names      ('jwt', 'decode', 'configs', 'secret_key', 'algorithm')
+         varnames   ('token', 'payload')
+         freevars   ()
+         cellvars   ()
+         filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\util\\security.py'
+         name       'get_user_id'
+         firstlineno 41
+         lnotab 0x02015601
+      code
+         argcount  : 1
          nlocals   : 4
          stacksize : 5
          flags     : 131
          code
             0x4b00010097007401000000000000000000007c00a6010000ab01000000
             0000000000830064007b035600970386047d017c01a00100000000000000
             000000000000000000000000006401a6010000ab0100000000000000007d
             027405000000000000000000006a030000000000000000a6000000ab0000
             000000000000007d037c02722b7405000000000000000000006a04000000
             00000000007c02a6010000ab0100000000000000007c036b000000000072
             15740b000000000000000000006402640364046901ac05a6020000ab0200
             0000000000000053006400530064005300
-          41           0 RETURN_GENERATOR
+          46           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-          42           6 LOAD_GLOBAL              1 (NULL + get_payload)
+          47           6 LOAD_GLOBAL              1 (NULL + get_payload)
                       18 LOAD_FAST                0 (token)
                       20 PRECALL                  1
                       24 CALL                     1
                       34 GET_AWAITABLE            0
                       36 LOAD_CONST               0 (None)
                  >>   38 SEND                     3 (to 46)
                       40 YIELD_VALUE
                       42 RESUME                   3
                       44 JUMP_BACKWARD_NO_INTERRUPT     4 (to 38)
                  >>   46 STORE_FAST               1 (payload)
          
-          43          48 LOAD_FAST                1 (payload)
+          48          48 LOAD_FAST                1 (payload)
                       50 LOAD_METHOD              1 (get)
                       72 LOAD_CONST               1 ('exp')
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_FAST               2 (exp)
          
-          44          90 LOAD_GLOBAL              5 (NULL + datetime)
+          49          90 LOAD_GLOBAL              5 (NULL + datetime)
                      102 LOAD_ATTR                3 (now)
                      112 PRECALL                  0
                      116 CALL                     0
                      126 STORE_FAST               3 (now)
          
-          45         128 LOAD_FAST                2 (exp)
+          50         128 LOAD_FAST                2 (exp)
                      130 POP_JUMP_FORWARD_IF_FALSE    43 (to 218)
                      132 LOAD_GLOBAL              5 (NULL + datetime)
                      144 LOAD_ATTR                4 (fromtimestamp)
                      154 LOAD_FAST                2 (exp)
                      156 PRECALL                  1
                      160 CALL                     1
                      170 LOAD_FAST                3 (now)
                      172 COMPARE_OP               0 (<)
                      178 POP_JUMP_FORWARD_IF_FALSE    21 (to 222)
          
-          46         180 LOAD_GLOBAL             11 (NULL + JSONResponse)
+          51         180 LOAD_GLOBAL             11 (NULL + JSONResponse)
          
-          47         192 LOAD_CONST               2 (401)
+          52         192 LOAD_CONST               2 (401)
          
-          48         194 LOAD_CONST               3 ('detail')
+          53         194 LOAD_CONST               3 ('detail')
                      196 LOAD_CONST               4 ('Token has expired')
                      198 BUILD_MAP                1
          
-          46         200 KW_NAMES                 5
+          51         200 KW_NAMES                 5
                      202 PRECALL                  2
                      206 CALL                     2
                      216 RETURN_VALUE
          
-          45     >>  218 LOAD_CONST               0 (None)
+          50     >>  218 LOAD_CONST               0 (None)
                      220 RETURN_VALUE
                  >>  222 LOAD_CONST               0 (None)
                      224 RETURN_VALUE
          consts
             None
             'exp'
             401
@@ -421,20 +468,20 @@
             ('status_code', 'content')
          names      ('get_payload', 'get', 'datetime', 'now', 'fromtimestamp', 'JSONResponse')
          varnames   ('token', 'payload', 'exp', 'now')
          freevars   ()
          cellvars   ()
          filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\util\\security.py'
          name       'is_valid_token'
-         firstlineno 41
+         firstlineno 46
          lnotab 0x06012a012a01260134010c01020106fe12ff
       (None, None)
-   names      ('__doc__', 'datetime', 'timedelta', 'typing', 'Any', 'Union', 'jose', 'jwt', 'passlib.context', 'CryptContext', 'starlette.responses', 'JSONResponse', 'fss.common.config', 'configs', 'pwd_context', 'DAYS_WITHOUT_LOGIN', 'str', 'create_token', 'bool', 'verify_password', 'get_password_hash', 'get_payload', 'is_valid_token')
+   names      ('__doc__', 'datetime', 'timedelta', 'typing', 'Any', 'Union', 'jose', 'jwt', 'passlib.context', 'CryptContext', 'starlette.responses', 'JSONResponse', 'fss.common.config', 'configs', 'pwd_context', 'DAYS_WITHOUT_LOGIN', 'str', 'create_token', 'bool', 'verify_password', 'get_password_hash', 'get_payload', 'get_user_id', 'is_valid_token')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'E:\\user\\train\\production\\fastapi-sqlmodel-starter\\src\\fss\\common\\util\\security.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010402100110020c010c010c020c021c01040402ff040112ff02
-      0102ff020102ff020202fe080c140510040c04
+      0102ff020102ff020202fe080c140510040c040c05
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/__pycache__/snowflake.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/__pycache__/snowflake.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x9b601366 (Mon Apr  8 03:12:27 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 1580
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/security.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/security.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,14 +34,19 @@
     return pwd_context.hash(password)
 
 
 async def get_payload(token: str):
     return jwt.decode(token, configs.secret_key, algorithms=configs.algorithm)
 
 
+def get_user_id(token: str):
+    payload = jwt.decode(token, configs.secret_key, algorithms=configs.algorithm)
+    return payload["sub"]
+
+
 async def is_valid_token(token: str):
     payload = await get_payload(token)
     exp = payload.get("exp")
     now = datetime.now()
     if exp and datetime.fromtimestamp(exp) < now:
         return JSONResponse(
             status_code=401,
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/common/util/snowflake.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/common/util/snowflake.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/middleware/__pycache__/db_session_middleware.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/__pycache__/db_session_middleware.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xde4b1566 (Tue Apr  9 14:08:30 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 4684
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/middleware/db_session_middleware.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/middleware/db_session_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/__pycache__/__init__.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/__init__.cpython-311.pyc`

 * *Files 17% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x64c01766 (Thu Apr 11 10:50:12 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 221
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/__pycache__/server.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/__pycache__/server.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 5977
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/server.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/server.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/v1/__pycache__/probe_controller.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/__pycache__/probe_controller.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 981
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/api/v1/probe_controller.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/api/v1/probe_controller.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/enum/__pycache__/system.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/enum/__pycache__/system.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Tue Apr  9 14:08:30 2024 UTC, .py size: 454 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,67 @@
-00000000: a70d 0d0a 0000 0000 de4b 1566 c601 0000  .........K.f....
-00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 4e00 0000 9700 6400 5a00  ......N.....d.Z.
-00000030: 6401 6402 6c01 6d02 5a02 0100 0200 4700  d.d.l.m.Z.....G.
-00000040: 6403 8400 6404 6502 a603 0000 ab03 0000  d...d.e.........
-00000050: 0000 0000 0000 5a03 0200 4700 6405 8400  ......Z...G.d...
-00000060: 6406 6502 a603 0000 ab03 0000 0000 0000  d.e.............
-00000070: 0000 5a04 6407 5300 2908 7a14 5379 7374  ..Z.d.S.).z.Syst
-00000080: 656d 2072 6573 706f 6e73 6520 636f 6465  em response code
-00000090: e900 0000 0029 01da 0445 6e75 6d63 0000  .....)...Enumc..
-000000a0: 0000 0000 0000 0000 0000 0100 0000 0000  ................
-000000b0: 0000 f320 0000 0097 0065 005a 0164 005a  ... .....e.Z.d.Z
-000000c0: 0264 015a 0364 025a 0464 035a 0564 0484  .d.Z.d.Z.d.Z.d..
-000000d0: 005a 0664 0553 0029 06da 1253 7973 7465  .Z.d.S.)...Syste
-000000e0: 6d52 6573 706f 6e73 6543 6f64 6529 0272  mResponseCode).r
-000000f0: 0200 0000 da07 5375 6363 6573 7329 02e9  ......Success)..
-00000100: ffff ffff fa16 7365 7276 6963 6520 696e  ......service in
-00000110: 7465 726e 616c 2065 7272 6f72 2902 6991  ternal error).i.
-00000120: 0100 0072 0800 0000 6303 0000 0000 0000  ...r....c.......
-00000130: 0000 0000 0002 0000 0003 0000 00f3 2200  ..............".
-00000140: 0000 9700 7c01 7c00 5f00 0000 0000 0000  ....|.|._.......
-00000150: 0000 7c02 7c00 5f01 0000 0000 0000 0000  ..|.|._.........
-00000160: 6400 5300 a901 4ea9 02da 0463 6f64 65da  d.S...N....code.
-00000170: 036d 7367 a903 da04 7365 6c66 720c 0000  .msg....selfr...
-00000180: 0072 0d00 0000 7303 0000 0020 2020 fa57  .r....s....   .W
-00000190: 453a 5c75 7365 725c 7472 6169 6e5c 7072  E:\user\train\pr
-000001a0: 6f64 7563 7469 6f6e 5c66 6173 7461 7069  oduction\fastapi
-000001b0: 2d73 716c 6d6f 6465 6c2d 7374 6172 7465  -sqlmodel-starte
-000001c0: 725c 7372 635c 6673 735c 7374 6172 7465  r\src\fss\starte
-000001d0: 725c 7379 7374 656d 5c65 6e75 6d5c 7379  r\system\enum\sy
-000001e0: 7374 656d 2e70 79da 085f 5f69 6e69 745f  stem.py..__init_
-000001f0: 5f7a 1b53 7973 7465 6d52 6573 706f 6e73  _z.SystemRespons
-00000200: 6543 6f64 652e 5f5f 696e 6974 5f5f 0b00  eCode.__init__..
-00000210: 0000 f314 0000 0080 00d8 1418 8804 8c09  ................
-00000220: d813 1688 048c 0888 0888 08f3 0000 0000  ................
-00000230: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000240: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00000250: 6c6e 616d 655f 5fda 0753 5543 4345 5353  lname__..SUCCESS
-00000260: da16 5345 5256 4943 455f 494e 5445 524e  ..SERVICE_INTERN
-00000270: 414c 5f45 5252 4f52 da0b 4155 5448 5f46  AL_ERROR..AUTH_F
-00000280: 4149 4c45 4472 1100 0000 a900 7213 0000  AILEDr......r...
-00000290: 0072 1000 0000 7205 0000 0072 0500 0000  .r....r....r....
-000002a0: 0600 0000 7333 0000 0080 0080 0080 0080  ....s3..........
-000002b0: 0080 00d8 0e1c 8047 d81d 3bd0 041a d812  .......G..;.....
-000002c0: 3180 4bf0 0402 0517 f000 0205 17f0 0002  1.K.............
-000002d0: 0517 f000 0205 17f0 0002 0517 7213 0000  ............r...
-000002e0: 0072 0500 0000 6300 0000 0000 0000 0000  .r....c.........
-000002f0: 0000 0001 0000 0000 0000 00f3 1800 0000  ................
-00000300: 9700 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00000310: 8400 5a04 6403 5300 2904 da12 5379 7374  ..Z.d.S.)...Syst
-00000320: 656d 436f 6e73 7461 6e74 436f 6465 2902  emConstantCode).
-00000330: e90a 0000 007a 0575 7365 723a 6303 0000  .....z.user:c...
-00000340: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00000350: 00f3 2200 0000 9700 7c01 7c00 5f00 0000  ..".....|.|._...
-00000360: 0000 0000 0000 7c02 7c00 5f01 0000 0000  ......|.|._.....
-00000370: 0000 0000 6400 5300 720a 0000 0072 0b00  ....d.S.r....r..
-00000380: 0000 720e 0000 0073 0300 0000 2020 2072  ..r....s....   r
-00000390: 1000 0000 7211 0000 007a 1b53 7973 7465  ....r....z.Syste
-000003a0: 6d43 6f6e 7374 616e 7443 6f64 652e 5f5f  mConstantCode.__
-000003b0: 696e 6974 5f5f 1300 0000 7212 0000 0072  init__....r....r
-000003c0: 1300 0000 4e29 0572 1400 0000 7215 0000  ....N).r....r...
-000003d0: 0072 1600 0000 da08 5553 4552 5f4b 4559  .r......USER_KEY
-000003e0: 7211 0000 0072 1a00 0000 7213 0000 0072  r....r....r....r
-000003f0: 1000 0000 721c 0000 0072 1c00 0000 1000  ....r....r......
-00000400: 0000 7328 0000 0080 0080 0080 0080 0080  ..s(............
-00000410: 00d8 0f1c 8048 f004 0205 17f0 0002 0517  .....H..........
-00000420: f000 0205 17f0 0002 0517 f000 0205 1772  ...............r
-00000430: 1300 0000 721c 0000 004e 2905 da07 5f5f  ....r....N)...__
-00000440: 646f 635f 5fda 0465 6e75 6d72 0300 0000  doc__..enumr....
-00000450: 7205 0000 0072 1c00 0000 721a 0000 0072  r....r....r....r
-00000460: 1300 0000 7210 0000 00fa 083c 6d6f 6475  ....r......<modu
-00000470: 6c65 3e72 2200 0000 0100 0000 737b 0000  le>r".......s{..
-00000480: 00f0 0301 0101 d800 1ad0 001a e000 15d0  ................
-00000490: 0015 d000 15d0 0015 d000 15d0 0015 f006  ................
-000004a0: 0701 17f0 0007 0117 f000 0701 17f0 0007  ................
-000004b0: 0117 f000 0701 1798 14f1 0007 0117 f400  ................
-000004c0: 0701 17f0 0007 0117 f014 0501 17f0 0005  ................
-000004d0: 0117 f000 0501 17f0 0005 0117 f000 0501  ................
-000004e0: 1798 14f1 0005 0117 f400 0501 17f0 0005  ................
-000004f0: 0117 f000 0501 17f0 0005 0117 7213 0000  ............r...
-00000500: 00                                       .
+00000000: 550d 0d0a 0000 0000 3120 1966 f501 0000  U.......1 .f....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 4700  Z.d.d.l.m.Z...G.
+00000040: 6403 6404 8400 6404 6502 8303 5a03 4700  d.d...d.e...Z.G.
+00000050: 6405 6406 8400 6406 6502 8303 5a04 6407  d.d...d.e...Z.d.
+00000060: 5300 2908 7a14 5379 7374 656d 2072 6573  S.).z.System res
+00000070: 706f 6e73 6520 636f 6465 e900 0000 0029  ponse code.....)
+00000080: 01da 0445 6e75 6d63 0000 0000 0000 0000  ...Enumc........
+00000090: 0000 0000 0000 0000 0200 0000 4000 0000  ............@...
+000000a0: 7324 0000 0065 005a 0164 005a 0264 015a  s$...e.Z.d.Z.d.Z
+000000b0: 0364 025a 0464 035a 0564 045a 0664 0564  .d.Z.d.Z.d.Z.d.d
+000000c0: 0684 005a 0764 0753 0029 08da 1253 7973  ...Z.d.S.)...Sys
+000000d0: 7465 6d52 6573 706f 6e73 6543 6f64 6529  temResponseCode)
+000000e0: 0272 0100 0000 da07 5375 6363 6573 7329  .r......Success)
+000000f0: 02e9 ffff ffff fa16 7365 7276 6963 6520  ........service 
+00000100: 696e 7465 726e 616c 2065 7272 6f72 2902  internal error).
+00000110: 6991 0100 0072 0600 0000 2902 6990 0100  i....r....).i...
+00000120: 005a 0f70 6172 616d 6574 6572 5f65 7272  .Z.parameter_err
+00000130: 6f72 6303 0000 0000 0000 0000 0000 0003  orc.............
+00000140: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
+00000150: 7c01 7c00 5f00 7c02 7c00 5f01 6400 5300  |.|._.|.|._.d.S.
+00000160: a901 4ea9 02da 0463 6f64 65da 036d 7367  ..N....code..msg
+00000170: a903 da04 7365 6c66 7209 0000 0072 0a00  ....selfr....r..
+00000180: 0000 a900 720d 0000 00fa 5745 3a5c 7573  ....r.....WE:\us
+00000190: 6572 5c74 7261 696e 5c70 726f 6475 6374  er\train\product
+000001a0: 696f 6e5c 6661 7374 6170 692d 7371 6c6d  ion\fastapi-sqlm
+000001b0: 6f64 656c 2d73 7461 7274 6572 5c73 7263  odel-starter\src
+000001c0: 5c66 7373 5c73 7461 7274 6572 5c73 7973  \fss\starter\sys
+000001d0: 7465 6d5c 656e 756d 5c73 7973 7465 6d2e  tem\enum\system.
+000001e0: 7079 da08 5f5f 696e 6974 5f5f 0c00 0000  py..__init__....
+000001f0: 7304 0000 0000 0106 017a 1b53 7973 7465  s........z.Syste
+00000200: 6d52 6573 706f 6e73 6543 6f64 652e 5f5f  mResponseCode.__
+00000210: 696e 6974 5f5f 4e29 08da 085f 5f6e 616d  init__N)...__nam
+00000220: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000230: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0753  .__qualname__..S
+00000240: 5543 4345 5353 da16 5345 5256 4943 455f  UCCESS..SERVICE_
+00000250: 494e 5445 524e 414c 5f45 5252 4f52 5a0b  INTERNAL_ERRORZ.
+00000260: 4155 5448 5f46 4149 4c45 445a 0f50 4152  AUTH_FAILEDZ.PAR
+00000270: 414d 4554 4552 5f45 5252 4f52 720f 0000  AMETER_ERRORr...
+00000280: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000290: 720e 0000 0072 0300 0000 0600 0000 730a  r....r........s.
+000002a0: 0000 0008 0104 0104 0104 0104 0272 0300  .............r..
+000002b0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000002c0: 0000 0002 0000 0040 0000 0073 1800 0000  .......@...s....
+000002d0: 6500 5a01 6400 5a02 6401 5a03 6402 6403  e.Z.d.Z.d.Z.d.d.
+000002e0: 8400 5a04 6404 5300 2905 da12 5379 7374  ..Z.d.S.)...Syst
+000002f0: 656d 436f 6e73 7461 6e74 436f 6465 2902  emConstantCode).
+00000300: e90a 0000 007a 0575 7365 723a 6303 0000  .....z.user:c...
+00000310: 0000 0000 0000 0000 0003 0000 0002 0000  ................
+00000320: 0043 0000 0073 1000 0000 7c01 7c00 5f00  .C...s....|.|._.
+00000330: 7c02 7c00 5f01 6400 5300 7207 0000 0072  |.|._.d.S.r....r
+00000340: 0800 0000 720b 0000 0072 0d00 0000 720d  ....r....r....r.
+00000350: 0000 0072 0e00 0000 720f 0000 0014 0000  ...r....r.......
+00000360: 0073 0400 0000 0001 0601 7a1b 5379 7374  .s........z.Syst
+00000370: 656d 436f 6e73 7461 6e74 436f 6465 2e5f  emConstantCode._
+00000380: 5f69 6e69 745f 5f4e 2905 7210 0000 0072  _init__N).r....r
+00000390: 1100 0000 7212 0000 005a 0855 5345 525f  ....r....Z.USER_
+000003a0: 4b45 5972 0f00 0000 720d 0000 0072 0d00  KEYr....r....r..
+000003b0: 0000 720d 0000 0072 0e00 0000 7215 0000  ..r....r....r...
+000003c0: 0011 0000 0073 0400 0000 0801 0402 7215  .....s........r.
+000003d0: 0000 004e 2905 da07 5f5f 646f 635f 5fda  ...N)...__doc__.
+000003e0: 0465 6e75 6d72 0200 0000 7203 0000 0072  .enumr....r....r
+000003f0: 1500 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
+00000400: 0000 0072 0e00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000410: 653e 0100 0000 7306 0000 0004 020c 0310  e>....s.........
+00000420: 0b                                       .
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/exception/__pycache__/system.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/exception/__pycache__/system.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 358
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/mapper/__pycache__/user_mapper.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/__pycache__/user_mapper.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 1045
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/mapper/user_mapper.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/mapper/user_mapper.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/model/__pycache__/user_do.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/__pycache__/user_do.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 728
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/model/user_do.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/model/user_do.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/router/__pycache__/system.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/router/__pycache__/system.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 376
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/fss/starter/system/service/__pycache__/user_service.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/fss/starter/system/service/__pycache__/user_service.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.11, timestamp-based, .py timestamp: Thu Apr 11 10:49:23 2024 UTC, .py size: 548 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,89 +1,68 @@
-00000000: a70d 0d0a 0000 0000 33c0 1766 2402 0000  ........3..f$...
-00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
-00000020: 0000 0000 00f3 7800 0000 9700 6400 5a00  ......x.....d.Z.
-00000030: 6401 6402 6c01 6d02 5a02 6d03 5a03 0100  d.d.l.m.Z.m.Z...
-00000040: 6401 6403 6c04 6d05 5a05 0100 6401 6404  d.d.l.m.Z...d.d.
-00000050: 6c06 6d07 5a07 0100 6401 6405 6c08 6d09  l.m.Z...d.d.l.m.
-00000060: 5a09 0100 6401 6406 6c0a 6d0b 5a0b 6d0c  Z...d.d.l.m.Z.m.
-00000070: 5a0c 0100 0200 4700 6407 8400 6408 6507  Z.....G.d...d.e.
-00000080: 6509 1900 0000 0000 0000 0000 6502 a604  e...........e...
-00000090: 0000 ab04 0000 0000 0000 0000 5a0d 6409  ............Z.d.
-000000a0: 5300 290a 7a1d 5573 6572 2064 6f6d 6169  S.).z.User domai
-000000b0: 6e20 7365 7276 6963 6520 696e 7465 7266  n service interf
-000000c0: 6163 65e9 0000 0000 2902 da03 4142 43da  ace.....)...ABC.
-000000d0: 0e61 6273 7472 6163 746d 6574 686f 6429  .abstractmethod)
-000000e0: 01da 0554 6f6b 656e 2901 da07 5365 7276  ...Token)...Serv
-000000f0: 6963 6529 01da 0655 7365 7244 4f29 02da  ice)...UserDO)..
-00000100: 0955 7365 7251 7565 7279 da08 4c6f 6769  .UserQuery..Logi
-00000110: 6e43 6d64 6300 0000 0000 0000 0000 0000  nCmdc...........
-00000120: 0005 0000 0000 0000 00f3 4e00 0000 9700  ..........N.....
-00000130: 6500 5a01 6400 5a02 6503 6401 6504 6402  e.Z.d.Z.e.d.e.d.
-00000140: 6505 6604 6403 8404 a600 0000 ab00 0000  e.f.d...........
-00000150: 0000 0000 0000 5a06 6503 6404 6507 6402  ......Z.e.d.e.d.
-00000160: 6508 6604 6405 8404 a600 0000 ab00 0000  e.f.d...........
-00000170: 0000 0000 0000 5a09 6406 5300 2907 da0b  ......Z.d.S.)...
-00000180: 5573 6572 5365 7276 6963 65da 0269 64da  UserService..id.
-00000190: 0672 6574 7572 6e63 0200 0000 0000 0000  .returnc........
-000001a0: 0000 0000 0100 0000 8300 0000 f314 0000  ................
-000001b0: 004b 0001 0097 0074 0000 0000 0000 0000  .K.....t........
-000001c0: 0000 0082 01a9 014e a901 da13 4e6f 7449  .......N....NotI
-000001d0: 6d70 6c65 6d65 6e74 6564 4572 726f 7229  mplementedError)
-000001e0: 02da 0473 656c 6672 0c00 0000 7302 0000  ...selfr....s...
-000001f0: 0020 20fa 6045 3a5c 7573 6572 5c74 7261  .  .`E:\user\tra
-00000200: 696e 5c70 726f 6475 6374 696f 6e5c 6661  in\production\fa
-00000210: 7374 6170 692d 7371 6c6d 6f64 656c 2d73  stapi-sqlmodel-s
-00000220: 7461 7274 6572 5c73 7263 5c66 7373 5c73  tarter\src\fss\s
-00000230: 7461 7274 6572 5c73 7973 7465 6d5c 7365  tarter\system\se
-00000240: 7276 6963 655c 7573 6572 5f73 6572 7669  rvice\user_servi
-00000250: 6365 2e70 79da 0a66 696e 645f 6279 5f69  ce.py..find_by_i
-00000260: 647a 1655 7365 7253 6572 7669 6365 2e66  dz.UserService.f
-00000270: 696e 645f 6279 5f69 640c 0000 00f3 0c00  ind_by_id.......
-00000280: 0000 e800 e800 8000 e50e 21d0 0821 f300  ..........!..!..
-00000290: 0000 00da 086c 6f67 696e 436d 6463 0200  .....loginCmdc..
-000002a0: 0000 0000 0000 0000 0000 0100 0000 8300  ................
-000002b0: 0000 f314 0000 004b 0001 0097 0074 0000  .......K.....t..
-000002c0: 0000 0000 0000 0000 0082 0172 0f00 0000  ...........r....
-000002d0: 7210 0000 0029 0272 1200 0000 7217 0000  r....).r....r...
-000002e0: 0073 0200 0000 2020 7213 0000 00da 056c  .s....  r......l
-000002f0: 6f67 696e 7a11 5573 6572 5365 7276 6963  oginz.UserServic
-00000300: 652e 6c6f 6769 6e10 0000 0072 1500 0000  e.login....r....
-00000310: 7216 0000 004e 290a da08 5f5f 6e61 6d65  r....N)...__name
-00000320: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000330: 5f5f 7175 616c 6e61 6d65 5f5f 7204 0000  __qualname__r...
-00000340: 00da 0369 6e74 7208 0000 0072 1400 0000  ...intr....r....
-00000350: 7209 0000 0072 0500 0000 7219 0000 00a9  r....r....r.....
-00000360: 0072 1600 0000 7213 0000 0072 0b00 0000  .r....r....r....
-00000370: 720b 0000 000b 0000 0073 6e00 0000 8000  r........sn.....
-00000380: 8000 8000 8000 8000 d805 13f0 0201 0522  ..............."
-00000390: a033 f000 0105 22a8 39f0 0001 0522 f000  .3....".9...."..
-000003a0: 0105 22f0 0001 0522 f103 0006 1484 5ef0  .."...."......^.
-000003b0: 0201 0522 f006 0006 14f0 0201 0522 a048  ...".........".H
-000003c0: f000 0105 22b0 15f0 0001 0522 f000 0105  ...."......"....
-000003d0: 22f0 0001 0522 f103 0006 1484 5ef0 0201  "...."......^...
-000003e0: 0522 f000 0105 22f0 0001 0522 7216 0000  ."...."...."r...
-000003f0: 0072 0b00 0000 4e29 0eda 075f 5f64 6f63  .r....N)...__doc
-00000400: 5f5f da03 6162 6372 0300 0000 7204 0000  __..abcr....r...
-00000410: 00da 1866 7373 2e63 6f6d 6d6f 6e2e 7363  ...fss.common.sc
-00000420: 6865 6d61 2e73 6368 656d 6172 0500 0000  hema.schemar....
-00000430: da1a 6673 732e 636f 6d6d 6f6e 2e73 6572  ..fss.common.ser
-00000440: 7669 6365 2e73 6572 7669 6365 7206 0000  vice.servicer...
-00000450: 00da 2066 7373 2e73 7461 7274 6572 2e73  .. fss.starter.s
-00000460: 7973 7465 6d2e 6d6f 6465 6c2e 7573 6572  ystem.model.user
-00000470: 5f64 6f72 0700 0000 da25 6673 732e 7374  _dor.....%fss.st
-00000480: 6172 7465 722e 7379 7374 656d 2e73 6368  arter.system.sch
-00000490: 656d 612e 7573 6572 5f73 6368 656d 6172  ema.user_schemar
-000004a0: 0800 0000 7209 0000 0072 0b00 0000 721e  ....r....r....r.
-000004b0: 0000 0072 1600 0000 7213 0000 00fa 083c  ...r....r......<
-000004c0: 6d6f 6475 6c65 3e72 2500 0000 0100 0000  module>r%.......
-000004d0: 73ab 0000 00f0 0301 0101 d800 23d0 0023  s...........#..#
-000004e0: e000 23d0 0023 d000 23d0 0023 d000 23d0  ..#..#..#..#..#.
-000004f0: 0023 d000 23d0 0023 e000 2ad0 002a d000  .#..#..#..*..*..
-00000500: 2ad0 002a d000 2ad0 002a d800 2ed0 002e  *..*..*..*......
-00000510: d000 2ed0 002e d000 2ed0 002e d800 33d0  ..............3.
-00000520: 0033 d000 33d0 0033 d000 33d0 0033 d800  .3..3..3..3..3..
-00000530: 45d0 0045 d000 45d0 0045 d000 45d0 0045  E..E..E..E..E..E
-00000540: d000 45d0 0045 f006 0701 22f0 0007 0122  ..E..E...."...."
-00000550: f000 0701 22f0 0007 0122 f000 0701 2290  ...."...."....".
-00000560: 2798 2694 2fa0 33f1 0007 0122 f400 0701  '.&./.3...."....
-00000570: 22f0 0007 0122 f000 0701 22f0 0007 0122  "...."...."...."
-00000580: 7216 0000 00                             r....
+00000000: 550d 0d0a 0000 0000 3120 1966 2402 0000  U.......1 .f$...
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0005 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
+00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6401  ..d.d.l.m.Z...d.
+00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 6d0c 5a0c 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
+00000080: 6507 6509 1900 6502 8304 5a0d 6409 5300  e.e...e...Z.d.S.
+00000090: 290a 7a1d 5573 6572 2064 6f6d 6169 6e20  ).z.User domain 
+000000a0: 7365 7276 6963 6520 696e 7465 7266 6163  service interfac
+000000b0: 65e9 0000 0000 2902 da03 4142 43da 0e61  e.....)...ABC..a
+000000c0: 6273 7472 6163 746d 6574 686f 6429 01da  bstractmethod)..
+000000d0: 0554 6f6b 656e 2901 da07 5365 7276 6963  .Token)...Servic
+000000e0: 6529 01da 0655 7365 7244 4f29 02da 0955  e)...UserDO)...U
+000000f0: 7365 7251 7565 7279 da08 4c6f 6769 6e43  serQuery..LoginC
+00000100: 6d64 6300 0000 0000 0000 0000 0000 0000  mdc.............
+00000110: 0000 0004 0000 0040 0000 0073 3400 0000  .......@...s4...
+00000120: 6500 5a01 6400 5a02 6503 6504 6505 6401  e.Z.d.Z.e.e.e.d.
+00000130: 9c02 6402 6403 8404 8301 5a06 6503 6507  ..d.d.....Z.e.e.
+00000140: 6508 6404 9c02 6405 6406 8404 8301 5a09  e.d...d.d.....Z.
+00000150: 6407 5300 2908 da0b 5573 6572 5365 7276  d.S.)...UserServ
+00000160: 6963 6529 02da 0269 64da 0672 6574 7572  ice)...id..retur
+00000170: 6e63 0200 0000 0000 0000 0000 0000 0200  nc..............
+00000180: 0000 0100 0000 c300 0000 7308 0000 0074  ..........s....t
+00000190: 0082 0164 0053 00a9 014e a901 da13 4e6f  ...d.S...N....No
+000001a0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
+000001b0: 7229 02da 0473 656c 6672 0a00 0000 a900  r)...selfr......
+000001c0: 7210 0000 00fa 6045 3a5c 7573 6572 5c74  r.....`E:\user\t
+000001d0: 7261 696e 5c70 726f 6475 6374 696f 6e5c  rain\production\
+000001e0: 6661 7374 6170 692d 7371 6c6d 6f64 656c  fastapi-sqlmodel
+000001f0: 2d73 7461 7274 6572 5c73 7263 5c66 7373  -starter\src\fss
+00000200: 5c73 7461 7274 6572 5c73 7973 7465 6d5c  \starter\system\
+00000210: 7365 7276 6963 655c 7573 6572 5f73 6572  service\user_ser
+00000220: 7669 6365 2e70 79da 0a66 696e 645f 6279  vice.py..find_by
+00000230: 5f69 640c 0000 0073 0200 0000 0002 7a16  _id....s......z.
+00000240: 5573 6572 5365 7276 6963 652e 6669 6e64  UserService.find
+00000250: 5f62 795f 6964 2902 da08 6c6f 6769 6e43  _by_id)...loginC
+00000260: 6d64 720b 0000 0063 0200 0000 0000 0000  mdr....c........
+00000270: 0000 0000 0200 0000 0100 0000 c300 0000  ................
+00000280: 7308 0000 0074 0082 0164 0053 0072 0c00  s....t...d.S.r..
+00000290: 0000 720d 0000 0029 0272 0f00 0000 7213  ..r....).r....r.
+000002a0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+000002b0: 0000 da05 6c6f 6769 6e10 0000 0073 0200  ....login....s..
+000002c0: 0000 0002 7a11 5573 6572 5365 7276 6963  ....z.UserServic
+000002d0: 652e 6c6f 6769 6e4e 290a da08 5f5f 6e61  e.loginN)...__na
+000002e0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+000002f0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7203  ..__qualname__r.
+00000300: 0000 00da 0369 6e74 7207 0000 0072 1200  .....intr....r..
+00000310: 0000 7208 0000 0072 0400 0000 7214 0000  ..r....r....r...
+00000320: 0072 1000 0000 7210 0000 0072 1000 0000  .r....r....r....
+00000330: 7211 0000 0072 0900 0000 0b00 0000 7308  r....r........s.
+00000340: 0000 0008 0102 0112 0302 0172 0900 0000  ...........r....
+00000350: 4e29 0eda 075f 5f64 6f63 5f5f da03 6162  N)...__doc__..ab
+00000360: 6372 0200 0000 7203 0000 00da 1866 7373  cr....r......fss
+00000370: 2e63 6f6d 6d6f 6e2e 7363 6865 6d61 2e73  .common.schema.s
+00000380: 6368 656d 6172 0400 0000 da1a 6673 732e  chemar......fss.
+00000390: 636f 6d6d 6f6e 2e73 6572 7669 6365 2e73  common.service.s
+000003a0: 6572 7669 6365 7205 0000 00da 2066 7373  ervicer..... fss
+000003b0: 2e73 7461 7274 6572 2e73 7973 7465 6d2e  .starter.system.
+000003c0: 6d6f 6465 6c2e 7573 6572 5f64 6f72 0600  model.user_dor..
+000003d0: 0000 da25 6673 732e 7374 6172 7465 722e  ...%fss.starter.
+000003e0: 7379 7374 656d 2e73 6368 656d 612e 7573  system.schema.us
+000003f0: 6572 5f73 6368 656d 6172 0700 0000 7208  er_schemar....r.
+00000400: 0000 0072 0900 0000 7210 0000 0072 1000  ...r....r....r..
+00000410: 0000 7210 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
+00000420: 6f64 756c 653e 0100 0000 730c 0000 0004  odule>....s.....
+00000430: 0210 020c 010c 010c 0110 03              ...........
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/coverage_html.js` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_07ed4fb7c74d9876___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_07ed4fb7c74d9876___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_3be97aced3f710c9_user_mapper_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_07ed4fb7c74d9876_user_do_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_3be97aced3f710c9_user_mapper_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_07ed4fb7c74d9876_user_do_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_07ed4fb7c74d9876_user_do_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_07ed4fb7c74d9876_user_do_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_07ed4fb7c74d9876___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_ebd618dd09682660___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -111,13 +111,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_07ed4fb7c74d9876___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_ebd618dd09682660___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1100 ssttaatteemmeennttss ?  1100 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""User data object""" 
 _2 
 _3from typing import Optional 
 _4 
 _5from sqlmodel import Field, Column, String, SQLModel 
 _6 
 _7from fss.common.persistence.base_model import ModelExt, BaseModel 
@@ -34,8 +34,8 @@
 _2_1 ) 
 _2_2 
 _2_3 
 _2_4class UserDO(ModelExt, BaseUser, BaseModel, table=True): 
 _2_5 __tablename__ = "system_user" 
 _2_6 __table_args__ = {"comment": "用户信息表"} 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_0e53216603666de3___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_0e53216603666de3___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695_sqlmodel_impl_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0e53216603666de3_result_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695_sqlmodel_impl_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0e53216603666de3_result_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_0e53216603666de3_result_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_0e53216603666de3_result_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\common\result\result.py: 82%</title>
+    <title>Coverage for fss\common\result\result.py: 85%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>fss\common\result\result.py</b>:
-            <span class="pc_cov">82%</span>
+            <span class="pc_cov">85%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,25 +51,25 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">34 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">28<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">6<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">29<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">5<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_0e53216603666de3___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8efc05ae27a1a50a___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -146,28 +146,28 @@
     <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t"><span class="key">def</span> <span class="nam">success</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">data</span><span class="op">:</span> <span class="nam">DataType</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="nam">msg</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">str</span><span class="op">]</span> <span class="op">=</span> <span class="str">"success"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="nam">code</span><span class="op">:</span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span> <span class="op">=</span> <span class="nam">DEFAULT_SUCCESS_CODE</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="key">if</span> <span class="nam">data</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="str">"code"</span><span class="op">:</span> <span class="nam">code</span><span class="op">,</span> <span class="str">"msg"</span><span class="op">:</span> <span class="nam">msg</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span><span class="str">"code"</span><span class="op">:</span> <span class="nam">code</span><span class="op">,</span> <span class="str">"msg"</span><span class="op">:</span> <span class="nam">msg</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="str">"code"</span><span class="op">:</span> <span class="nam">code</span><span class="op">,</span> <span class="str">"msg"</span><span class="op">:</span> <span class="nam">msg</span><span class="op">,</span> <span class="str">"data"</span><span class="op">:</span> <span class="nam">data</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="key">def</span> <span class="nam">fail</span><span class="op">(</span><span class="nam">msg</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">code</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="str">"code"</span><span class="op">:</span> <span class="nam">code</span><span class="op">,</span> <span class="str">"msg"</span><span class="op">:</span> <span class="nam">msg</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_0e53216603666de3___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8efc05ae27a1a50a___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\rreessuulltt\\rreessuulltt..ppyy:: 8822%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\rreessuulltt\\rreessuulltt..ppyy:: 8855%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 3344 ssttaatteemmeennttss ?  2288 rruunn 66 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 3344 ssttaatteemmeennttss ?  2299 rruunn 55 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""The results returned by the project""" 
 _2 
 _3from typing import Sequence 
 _4from math import ceil 
 _5from typing import Generic, TypeVar, Any, Optional 
 _6 
 _7from fastapi_pagination import Params, Page 
@@ -84,8 +84,8 @@
 _7_1 return {"code": code, "msg": msg} 
 _7_2 return {"code": code, "msg": msg, "data": data} 
 _7_3 
 _7_4 
 _7_5def fail(msg: str, code: int) -> Any: 
 _7_6 return {"code": code, "msg": msg} 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_160d2543108c5886___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_160d2543108c5886___init___py.html`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a44f0ac069e85531___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2ddb7f614afd77c0___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a44f0ac069e85531___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2ddb7f614afd77c0___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_1e0a65662954c73a___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_23127160240ab4f6___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_1e0a65662954c73a_cache_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_23127160240ab4f6___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_1e0a65662954c73a_cache_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_1e0a65662954c73a_cache_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a_cache_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_1e0a65662954c73a___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_1e0a65662954c73a_page_cache_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -129,13 +129,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_1e0a65662954c73a___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_1e0a65662954c73a_page_cache_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2233 ssttaatteemmeennttss ?  1155 rruunn 88 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Abstract base class for Cache""" 
 _2 
 _3from abc import ABC, abstractmethod 
 _4 
 _5 
 _6from fss.common.config import configs 
 _7 
@@ -52,8 +52,8 @@
 _3_9 
 _4_0 redis_client = await RedisManager.get_instance() 
 _4_1 return RedisCache(redis_client) 
 _4_2 from fss.common.cache.page_cache import PageCache 
 _4_3 
 _4_4 return PageCache() 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_1e0a65662954c73a_page_cache_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_1e0a65662954c73a_page_cache_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_1e0a65662954c73a_cache_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_23127160240ab4f6_config_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -120,13 +120,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_1e0a65662954c73a_cache_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_23127160240ab4f6_config_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2211 ssttaatteemmeennttss ?  1133 rruunn 88 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Simple in-memory page cache implementation""" 
 _2 
 _3from typing import Any 
 _4 
 _5import diskcache 
 _6 
 _7from fss.common.cache.cache import Cache 
@@ -43,8 +43,8 @@
 _3_0 
 _3_1 async def exists(self, key: str) -> bool: 
 _3_2 """Check if a key exists in the in-memory cache.""" 
 _3_3 if key in self.cache: 
 _3_4 return True 
 _3_5 return False 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_204be9a6e4696b99___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_204be9a6e4696b99___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_5d95fe6a529b7852___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9c41cf131237e8e8___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_5d95fe6a529b7852___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9c41cf131237e8e8___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_23127160240ab4f6___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_737f82a7e813f983___init___py.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\common\__init__.py: 100%</title>
+    <title>Coverage for fss\common\service\__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\common\__init__.py</b>:
+            <span class="text">Coverage for </span><b>fss\common\service\__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_794d731f07d9e36c___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2a5f9cf02f67ac9f_security_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_1e0a65662954c73a___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_9373b28d605cd29a___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,18 +80,18 @@
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_794d731f07d9e36c___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2a5f9cf02f67ac9f_security_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_1e0a65662954c73a___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_9373b28d605cd29a___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\sseerrvviiccee\\____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_23127160240ab4f6_config_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_23127160240ab4f6_config_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_1e0a65662954c73a_page_cache_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8e9ea00a623205ec___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -166,13 +166,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_1e0a65662954c73a_page_cache_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8e9ea00a623205ec___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 6611 ssttaatteemmeennttss ?  4400 rruunn 2211 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Configuration in the project""" 
 _2 
 _3import os 
 _4import subprocess 
 _5import time 
 _6from typing import Union, Tuple 
 _7from loguru import logger 
@@ -89,8 +89,8 @@
 _7_6 except ValueError: 
 _7_7 import multiprocessing 
 _7_8 
 _7_9 cpu_count = multiprocessing.cpu_count() 
 _8_0 workers = max(cpu_count - 2, 1) 
 _8_1 return port, workers 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2488d75dd8f8469d___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2488d75dd8f8469d___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8e9ea00a623205ec_enum_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2488d75dd8f8469d_exception_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8e9ea00a623205ec_enum_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2488d75dd8f8469d_exception_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2488d75dd8f8469d_exception_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2488d75dd8f8469d_exception_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_2488d75dd8f8469d___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -101,13 +101,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_2488d75dd8f8469d___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 66 ssttaatteemmeennttss ?  33 rruunn 33 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""The exceptions used in the project""" 
 _2 
 _3import http 
 _4 
 _5 
 _6class ServiceException(Exception): 
 _7 def __init__(self, code: int, msg: str, status_code: int =
@@ -25,8 +25,8 @@
 _1_1 :param msg: error message 
 _1_2 :param status_code: http status code 
 _1_3 """ 
 _1_4 self.code = code 
 _1_5 self.msg = msg 
 _1_6 self.status_code = status_code 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2a5f9cf02f67ac9f___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2a5f9cf02f67ac9f___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8efc05ae27a1a50a_schema_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2a5f9cf02f67ac9f_security_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8efc05ae27a1a50a_schema_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2a5f9cf02f67ac9f_security_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2a5f9cf02f67ac9f_security_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2a5f9cf02f67ac9f_security_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_2a5f9cf02f67ac9f___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_737f82a7e813f983___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -126,13 +126,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_2a5f9cf02f67ac9f___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_737f82a7e813f983___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2211 ssttaatteemmeennttss ?  1177 rruunn 44 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1from typing import Callable 
 _2 
 _3from fastapi import Depends, HTTPException 
 _4from fastapi.security import OAuth2PasswordBearer 
 _5from jose import ExpiredSignatureError 
 _6from multipart.exceptions import DecodeError 
 _7from starlette import status 
@@ -50,8 +50,8 @@
 _3_6 ) 
 _3_7 user_id = payload["sub"] 
 _3_8 
 _3_9 return CurrentUser(user_id=user_id) 
 _4_0 
 _4_1 return current_user 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2ddb7f614afd77c0___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_160d2543108c5886___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2ddb7f614afd77c0_probe_test_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_160d2543108c5886___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2ddb7f614afd77c0_probe_test_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2ddb7f614afd77c0_probe_test_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0_probe_test_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_2ddb7f614afd77c0___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2ddb7f614afd77c0_user_test_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -103,13 +103,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_2ddb7f614afd77c0___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2ddb7f614afd77c0_user_test_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1122 ssttaatteemmeennttss ?  1122 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1from fastapi.testclient import TestClient 
 _2 
 _3from fss.common.config import configs 
 _4from fss.starter.server import app 
 _5 
 _6client = TestClient(app) 
 _7 
@@ -26,8 +26,8 @@
 _1_3 
 _1_4 
 _1_5def test_probe_readiness(): 
 _1_6 response = client.get(f"{configs.api_version}/probe/readiness") 
 _1_7 assert response.status_code == 200 
 _1_8 assert response.json() == {"code": 0, "msg": "hello"} 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_2ddb7f614afd77c0_user_test_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8_probe_controller_py.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for tests\system\v1\user_test.py: 100%</title>
+    <title>Coverage for fss\starter\system\api\v1\probe_controller.py: 80%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>tests\system\v1\user_test.py</b>:
-            <span class="pc_cov">100%</span>
+            <span class="text">Coverage for </span><b>fss\starter\system\api\v1\probe_controller.py</b>:
+            <span class="pc_cov">80%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,87 +50,82 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">21 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">21<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
+            <span class="text">20 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">16<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">4<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_2ddb7f614afd77c0_probe_test_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_9c41cf131237e8e8_user_controller_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span><span class="op">.</span><span class="nam">testclient</span> <span class="key">import</span> <span class="nam">TestClient</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Project health probe"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">config</span> <span class="key">import</span> <span class="nam">configs</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">server</span> <span class="key">import</span> <span class="nam">app</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">APIRouter</span><span class="op">,</span> <span class="nam">Depends</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">loguru</span> <span class="key">import</span> <span class="nam">logger</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="nam">client</span> <span class="op">=</span> <span class="nam">TestClient</span><span class="op">(</span><span class="nam">app</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">def</span> <span class="nam">test_user_register</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">user_data</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">        <span class="str">"username"</span><span class="op">:</span> <span class="str">"example_user"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">        <span class="str">"password"</span><span class="op">:</span> <span class="str">"example_password"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="str">"nickname"</span><span class="op">:</span> <span class="str">"Example Nickname"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span><span class="str">f"{configs.api_version}/user/register"</span><span class="op">,</span> <span class="nam">json</span><span class="op">=</span><span class="nam">user_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"code"</span><span class="op">]</span> <span class="op">==</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">def</span> <span class="nam">test_user_login</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="str">f"{configs.api_version}/user/login"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="nam">data</span><span class="op">=</span><span class="op">{</span><span class="str">"username"</span><span class="op">:</span> <span class="str">"example_user"</span><span class="op">,</span> <span class="str">"password"</span><span class="op">:</span> <span class="str">"example_password"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"token_type"</span><span class="op">]</span> <span class="op">==</span> <span class="str">"bearer"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="key">def</span> <span class="nam">test_user_me</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="nam">login_response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="str">f"{configs.api_version}/user/login"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">data</span><span class="op">=</span><span class="op">{</span><span class="str">"username"</span><span class="op">:</span> <span class="str">"example_user"</span><span class="op">,</span> <span class="str">"password"</span><span class="op">:</span> <span class="str">"example_password"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">assert</span> <span class="nam">login_response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">access_token</span> <span class="op">=</span> <span class="nam">login_response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"access_token"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">headers</span> <span class="op">=</span> <span class="op">{</span><span class="str">"Authorization"</span><span class="op">:</span> <span class="str">f"Bearer {access_token}"</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">f"{configs.api_version}/user/me"</span><span class="op">,</span> <span class="nam">headers</span><span class="op">=</span><span class="nam">headers</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"code"</span><span class="op">]</span> <span class="op">==</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">enum</span><span class="op">.</span><span class="nam">system</span> <span class="key">import</span> <span class="nam">SystemResponseCode</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">impl</span><span class="op">.</span><span class="nam">user_service_impl</span> <span class="key">import</span> <span class="nam">get_user_service</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">user_service</span> <span class="key">import</span> <span class="nam">UserService</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">probe_router</span> <span class="op">=</span> <span class="nam">APIRouter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="nam">USER_ID</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="nam">HI</span> <span class="op">=</span> <span class="str">"hi"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="nam">HELLO</span> <span class="op">=</span> <span class="str">"hello"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="com"># Liveness probe</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="op">@</span><span class="nam">probe_router</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/liveness"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">def</span> <span class="nam">liveness</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="str">"code"</span><span class="op">:</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">.</span><span class="nam">code</span><span class="op">,</span> <span class="str">"msg"</span><span class="op">:</span> <span class="nam">HI</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="com"># Readiness probe</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="op">@</span><span class="nam">probe_router</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/readiness"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">readiness</span><span class="op">(</span><span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">find_by_id</span><span class="op">(</span><span class="nam">USER_ID</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">except</span> <span class="nam">Exception</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">logger</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"readiness error: {e}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="str">"code"</span><span class="op">:</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">SERVICE_INTERNAL_ERROR</span><span class="op">.</span><span class="nam">code</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="str">"msg"</span><span class="op">:</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">SERVICE_INTERNAL_ERROR</span><span class="op">.</span><span class="nam">msg</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="str">"code"</span><span class="op">:</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">.</span><span class="nam">code</span><span class="op">,</span> <span class="str">"msg"</span><span class="op">:</span> <span class="nam">HELLO</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_2ddb7f614afd77c0_probe_test_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_9c41cf131237e8e8_user_controller_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,55 +1,50 @@
-************ CCoovveerraaggee ffoorr tteessttss\\ssyysstteemm\\vv11\\uusseerr__tteesstt..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\aappii\\vv11\\pprroobbee__ccoonnttrroolllleerr..ppyy:: 8800%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 2211 ssttaatteemmeennttss ?  2211 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 2200 ssttaatteemmeennttss ?  1166 rruunn 44 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
-_1from fastapi.testclient import TestClient 
+12 22:20 +0800
+_1"""Project health probe""" 
 _2 
-_3from fss.common.config import configs 
-_4from fss.starter.server import app 
+_3from fastapi import APIRouter, Depends 
+_4from loguru import logger 
 _5 
-_6client = TestClient(app) 
-_7 
-_8 
-_9def test_user_register(): 
-_1_0 user_data = { 
-_1_1 "username": "example_user", 
-_1_2 "password": "example_password", 
-_1_3 "nickname": "Example Nickname", 
-_1_4 } 
-_1_5 response = client.post(f"{configs.api_version}/user/register",
-json=user_data) 
-_1_6 assert response.status_code == 200 
-_1_7 assert response.json()["code"] == 0 
-_1_8 
-_1_9 
-_2_0def test_user_login(): 
-_2_1 response = client.post( 
-_2_2 f"{configs.api_version}/user/login", 
-_2_3 data={"username": "example_user", "password": "example_password"}, 
-_2_4 ) 
-_2_5 assert response.status_code == 200 
-_2_6 assert response.json()["token_type"] == "bearer" 
-_2_7 
-_2_8 
-_2_9def test_user_me(): 
-_3_0 login_response = client.post( 
-_3_1 f"{configs.api_version}/user/login", 
-_3_2 data={"username": "example_user", "password": "example_password"}, 
-_3_3 ) 
-_3_4 assert login_response.status_code == 200 
-_3_5 access_token = login_response.json()["access_token"] 
-_3_6 headers = {"Authorization": f"Bearer {access_token}"} 
-_3_7 response = client.get(f"{configs.api_version}/user/me", headers=headers) 
-_3_8 assert response.status_code == 200 
-_3_9 assert response.json()["code"] == 0 
+_6from fss.starter.system.enum.system import SystemResponseCode 
+_7from fss.starter.system.service.impl.user_service_impl import
+get_user_service 
+_8from fss.starter.system.service.user_service import UserService 
+_9 
+_1_0probe_router = APIRouter() 
+_1_1 
+_1_2USER_ID = 1 
+_1_3HI = "hi" 
+_1_4HELLO = "hello" 
+_1_5 
+_1_6 
+_1_7# Liveness probe 
+_1_8@probe_router.get("/liveness") 
+_1_9def liveness(): 
+_2_0 return {"code": SystemResponseCode.SUCCESS.code, "msg": HI} 
+_2_1 
+_2_2 
+_2_3# Readiness probe 
+_2_4@probe_router.get("/readiness") 
+_2_5async def readiness(user_service: UserService = Depends(get_user_service)): 
+_2_6 try: 
+_2_7 await user_service.find_by_id(USER_ID) 
+_2_8 except Exception as e: 
+_2_9 logger.error(f"readiness error: {e}") 
+_3_0 return { 
+_3_1 "code": SystemResponseCode.SERVICE_INTERNAL_ERROR.code, 
+_3_2 "msg": SystemResponseCode.SERVICE_INTERNAL_ERROR.msg, 
+_3_3 } 
+_3_4 return {"code": SystemResponseCode.SUCCESS.code, "msg": HELLO} 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_392b9405ba6460b0___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0___init___py.html`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_737f82a7e813f983_service_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_392b9405ba6460b0_security_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_737f82a7e813f983_service_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_392b9405ba6460b0_security_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_392b9405ba6460b0_security_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0_security_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\common\util\security.py: 93%</title>
+    <title>Coverage for fss\common\util\security.py: 94%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>fss\common\util\security.py</b>:
-            <span class="pc_cov">93%</span>
+            <span class="pc_cov">94%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">28 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">26<span class="text"> run</span></button>
+            <span class="text">31 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">29<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">2<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_392b9405ba6460b0___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_392b9405ba6460b0_snowflake_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -116,31 +116,36 @@
     <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">return</span> <span class="nam">pwd_context</span><span class="op">.</span><span class="nam">hash</span><span class="op">(</span><span class="nam">password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">get_payload</span><span class="op">(</span><span class="nam">token</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">return</span> <span class="nam">jwt</span><span class="op">.</span><span class="nam">decode</span><span class="op">(</span><span class="nam">token</span><span class="op">,</span> <span class="nam">configs</span><span class="op">.</span><span class="nam">secret_key</span><span class="op">,</span> <span class="nam">algorithms</span><span class="op">=</span><span class="nam">configs</span><span class="op">.</span><span class="nam">algorithm</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">is_valid_token</span><span class="op">(</span><span class="nam">token</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">payload</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">get_payload</span><span class="op">(</span><span class="nam">token</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">exp</span> <span class="op">=</span> <span class="nam">payload</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"exp"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="nam">now</span> <span class="op">=</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">if</span> <span class="nam">exp</span> <span class="key">and</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">fromtimestamp</span><span class="op">(</span><span class="nam">exp</span><span class="op">)</span> <span class="op">&lt;</span> <span class="nam">now</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="key">return</span> <span class="nam">JSONResponse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="nam">status_code</span><span class="op">=</span><span class="num">401</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">content</span><span class="op">=</span><span class="op">{</span><span class="str">"detail"</span><span class="op">:</span> <span class="str">"Token has expired"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="key">def</span> <span class="nam">get_user_id</span><span class="op">(</span><span class="nam">token</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">payload</span> <span class="op">=</span> <span class="nam">jwt</span><span class="op">.</span><span class="nam">decode</span><span class="op">(</span><span class="nam">token</span><span class="op">,</span> <span class="nam">configs</span><span class="op">.</span><span class="nam">secret_key</span><span class="op">,</span> <span class="nam">algorithms</span><span class="op">=</span><span class="nam">configs</span><span class="op">.</span><span class="nam">algorithm</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="key">return</span> <span class="nam">payload</span><span class="op">[</span><span class="str">"sub"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">is_valid_token</span><span class="op">(</span><span class="nam">token</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="nam">payload</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">get_payload</span><span class="op">(</span><span class="nam">token</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="nam">exp</span> <span class="op">=</span> <span class="nam">payload</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"exp"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="nam">now</span> <span class="op">=</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">now</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">if</span> <span class="nam">exp</span> <span class="key">and</span> <span class="nam">datetime</span><span class="op">.</span><span class="nam">fromtimestamp</span><span class="op">(</span><span class="nam">exp</span><span class="op">)</span> <span class="op">&lt;</span> <span class="nam">now</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="key">return</span> <span class="nam">JSONResponse</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="nam">status_code</span><span class="op">=</span><span class="num">401</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">            <span class="nam">content</span><span class="op">=</span><span class="op">{</span><span class="str">"detail"</span><span class="op">:</span> <span class="str">"Token has expired"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_392b9405ba6460b0___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_392b9405ba6460b0_snowflake_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\uuttiill\\sseeccuurriittyy..ppyy:: 9933%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\uuttiill\\sseeccuurriittyy..ppyy:: 9944%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 2288 ssttaatteemmeennttss ?  2266 rruunn 22 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 3311 ssttaatteemmeennttss ?  2299 rruunn 22 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Security util, such as encode decode and etc""" 
 _2 
 _3from datetime import timedelta, datetime 
 _4from typing import Any, Union 
 _5 
 _6from jose import jwt 
 _7from passlib.context import CryptContext 
@@ -50,18 +50,24 @@
 _3_4 return pwd_context.hash(password) 
 _3_5 
 _3_6 
 _3_7async def get_payload(token: str): 
 _3_8 return jwt.decode(token, configs.secret_key, algorithms=configs.algorithm) 
 _3_9 
 _4_0 
-_4_1async def is_valid_token(token: str): 
-_4_2 payload = await get_payload(token) 
-_4_3 exp = payload.get("exp") 
-_4_4 now = datetime.now() 
-_4_5 if exp and datetime.fromtimestamp(exp) < now: 
-_4_6 return JSONResponse( 
-_4_7 status_code=401, 
-_4_8 content={"detail": "Token has expired"}, 
-_4_9 ) 
+_4_1def get_user_id(token: str): 
+_4_2 payload = jwt.decode(token, configs.secret_key,
+algorithms=configs.algorithm) 
+_4_3 return payload["sub"] 
+_4_4 
+_4_5 
+_4_6async def is_valid_token(token: str): 
+_4_7 payload = await get_payload(token) 
+_4_8 exp = payload.get("exp") 
+_4_9 now = datetime.now() 
+_5_0 if exp and datetime.fromtimestamp(exp) < now: 
+_5_1 return JSONResponse( 
+_5_2 status_code=401, 
+_5_3 content={"detail": "Token has expired"}, 
+_5_4 ) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_392b9405ba6460b0_snowflake_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_392b9405ba6460b0_snowflake_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_392b9405ba6460b0_security_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_dcf1c620283c9c76___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -150,13 +150,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_392b9405ba6460b0_security_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_dcf1c620283c9c76___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3399 ssttaatteemmeennttss ?  2288 rruunn 1111 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Snowflake util to generate unique id""" 
 _2 
 _3import os 
 _4import time 
 _5from typing import Generator 
 _6 
 _7API_EPOCH = 1640995200000 
@@ -73,8 +73,8 @@
 _6_0 | sequence 
 _6_1 ) 
 _6_2 
 _6_3 
 _6_4def snowflake_id() -> int: 
 _6_5 return next(generator()) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_3be97aced3f710c9___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3be97aced3f710c9___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b6eeb7fba27ca014_system_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_3be97aced3f710c9_user_mapper_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b6eeb7fba27ca014_system_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_3be97aced3f710c9_user_mapper_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_3be97aced3f710c9_user_mapper_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3be97aced3f710c9_user_mapper_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_3be97aced3f710c9___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_07ed4fb7c74d9876___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -119,13 +119,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_3be97aced3f710c9___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_07ed4fb7c74d9876___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1111 ssttaatteemmeennttss ?  1100 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""User operation mapper""" 
 _2 
 _3from typing import Union 
 _4 
 _5from sqlmodel import select 
 _6from sqlmodel.ext.asyncio.session import AsyncSession 
 _7 
@@ -43,8 +43,8 @@
 _2_9 select(UserDO).where(UserDO.username == username) 
 _3_0 ) 
 _3_1 return user.scalar_one_or_none() 
 _3_2 
 _3_3 
 _3_4userMapper = UserMapper(UserDO) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_3c9f025fb530798e___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3c9f025fb530798e___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_dcf1c620283c9c76_db_session_middleware_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_3c9f025fb530798e_server_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -94,13 +94,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_dcf1c620283c9c76_db_session_middleware_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_3c9f025fb530798e_server_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,19 +6,19 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 66 ssttaatteemmeennttss ?  66 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Add project to python path""" 
 _2 
 _3import os 
 _4import sys 
 _5from pathlib import Path 
 _6 
 _7current_dir = os.path.dirname(os.path.abspath(__file__)) 
 _8project_dir = str(Path(current_dir).parent.parent) 
 _9sys.path.insert(0, project_dir) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_3c9f025fb530798e_server_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_3c9f025fb530798e_server_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_3c9f025fb530798e___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d95fe6a529b7852___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -266,13 +266,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_3c9f025fb530798e___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d95fe6a529b7852___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 7711 ssttaatteemmeennttss ?  5500 rruunn 2211 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Server init""" 
 _2 
 _3import uvicorn 
 _4from fastapi import Request 
 _5from fastapi.exception_handlers import ( 
 _6 http_exception_handler, 
 _7 request_validation_exception_handler, 
@@ -194,8 +194,8 @@
 _1_7_6# Project run 
 _1_7_7def run() -> None: 
 _1_7_8 port, workers = prepare_run() 
 _1_7_9 uvicorn.run( 
 _1_8_0 app="fss.starter.server:app", host="0.0.0.0", port=port, workers=workers 
 _1_8_1 ) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_4c5c7dd0d2e26036___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_4c5c7dd0d2e26036___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8_user_controller_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_4c5c7dd0d2e26036_system_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8_user_controller_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_4c5c7dd0d2e26036_system_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_4c5c7dd0d2e26036_system_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_4c5c7dd0d2e26036_system_py.html`

 * *Files 4% similar despite different names*

```diff
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">13 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">13<span class="text"> run</span></button>
+            <span class="text">14 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">14<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_4c5c7dd0d2e26036___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b6eeb7fba27ca014___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,34 +85,35 @@
     <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">enum</span> <span class="key">import</span> <span class="nam">Enum</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">class</span> <span class="nam">SystemResponseCode</span><span class="op">(</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">    <span class="nam">SUCCESS</span> <span class="op">=</span> <span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="str">"Success"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="nam">SERVICE_INTERNAL_ERROR</span> <span class="op">=</span> <span class="op">(</span><span class="op">-</span><span class="num">1</span><span class="op">,</span> <span class="str">"service internal error"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="nam">AUTH_FAILED</span> <span class="op">=</span> <span class="op">(</span><span class="num">401</span><span class="op">,</span> <span class="str">"service internal error"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">code</span><span class="op">,</span> <span class="nam">msg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">code</span> <span class="op">=</span> <span class="nam">code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">msg</span> <span class="op">=</span> <span class="nam">msg</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">PARAMETER_ERROR</span> <span class="op">=</span> <span class="op">(</span><span class="num">400</span><span class="op">,</span> <span class="str">"parameter_error"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">code</span><span class="op">,</span> <span class="nam">msg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">code</span> <span class="op">=</span> <span class="nam">code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">msg</span> <span class="op">=</span> <span class="nam">msg</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">class</span> <span class="nam">SystemConstantCode</span><span class="op">(</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">USER_KEY</span> <span class="op">=</span> <span class="op">(</span><span class="num">10</span><span class="op">,</span> <span class="str">"user:"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">code</span><span class="op">,</span> <span class="nam">msg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">code</span> <span class="op">=</span> <span class="nam">code</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">msg</span> <span class="op">=</span> <span class="nam">msg</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">class</span> <span class="nam">SystemConstantCode</span><span class="op">(</span><span class="nam">Enum</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">USER_KEY</span> <span class="op">=</span> <span class="op">(</span><span class="num">10</span><span class="op">,</span> <span class="str">"user:"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">code</span><span class="op">,</span> <span class="nam">msg</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">code</span> <span class="op">=</span> <span class="nam">code</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">msg</span> <span class="op">=</span> <span class="nam">msg</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_4c5c7dd0d2e26036___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b6eeb7fba27ca014___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -4,33 +4,34 @@
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 1133 ssttaatteemmeennttss ?  1133 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 1144 ssttaatteemmeennttss ?  1144 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""System response code""" 
 _2 
 _3from enum import Enum 
 _4 
 _5 
 _6class SystemResponseCode(Enum): 
 _7 SUCCESS = (0, "Success") 
 _8 SERVICE_INTERNAL_ERROR = (-1, "service internal error") 
 _9 AUTH_FAILED = (401, "service internal error") 
-_1_0 
-_1_1 def __init__(self, code, msg): 
-_1_2 self.code = code 
-_1_3 self.msg = msg 
-_1_4 
+_1_0 PARAMETER_ERROR = (400, "parameter_error") 
+_1_1 
+_1_2 def __init__(self, code, msg): 
+_1_3 self.code = code 
+_1_4 self.msg = msg 
 _1_5 
-_1_6class SystemConstantCode(Enum): 
-_1_7 USER_KEY = (10, "user:") 
-_1_8 
-_1_9 def __init__(self, code, msg): 
-_2_0 self.code = code 
-_2_1 self.msg = msg 
+_1_6 
+_1_7class SystemConstantCode(Enum): 
+_1_8 USER_KEY = (10, "user:") 
+_1_9 
+_2_0 def __init__(self, code, msg): 
+_2_1 self.code = code 
+_2_2 self.msg = msg 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_5d95fe6a529b7852___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_5d95fe6a529b7852___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_3c9f025fb530798e_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_204be9a6e4696b99___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_3c9f025fb530798e_server_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_204be9a6e4696b99___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_737f82a7e813f983___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_23127160240ab4f6___init___py.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\common\service\__init__.py: 100%</title>
+    <title>Coverage for fss\common\__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\common\service\__init__.py</b>:
+            <span class="text">Coverage for </span><b>fss\common\__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_2a5f9cf02f67ac9f_security_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_794d731f07d9e36c___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_9373b28d605cd29a___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_1e0a65662954c73a___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,18 +80,18 @@
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_2a5f9cf02f67ac9f_security_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_794d731f07d9e36c___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_9373b28d605cd29a___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_1e0a65662954c73a___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\sseerrvviiccee\\____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_737f82a7e813f983_service_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_737f82a7e813f983_service_py.html`

 * *Files identical despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_9373b28d605cd29a_service_impl_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_392b9405ba6460b0___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -158,13 +158,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_9373b28d605cd29a_service_impl_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_392b9405ba6460b0___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 5500 ssttaatteemmeennttss ?  3355 rruunn 1155 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Abstract Service used in the project""" 
 _2 
 _3from abc import ABC, abstractmethod 
 _4from typing import Any, List, TypeVar, Generic 
 _5 
 _6T = TypeVar("T", bound=Any) 
 _7DEFAULT_BATCH_SIZE: int = 1000 
@@ -82,8 +82,8 @@
 _6_8 async def remove_by_id(self, *, id: T) -> bool: 
 _6_9 raise NotImplementedError 
 _7_0 
 _7_1 @abstractmethod 
 _7_2 async def remove_batch_by_ids(self, *, ids: List[Any]) -> bool: 
 _7_3 raise NotImplementedError 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_794d731f07d9e36c___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_a44f0ac069e85531___init___py.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\__init__.py: 100%</title>
+    <title>Coverage for tests\__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\__init__.py</b>:
+            <span class="text">Coverage for </span><b>tests\__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_fc0d8786bb154269_user_service_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_23127160240ab4f6___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_160d2543108c5886___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,18 +80,18 @@
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_fc0d8786bb154269_user_service_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_23127160240ab4f6___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_160d2543108c5886___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee ffoorr ffssss\\____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr tteessttss\\____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_8e9ea00a623205ec___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8e9ea00a623205ec___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_23127160240ab4f6_config_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8e9ea00a623205ec_enum_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_23127160240ab4f6_config_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8e9ea00a623205ec_enum_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_8e9ea00a623205ec_enum_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8e9ea00a623205ec_enum_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8e9ea00a623205ec___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2488d75dd8f8469d___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -116,13 +116,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8e9ea00a623205ec___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2488d75dd8f8469d___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1111 ssttaatteemmeennttss ?  1111 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""The enumerations used in the project""" 
 _2 
 _3from enum import Enum 
 _4 
 _5 
 _6class ModeEnum(str, Enum): 
 _7 """ 
@@ -39,8 +39,8 @@
 _2_6 """ 
 _2_7 Enum for token type. 
 _2_8 """ 
 _2_9 
 _3_0 access = "access" 
 _3_1 refresh = "refresh" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_8efc05ae27a1a50a___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8efc05ae27a1a50a___init___py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_0e53216603666de3_result_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8efc05ae27a1a50a_schema_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_0e53216603666de3_result_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_8efc05ae27a1a50a_schema_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_8efc05ae27a1a50a_schema_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_8efc05ae27a1a50a_schema_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_8efc05ae27a1a50a___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2a5f9cf02f67ac9f___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -100,13 +100,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_8efc05ae27a1a50a___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_2a5f9cf02f67ac9f___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1111 ssttaatteemmeennttss ?  1111 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1from pydantic import BaseModel, Field 
 _2 
 _3 
 _4class Token(BaseModel): 
 _5 access_token: str 
 _6 token_type: str 
 _7 expired_at: int 
@@ -23,8 +23,8 @@
 _1_0 
 _1_1 
 _1_2class CurrentUser(BaseModel): 
 _1_3 user_id: int 
 _1_4 roles: set = Field(default_factory=set) 
 _1_5 authorities: set = Field(default_factory=set) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9373b28d605cd29a___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9373b28d605cd29a___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_737f82a7e813f983___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9373b28d605cd29a_service_impl_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_737f82a7e813f983___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9373b28d605cd29a_service_impl_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9373b28d605cd29a_service_impl_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9373b28d605cd29a_service_impl_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\common\service\impl\service_impl.py: 53%</title>
+    <title>Coverage for fss\common\service\impl\service_impl.py: 57%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>fss\common\service\impl\service_impl.py</b>:
-            <span class="pc_cov">53%</span>
+            <span class="pc_cov">57%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,25 +51,25 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">47 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">25<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">22<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">27<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">20<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_9373b28d605cd29a___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_737f82a7e813f983_service_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -124,50 +124,50 @@
     <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">get_by_ids</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">T</span><span class="op">]</span><span class="op">,</span> <span class="nam">batch_size</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">1000</span><span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_by_ids</span><span class="op">(</span><span class="nam">ids</span><span class="op">=</span><span class="nam">ids</span><span class="op">,</span> <span class="nam">batch_size</span><span class="op">=</span><span class="nam">batch_size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">count</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_count</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">list</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_list</span><span class="op">(</span><span class="nam">page</span><span class="op">=</span><span class="nam">page</span><span class="op">,</span> <span class="nam">size</span><span class="op">=</span><span class="nam">size</span><span class="op">,</span> <span class="nam">query</span><span class="op">=</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_list</span><span class="op">(</span><span class="nam">page</span><span class="op">=</span><span class="nam">page</span><span class="op">,</span> <span class="nam">size</span><span class="op">=</span><span class="nam">size</span><span class="op">,</span> <span class="nam">query</span><span class="op">=</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">list_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">T</span><span class="op">,</span> <span class="nam">order_by</span><span class="op">:</span> <span class="nam">T</span><span class="op">,</span> <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">T</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_list_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_list_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">            <span class="nam">page</span><span class="op">=</span><span class="nam">page</span><span class="op">,</span> <span class="nam">size</span><span class="op">=</span><span class="nam">size</span><span class="op">,</span> <span class="nam">query</span><span class="op">=</span><span class="nam">query</span><span class="op">,</span> <span class="nam">order_by</span><span class="op">=</span><span class="nam">order_by</span><span class="op">,</span> <span class="nam">sort_order</span><span class="op">=</span><span class="nam">sort_order</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">list_page</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">params</span><span class="op">:</span> <span class="nam">T</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_list_page</span><span class="op">(</span><span class="nam">params</span><span class="op">=</span><span class="nam">params</span><span class="op">,</span> <span class="nam">query</span><span class="op">=</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_list_page</span><span class="op">(</span><span class="nam">params</span><span class="op">=</span><span class="nam">params</span><span class="op">,</span> <span class="nam">query</span><span class="op">=</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">list_page_ordered</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">params</span><span class="op">:</span> <span class="nam">T</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">T</span><span class="op">,</span> <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">T</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_list_page_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_list_page_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="nam">params</span><span class="op">=</span><span class="nam">params</span><span class="op">,</span> <span class="nam">query</span><span class="op">=</span><span class="nam">query</span><span class="op">,</span> <span class="nam">sort_order</span><span class="op">=</span><span class="nam">sort_order</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">update_by_id</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">update_by_id</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_batch_by_ids</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data_list</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">T</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">update_batch_by_ids</span><span class="op">(</span><span class="nam">data_list</span><span class="op">=</span><span class="nam">data_list</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">update_batch_by_ids</span><span class="op">(</span><span class="nam">data_list</span><span class="op">=</span><span class="nam">data_list</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">remove_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">T</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">delete_by_id</span><span class="op">(</span><span class="nam">id</span><span class="op">=</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">delete_by_id</span><span class="op">(</span><span class="nam">id</span><span class="op">=</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">remove_batch_by_ids</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">)</span> <span class="op">-></span> <span class="nam">bool</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">delete_batch_by_ids</span><span class="op">(</span><span class="nam">ids</span><span class="op">=</span><span class="nam">ids</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">delete_batch_by_ids</span><span class="op">(</span><span class="nam">ids</span><span class="op">=</span><span class="nam">ids</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_9373b28d605cd29a___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_737f82a7e813f983_service_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\sseerrvviiccee\\iimmppll\\sseerrvviiccee__iimmppll..ppyy:: 5533%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\sseerrvviiccee\\iimmppll\\sseerrvviiccee__iimmppll..ppyy:: 5577%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 4477 ssttaatteemmeennttss ?  2255 rruunn 2222 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 4477 ssttaatteemmeennttss ?  2277 rruunn 2200 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+13 15:26 +0800
 _1"""Common service impl""" 
 _2 
 _3from typing import Any, TypeVar, List, Generic, Type 
 _4 
 _5from fss.common.persistence.base_mapper import BaseMapper 
 _6from fss.common.service.service import Service 
 _7 
@@ -56,38 +56,38 @@
 [Any]: 
 _4_3 return await self.mapper.select_by_ids(ids=ids, batch_size=batch_size) 
 _4_4 
 _4_5 async def count(self) -> int: 
 _4_6 return await self.mapper.select_count() 
 _4_7 
 _4_8 async def list(self, *, page: int, size: int, query: T) -> List[T]: 
-_4_9 return self.mapper.select_list(page=page, size=size, query=query) 
+_4_9 return await self.mapper.select_list(page=page, size=size, query=query) 
 _5_0 
 _5_1 async def list_ordered( 
 _5_2 self, *, page: int, size: int, query: T, order_by: T, sort_order: T 
 _5_3 ) -> List[T]: 
-_5_4 return self.mapper.select_list_ordered( 
+_5_4 return await self.mapper.select_list_ordered( 
 _5_5 page=page, size=size, query=query, order_by=order_by, sort_order=sort_order 
 _5_6 ) 
 _5_7 
 _5_8 async def list_page(self, *, params: T, query: T) -> List[T]: 
-_5_9 return self.mapper.select_list_page(params=params, query=query) 
+_5_9 return await self.mapper.select_list_page(params=params, query=query) 
 _6_0 
 _6_1 async def list_page_ordered(self, *, params: T, query: T, sort_order: T) -
 > List[T]: 
-_6_2 return self.mapper.select_list_page_ordered( 
+_6_2 return await self.mapper.select_list_page_ordered( 
 _6_3 params=params, query=query, sort_order=sort_order 
 _6_4 ) 
 _6_5 
 _6_6 async def update_by_id(self, *, data: T) -> bool: 
-_6_7 return self.mapper.update_by_id(data=data) 
+_6_7 return await self.mapper.update_by_id(data=data) 
 _6_8 
 _6_9 async def update_batch_by_ids(self, *, data_list: List[T]) -> bool: 
-_7_0 return self.mapper.update_batch_by_ids(data_list=data_list) 
+_7_0 return await self.mapper.update_batch_by_ids(data_list=data_list) 
 _7_1 
 _7_2 async def remove_by_id(self, *, id: T) -> bool: 
-_7_3 return self.mapper.delete_by_id(id=id) 
+_7_3 return await self.mapper.delete_by_id(id=id) 
 _7_4 
 _7_5 async def remove_batch_by_ids(self, *, ids: List[Any]) -> bool: 
-_7_6 return self.mapper.delete_batch_by_ids(ids=ids) 
+_7_6 return await self.mapper.delete_batch_by_ids(ids=ids) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+13 15:26 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9c41cf131237e8e8___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_204be9a6e4696b99___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9c41cf131237e8e8_probe_controller_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_204be9a6e4696b99___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9c41cf131237e8e8_probe_controller_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9c41cf131237e8e8_probe_controller_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_fc0d8786bb154269_user_service_py.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\starter\system\api\v1\probe_controller.py: 80%</title>
+    <title>Coverage for fss\starter\system\service\user_service.py: 79%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\starter\system\api\v1\probe_controller.py</b>:
-            <span class="pc_cov">80%</span>
+            <span class="text">Coverage for </span><b>fss\starter\system\service\user_service.py</b>:
+            <span class="pc_cov">79%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,82 +50,82 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">20 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">16<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">4<span class="text"> missing</span></button>
+            <span class="text">24 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">19<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">5<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_f83affef05b47916_user_service_impl_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_9c41cf131237e8e8_user_controller_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a44f0ac069e85531___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Project health probe"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""User domain service interface"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">APIRouter</span><span class="op">,</span> <span class="nam">Depends</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">loguru</span> <span class="key">import</span> <span class="nam">logger</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">enum</span><span class="op">.</span><span class="nam">system</span> <span class="key">import</span> <span class="nam">SystemResponseCode</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">impl</span><span class="op">.</span><span class="nam">user_service_impl</span> <span class="key">import</span> <span class="nam">get_user_service</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">user_service</span> <span class="key">import</span> <span class="nam">UserService</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">probe_router</span> <span class="op">=</span> <span class="nam">APIRouter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="nam">USER_ID</span> <span class="op">=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="nam">HI</span> <span class="op">=</span> <span class="str">"hi"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="nam">HELLO</span> <span class="op">=</span> <span class="str">"hello"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="com"># Liveness probe</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="op">@</span><span class="nam">probe_router</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/liveness"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="key">def</span> <span class="nam">liveness</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="str">"code"</span><span class="op">:</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">.</span><span class="nam">code</span><span class="op">,</span> <span class="str">"msg"</span><span class="op">:</span> <span class="nam">HI</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="com"># Readiness probe</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="op">@</span><span class="nam">probe_router</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/readiness"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">readiness</span><span class="op">(</span><span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">        <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">find_by_id</span><span class="op">(</span><span class="nam">USER_ID</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">except</span> <span class="nam">Exception</span> <span class="key">as</span> <span class="nam">e</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">logger</span><span class="op">.</span><span class="nam">error</span><span class="op">(</span><span class="str">f"readiness error: {e}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">return</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="str">"code"</span><span class="op">:</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">SERVICE_INTERNAL_ERROR</span><span class="op">.</span><span class="nam">code</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">            <span class="str">"msg"</span><span class="op">:</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">SERVICE_INTERNAL_ERROR</span><span class="op">.</span><span class="nam">msg</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span><span class="str">"code"</span><span class="op">:</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">SUCCESS</span><span class="op">.</span><span class="nam">code</span><span class="op">,</span> <span class="str">"msg"</span><span class="op">:</span> <span class="nam">HELLO</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">abc</span> <span class="key">import</span> <span class="nam">ABC</span><span class="op">,</span> <span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">UploadFile</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi_pagination</span> <span class="key">import</span> <span class="nam">Params</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">starlette</span><span class="op">.</span><span class="nam">responses</span> <span class="key">import</span> <span class="nam">StreamingResponse</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">schema</span> <span class="key">import</span> <span class="nam">Token</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">service</span> <span class="key">import</span> <span class="nam">Service</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">user_do</span> <span class="key">import</span> <span class="nam">UserDO</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">user_schema</span> <span class="key">import</span> <span class="nam">UserQuery</span><span class="op">,</span> <span class="nam">LoginCmd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">class</span> <span class="nam">UserService</span><span class="op">(</span><span class="nam">Service</span><span class="op">[</span><span class="nam">UserDO</span><span class="op">]</span><span class="op">,</span> <span class="nam">ABC</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">find_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="nam">UserQuery</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">login</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">loginCmd</span><span class="op">:</span> <span class="nam">LoginCmd</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Token</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">export_user_template</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">StreamingResponse</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">import_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">file</span><span class="op">:</span> <span class="nam">UploadFile</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">export_user</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">params</span><span class="op">:</span> <span class="nam">Params</span><span class="op">)</span> <span class="op">-></span> <span class="nam">StreamingResponse</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_f83affef05b47916_user_service_impl_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_9c41cf131237e8e8_user_controller_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a44f0ac069e85531___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,50 +1,49 @@
-************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\aappii\\vv11\\pprroobbee__ccoonnttrroolllleerr..ppyy:: 8800%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\sseerrvviiccee\\uusseerr__sseerrvviiccee..ppyy:: 7799%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 2200 ssttaatteemmeennttss ?  1166 rruunn 44 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 2244 ssttaatteemmeennttss ?  1199 rruunn 55 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
-_1"""Project health probe""" 
+13 15:26 +0800
+_1"""User domain service interface""" 
 _2 
-_3from fastapi import APIRouter, Depends 
-_4from loguru import logger 
-_5 
-_6from fss.starter.system.enum.system import SystemResponseCode 
-_7from fss.starter.system.service.impl.user_service_impl import
-get_user_service 
-_8from fss.starter.system.service.user_service import UserService 
-_9 
-_1_0probe_router = APIRouter() 
-_1_1 
-_1_2USER_ID = 1 
-_1_3HI = "hi" 
-_1_4HELLO = "hello" 
-_1_5 
-_1_6 
-_1_7# Liveness probe 
-_1_8@probe_router.get("/liveness") 
-_1_9def liveness(): 
-_2_0 return {"code": SystemResponseCode.SUCCESS.code, "msg": HI} 
-_2_1 
-_2_2 
-_2_3# Readiness probe 
-_2_4@probe_router.get("/readiness") 
-_2_5async def readiness(user_service: UserService = Depends(get_user_service)): 
-_2_6 try: 
-_2_7 await user_service.find_by_id(USER_ID) 
-_2_8 except Exception as e: 
-_2_9 logger.error(f"readiness error: {e}") 
-_3_0 return { 
-_3_1 "code": SystemResponseCode.SERVICE_INTERNAL_ERROR.code, 
-_3_2 "msg": SystemResponseCode.SERVICE_INTERNAL_ERROR.msg, 
-_3_3 } 
-_3_4 return {"code": SystemResponseCode.SUCCESS.code, "msg": HELLO} 
+_3from abc import ABC, abstractmethod 
+_4 
+_5from fastapi import UploadFile 
+_6from fastapi_pagination import Params 
+_7from starlette.responses import StreamingResponse 
+_8 
+_9from fss.common.schema.schema import Token 
+_1_0from fss.common.service.service import Service 
+_1_1from fss.starter.system.model.user_do import UserDO 
+_1_2from fss.starter.system.schema.user_schema import UserQuery, LoginCmd 
+_1_3 
+_1_4 
+_1_5class UserService(Service[UserDO], ABC): 
+_1_6 @abstractmethod 
+_1_7 async def find_by_id(self, id: int) -> UserQuery: 
+_1_8 raise NotImplementedError 
+_1_9 
+_2_0 @abstractmethod 
+_2_1 async def login(self, loginCmd: LoginCmd) -> Token: 
+_2_2 raise NotImplementedError 
+_2_3 
+_2_4 @abstractmethod 
+_2_5 async def export_user_template(self) -> StreamingResponse: 
+_2_6 raise NotImplementedError 
+_2_7 
+_2_8 @abstractmethod 
+_2_9 async def import_user(self, file: UploadFile): 
+_3_0 raise NotImplementedError 
+_3_1 
+_3_2 @abstractmethod 
+_3_3 async def export_user(self, params: Params) -> StreamingResponse: 
+_3_4 raise NotImplementedError 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+13 15:26 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_9c41cf131237e8e8_user_controller_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_base_mapper_py.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\starter\system\api\v1\user_controller.py: 96%</title>
+    <title>Coverage for fss\common\persistence\base_mapper.py: 67%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\starter\system\api\v1\user_controller.py</b>:
-            <span class="pc_cov">96%</span>
+            <span class="text">Coverage for </span><b>fss\common\persistence\base_mapper.py</b>:
+            <span class="pc_cov">67%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,94 +50,143 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">25 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">24<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">1<span class="text"> missing</span></button>
+            <span class="text">51 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">34<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">17<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8_probe_controller_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_4c5c7dd0d2e26036___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_base_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""User operation controller"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""BaseMapper defines the implemented functionalities"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">APIRouter</span><span class="op">,</span> <span class="nam">Depends</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span><span class="op">.</span><span class="nam">security</span> <span class="key">import</span> <span class="nam">OAuth2PasswordRequestForm</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">abc</span> <span class="key">import</span> <span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">List</span><span class="op">,</span> <span class="nam">Type</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">result</span> <span class="key">import</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">result</span><span class="op">.</span><span class="nam">result</span> <span class="key">import</span> <span class="nam">BaseResponse</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">schema</span> <span class="key">import</span> <span class="nam">Token</span><span class="op">,</span> <span class="nam">CurrentUser</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">security</span><span class="op">.</span><span class="nam">security</span> <span class="key">import</span> <span class="nam">get_current_user</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">util</span><span class="op">.</span><span class="nam">security</span> <span class="key">import</span> <span class="nam">get_password_hash</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">user_do</span> <span class="key">import</span> <span class="nam">UserDO</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">user_schema</span> <span class="key">import</span> <span class="nam">UserCreateCmd</span><span class="op">,</span> <span class="nam">UserQuery</span><span class="op">,</span> <span class="nam">LoginCmd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">impl</span><span class="op">.</span><span class="nam">user_service_impl</span> <span class="key">import</span> <span class="nam">get_user_service</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">user_service</span> <span class="key">import</span> <span class="nam">UserService</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">persistence</span><span class="op">.</span><span class="nam">mapper</span> <span class="key">import</span> <span class="nam">Mapper</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">class</span> <span class="nam">BaseMapper</span><span class="op">(</span><span class="nam">Mapper</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">def</span> <span class="nam">count_affected_rows</span><span class="op">(</span><span class="nam">new_record</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">        <span class="key">if</span> <span class="nam">new_record</span><span class="op">.</span><span class="nam">id</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">            <span class="key">return</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="key">return</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="nam">user_router</span> <span class="op">=</span> <span class="nam">APIRouter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="com"># User registration</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span><span class="str">"/register"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">create_user</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">create_data</span><span class="op">:</span> <span class="nam">UserCreateCmd</span><span class="op">,</span> <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">BaseResponse</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="nam">create_data</span><span class="op">.</span><span class="nam">password</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">get_password_hash</span><span class="op">(</span><span class="nam">create_data</span><span class="op">.</span><span class="nam">password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="nam">user</span><span class="op">:</span> <span class="nam">UserDO</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">save</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">create_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">.</span><span class="nam">success</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">user</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_db_session</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Type</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">insert</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">insert_batch</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data_list</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="com"># Query user info</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/me"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">get_user</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">current_user</span><span class="op">:</span> <span class="nam">CurrentUser</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_current_user</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">BaseResponse</span><span class="op">[</span><span class="nam">UserQuery</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">user</span><span class="op">:</span> <span class="nam">UserQuery</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">find_by_id</span><span class="op">(</span><span class="nam">id</span><span class="op">=</span><span class="nam">current_user</span><span class="op">.</span><span class="nam">user_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">.</span><span class="nam">success</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">user</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">batch_size</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="com"># User login</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span><span class="str">"/login"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">login</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="nam">login_form</span><span class="op">:</span> <span class="nam">OAuth2PasswordRequestForm</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">Token</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="nam">loginCmd</span> <span class="op">=</span> <span class="nam">LoginCmd</span><span class="op">(</span><span class="nam">username</span><span class="op">=</span><span class="nam">login_form</span><span class="op">.</span><span class="nam">username</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="nam">login_form</span><span class="op">.</span><span class="nam">password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">return</span> <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">login</span><span class="op">(</span><span class="nam">loginCmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">order_by</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_page</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">params</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_page_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">params</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">order_by</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_batch_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data_list</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">delete_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">delete_batch_by_ids</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8_probe_controller_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_4c5c7dd0d2e26036___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_base_model_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,65 +1,112 @@
-************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\aappii\\vv11\\uusseerr__ccoonnttrroolllleerr..ppyy:: 9966%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\ppeerrssiisstteennccee\\bbaassee__mmaappppeerr..ppyy:: 6677%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 2255 ssttaatteemmeennttss ?  2244 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 5511 ssttaatteemmeennttss ?  3344 rruunn 1177 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
-_1"""User operation controller""" 
+12 22:20 +0800
+_1"""BaseMapper defines the implemented functionalities""" 
 _2 
-_3from fastapi import APIRouter, Depends 
-_4from fastapi.security import OAuth2PasswordRequestForm 
+_3from abc import abstractmethod 
+_4from typing import Any, List, Type 
 _5 
-_6from fss.common.result import result 
-_7from fss.common.result.result import BaseResponse 
-_8from fss.common.schema.schema import Token, CurrentUser 
-_9from fss.common.security.security import get_current_user 
-_1_0from fss.common.util.security import get_password_hash 
-_1_1from fss.starter.system.model.user_do import UserDO 
-_1_2from fss.starter.system.schema.user_schema import UserCreateCmd, UserQuery,
-LoginCmd 
-_1_3from fss.starter.system.service.impl.user_service_impl import
-get_user_service 
-_1_4from fss.starter.system.service.user_service import UserService 
+_6from fss.common.persistence.mapper import Mapper 
+_7 
+_8 
+_9class BaseMapper(Mapper): 
+_1_0 @staticmethod 
+_1_1 def count_affected_rows(new_record: Any) -> int: 
+_1_2 if new_record.id is not None: 
+_1_3 return 1 
+_1_4 return 0 
 _1_5 
-_1_6user_router = APIRouter() 
-_1_7 
-_1_8 
-_1_9# User registration 
-_2_0@user_router.post("/register") 
-_2_1async def create_user( 
-_2_2 create_data: UserCreateCmd, user_service: UserService = Depends
-(get_user_service) 
-_2_3) -> BaseResponse[int]: 
-_2_4 create_data.password = await get_password_hash(create_data.password) 
-_2_5 user: UserDO = await user_service.save(data=create_data) 
-_2_6 return result.success(data=user.id) 
+_1_6 @abstractmethod 
+_1_7 def get_db_session(self) -> Type[Any]: 
+_1_8 raise NotImplementedError 
+_1_9 
+_2_0 @abstractmethod 
+_2_1 async def insert(self, *, data: Any, db_session: Any) -> int: 
+_2_2 raise NotImplementedError 
+_2_3 
+_2_4 @abstractmethod 
+_2_5 async def insert_batch(self, *, data_list: List[Any], db_session: Any) -
+> int: 
+_2_6 raise NotImplementedError 
 _2_7 
-_2_8 
-_2_9# Query user info 
-_3_0@user_router.get("/me") 
-_3_1async def get_user( 
-_3_2 user_service: UserService = Depends(get_user_service), 
-_3_3 current_user: CurrentUser = Depends(get_current_user()), 
-_3_4) -> BaseResponse[UserQuery]: 
-_3_5 user: UserQuery = await user_service.find_by_id(id=current_user.user_id) 
-_3_6 return result.success(data=user) 
+_2_8 @abstractmethod 
+_2_9 async def select_by_id(self, *, id: Any, db_session: Any) -> Any: 
+_3_0 raise NotImplementedError 
+_3_1 
+_3_2 @abstractmethod 
+_3_3 async def select_by_ids( 
+_3_4 self, *, ids: List[Any], batch_size: int, db_session: Any 
+_3_5 ) -> List[Any]: 
+_3_6 raise NotImplementedError 
 _3_7 
-_3_8 
-_3_9# User login 
-_4_0@user_router.post("/login") 
-_4_1async def login( 
-_4_2 login_form: OAuth2PasswordRequestForm = Depends(), 
-_4_3 user_service: UserService = Depends(get_user_service), 
-_4_4) -> Token: 
-_4_5 loginCmd = LoginCmd(username=login_form.username,
-password=login_form.password) 
-_4_6 return await user_service.login(loginCmd) 
+_3_8 @abstractmethod 
+_3_9 async def select_count(self, *, db_session: Any) -> int: 
+_4_0 raise NotImplementedError 
+_4_1 
+_4_2 @abstractmethod 
+_4_3 async def select_list( 
+_4_4 self, *, page: int, size: int, query: Any, db_session: Any 
+_4_5 ) -> List[Any]: 
+_4_6 raise NotImplementedError 
+_4_7 
+_4_8 @abstractmethod 
+_4_9 async def select_list_ordered( 
+_5_0 self, 
+_5_1 *, 
+_5_2 page: int, 
+_5_3 size: int, 
+_5_4 query: Any, 
+_5_5 order_by: Any, 
+_5_6 sort_order: Any, 
+_5_7 db_session: Any, 
+_5_8 ) -> List[Any]: 
+_5_9 raise NotImplementedError 
+_6_0 
+_6_1 @abstractmethod 
+_6_2 async def select_list_page( 
+_6_3 self, *, params: Any, query: Any, db_session: Any 
+_6_4 ) -> List[Any]: 
+_6_5 raise NotImplementedError 
+_6_6 
+_6_7 @abstractmethod 
+_6_8 async def select_list_page_ordered( 
+_6_9 self, 
+_7_0 *, 
+_7_1 params: Any, 
+_7_2 query: Any, 
+_7_3 order_by: Any, 
+_7_4 sort_order: Any, 
+_7_5 db_session: Any, 
+_7_6 ) -> List[Any]: 
+_7_7 raise NotImplementedError 
+_7_8 
+_7_9 @abstractmethod 
+_8_0 async def update_by_id(self, *, data: Any, db_session: Any) -> int: 
+_8_1 raise NotImplementedError 
+_8_2 
+_8_3 @abstractmethod 
+_8_4 async def update_batch_by_ids( 
+_8_5 self, *, data_list: List[Any], db_session: Any 
+_8_6 ) -> int: 
+_8_7 raise NotImplementedError 
+_8_8 
+_8_9 @abstractmethod 
+_9_0 async def delete_by_id(self, *, id: Any, db_session: Any) -> int: 
+_9_1 raise NotImplementedError 
+_9_2 
+_9_3 @abstractmethod 
+_9_4 async def delete_batch_by_ids(self, *, ids: List[Any], db_session: Any) -
+> int: 
+_9_5 raise NotImplementedError 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_a44f0ac069e85531___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_f83affef05b47916___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for tests\__init__.py: 100%</title>
+    <title>Coverage for fss\starter\system\service\impl\__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>tests\__init__.py</b>:
+            <span class="text">Coverage for </span><b>fss\starter\system\service\impl\__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_fc0d8786bb154269_user_service_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_fc0d8786bb154269___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_160d2543108c5886___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_f83affef05b47916_user_service_impl_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,18 +80,18 @@
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_fc0d8786bb154269_user_service_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_fc0d8786bb154269___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_160d2543108c5886___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_f83affef05b47916_user_service_impl_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee ffoorr tteessttss\\____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\sseerrvviiccee\\iimmppll\\____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_b6eeb7fba27ca014___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_b6eeb7fba27ca014___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_4c5c7dd0d2e26036_system_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b6eeb7fba27ca014_system_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_4c5c7dd0d2e26036_system_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_b6eeb7fba27ca014_system_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_b6eeb7fba27ca014_system_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_b6eeb7fba27ca014_system_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_b6eeb7fba27ca014___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_3be97aced3f710c9___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -99,13 +99,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_b6eeb7fba27ca014___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_3be97aced3f710c9___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 55 ssttaatteemmeennttss ?  44 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1import http 
 _2 
 _3from fss.common.exception.exception import ServiceException 
 _4 
 _5 
 _6class SystemException(ServiceException): 
 _7 """ 
@@ -23,8 +23,8 @@
 _1_0 
 _1_1 def __init__(self, code: int, msg: str, status_code: int =
 http.HTTPStatus.OK): 
 _1_2 super(SystemException, self).__init__( 
 _1_3 code=code, msg=msg, status_code=status_code 
 _1_4 ) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_2488d75dd8f8469d_exception_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_base_mapper_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_2488d75dd8f8469d_exception_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_base_mapper_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695_base_mapper_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_2ddb7f614afd77c0_user_test_py.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\common\persistence\base_mapper.py: 67%</title>
+    <title>Coverage for tests\system\v1\user_test.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\common\persistence\base_mapper.py</b>:
-            <span class="pc_cov">67%</span>
+            <span class="text">Coverage for </span><b>tests\system\v1\user_test.py</b>:
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,143 +50,169 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">51 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">34<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">17<span class="text"> missing</span></button>
+            <span class="text">69 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">69<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2ddb7f614afd77c0_probe_test_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_base_model_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""BaseMapper defines the implemented functionalities"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="key">import</span> <span class="nam">io</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">abc</span> <span class="key">import</span> <span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">List</span><span class="op">,</span> <span class="nam">Type</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">persistence</span><span class="op">.</span><span class="nam">mapper</span> <span class="key">import</span> <span class="nam">Mapper</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">import</span> <span class="nam">pandas</span> <span class="key">as</span> <span class="nam">pd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">import</span> <span class="nam">pytest</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">UploadFile</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span><span class="op">.</span><span class="nam">testclient</span> <span class="key">import</span> <span class="nam">TestClient</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">class</span> <span class="nam">BaseMapper</span><span class="op">(</span><span class="nam">Mapper</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="op">@</span><span class="nam">staticmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">    <span class="key">def</span> <span class="nam">count_affected_rows</span><span class="op">(</span><span class="nam">new_record</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">        <span class="key">if</span> <span class="nam">new_record</span><span class="op">.</span><span class="nam">id</span> <span class="key">is</span> <span class="key">not</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">            <span class="key">return</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="key">return</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">config</span> <span class="key">import</span> <span class="nam">configs</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">util</span><span class="op">.</span><span class="nam">security</span> <span class="key">import</span> <span class="nam">get_user_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">server</span> <span class="key">import</span> <span class="nam">app</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">user_schema</span> <span class="key">import</span> <span class="nam">UpdateUserCmd</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="nam">client</span> <span class="op">=</span> <span class="nam">TestClient</span><span class="op">(</span><span class="nam">app</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_db_session</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Type</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">insert</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">insert_batch</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data_list</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">batch_size</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">def</span> <span class="nam">test_user_register</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">user_data</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">"username"</span><span class="op">:</span> <span class="str">"example_user"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="str">"password"</span><span class="op">:</span> <span class="str">"example_password"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="str">"nickname"</span><span class="op">:</span> <span class="str">"Example Nickname"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span><span class="str">f"{configs.api_version}/user/register"</span><span class="op">,</span> <span class="nam">json</span><span class="op">=</span><span class="nam">user_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"code"</span><span class="op">]</span> <span class="op">==</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"class"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="key">def</span> <span class="nam">login</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="str">f"{configs.api_version}/user/login"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">data</span><span class="op">=</span><span class="op">{</span><span class="str">"username"</span><span class="op">:</span> <span class="str">"example_user"</span><span class="op">,</span> <span class="str">"password"</span><span class="op">:</span> <span class="str">"example_password"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"token_type"</span><span class="op">]</span> <span class="op">==</span> <span class="str">"bearer"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="nam">access_token</span> <span class="op">=</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"access_token"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">    <span class="nam">user_id</span> <span class="op">=</span> <span class="nam">get_user_id</span><span class="op">(</span><span class="nam">access_token</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">yield</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"access_token"</span><span class="op">]</span><span class="op">,</span> <span class="nam">user_id</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="key">def</span> <span class="nam">test_user_login</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">        <span class="str">f"{configs.api_version}/user/login"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">data</span><span class="op">=</span><span class="op">{</span><span class="str">"username"</span><span class="op">:</span> <span class="str">"example_user"</span><span class="op">,</span> <span class="str">"password"</span><span class="op">:</span> <span class="str">"example_password"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"token_type"</span><span class="op">]</span> <span class="op">==</span> <span class="str">"bearer"</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">order_by</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t"><span class="key">def</span> <span class="nam">test_user_me</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="nam">login_response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="str">f"{configs.api_version}/user/login"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">data</span><span class="op">=</span><span class="op">{</span><span class="str">"username"</span><span class="op">:</span> <span class="str">"example_user"</span><span class="op">,</span> <span class="str">"password"</span><span class="op">:</span> <span class="str">"example_password"</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">assert</span> <span class="nam">login_response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="nam">access_token</span> <span class="op">=</span> <span class="nam">login_response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"access_token"</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">    <span class="nam">headers</span> <span class="op">=</span> <span class="op">{</span><span class="str">"Authorization"</span><span class="op">:</span> <span class="str">f"Bearer {access_token}"</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">f"{configs.api_version}/user/me"</span><span class="op">,</span> <span class="nam">headers</span><span class="op">=</span><span class="nam">headers</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"code"</span><span class="op">]</span> <span class="op">==</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_page</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">params</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_page_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">params</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">order_by</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_batch_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data_list</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="key">def</span> <span class="nam">test_update_user</span><span class="op">(</span><span class="nam">login</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">    <span class="nam">access_token</span><span class="op">,</span> <span class="nam">user_id</span> <span class="op">=</span> <span class="nam">login</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="nam">headers</span> <span class="op">=</span> <span class="op">{</span><span class="str">"Authorization"</span><span class="op">:</span> <span class="str">f"Bearer {access_token}"</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="nam">updateUserCmd</span> <span class="op">=</span> <span class="nam">UpdateUserCmd</span><span class="op">(</span><span class="nam">id</span><span class="op">=</span><span class="str">f"{user_id}"</span><span class="op">,</span> <span class="nam">nickname</span><span class="op">=</span><span class="str">"example_nickname"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="str">f"{configs.api_version}/user"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="nam">json</span><span class="op">=</span><span class="op">(</span><span class="nam">updateUserCmd</span><span class="op">.</span><span class="nam">model_dump</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="nam">headers</span><span class="op">=</span><span class="nam">headers</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"code"</span><span class="op">]</span> <span class="op">==</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="key">def</span> <span class="nam">test_export_user_template</span><span class="op">(</span><span class="nam">login</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="nam">access_token</span><span class="op">,</span> <span class="nam">user_id</span> <span class="op">=</span> <span class="nam">login</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="nam">headers</span> <span class="op">=</span> <span class="op">{</span><span class="str">"Authorization"</span><span class="op">:</span> <span class="str">f"Bearer {access_token}"</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">f"{configs.api_version}/user/exportTemplate"</span><span class="op">,</span> <span class="nam">headers</span><span class="op">=</span><span class="nam">headers</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="key">def</span> <span class="nam">test_export_user</span><span class="op">(</span><span class="nam">login</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">    <span class="nam">access_token</span><span class="op">,</span> <span class="nam">user_id</span> <span class="op">=</span> <span class="nam">login</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="nam">headers</span> <span class="op">=</span> <span class="op">{</span><span class="str">"Authorization"</span><span class="op">:</span> <span class="str">f"Bearer {access_token}"</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">f"{configs.api_version}/user/export"</span><span class="op">,</span> <span class="nam">headers</span><span class="op">=</span><span class="nam">headers</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">delete_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="op">@</span><span class="nam">abstractmethod</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">delete_batch_by_ids</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="key">raise</span> <span class="nam">NotImplementedError</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="key">def</span> <span class="nam">test_import_user</span><span class="op">(</span><span class="nam">login</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="nam">access_token</span><span class="op">,</span> <span class="nam">user_id</span> <span class="op">=</span> <span class="nam">login</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="nam">headers</span> <span class="op">=</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="str">"Authorization"</span><span class="op">:</span> <span class="str">f"Bearer {access_token}"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="str">"content_type"</span><span class="op">:</span> <span class="str">"multipart/form-data"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">    <span class="nam">df</span> <span class="op">=</span> <span class="nam">pd</span><span class="op">.</span><span class="nam">DataFrame</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">            <span class="str">"username"</span><span class="op">:</span> <span class="op">[</span><span class="str">"example_user_2"</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">            <span class="str">"password"</span><span class="op">:</span> <span class="op">[</span><span class="str">"password"</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">            <span class="str">"nickname"</span><span class="op">:</span> <span class="op">[</span><span class="str">"nickname"</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="nam">buffer</span> <span class="op">=</span> <span class="nam">io</span><span class="op">.</span><span class="nam">BytesIO</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="nam">df</span><span class="op">.</span><span class="nam">to_excel</span><span class="op">(</span><span class="nam">buffer</span><span class="op">,</span> <span class="nam">index</span><span class="op">=</span><span class="key">False</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">    <span class="nam">buffer</span><span class="op">.</span><span class="nam">seek</span><span class="op">(</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="nam">file</span> <span class="op">=</span> <span class="nam">UploadFile</span><span class="op">(</span><span class="nam">filename</span><span class="op">=</span><span class="str">"test_users.xlsx"</span><span class="op">,</span> <span class="nam">file</span><span class="op">=</span><span class="nam">buffer</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">        <span class="str">f"{configs.api_version}/user/import"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">        <span class="nam">headers</span><span class="op">=</span><span class="nam">headers</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">        <span class="nam">files</span><span class="op">=</span><span class="op">{</span><span class="str">"file"</span><span class="op">:</span> <span class="op">(</span><span class="nam">file</span><span class="op">.</span><span class="nam">filename</span><span class="op">,</span> <span class="nam">file</span><span class="op">.</span><span class="nam">file</span><span class="op">,</span> <span class="nam">file</span><span class="op">.</span><span class="nam">content_type</span><span class="op">)</span><span class="op">}</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">    <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"code"</span><span class="op">]</span> <span class="op">==</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t"><span class="key">def</span> <span class="nam">test_remove_user</span><span class="op">(</span><span class="nam">login</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">    <span class="nam">access_token</span><span class="op">,</span> <span class="nam">user_id</span> <span class="op">=</span> <span class="nam">login</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">    <span class="nam">headers</span> <span class="op">=</span> <span class="op">{</span><span class="str">"Authorization"</span><span class="op">:</span> <span class="str">f"Bearer {access_token}"</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="str">f"{configs.api_version}/user/{user_id}"</span><span class="op">,</span> <span class="nam">headers</span><span class="op">=</span><span class="nam">headers</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">status_code</span> <span class="op">==</span> <span class="num">200</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="key">assert</span> <span class="nam">response</span><span class="op">.</span><span class="nam">json</span><span class="op">(</span><span class="op">)</span><span class="op">[</span><span class="str">"code"</span><span class="op">]</span> <span class="op">==</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_2ddb7f614afd77c0_probe_test_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_base_model_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,112 +1,140 @@
-************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\ppeerrssiisstteennccee\\bbaassee__mmaappppeerr..ppyy:: 6677%% ************
+************ CCoovveerraaggee ffoorr tteessttss\\ssyysstteemm\\vv11\\uusseerr__tteesstt..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 5511 ssttaatteemmeennttss ?  3344 rruunn 1177 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 6699 ssttaatteemmeennttss ?  6699 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
-_1"""BaseMapper defines the implemented functionalities""" 
+13 15:26 +0800
+_1import io 
 _2 
-_3from abc import abstractmethod 
-_4from typing import Any, List, Type 
-_5 
-_6from fss.common.persistence.mapper import Mapper 
+_3import pandas as pd 
+_4import pytest 
+_5from fastapi import UploadFile 
+_6from fastapi.testclient import TestClient 
 _7 
-_8 
-_9class BaseMapper(Mapper): 
-_1_0 @staticmethod 
-_1_1 def count_affected_rows(new_record: Any) -> int: 
-_1_2 if new_record.id is not None: 
-_1_3 return 1 
-_1_4 return 0 
+_8from fss.common.config import configs 
+_9from fss.common.util.security import get_user_id 
+_1_0from fss.starter.server import app 
+_1_1from fss.starter.system.schema.user_schema import UpdateUserCmd 
+_1_2 
+_1_3client = TestClient(app) 
+_1_4 
 _1_5 
-_1_6 @abstractmethod 
-_1_7 def get_db_session(self) -> Type[Any]: 
-_1_8 raise NotImplementedError 
-_1_9 
-_2_0 @abstractmethod 
-_2_1 async def insert(self, *, data: Any, db_session: Any) -> int: 
-_2_2 raise NotImplementedError 
-_2_3 
-_2_4 @abstractmethod 
-_2_5 async def insert_batch(self, *, data_list: List[Any], db_session: Any) -
-> int: 
-_2_6 raise NotImplementedError 
-_2_7 
-_2_8 @abstractmethod 
-_2_9 async def select_by_id(self, *, id: Any, db_session: Any) -> Any: 
-_3_0 raise NotImplementedError 
-_3_1 
-_3_2 @abstractmethod 
-_3_3 async def select_by_ids( 
-_3_4 self, *, ids: List[Any], batch_size: int, db_session: Any 
-_3_5 ) -> List[Any]: 
-_3_6 raise NotImplementedError 
-_3_7 
-_3_8 @abstractmethod 
-_3_9 async def select_count(self, *, db_session: Any) -> int: 
-_4_0 raise NotImplementedError 
-_4_1 
-_4_2 @abstractmethod 
-_4_3 async def select_list( 
-_4_4 self, *, page: int, size: int, query: Any, db_session: Any 
-_4_5 ) -> List[Any]: 
-_4_6 raise NotImplementedError 
+_1_6def test_user_register(): 
+_1_7 user_data = { 
+_1_8 "username": "example_user", 
+_1_9 "password": "example_password", 
+_2_0 "nickname": "Example Nickname", 
+_2_1 } 
+_2_2 response = client.post(f"{configs.api_version}/user/register",
+json=user_data) 
+_2_3 assert response.status_code == 200 
+_2_4 assert response.json()["code"] == 0 
+_2_5 
+_2_6 
+_2_7@pytest.fixture(scope="class") 
+_2_8def login(): 
+_2_9 response = client.post( 
+_3_0 f"{configs.api_version}/user/login", 
+_3_1 data={"username": "example_user", "password": "example_password"}, 
+_3_2 ) 
+_3_3 assert response.status_code == 200 
+_3_4 assert response.json()["token_type"] == "bearer" 
+_3_5 access_token = response.json()["access_token"] 
+_3_6 user_id = get_user_id(access_token) 
+_3_7 yield response.json()["access_token"], user_id 
+_3_8 
+_3_9 
+_4_0def test_user_login(): 
+_4_1 response = client.post( 
+_4_2 f"{configs.api_version}/user/login", 
+_4_3 data={"username": "example_user", "password": "example_password"}, 
+_4_4 ) 
+_4_5 assert response.status_code == 200 
+_4_6 assert response.json()["token_type"] == "bearer" 
 _4_7 
-_4_8 @abstractmethod 
-_4_9 async def select_list_ordered( 
-_5_0 self, 
-_5_1 *, 
-_5_2 page: int, 
-_5_3 size: int, 
-_5_4 query: Any, 
-_5_5 order_by: Any, 
-_5_6 sort_order: Any, 
-_5_7 db_session: Any, 
-_5_8 ) -> List[Any]: 
-_5_9 raise NotImplementedError 
+_4_8 
+_4_9def test_user_me(): 
+_5_0 login_response = client.post( 
+_5_1 f"{configs.api_version}/user/login", 
+_5_2 data={"username": "example_user", "password": "example_password"}, 
+_5_3 ) 
+_5_4 assert login_response.status_code == 200 
+_5_5 access_token = login_response.json()["access_token"] 
+_5_6 headers = {"Authorization": f"Bearer {access_token}"} 
+_5_7 response = client.get(f"{configs.api_version}/user/me", headers=headers) 
+_5_8 assert response.status_code == 200 
+_5_9 assert response.json()["code"] == 0 
 _6_0 
-_6_1 @abstractmethod 
-_6_2 async def select_list_page( 
-_6_3 self, *, params: Any, query: Any, db_session: Any 
-_6_4 ) -> List[Any]: 
-_6_5 raise NotImplementedError 
-_6_6 
-_6_7 @abstractmethod 
-_6_8 async def select_list_page_ordered( 
-_6_9 self, 
-_7_0 *, 
-_7_1 params: Any, 
-_7_2 query: Any, 
-_7_3 order_by: Any, 
-_7_4 sort_order: Any, 
-_7_5 db_session: Any, 
-_7_6 ) -> List[Any]: 
-_7_7 raise NotImplementedError 
-_7_8 
-_7_9 @abstractmethod 
-_8_0 async def update_by_id(self, *, data: Any, db_session: Any) -> int: 
-_8_1 raise NotImplementedError 
-_8_2 
-_8_3 @abstractmethod 
-_8_4 async def update_batch_by_ids( 
-_8_5 self, *, data_list: List[Any], db_session: Any 
-_8_6 ) -> int: 
-_8_7 raise NotImplementedError 
+_6_1 
+_6_2def test_update_user(login): 
+_6_3 access_token, user_id = login 
+_6_4 headers = {"Authorization": f"Bearer {access_token}"} 
+_6_5 updateUserCmd = UpdateUserCmd(id=f"{user_id}", nickname="example_nickname") 
+_6_6 response = client.put( 
+_6_7 f"{configs.api_version}/user", 
+_6_8 json=(updateUserCmd.model_dump()), 
+_6_9 headers=headers, 
+_7_0 ) 
+_7_1 assert response.status_code == 200 
+_7_2 assert response.json()["code"] == 0 
+_7_3 
+_7_4 
+_7_5def test_export_user_template(login): 
+_7_6 access_token, user_id = login 
+_7_7 headers = {"Authorization": f"Bearer {access_token}"} 
+_7_8 response = client.get(f"{configs.api_version}/user/exportTemplate",
+headers=headers) 
+_7_9 assert response.status_code == 200 
+_8_0 
+_8_1 
+_8_2def test_export_user(login): 
+_8_3 access_token, user_id = login 
+_8_4 headers = {"Authorization": f"Bearer {access_token}"} 
+_8_5 response = client.get(f"{configs.api_version}/user/export",
+headers=headers) 
+_8_6 assert response.status_code == 200 
+_8_7 
 _8_8 
-_8_9 @abstractmethod 
-_9_0 async def delete_by_id(self, *, id: Any, db_session: Any) -> int: 
-_9_1 raise NotImplementedError 
-_9_2 
-_9_3 @abstractmethod 
-_9_4 async def delete_batch_by_ids(self, *, ids: List[Any], db_session: Any) -
-> int: 
-_9_5 raise NotImplementedError 
+_8_9def test_import_user(login): 
+_9_0 access_token, user_id = login 
+_9_1 headers = { 
+_9_2 "Authorization": f"Bearer {access_token}", 
+_9_3 "content_type": "multipart/form-data", 
+_9_4 } 
+_9_5 df = pd.DataFrame( 
+_9_6 { 
+_9_7 "username": ["example_user_2"], 
+_9_8 "password": ["password"], 
+_9_9 "nickname": ["nickname"], 
+_1_0_0 } 
+_1_0_1 ) 
+_1_0_2 buffer = io.BytesIO() 
+_1_0_3 df.to_excel(buffer, index=False) 
+_1_0_4 buffer.seek(0) 
+_1_0_5 file = UploadFile(filename="test_users.xlsx", file=buffer) 
+_1_0_6 
+_1_0_7 response = client.post( 
+_1_0_8 f"{configs.api_version}/user/import", 
+_1_0_9 headers=headers, 
+_1_1_0 files={"file": (file.filename, file.file, file.content_type)}, 
+_1_1_1 ) 
+_1_1_2 assert response.status_code == 200 
+_1_1_3 assert response.json()["code"] == 0 
+_1_1_4 
+_1_1_5 
+_1_1_6def test_remove_user(login): 
+_1_1_7 access_token, user_id = login 
+_1_1_8 headers = {"Authorization": f"Bearer {access_token}"} 
+_1_1_9 response = client.delete(f"{configs.api_version}/user/{user_id}",
+headers=headers) 
+_1_2_0 assert response.status_code == 200 
+_1_2_1 assert response.json()["code"] == 0 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+13 15:26 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695_base_model_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_base_model_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695_base_mapper_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_mapper_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -119,13 +119,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695_base_mapper_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_mapper_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1100 ssttaatteemmeennttss ?  1100 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Common attributes for data object""" 
 _2 
 _3from datetime import datetime 
 _4from typing import Optional 
 _5 
 _6from sqlalchemy import BigInteger 
 _7from sqlmodel import SQLModel as _SQLModel, Field 
@@ -43,8 +43,8 @@
 _2_9 """ 
 _3_0 
 _3_1 create_time: Optional[datetime] = Field(default_factory=datetime.now) 
 _3_2 update_time: Optional[datetime] = Field( 
 _3_3 default_factory=datetime.now, sa_column_kwargs={"onupdate": datetime.now} 
 _3_4 ) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695_mapper_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_mapper_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695_base_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_sqlmodel_impl_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -92,13 +92,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695_base_model_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_bbb369617a9e5695_sqlmodel_impl_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,17 +6,17 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 33 ssttaatteemmeennttss ?  33 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Top level mapper class""" 
 _2 
 _3from abc import ABC 
 _4 
 _5 
 _6class Mapper(ABC): 
 _7 pass 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_bbb369617a9e5695_sqlmodel_impl_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_bbb369617a9e5695_sqlmodel_impl_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\common\persistence\sqlmodel_impl.py: 35%</title>
+    <title>Coverage for fss\common\persistence\sqlmodel_impl.py: 51%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>fss\common\persistence\sqlmodel_impl.py</b>:
-            <span class="pc_cov">35%</span>
+            <span class="pc_cov">51%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,26 +50,26 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">109 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">38<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">71<span class="text"> missing</span></button>
+            <span class="text">114 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">58<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">56<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695_mapper_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0e53216603666de3___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -118,158 +118,158 @@
     <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">orm_data</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">model_validate</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="nam">db_session</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">orm_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="key">return</span> <span class="nam">orm_data</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">insert_batch</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data_list</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="nam">orm_datas</span> <span class="op">=</span> <span class="op">[</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">model_validate</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">            <span class="key">else</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="key">for</span> <span class="nam">data</span> <span class="key">in</span> <span class="nam">data_list</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">statement</span> <span class="op">=</span> <span class="nam">insert</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">[</span><span class="nam">data</span><span class="op">.</span><span class="nam">model_dump</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">data</span> <span class="key">in</span> <span class="nam">orm_datas</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="key">return</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data_list</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">statement</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalar_one_or_none</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">batch_size</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">1000</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="nam">result_set</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">        <span class="key">for</span> <span class="nam">i</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">ids</span><span class="op">)</span><span class="op">,</span> <span class="nam">batch_size</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="nam">batch_ids</span> <span class="op">=</span> <span class="nam">ids</span><span class="op">[</span><span class="nam">i</span> <span class="op">:</span> <span class="nam">i</span> <span class="op">+</span> <span class="nam">batch_size</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">            <span class="nam">statement</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span><span class="op">.</span><span class="nam">in_</span><span class="op">(</span><span class="nam">batch_ids</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="nam">results</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">exec</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span><span class="op">.</span><span class="nam">all</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">            <span class="nam">result_set</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="nam">results</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="key">return</span> <span class="nam">result_set</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">            <span class="nam">select</span><span class="op">(</span><span class="nam">func</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">select_from</span><span class="op">(</span><span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">subquery</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalar_one</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">1</span><span class="op">,</span> <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">100</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="key">if</span> <span class="nam">query</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">            <span class="nam">query</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">                <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">                <span class="op">.</span><span class="nam">offset</span><span class="op">(</span><span class="op">(</span><span class="nam">page</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">*</span> <span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">                <span class="op">.</span><span class="nam">limit</span><span class="op">(</span><span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">                <span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalars</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">all</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">100</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">        <span class="nam">order_by</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="nam">columns</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">__table__</span><span class="op">.</span><span class="nam">columns</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">        <span class="key">if</span> <span class="nam">order_by</span> <span class="key">is</span> <span class="key">None</span> <span class="key">or</span> <span class="nam">order_by</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">columns</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">            <span class="nam">order_by</span> <span class="op">=</span> <span class="str">"id"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">        <span class="key">if</span> <span class="nam">sort_order</span> <span class="op">==</span> <span class="nam">SortEnum</span><span class="op">.</span><span class="nam">ascending</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">            <span class="nam">query</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                <span class="op">.</span><span class="nam">offset</span><span class="op">(</span><span class="op">(</span><span class="nam">page</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">*</span> <span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                <span class="op">.</span><span class="nam">limit</span><span class="op">(</span><span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                <span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">columns</span><span class="op">[</span><span class="nam">order_by</span><span class="op">]</span><span class="op">.</span><span class="nam">asc</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">            <span class="nam">query</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">                <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">                <span class="op">.</span><span class="nam">offset</span><span class="op">(</span><span class="op">(</span><span class="nam">page</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">*</span> <span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">                <span class="op">.</span><span class="nam">limit</span><span class="op">(</span><span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">                <span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">columns</span><span class="op">[</span><span class="nam">order_by</span><span class="op">]</span><span class="op">.</span><span class="nam">desc</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalars</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">all</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_page</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">params</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="key">if</span> <span class="nam">query</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">            <span class="nam">query</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">paginate</span><span class="op">(</span><span class="nam">db_session</span><span class="op">,</span> <span class="nam">query</span><span class="op">,</span> <span class="nam">params</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_page_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">params</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">        <span class="nam">order_by</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="nam">columns</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">__table__</span><span class="op">.</span><span class="nam">columns</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">        <span class="key">if</span> <span class="nam">order_by</span> <span class="key">is</span> <span class="key">None</span> <span class="key">or</span> <span class="nam">order_by</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">columns</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">            <span class="nam">order_by</span> <span class="op">=</span> <span class="str">"id"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">        <span class="key">if</span> <span class="nam">query</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">            <span class="key">if</span> <span class="nam">sort_order</span> <span class="op">==</span> <span class="nam">SortEnum</span><span class="op">.</span><span class="nam">ascending</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">                <span class="nam">query</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">columns</span><span class="op">[</span><span class="nam">order_by</span><span class="op">]</span><span class="op">.</span><span class="nam">asc</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                <span class="nam">query</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">columns</span><span class="op">[</span><span class="nam">order_by</span><span class="op">]</span><span class="op">.</span><span class="nam">desc</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">paginate</span><span class="op">(</span><span class="nam">db_session</span><span class="op">,</span> <span class="nam">query</span><span class="op">,</span> <span class="nam">params</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">data</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="key">if</span> <span class="nam">result</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">            <span class="key">return</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="nam">db_data</span> <span class="op">=</span> <span class="nam">result</span><span class="op">.</span><span class="nam">scalar_one</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">        <span class="key">for</span> <span class="nam">attr</span><span class="op">,</span> <span class="nam">value</span> <span class="key">in</span> <span class="nam">data</span><span class="op">.</span><span class="nam">items</span><span class="op">(</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">            <span class="nam">setattr</span><span class="op">(</span><span class="nam">db_data</span><span class="op">,</span> <span class="nam">attr</span><span class="op">,</span> <span class="nam">value</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="nam">db_session</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">db_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">count_affected_rows</span><span class="op">(</span><span class="nam">db_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_batch_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data_list</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">        <span class="key">for</span> <span class="nam">data</span> <span class="key">in</span> <span class="nam">data_list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">            <span class="key">if</span> <span class="nam">hasattr</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="str">"id"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">                <span class="nam">statement</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">                    <span class="nam">update</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">                    <span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">data</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">                    <span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">**</span><span class="nam">data</span><span class="op">.</span><span class="nam">dict</span><span class="op">(</span><span class="nam">exclude_unset</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">                <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">        <span class="key">return</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data_list</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">delete_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">            <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalar_one</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="key">return</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="nam">orm_datas</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="key">for</span> <span class="nam">data</span> <span class="key">in</span> <span class="nam">data_list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">            <span class="nam">orm_datas</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">model_validate</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="nam">statement</span> <span class="op">=</span> <span class="nam">insert</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">[</span><span class="nam">data</span><span class="op">.</span><span class="nam">model_dump</span><span class="op">(</span><span class="op">)</span> <span class="key">for</span> <span class="nam">data</span> <span class="key">in</span> <span class="nam">orm_datas</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">        <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="key">return</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data_list</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Any</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">statement</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalar_one_or_none</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">batch_size</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">1000</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="nam">result_set</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="key">for</span> <span class="nam">i</span> <span class="key">in</span> <span class="nam">range</span><span class="op">(</span><span class="num">0</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">ids</span><span class="op">)</span><span class="op">,</span> <span class="nam">batch_size</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="nam">batch_ids</span> <span class="op">=</span> <span class="nam">ids</span><span class="op">[</span><span class="nam">i</span> <span class="op">:</span> <span class="nam">i</span> <span class="op">+</span> <span class="nam">batch_size</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="nam">statement</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span><span class="op">.</span><span class="nam">in_</span><span class="op">(</span><span class="nam">batch_ids</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="nam">results</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">exec</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span><span class="op">.</span><span class="nam">all</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="nam">result_set</span><span class="op">.</span><span class="nam">extend</span><span class="op">(</span><span class="nam">results</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">return</span> <span class="nam">result_set</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">            <span class="nam">select</span><span class="op">(</span><span class="nam">func</span><span class="op">.</span><span class="nam">count</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">.</span><span class="nam">select_from</span><span class="op">(</span><span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">subquery</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalar_one</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">1</span><span class="op">,</span> <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">100</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">        <span class="key">if</span> <span class="nam">query</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="nam">query</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">                <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">                <span class="op">.</span><span class="nam">offset</span><span class="op">(</span><span class="op">(</span><span class="nam">page</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">*</span> <span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">                <span class="op">.</span><span class="nam">limit</span><span class="op">(</span><span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">                <span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalars</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">all</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">        <span class="nam">page</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">        <span class="nam">size</span><span class="op">:</span> <span class="nam">int</span> <span class="op">=</span> <span class="num">100</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">        <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">        <span class="nam">order_by</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">        <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">        <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">        <span class="nam">columns</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">__table__</span><span class="op">.</span><span class="nam">columns</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">        <span class="key">if</span> <span class="nam">order_by</span> <span class="key">is</span> <span class="key">None</span> <span class="key">or</span> <span class="nam">order_by</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">columns</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">            <span class="nam">order_by</span> <span class="op">=</span> <span class="str">"id"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">        <span class="key">if</span> <span class="nam">sort_order</span> <span class="op">==</span> <span class="nam">SortEnum</span><span class="op">.</span><span class="nam">ascending</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">            <span class="nam">query</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">                <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                <span class="op">.</span><span class="nam">offset</span><span class="op">(</span><span class="op">(</span><span class="nam">page</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">*</span> <span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">                <span class="op">.</span><span class="nam">limit</span><span class="op">(</span><span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                <span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">columns</span><span class="op">[</span><span class="nam">order_by</span><span class="op">]</span><span class="op">.</span><span class="nam">asc</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">            <span class="nam">query</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">                <span class="op">.</span><span class="nam">offset</span><span class="op">(</span><span class="op">(</span><span class="nam">page</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span> <span class="op">*</span> <span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">                <span class="op">.</span><span class="nam">limit</span><span class="op">(</span><span class="nam">size</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">                <span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">columns</span><span class="op">[</span><span class="nam">order_by</span><span class="op">]</span><span class="op">.</span><span class="nam">desc</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalars</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">all</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_page</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">params</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">        <span class="key">if</span> <span class="nam">query</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">            <span class="nam">query</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">paginate</span><span class="op">(</span><span class="nam">db_session</span><span class="op">,</span> <span class="nam">query</span><span class="op">,</span> <span class="nam">params</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">        <span class="key">return</span> <span class="nam">response</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">select_list_page_ordered</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">        <span class="op">*</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">        <span class="nam">params</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">        <span class="nam">query</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">        <span class="nam">order_by</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">        <span class="nam">sort_order</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">        <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">        <span class="nam">columns</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">__table__</span><span class="op">.</span><span class="nam">columns</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">        <span class="key">if</span> <span class="nam">order_by</span> <span class="key">is</span> <span class="key">None</span> <span class="key">or</span> <span class="nam">order_by</span> <span class="key">not</span> <span class="key">in</span> <span class="nam">columns</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">            <span class="nam">order_by</span> <span class="op">=</span> <span class="str">"id"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">        <span class="key">if</span> <span class="nam">query</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">            <span class="key">if</span> <span class="nam">sort_order</span> <span class="op">==</span> <span class="nam">SortEnum</span><span class="op">.</span><span class="nam">ascending</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">                <span class="nam">query</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">columns</span><span class="op">[</span><span class="nam">order_by</span><span class="op">]</span><span class="op">.</span><span class="nam">asc</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                <span class="nam">query</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">order_by</span><span class="op">(</span><span class="nam">columns</span><span class="op">[</span><span class="nam">order_by</span><span class="op">]</span><span class="op">.</span><span class="nam">desc</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">paginate</span><span class="op">(</span><span class="nam">db_session</span><span class="op">,</span> <span class="nam">query</span><span class="op">,</span> <span class="nam">params</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">        <span class="nam">query</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">data</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">query</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">        <span class="key">if</span> <span class="nam">result</span> <span class="key">is</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">            <span class="key">return</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">        <span class="nam">db_data</span> <span class="op">=</span> <span class="nam">result</span><span class="op">.</span><span class="nam">scalar_one</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">        <span class="key">if</span> <span class="nam">isinstance</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="nam">dict</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">            <span class="nam">update_data</span> <span class="op">=</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="nam">update_data</span> <span class="op">=</span> <span class="nam">data</span><span class="op">.</span><span class="nam">model_dump</span><span class="op">(</span><span class="nam">exclude_unset</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="key">for</span> <span class="nam">field</span> <span class="key">in</span> <span class="nam">update_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="nam">setattr</span><span class="op">(</span><span class="nam">db_data</span><span class="op">,</span> <span class="nam">field</span><span class="op">,</span> <span class="nam">update_data</span><span class="op">[</span><span class="nam">field</span><span class="op">]</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">        <span class="nam">db_session</span><span class="op">.</span><span class="nam">add</span><span class="op">(</span><span class="nam">db_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">        <span class="key">return</span> <span class="nam">db_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">update_batch_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">data_list</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">        <span class="key">for</span> <span class="nam">data</span> <span class="key">in</span> <span class="nam">data_list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">            <span class="key">if</span> <span class="nam">hasattr</span><span class="op">(</span><span class="nam">data</span><span class="op">,</span> <span class="str">"id"</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">                <span class="nam">statement</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">                    <span class="nam">update</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">                    <span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">data</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">                    <span class="op">.</span><span class="nam">values</span><span class="op">(</span><span class="op">**</span><span class="nam">data</span><span class="op">.</span><span class="nam">dict</span><span class="op">(</span><span class="nam">exclude_unset</span><span class="op">=</span><span class="key">True</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">                <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">        <span class="key">return</span> <span class="nam">len</span><span class="op">(</span><span class="nam">data_list</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">delete_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">Any</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span><span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">        <span class="nam">statement</span> <span class="op">=</span> <span class="nam">select</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span> <span class="op">==</span> <span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">        <span class="nam">response</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">        <span class="nam">data</span> <span class="op">=</span> <span class="nam">response</span><span class="op">.</span><span class="nam">scalar_one</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">        <span class="key">return</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="nam">data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">delete_batch_by_ids</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">        <span class="nam">self</span><span class="op">,</span> <span class="op">*</span><span class="op">,</span> <span class="nam">ids</span><span class="op">:</span> <span class="nam">List</span><span class="op">[</span><span class="nam">Any</span><span class="op">]</span><span class="op">,</span> <span class="nam">db_session</span><span class="op">:</span> <span class="nam">Any</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">    <span class="op">)</span> <span class="op">-></span> <span class="nam">int</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">        <span class="nam">db_session</span> <span class="op">=</span> <span class="nam">db_session</span> <span class="key">or</span> <span class="nam">self</span><span class="op">.</span><span class="nam">db</span><span class="op">.</span><span class="nam">session</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">        <span class="nam">statement</span> <span class="op">=</span> <span class="nam">delete</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">)</span><span class="op">.</span><span class="nam">where</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">id</span><span class="op">.</span><span class="nam">in_</span><span class="op">(</span><span class="nam">ids</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">db_session</span><span class="op">.</span><span class="nam">execute</span><span class="op">(</span><span class="nam">statement</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
@@ -279,13 +279,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_bbb369617a9e5695_mapper_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_0e53216603666de3___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\ppeerrssiisstteennccee\\ssqqllmmooddeell__iimmppll..ppyy:: 3355%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ccoommmmoonn\\ppeerrssiisstteennccee\\ssqqllmmooddeell__iimmppll..ppyy:: 5511%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 110099 ssttaatteemmeennttss ?  3388 rruunn 7711 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 111144 ssttaatteemmeennttss ?  5588 rruunn 5566 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+13 15:26 +0800
 _1"""Sqlmodel impl that do database operations""" 
 _2 
 _3from typing import Generic, TypeVar, List, Any, Type, Union 
 _4 
 _5from fastapi_pagination.ext.sqlmodel import paginate 
 _6from pydantic import BaseModel 
 _7from sqlmodel import SQLModel, select, func, insert, update, delete 
@@ -50,161 +50,161 @@
 _3_7 db_session.add(orm_data) 
 _3_8 return orm_data 
 _3_9 
 _4_0 async def insert_batch( 
 _4_1 self, *, data_list: List[Any], db_session: Any = None 
 _4_2 ) -> int: 
 _4_3 db_session = db_session or self.db.session 
-_4_4 orm_datas = [ 
-_4_5 self.model.model_validate(data) 
-_4_6 if not isinstance(data, self.model) 
-_4_7 else data 
-_4_8 for data in data_list 
-_4_9 ] 
-_5_0 statement = insert(self.model).values([data.model_dump() for data in
+_4_4 orm_datas = [] 
+_4_5 for data in data_list: 
+_4_6 orm_datas.append(self.model.model_validate(data)) 
+_4_7 statement = insert(self.model).values([data.model_dump() for data in
 orm_datas]) 
-_5_1 await db_session.execute(statement) 
-_5_2 return len(data_list) 
-_5_3 
-_5_4 async def select_by_id(self, *, id: Any, db_session: Any = None) -> Any: 
-_5_5 db_session = db_session or self.db.session 
-_5_6 statement = select(self.model).where(self.model.id == id) 
-_5_7 response = await db_session.execute(statement) 
-_5_8 return response.scalar_one_or_none() 
-_5_9 
-_6_0 async def select_by_ids( 
-_6_1 self, *, ids: List[Any], batch_size: int = 1000, db_session: Any = None 
-_6_2 ) -> List[Any]: 
-_6_3 db_session = db_session or self.db.session 
-_6_4 result_set = [] 
-_6_5 for i in range(0, len(ids), batch_size): 
-_6_6 batch_ids = ids[i : i + batch_size] 
-_6_7 statement = select(self.model).where(self.model.id.in_(batch_ids)) 
-_6_8 results = await db_session.exec(statement).all() 
-_6_9 result_set.extend(results) 
-_7_0 return result_set 
-_7_1 
-_7_2 async def select_count(self, *, db_session: Any = None) -> int: 
-_7_3 db_session = db_session or self.db.session 
-_7_4 response = await db_session.execute( 
-_7_5 select(func.count()).select_from(select(self.model).subquery()) 
-_7_6 ) 
-_7_7 return response.scalar_one() 
-_7_8 
-_7_9 async def select_list( 
-_8_0 self, *, page: int = 1, size: int = 100, query: Any, db_session: Any = None 
-_8_1 ) -> List[Any]: 
-_8_2 db_session = db_session or self.db.session 
-_8_3 if query is None: 
-_8_4 query = ( 
-_8_5 select(self.model) 
-_8_6 .offset((page - 1) * size) 
-_8_7 .limit(size) 
-_8_8 .order_by(self.model.id) 
-_8_9 ) 
-_9_0 response = await db_session.execute(query) 
-_9_1 return response.scalars().all() 
-_9_2 
-_9_3 async def select_list_ordered( 
-_9_4 self, 
-_9_5 *, 
-_9_6 page: int = 1, 
-_9_7 size: int = 100, 
-_9_8 query: Any, 
-_9_9 order_by: Any, 
-_1_0_0 sort_order: Any, 
-_1_0_1 db_session: Any = None, 
-_1_0_2 ) -> List[Any]: 
-_1_0_3 db_session = db_session or self.db.session 
-_1_0_4 columns = self.model.__table__.columns 
-_1_0_5 if order_by is None or order_by not in columns: 
-_1_0_6 order_by = "id" 
-_1_0_7 if sort_order == SortEnum.ascending: 
-_1_0_8 query = ( 
-_1_0_9 select(self.model) 
-_1_1_0 .offset((page - 1) * size) 
-_1_1_1 .limit(size) 
-_1_1_2 .order_by(columns[order_by].asc()) 
-_1_1_3 ) 
-_1_1_4 else: 
-_1_1_5 query = ( 
-_1_1_6 select(self.model) 
-_1_1_7 .offset((page - 1) * size) 
-_1_1_8 .limit(size) 
-_1_1_9 .order_by(columns[order_by].desc()) 
-_1_2_0 ) 
-_1_2_1 response = await db_session.execute(query) 
-_1_2_2 return response.scalars().all() 
-_1_2_3 
-_1_2_4 async def select_list_page( 
-_1_2_5 self, *, params: Any, query: Any, db_session: Any = None 
-_1_2_6 ) -> List[Any]: 
-_1_2_7 db_session = db_session or self.db.session 
-_1_2_8 if query is None: 
-_1_2_9 query = select(self.model) 
-_1_3_0 response = await paginate(db_session, query, params) 
-_1_3_1 return response 
-_1_3_2 
-_1_3_3 async def select_list_page_ordered( 
-_1_3_4 self, 
-_1_3_5 *, 
-_1_3_6 params: Any, 
-_1_3_7 query: Any, 
-_1_3_8 order_by: Any, 
-_1_3_9 sort_order: Any, 
-_1_4_0 db_session: Any = None, 
-_1_4_1 ) -> List[Any]: 
-_1_4_2 db_session = db_session or self.db.session 
-_1_4_3 columns = self.model.__table__.columns 
-_1_4_4 if order_by is None or order_by not in columns: 
-_1_4_5 order_by = "id" 
-_1_4_6 if query is None: 
-_1_4_7 if sort_order == SortEnum.ascending: 
-_1_4_8 query = select(self.model).order_by(columns[order_by].asc()) 
-_1_4_9 else: 
-_1_5_0 query = select(self.model).order_by(columns[order_by].desc()) 
-_1_5_1 return await paginate(db_session, query, params) 
-_1_5_2 
-_1_5_3 async def update_by_id(self, *, data: Any, db_session: Any = None) -> int: 
-_1_5_4 db_session = db_session or self.db.session 
-_1_5_5 query = select(self.model).where(self.model.id == data.id) 
-_1_5_6 result = await db_session.execute(query) 
-_1_5_7 if result is None: 
-_1_5_8 return 0 
-_1_5_9 db_data = result.scalar_one() 
-_1_6_0 for attr, value in data.items(): 
-_1_6_1 setattr(db_data, attr, value) 
-_1_6_2 db_session.add(db_data) 
-_1_6_3 return self.count_affected_rows(db_data) 
-_1_6_4 
-_1_6_5 async def update_batch_by_ids( 
-_1_6_6 self, *, data_list: List[Any], db_session: Any = None 
-_1_6_7 ) -> int: 
-_1_6_8 db_session = db_session or self.db.session 
-_1_6_9 for data in data_list: 
-_1_7_0 if hasattr(data, "id"): 
-_1_7_1 statement = ( 
-_1_7_2 update(self.model) 
-_1_7_3 .where(self.model.id == data.id) 
-_1_7_4 .values(**data.dict(exclude_unset=True)) 
-_1_7_5 ) 
-_1_7_6 await db_session.execute(statement) 
-_1_7_7 return len(data_list) 
-_1_7_8 
-_1_7_9 async def delete_by_id(self, *, id: Any, db_session: Any = None) -> int: 
-_1_8_0 db_session = db_session or self.db.session 
-_1_8_1 response = await db_session.execute( 
-_1_8_2 select(self.model).where(self.model.id == id) 
-_1_8_3 ) 
-_1_8_4 data = response.scalar_one() 
-_1_8_5 await db_session.delete(data) 
-_1_8_6 return 1 
+_4_8 await db_session.execute(statement) 
+_4_9 return len(data_list) 
+_5_0 
+_5_1 async def select_by_id(self, *, id: Any, db_session: Any = None) -> Any: 
+_5_2 db_session = db_session or self.db.session 
+_5_3 statement = select(self.model).where(self.model.id == id) 
+_5_4 response = await db_session.execute(statement) 
+_5_5 return response.scalar_one_or_none() 
+_5_6 
+_5_7 async def select_by_ids( 
+_5_8 self, *, ids: List[Any], batch_size: int = 1000, db_session: Any = None 
+_5_9 ) -> List[Any]: 
+_6_0 db_session = db_session or self.db.session 
+_6_1 result_set = [] 
+_6_2 for i in range(0, len(ids), batch_size): 
+_6_3 batch_ids = ids[i : i + batch_size] 
+_6_4 statement = select(self.model).where(self.model.id.in_(batch_ids)) 
+_6_5 results = await db_session.exec(statement).all() 
+_6_6 result_set.extend(results) 
+_6_7 return result_set 
+_6_8 
+_6_9 async def select_count(self, *, db_session: Any = None) -> int: 
+_7_0 db_session = db_session or self.db.session 
+_7_1 response = await db_session.execute( 
+_7_2 select(func.count()).select_from(select(self.model).subquery()) 
+_7_3 ) 
+_7_4 return response.scalar_one() 
+_7_5 
+_7_6 async def select_list( 
+_7_7 self, *, page: int = 1, size: int = 100, query: Any, db_session: Any = None 
+_7_8 ) -> List[Any]: 
+_7_9 db_session = db_session or self.db.session 
+_8_0 if query is None: 
+_8_1 query = ( 
+_8_2 select(self.model) 
+_8_3 .offset((page - 1) * size) 
+_8_4 .limit(size) 
+_8_5 .order_by(self.model.id) 
+_8_6 ) 
+_8_7 response = await db_session.execute(query) 
+_8_8 return response.scalars().all() 
+_8_9 
+_9_0 async def select_list_ordered( 
+_9_1 self, 
+_9_2 *, 
+_9_3 page: int = 1, 
+_9_4 size: int = 100, 
+_9_5 query: Any, 
+_9_6 order_by: Any, 
+_9_7 sort_order: Any, 
+_9_8 db_session: Any = None, 
+_9_9 ) -> List[Any]: 
+_1_0_0 db_session = db_session or self.db.session 
+_1_0_1 columns = self.model.__table__.columns 
+_1_0_2 if order_by is None or order_by not in columns: 
+_1_0_3 order_by = "id" 
+_1_0_4 if sort_order == SortEnum.ascending: 
+_1_0_5 query = ( 
+_1_0_6 select(self.model) 
+_1_0_7 .offset((page - 1) * size) 
+_1_0_8 .limit(size) 
+_1_0_9 .order_by(columns[order_by].asc()) 
+_1_1_0 ) 
+_1_1_1 else: 
+_1_1_2 query = ( 
+_1_1_3 select(self.model) 
+_1_1_4 .offset((page - 1) * size) 
+_1_1_5 .limit(size) 
+_1_1_6 .order_by(columns[order_by].desc()) 
+_1_1_7 ) 
+_1_1_8 response = await db_session.execute(query) 
+_1_1_9 return response.scalars().all() 
+_1_2_0 
+_1_2_1 async def select_list_page( 
+_1_2_2 self, *, params: Any, query: Any, db_session: Any = None 
+_1_2_3 ) -> List[Any]: 
+_1_2_4 db_session = db_session or self.db.session 
+_1_2_5 if query is None: 
+_1_2_6 query = select(self.model) 
+_1_2_7 response = await paginate(db_session, query, params) 
+_1_2_8 return response 
+_1_2_9 
+_1_3_0 async def select_list_page_ordered( 
+_1_3_1 self, 
+_1_3_2 *, 
+_1_3_3 params: Any, 
+_1_3_4 query: Any = None, 
+_1_3_5 order_by: Any = None, 
+_1_3_6 sort_order: Any = None, 
+_1_3_7 db_session: Any = None, 
+_1_3_8 ) -> List[Any]: 
+_1_3_9 db_session = db_session or self.db.session 
+_1_4_0 columns = self.model.__table__.columns 
+_1_4_1 if order_by is None or order_by not in columns: 
+_1_4_2 order_by = "id" 
+_1_4_3 if query is None: 
+_1_4_4 if sort_order == SortEnum.ascending: 
+_1_4_5 query = select(self.model).order_by(columns[order_by].asc()) 
+_1_4_6 else: 
+_1_4_7 query = select(self.model).order_by(columns[order_by].desc()) 
+_1_4_8 return await paginate(db_session, query, params) 
+_1_4_9 
+_1_5_0 async def update_by_id(self, *, data: Any, db_session: Any = None) -> int: 
+_1_5_1 db_session = db_session or self.db.session 
+_1_5_2 query = select(self.model).where(self.model.id == data.id) 
+_1_5_3 result = await db_session.execute(query) 
+_1_5_4 if result is None: 
+_1_5_5 return 0 
+_1_5_6 db_data = result.scalar_one() 
+_1_5_7 if isinstance(data, dict): 
+_1_5_8 update_data = data 
+_1_5_9 else: 
+_1_6_0 update_data = data.model_dump(exclude_unset=True) 
+_1_6_1 for field in update_data: 
+_1_6_2 setattr(db_data, field, update_data[field]) 
+_1_6_3 
+_1_6_4 db_session.add(db_data) 
+_1_6_5 return db_data 
+_1_6_6 
+_1_6_7 async def update_batch_by_ids( 
+_1_6_8 self, *, data_list: List[Any], db_session: Any = None 
+_1_6_9 ) -> int: 
+_1_7_0 db_session = db_session or self.db.session 
+_1_7_1 for data in data_list: 
+_1_7_2 if hasattr(data, "id"): 
+_1_7_3 statement = ( 
+_1_7_4 update(self.model) 
+_1_7_5 .where(self.model.id == data.id) 
+_1_7_6 .values(**data.dict(exclude_unset=True)) 
+_1_7_7 ) 
+_1_7_8 await db_session.execute(statement) 
+_1_7_9 return len(data_list) 
+_1_8_0 
+_1_8_1 async def delete_by_id(self, *, id: Any, db_session: Any = None) -> int: 
+_1_8_2 db_session = db_session or self.db.session 
+_1_8_3 statement = select(self.model).where(self.model.id == id) 
+_1_8_4 response = await db_session.execute(statement) 
+_1_8_5 data = response.scalar_one() 
+_1_8_6 return await db_session.delete(data) 
 _1_8_7 
 _1_8_8 async def delete_batch_by_ids( 
 _1_8_9 self, *, ids: List[Any], db_session: Any = None 
 _1_9_0 ) -> int: 
 _1_9_1 db_session = db_session or self.db.session 
 _1_9_2 statement = delete(self.model).where(self.model.id.in_(ids)) 
 _1_9_3 result = await db_session.execute(statement) 
 _1_9_4 return result.rowcount 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+13 15:26 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_dab9b2a1903716f2___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dab9b2a1903716f2___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_ebd618dd09682660_system_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_dab9b2a1903716f2_user_schema_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_ebd618dd09682660_system_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_dab9b2a1903716f2_user_schema_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_dab9b2a1903716f2_user_schema_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_ebd618dd09682660_system_py.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\starter\system\schema\user_schema.py: 100%</title>
+    <title>Coverage for fss\starter\system\router\system.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\starter\system\schema\user_schema.py</b>:
+            <span class="text">Coverage for </span><b>fss\starter\system\router\system.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -50,71 +50,58 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">12 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">12<span class="text"> run</span></button>
+            <span class="text">6 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">6<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_dab9b2a1903716f2___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_ebd618dd09682660___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_fc0d8786bb154269___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_dab9b2a1903716f2___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""User domain schema"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Routing of system modules"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">pydantic</span> <span class="key">import</span> <span class="nam">BaseModel</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">APIRouter</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com"># UserCreate schema</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">class</span> <span class="nam">UserCreateCmd</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">    <span class="nam">username</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="nam">password</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="nam">nickname</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="com"># UserQuery schema</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">class</span> <span class="nam">UserQuery</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">id</span><span class="op">:</span> <span class="nam">int</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="nam">username</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">nickname</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="com"># Login schema</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="key">class</span> <span class="nam">LoginCmd</span><span class="op">(</span><span class="nam">BaseModel</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="nam">username</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="nam">password</span><span class="op">:</span> <span class="nam">str</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">api</span><span class="op">.</span><span class="nam">v1</span><span class="op">.</span><span class="nam">probe_controller</span> <span class="key">import</span> <span class="nam">probe_router</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">api</span><span class="op">.</span><span class="nam">v1</span><span class="op">.</span><span class="nam">user_controller</span> <span class="key">import</span> <span class="nam">user_router</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="nam">system_router</span> <span class="op">=</span> <span class="nam">APIRouter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="nam">system_router</span><span class="op">.</span><span class="nam">include_router</span><span class="op">(</span><span class="nam">probe_router</span><span class="op">,</span> <span class="nam">tags</span><span class="op">=</span><span class="op">[</span><span class="str">"probe"</span><span class="op">]</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">=</span><span class="str">"/probe"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="nam">system_router</span><span class="op">.</span><span class="nam">include_router</span><span class="op">(</span><span class="nam">user_router</span><span class="op">,</span> <span class="nam">tags</span><span class="op">=</span><span class="op">[</span><span class="str">"user"</span><span class="op">]</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">=</span><span class="str">"/user"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_dab9b2a1903716f2___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_ebd618dd09682660___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_fc0d8786bb154269___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_dab9b2a1903716f2___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,38 +1,25 @@
-************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\sscchheemmaa\\uusseerr__sscchheemmaa..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\rroouutteerr\\ssyysstteemm..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 1122 ssttaatteemmeennttss ?  1122 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 66 ssttaatteemmeennttss ?  66 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
-_1"""User domain schema""" 
+12 22:20 +0800
+_1"""Routing of system modules""" 
 _2 
-_3from pydantic import BaseModel 
+_3from fastapi import APIRouter 
 _4 
-_5 
-_6# UserCreate schema 
-_7class UserCreateCmd(BaseModel): 
-_8 username: str 
-_9 password: str 
-_1_0 nickname: str 
-_1_1 
-_1_2 
-_1_3# UserQuery schema 
-_1_4class UserQuery(BaseModel): 
-_1_5 id: int 
-_1_6 username: str 
-_1_7 nickname: str 
-_1_8 
-_1_9 
-_2_0# Login schema 
-_2_1class LoginCmd(BaseModel): 
-_2_2 username: str 
-_2_3 password: str 
+_5from fss.starter.system.api.v1.probe_controller import probe_router 
+_6from fss.starter.system.api.v1.user_controller import user_router 
+_7 
+_8system_router = APIRouter() 
+_9system_router.include_router(probe_router, tags=["probe"], prefix="/probe") 
+_1_0system_router.include_router(user_router, tags=["user"], prefix="/user") 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_dcf1c620283c9c76___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dcf1c620283c9c76___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_392b9405ba6460b0_snowflake_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_dcf1c620283c9c76_db_session_middleware_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_392b9405ba6460b0_snowflake_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_dcf1c620283c9c76_db_session_middleware_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_dcf1c620283c9c76_db_session_middleware_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_dcf1c620283c9c76_db_session_middleware_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_dcf1c620283c9c76___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_3c9f025fb530798e___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -220,13 +220,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_dcf1c620283c9c76___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_3c9f025fb530798e___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 6688 ssttaatteemmeennttss ?  5566 rruunn 1122 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _1"""Session proxy used in the project""" 
 _2 
 _3from contextvars import ContextVar 
 _4from typing import Dict, Optional, Union 
 _5 
 _6from sqlalchemy.engine import Engine 
 _7from sqlalchemy.engine.url import URL 
@@ -153,8 +153,8 @@
 _1_3_1 Session not initialised! Ensure that DBSessionMiddleware has been
 initialised before 
 _1_3_2 attempting database access. 
 _1_3_3 """ 
 _1_3_4 
 _1_3_5 super().__init__(detail) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_ebd618dd09682660___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_ebd618dd09682660___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_07ed4fb7c74d9876_user_do_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_ebd618dd09682660_system_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -85,13 +85,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_07ed4fb7c74d9876_user_do_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_ebd618dd09682660_system_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_f83affef05b47916___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_fc0d8786bb154269___init___py.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\starter\system\service\impl\__init__.py: 100%</title>
+    <title>Coverage for fss\starter\system\service\__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\starter\system\service\impl\__init__.py</b>:
+            <span class="text">Coverage for </span><b>fss\starter\system\service\__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_fc0d8786bb154269___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_dab9b2a1903716f2_user_schema_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_f83affef05b47916_user_service_impl_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_f83affef05b47916___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,18 +80,18 @@
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_fc0d8786bb154269___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_dab9b2a1903716f2_user_schema_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_f83affef05b47916_user_service_impl_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_f83affef05b47916___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\sseerrvviiccee\\iimmppll\\____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\sseerrvviiccee\\____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_f83affef05b47916_user_service_impl_py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_9c41cf131237e8e8_user_controller_py.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\starter\system\service\impl\user_service_impl.py: 66%</title>
+    <title>Coverage for fss\starter\system\api\v1\user_controller.py: 91%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\starter\system\service\impl\user_service_impl.py</b>:
-            <span class="pc_cov">66%</span>
+            <span class="text">Coverage for </span><b>fss\starter\system\api\v1\user_controller.py</b>:
+            <span class="pc_cov">91%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -50,126 +50,169 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">38 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">25<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">13<span class="text"> missing</span></button>
+            <span class="text">45 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">41<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">4<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_f83affef05b47916___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8_probe_controller_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_fc0d8786bb154269_user_service_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_4c5c7dd0d2e26036___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
             <button type="button" class="button_next_file" data-shortcut="]"/>
             <button type="button" class="button_to_index" data-shortcut="u"/>
             <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
-    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""User domain service impl"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""User operation controller"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">datetime</span> <span class="key">import</span> <span class="nam">timedelta</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">typing</span> <span class="key">import</span> <span class="nam">Optional</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">cache</span><span class="op">.</span><span class="nam">cache</span> <span class="key">import</span> <span class="nam">get_cache_client</span><span class="op">,</span> <span class="nam">Cache</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">config</span> <span class="key">import</span> <span class="nam">configs</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">enum</span><span class="op">.</span><span class="nam">enum</span> <span class="key">import</span> <span class="nam">TokenTypeEnum</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">schema</span> <span class="key">import</span> <span class="nam">Token</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">impl</span><span class="op">.</span><span class="nam">service_impl</span> <span class="key">import</span> <span class="nam">ServiceImpl</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">util</span> <span class="key">import</span> <span class="nam">security</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">util</span><span class="op">.</span><span class="nam">security</span> <span class="key">import</span> <span class="nam">verify_password</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">enum</span><span class="op">.</span><span class="nam">system</span> <span class="key">import</span> <span class="nam">SystemResponseCode</span><span class="op">,</span> <span class="nam">SystemConstantCode</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">exception</span><span class="op">.</span><span class="nam">system</span> <span class="key">import</span> <span class="nam">SystemException</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">user_mapper</span> <span class="key">import</span> <span class="nam">UserMapper</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">user_do</span> <span class="key">import</span> <span class="nam">UserDO</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">user_schema</span> <span class="key">import</span> <span class="nam">UserQuery</span><span class="op">,</span> <span class="nam">LoginCmd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">user_service</span> <span class="key">import</span> <span class="nam">UserService</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="key">class</span> <span class="nam">UserServiceImpl</span><span class="op">(</span><span class="nam">ServiceImpl</span><span class="op">[</span><span class="nam">UserMapper</span><span class="op">,</span> <span class="nam">UserDO</span><span class="op">]</span><span class="op">,</span> <span class="nam">UserService</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">mapper</span><span class="op">:</span> <span class="nam">UserMapper</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">mapper</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span> <span class="key">import</span> <span class="nam">APIRouter</span><span class="op">,</span> <span class="nam">Depends</span><span class="op">,</span> <span class="nam">UploadFile</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi</span><span class="op">.</span><span class="nam">security</span> <span class="key">import</span> <span class="nam">OAuth2PasswordRequestForm</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">fastapi_pagination</span> <span class="key">import</span> <span class="nam">Params</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">starlette</span><span class="op">.</span><span class="nam">responses</span> <span class="key">import</span> <span class="nam">StreamingResponse</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">result</span> <span class="key">import</span> <span class="nam">result</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">result</span><span class="op">.</span><span class="nam">result</span> <span class="key">import</span> <span class="nam">BaseResponse</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">schema</span> <span class="key">import</span> <span class="nam">Token</span><span class="op">,</span> <span class="nam">CurrentUser</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">security</span><span class="op">.</span><span class="nam">security</span> <span class="key">import</span> <span class="nam">get_current_user</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">common</span><span class="op">.</span><span class="nam">util</span><span class="op">.</span><span class="nam">security</span> <span class="key">import</span> <span class="nam">get_password_hash</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">model</span><span class="op">.</span><span class="nam">user_do</span> <span class="key">import</span> <span class="nam">UserDO</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">schema</span><span class="op">.</span><span class="nam">user_schema</span> <span class="key">import</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">    <span class="nam">UserCreateCmd</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">    <span class="nam">UserQuery</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">    <span class="nam">LoginCmd</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">    <span class="nam">UpdateUserCmd</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t"><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">impl</span><span class="op">.</span><span class="nam">user_service_impl</span> <span class="key">import</span> <span class="nam">get_user_service</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t"><span class="key">from</span> <span class="nam">fss</span><span class="op">.</span><span class="nam">starter</span><span class="op">.</span><span class="nam">system</span><span class="op">.</span><span class="nam">service</span><span class="op">.</span><span class="nam">user_service</span> <span class="key">import</span> <span class="nam">UserService</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="nam">user_router</span> <span class="op">=</span> <span class="nam">APIRouter</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">find_by_id</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">id</span><span class="op">:</span> <span class="nam">int</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Optional</span><span class="op">[</span><span class="nam">UserQuery</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">        Retrieval user through user id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t"><span class="str">        :param id: user id</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="str">        :return: user or none</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">user_do</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">select_by_id</span><span class="op">(</span><span class="nam">id</span><span class="op">=</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">if</span> <span class="nam">user_do</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">            <span class="key">return</span> <span class="nam">UserQuery</span><span class="op">(</span><span class="op">**</span><span class="nam">user_do</span><span class="op">.</span><span class="nam">model_dump</span><span class="op">(</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span><span class="str">"/register"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">register_user</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="nam">create_data</span><span class="op">:</span> <span class="nam">UserCreateCmd</span><span class="op">,</span> <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">BaseResponse</span><span class="op">[</span><span class="nam">int</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t"><span class="str">    User registration</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">    <span class="nam">create_data</span><span class="op">.</span><span class="nam">password</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">get_password_hash</span><span class="op">(</span><span class="nam">create_data</span><span class="op">.</span><span class="nam">password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="nam">user</span><span class="op">:</span> <span class="nam">UserDO</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">save</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">create_data</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">.</span><span class="nam">success</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">user</span><span class="op">.</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">async</span> <span class="key">def</span> <span class="nam">login</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">loginCmd</span><span class="op">:</span> <span class="nam">LoginCmd</span><span class="op">)</span> <span class="op">-></span> <span class="nam">Token</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="str">        Do log in</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t"><span class="str">        :param loginCmd: loginCmd</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t"><span class="str">        :return: access token and refresh token</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">username</span><span class="op">:</span> <span class="nam">str</span> <span class="op">=</span> <span class="nam">loginCmd</span><span class="op">.</span><span class="nam">username</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="nam">userDO</span><span class="op">:</span> <span class="nam">UserDO</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">self</span><span class="op">.</span><span class="nam">mapper</span><span class="op">.</span><span class="nam">get_user_by_username</span><span class="op">(</span><span class="nam">username</span><span class="op">=</span><span class="nam">username</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">userDO</span> <span class="key">or</span> <span class="key">not</span> <span class="key">await</span> <span class="nam">verify_password</span><span class="op">(</span><span class="nam">loginCmd</span><span class="op">.</span><span class="nam">password</span><span class="op">,</span> <span class="nam">userDO</span><span class="op">.</span><span class="nam">password</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">            <span class="key">raise</span> <span class="nam">SystemException</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">                <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">AUTH_FAILED</span><span class="op">.</span><span class="nam">code</span><span class="op">,</span> <span class="nam">SystemResponseCode</span><span class="op">.</span><span class="nam">AUTH_FAILED</span><span class="op">.</span><span class="nam">msg</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">        <span class="nam">access_token_expires</span> <span class="op">=</span> <span class="nam">timedelta</span><span class="op">(</span><span class="nam">minutes</span><span class="op">=</span><span class="nam">configs</span><span class="op">.</span><span class="nam">access_token_expire_minutes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">refresh_token_expires</span> <span class="op">=</span> <span class="nam">timedelta</span><span class="op">(</span><span class="nam">minutes</span><span class="op">=</span><span class="nam">configs</span><span class="op">.</span><span class="nam">refresh_token_expire_minutes</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">access_token</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">security</span><span class="op">.</span><span class="nam">create_token</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="nam">subject</span><span class="op">=</span><span class="nam">userDO</span><span class="op">.</span><span class="nam">id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">            <span class="nam">expires_delta</span><span class="op">=</span><span class="nam">access_token_expires</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="nam">token_type</span><span class="op">=</span><span class="nam">TokenTypeEnum</span><span class="op">.</span><span class="nam">access</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">        <span class="nam">refresh_token</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">security</span><span class="op">.</span><span class="nam">create_token</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="nam">subject</span><span class="op">=</span><span class="nam">userDO</span><span class="op">.</span><span class="nam">id</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="nam">expires_delta</span><span class="op">=</span><span class="nam">refresh_token_expires</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="nam">token_type</span><span class="op">=</span><span class="nam">TokenTypeEnum</span><span class="op">.</span><span class="nam">refresh</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="nam">token</span> <span class="op">=</span> <span class="nam">Token</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">            <span class="nam">access_token</span><span class="op">=</span><span class="nam">access_token</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">            <span class="nam">expired_at</span><span class="op">=</span><span class="nam">int</span><span class="op">(</span><span class="nam">access_token_expires</span><span class="op">.</span><span class="nam">total_seconds</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="nam">token_type</span><span class="op">=</span><span class="str">"bearer"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="nam">refresh_token</span><span class="op">=</span><span class="nam">refresh_token</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="nam">re_expired_at</span><span class="op">=</span><span class="nam">int</span><span class="op">(</span><span class="nam">refresh_token_expires</span><span class="op">.</span><span class="nam">total_seconds</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="nam">cache_client</span><span class="op">:</span> <span class="nam">Cache</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">get_cache_client</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="key">await</span> <span class="nam">cache_client</span><span class="op">.</span><span class="nam">set</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">            <span class="str">f"{SystemConstantCode.USER_KEY.msg}{userDO.id}"</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">            <span class="nam">access_token</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">            <span class="nam">access_token_expires</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="key">return</span> <span class="nam">token</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t"><span class="key">def</span> <span class="nam">get_user_service</span><span class="op">(</span><span class="op">)</span> <span class="op">-></span> <span class="nam">UserService</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="key">return</span> <span class="nam">UserServiceImpl</span><span class="op">(</span><span class="nam">UserMapper</span><span class="op">(</span><span class="nam">UserDO</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/me"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">get_user</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">    <span class="nam">current_user</span><span class="op">:</span> <span class="nam">CurrentUser</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_current_user</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">BaseResponse</span><span class="op">[</span><span class="nam">UserQuery</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="str">    Query user info</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="nam">user</span><span class="op">:</span> <span class="nam">UserQuery</span> <span class="op">=</span> <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">find_by_id</span><span class="op">(</span><span class="nam">id</span><span class="op">=</span><span class="nam">current_user</span><span class="op">.</span><span class="nam">user_id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">.</span><span class="nam">success</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">user</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span><span class="str">"/login"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">login</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">    <span class="nam">login_form</span><span class="op">:</span> <span class="nam">OAuth2PasswordRequestForm</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">Token</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="str">    User login</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">    <span class="nam">loginCmd</span> <span class="op">=</span> <span class="nam">LoginCmd</span><span class="op">(</span><span class="nam">username</span><span class="op">=</span><span class="nam">login_form</span><span class="op">.</span><span class="nam">username</span><span class="op">,</span> <span class="nam">password</span><span class="op">=</span><span class="nam">login_form</span><span class="op">.</span><span class="nam">password</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">    <span class="key">return</span> <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">login</span><span class="op">(</span><span class="nam">loginCmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="str">"/{id}"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">remove_user</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">    <span class="nam">id</span><span class="op">:</span> <span class="nam">int</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">    <span class="nam">current_user</span><span class="op">:</span> <span class="nam">CurrentUser</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_current_user</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t"><span class="str">    Remove user</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">    <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">remove_by_id</span><span class="op">(</span><span class="nam">id</span><span class="op">=</span><span class="nam">id</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">.</span><span class="nam">success</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">put</span><span class="op">(</span><span class="str">"/"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">update_user</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">    <span class="nam">updateUserCmd</span><span class="op">:</span> <span class="nam">UpdateUserCmd</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">    <span class="nam">current_user</span><span class="op">:</span> <span class="nam">CurrentUser</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_current_user</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t"><span class="str">    Update user</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">    <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">update_by_id</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">updateUserCmd</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">.</span><span class="nam">success</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/exportTemplate"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">export_user_template</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">    <span class="nam">current_user</span><span class="op">:</span> <span class="nam">CurrentUser</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_current_user</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">StreamingResponse</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t"><span class="str">    Export user template</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">    <span class="key">return</span> <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">export_user_template</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">post</span><span class="op">(</span><span class="str">"/import"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">import_user</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">    <span class="nam">file</span><span class="op">:</span> <span class="nam">UploadFile</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">    <span class="nam">current_user</span><span class="op">:</span> <span class="nam">CurrentUser</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_current_user</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t"><span class="str">    Import user info</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">    <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">import_user</span><span class="op">(</span><span class="nam">file</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">    <span class="key">return</span> <span class="nam">result</span><span class="op">.</span><span class="nam">success</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t"><span class="op">@</span><span class="nam">user_router</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="str">"/export"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t"><span class="key">async</span> <span class="key">def</span> <span class="nam">export_user</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">    <span class="nam">params</span><span class="op">:</span> <span class="nam">Params</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">    <span class="nam">user_service</span><span class="op">:</span> <span class="nam">UserService</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_user_service</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">    <span class="nam">current_user</span><span class="op">:</span> <span class="nam">CurrentUser</span> <span class="op">=</span> <span class="nam">Depends</span><span class="op">(</span><span class="nam">get_current_user</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t"><span class="op">)</span> <span class="op">-></span> <span class="nam">StreamingResponse</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="str">    Export user info</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">    <span class="key">return</span> <span class="key">await</span> <span class="nam">user_service</span><span class="op">.</span><span class="nam">export_user</span><span class="op">(</span><span class="nam">params</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_f83affef05b47916___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_9c41cf131237e8e8_probe_controller_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_fc0d8786bb154269_user_service_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_4c5c7dd0d2e26036___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,98 +1,139 @@
-************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\sseerrvviiccee\\iimmppll\\uusseerr__sseerrvviiccee__iimmppll..ppyy:: 6666%%
-************
+************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\aappii\\vv11\\uusseerr__ccoonnttrroolllleerr..ppyy:: 9911%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 3388 ssttaatteemmeennttss ?  2255 rruunn 1133 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 4455 ssttaatteemmeennttss ?  4411 rruunn 44 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
-_1"""User domain service impl""" 
+13 15:26 +0800
+_1"""User operation controller""" 
 _2 
-_3from datetime import timedelta 
-_4from typing import Optional 
-_5 
-_6from fss.common.cache.cache import get_cache_client, Cache 
-_7from fss.common.config import configs 
-_8from fss.common.enum.enum import TokenTypeEnum 
-_9from fss.common.schema.schema import Token 
-_1_0from fss.common.service.impl.service_impl import ServiceImpl 
-_1_1from fss.common.util import security 
-_1_2from fss.common.util.security import verify_password 
-_1_3from fss.starter.system.enum.system import SystemResponseCode,
-SystemConstantCode 
-_1_4from fss.starter.system.exception.system import SystemException 
-_1_5from fss.starter.system.mapper.user_mapper import UserMapper 
-_1_6from fss.starter.system.model.user_do import UserDO 
-_1_7from fss.starter.system.schema.user_schema import UserQuery, LoginCmd 
-_1_8from fss.starter.system.service.user_service import UserService 
-_1_9 
-_2_0 
-_2_1class UserServiceImpl(ServiceImpl[UserMapper, UserDO], UserService): 
-_2_2 def __init__(self, mapper: UserMapper): 
-_2_3 super().__init__(mapper) 
+_3from fastapi import APIRouter, Depends, UploadFile 
+_4from fastapi.security import OAuth2PasswordRequestForm 
+_5from fastapi_pagination import Params 
+_6from starlette.responses import StreamingResponse 
+_7 
+_8from fss.common.result import result 
+_9from fss.common.result.result import BaseResponse 
+_1_0from fss.common.schema.schema import Token, CurrentUser 
+_1_1from fss.common.security.security import get_current_user 
+_1_2from fss.common.util.security import get_password_hash 
+_1_3from fss.starter.system.model.user_do import UserDO 
+_1_4from fss.starter.system.schema.user_schema import ( 
+_1_5 UserCreateCmd, 
+_1_6 UserQuery, 
+_1_7 LoginCmd, 
+_1_8 UpdateUserCmd, 
+_1_9) 
+_2_0from fss.starter.system.service.impl.user_service_impl import
+get_user_service 
+_2_1from fss.starter.system.service.user_service import UserService 
+_2_2 
+_2_3user_router = APIRouter() 
 _2_4 
-_2_5 async def find_by_id(self, id: int) -> Optional[UserQuery]: 
-_2_6 """ 
-_2_7 Retrieval user through user id 
-_2_8 :param id: user id 
-_2_9 :return: user or none 
+_2_5 
+_2_6@user_router.post("/register") 
+_2_7async def register_user( 
+_2_8 create_data: UserCreateCmd, user_service: UserService = Depends
+(get_user_service) 
+_2_9) -> BaseResponse[int]: 
 _3_0 """ 
-_3_1 user_do = await self.mapper.select_by_id(id=id) 
-_3_2 if user_do: 
-_3_3 return UserQuery(**user_do.model_dump()) 
-_3_4 else: 
-_3_5 return None 
+_3_1 User registration 
+_3_2 """ 
+_3_3 create_data.password = await get_password_hash(create_data.password) 
+_3_4 user: UserDO = await user_service.save(data=create_data) 
+_3_5 return result.success(data=user.id) 
 _3_6 
-_3_7 async def login(self, loginCmd: LoginCmd) -> Token: 
-_3_8 """ 
-_3_9 Do log in 
-_4_0 :param loginCmd: loginCmd 
-_4_1 :return: access token and refresh token 
-_4_2 """ 
-_4_3 username: str = loginCmd.username 
-_4_4 userDO: UserDO = await self.mapper.get_user_by_username(username=username) 
-_4_5 if not userDO or not await verify_password(loginCmd.password,
-userDO.password): 
-_4_6 raise SystemException( 
-_4_7 SystemResponseCode.AUTH_FAILED.code, SystemResponseCode.AUTH_FAILED.msg 
-_4_8 ) 
-_4_9 access_token_expires = timedelta
-(minutes=configs.access_token_expire_minutes) 
-_5_0 refresh_token_expires = timedelta
-(minutes=configs.refresh_token_expire_minutes) 
-_5_1 access_token = await security.create_token( 
-_5_2 subject=userDO.id, 
-_5_3 expires_delta=access_token_expires, 
-_5_4 token_type=TokenTypeEnum.access, 
-_5_5 ) 
-_5_6 refresh_token = await security.create_token( 
-_5_7 subject=userDO.id, 
-_5_8 expires_delta=refresh_token_expires, 
-_5_9 token_type=TokenTypeEnum.refresh, 
-_6_0 ) 
-_6_1 token = Token( 
-_6_2 access_token=access_token, 
-_6_3 expired_at=int(access_token_expires.total_seconds()), 
-_6_4 token_type="bearer", 
-_6_5 refresh_token=refresh_token, 
-_6_6 re_expired_at=int(refresh_token_expires.total_seconds()), 
-_6_7 ) 
-_6_8 cache_client: Cache = await get_cache_client() 
-_6_9 await cache_client.set( 
-_7_0 f"{SystemConstantCode.USER_KEY.msg}{userDO.id}", 
-_7_1 access_token, 
-_7_2 access_token_expires, 
-_7_3 ) 
-_7_4 return token 
-_7_5 
-_7_6 
-_7_7def get_user_service() -> UserService: 
-_7_8 return UserServiceImpl(UserMapper(UserDO)) 
+_3_7 
+_3_8@user_router.get("/me") 
+_3_9async def get_user( 
+_4_0 user_service: UserService = Depends(get_user_service), 
+_4_1 current_user: CurrentUser = Depends(get_current_user()), 
+_4_2) -> BaseResponse[UserQuery]: 
+_4_3 """ 
+_4_4 Query user info 
+_4_5 """ 
+_4_6 user: UserQuery = await user_service.find_by_id(id=current_user.user_id) 
+_4_7 return result.success(data=user) 
+_4_8 
+_4_9 
+_5_0@user_router.post("/login") 
+_5_1async def login( 
+_5_2 login_form: OAuth2PasswordRequestForm = Depends(), 
+_5_3 user_service: UserService = Depends(get_user_service), 
+_5_4) -> Token: 
+_5_5 """ 
+_5_6 User login 
+_5_7 """ 
+_5_8 loginCmd = LoginCmd(username=login_form.username,
+password=login_form.password) 
+_5_9 return await user_service.login(loginCmd) 
+_6_0 
+_6_1 
+_6_2@user_router.delete("/{id}") 
+_6_3async def remove_user( 
+_6_4 id: int, 
+_6_5 user_service: UserService = Depends(get_user_service), 
+_6_6 current_user: CurrentUser = Depends(get_current_user()), 
+_6_7) -> None: 
+_6_8 """ 
+_6_9 Remove user 
+_7_0 """ 
+_7_1 await user_service.remove_by_id(id=id) 
+_7_2 return result.success() 
+_7_3 
+_7_4 
+_7_5@user_router.put("/") 
+_7_6async def update_user( 
+_7_7 updateUserCmd: UpdateUserCmd, 
+_7_8 user_service: UserService = Depends(get_user_service), 
+_7_9 current_user: CurrentUser = Depends(get_current_user()), 
+_8_0) -> None: 
+_8_1 """ 
+_8_2 Update user 
+_8_3 """ 
+_8_4 await user_service.update_by_id(data=updateUserCmd) 
+_8_5 return result.success() 
+_8_6 
+_8_7 
+_8_8@user_router.get("/exportTemplate") 
+_8_9async def export_user_template( 
+_9_0 user_service: UserService = Depends(get_user_service), 
+_9_1 current_user: CurrentUser = Depends(get_current_user()), 
+_9_2) -> StreamingResponse: 
+_9_3 """ 
+_9_4 Export user template 
+_9_5 """ 
+_9_6 return await user_service.export_user_template() 
+_9_7 
+_9_8 
+_9_9@user_router.post("/import") 
+_1_0_0async def import_user( 
+_1_0_1 file: UploadFile, 
+_1_0_2 user_service: UserService = Depends(get_user_service), 
+_1_0_3 current_user: CurrentUser = Depends(get_current_user()), 
+_1_0_4) -> None: 
+_1_0_5 """ 
+_1_0_6 Import user info 
+_1_0_7 """ 
+_1_0_8 await user_service.import_user(file) 
+_1_0_9 return result.success() 
+_1_1_0 
+_1_1_1 
+_1_1_2@user_router.get("/export") 
+_1_1_3async def export_user( 
+_1_1_4 params: Params = Depends(), 
+_1_1_5 user_service: UserService = Depends(get_user_service), 
+_1_1_6 current_user: CurrentUser = Depends(get_current_user()), 
+_1_1_7) -> StreamingResponse: 
+_1_1_8 """ 
+_1_1_9 Export user info 
+_1_2_0 """ 
+_1_2_1 return await user_service.export_user(params) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+13 15:26 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/d_fc0d8786bb154269___init___py.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/d_794d731f07d9e36c___init___py.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for fss\starter\system\service\__init__.py: 100%</title>
+    <title>Coverage for fss\__init__.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>fss\starter\system\service\__init__.py</b>:
+            <span class="text">Coverage for </span><b>fss\__init__.py</b>:
             <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -56,20 +56,20 @@
         <h2>
             <span class="text">0 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">0<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_dab9b2a1903716f2_user_schema_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_f83affef05b47916___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_23127160240ab4f6___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -80,18 +80,18 @@
     </div>
 </header>
 <main id="source">
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_dab9b2a1903716f2_user_schema_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_f83affef05b47916___init___py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_23127160240ab4f6___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-12 22:20 +0800
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee ffoorr ffssss\\ssttaarrtteerr\\ssyysstteemm\\sseerrvviiccee\\____iinniitt____..ppyy:: 110000%% ************
+************ CCoovveerraaggee ffoorr ffssss\\____iinniitt____..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-11 19:09 +0800
+12 22:20 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/favicon_32.png` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/index.html` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">72%</span>
+            <span class="pc_cov">75%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -157,32 +157,32 @@
                 <td>3</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="3 3">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_bbb369617a9e5695_sqlmodel_impl_py.html">fss\common\persistence\sqlmodel_impl.py</a></td>
-                <td>109</td>
-                <td>71</td>
+                <td>114</td>
+                <td>56</td>
                 <td>0</td>
-                <td class="right" data-ratio="38 109">35%</td>
+                <td class="right" data-ratio="58 114">51%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_0e53216603666de3___init___py.html">fss\common\result\__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_0e53216603666de3_result_py.html">fss\common\result\result.py</a></td>
                 <td>34</td>
-                <td>6</td>
+                <td>5</td>
                 <td>0</td>
-                <td class="right" data-ratio="28 34">82%</td>
+                <td class="right" data-ratio="29 34">85%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_8efc05ae27a1a50a___init___py.html">fss\common\schema\__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
@@ -221,17 +221,17 @@
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_9373b28d605cd29a_service_impl_py.html">fss\common\service\impl\service_impl.py</a></td>
                 <td>47</td>
-                <td>22</td>
+                <td>20</td>
                 <td>0</td>
-                <td class="right" data-ratio="25 47">53%</td>
+                <td class="right" data-ratio="27 47">57%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_737f82a7e813f983_service_py.html">fss\common\service\service.py</a></td>
                 <td>50</td>
                 <td>15</td>
                 <td>0</td>
                 <td class="right" data-ratio="35 50">70%</td>
@@ -241,18 +241,18 @@
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_392b9405ba6460b0_security_py.html">fss\common\util\security.py</a></td>
-                <td>28</td>
+                <td>31</td>
                 <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="26 28">93%</td>
+                <td class="right" data-ratio="29 31">94%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_392b9405ba6460b0_snowflake_py.html">fss\common\util\snowflake.py</a></td>
                 <td>39</td>
                 <td>11</td>
                 <td>0</td>
                 <td class="right" data-ratio="28 39">72%</td>
@@ -311,32 +311,32 @@
                 <td>20</td>
                 <td>4</td>
                 <td>0</td>
                 <td class="right" data-ratio="16 20">80%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_9c41cf131237e8e8_user_controller_py.html">fss\starter\system\api\v1\user_controller.py</a></td>
-                <td>25</td>
-                <td>1</td>
+                <td>45</td>
+                <td>4</td>
                 <td>0</td>
-                <td class="right" data-ratio="24 25">96%</td>
+                <td class="right" data-ratio="41 45">91%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_4c5c7dd0d2e26036___init___py.html">fss\starter\system\enum\__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_4c5c7dd0d2e26036_system_py.html">fss\starter\system\enum\system.py</a></td>
-                <td>13</td>
+                <td>14</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="13 13">100%</td>
+                <td class="right" data-ratio="14 14">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_b6eeb7fba27ca014___init___py.html">fss\starter\system\exception\__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
@@ -395,18 +395,18 @@
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_dab9b2a1903716f2_user_schema_py.html">fss\starter\system\schema\user_schema.py</a></td>
-                <td>12</td>
+                <td>19</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="12 12">100%</td>
+                <td class="right" data-ratio="19 19">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_fc0d8786bb154269___init___py.html">fss\starter\system\service\__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
@@ -416,25 +416,25 @@
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_f83affef05b47916_user_service_impl_py.html">fss\starter\system\service\impl\user_service_impl.py</a></td>
-                <td>38</td>
-                <td>13</td>
+                <td>93</td>
+                <td>35</td>
                 <td>0</td>
-                <td class="right" data-ratio="25 38">66%</td>
+                <td class="right" data-ratio="58 93">62%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_fc0d8786bb154269_user_service_py.html">fss\starter\system\service\user_service.py</a></td>
-                <td>12</td>
-                <td>2</td>
+                <td>24</td>
+                <td>5</td>
                 <td>0</td>
-                <td class="right" data-ratio="10 12">83%</td>
+                <td class="right" data-ratio="19 24">79%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_a44f0ac069e85531___init___py.html">tests\__init__.py</a></td>
                 <td>0</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
@@ -458,39 +458,39 @@
                 <td>12</td>
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="12 12">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_2ddb7f614afd77c0_user_test_py.html">tests\system\v1\user_test.py</a></td>
-                <td>21</td>
+                <td>69</td>
                 <td>0</td>
                 <td>0</td>
-                <td class="right" data-ratio="21 21">100%</td>
+                <td class="right" data-ratio="69 69">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
-                <td>855</td>
-                <td>243</td>
+                <td>1006</td>
+                <td>253</td>
                 <td>0</td>
-                <td class="right" data-ratio="612 855">72%</td>
+                <td class="right" data-ratio="753 1006">75%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-11 19:09 +0800
+            created at 2024-04-13 15:26 +0800
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_2ddb7f614afd77c0_user_test_py.html"/>
         <a id="nextFileLink" class="nav" href="d_794d731f07d9e36c___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 7722%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 7755%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-11 19:09 +0800
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-13 15:26 +0800
 MMoodduullee                                               ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _f_s_s_\_____i_n_i_t_____._p_y                                      0          0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_____i_n_i_t_____._p_y                               0          0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_c_a_c_h_e_\_____i_n_i_t_____._p_y                         0          0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_c_a_c_h_e_\_c_a_c_h_e_._p_y                            23         8       0        65%
 _f_s_s_\_c_o_m_m_o_n_\_c_a_c_h_e_\_p_a_g_e___c_a_c_h_e_._p_y                       21         8       0        62%
 _f_s_s_\_c_o_m_m_o_n_\_c_o_n_f_i_g_._p_y                                 61         21      0        66%
@@ -17,54 +17,54 @@
 _f_s_s_\_c_o_m_m_o_n_\_e_n_u_m_\_e_n_u_m_._p_y                              11         0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_e_x_c_e_p_t_i_o_n_\_____i_n_i_t_____._p_y                     0          0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_e_x_c_e_p_t_i_o_n_\_e_x_c_e_p_t_i_o_n_._p_y                    6          3       0        50%
 _f_s_s_\_c_o_m_m_o_n_\_p_e_r_s_i_s_t_e_n_c_e_\_____i_n_i_t_____._p_y                   0          0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_p_e_r_s_i_s_t_e_n_c_e_\_b_a_s_e___m_a_p_p_e_r_._p_y                51         17      0        67%
 _f_s_s_\_c_o_m_m_o_n_\_p_e_r_s_i_s_t_e_n_c_e_\_b_a_s_e___m_o_d_e_l_._p_y                 10         0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_p_e_r_s_i_s_t_e_n_c_e_\_m_a_p_p_e_r_._p_y                     3          0       0        100%
-_f_s_s_\_c_o_m_m_o_n_\_p_e_r_s_i_s_t_e_n_c_e_\_s_q_l_m_o_d_e_l___i_m_p_l_._p_y              109        71      0        35%
+_f_s_s_\_c_o_m_m_o_n_\_p_e_r_s_i_s_t_e_n_c_e_\_s_q_l_m_o_d_e_l___i_m_p_l_._p_y              114        56      0        51%
 _f_s_s_\_c_o_m_m_o_n_\_r_e_s_u_l_t_\_____i_n_i_t_____._p_y                        0          0       0        100%
-_f_s_s_\_c_o_m_m_o_n_\_r_e_s_u_l_t_\_r_e_s_u_l_t_._p_y                          34         6       0        82%
+_f_s_s_\_c_o_m_m_o_n_\_r_e_s_u_l_t_\_r_e_s_u_l_t_._p_y                          34         5       0        85%
 _f_s_s_\_c_o_m_m_o_n_\_s_c_h_e_m_a_\_____i_n_i_t_____._p_y                        0          0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_s_c_h_e_m_a_\_s_c_h_e_m_a_._p_y                          11         0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_s_e_c_u_r_i_t_y_\_____i_n_i_t_____._p_y                      0          0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_s_e_c_u_r_i_t_y_\_s_e_c_u_r_i_t_y_._p_y                      21         4       0        81%
 _f_s_s_\_c_o_m_m_o_n_\_s_e_r_v_i_c_e_\_____i_n_i_t_____._p_y                       0          0       0        100%
 _f_s_s_\_c_o_m_m_o_n_\_s_e_r_v_i_c_e_\_i_m_p_l_\_____i_n_i_t_____._p_y                  0          0       0        100%
-_f_s_s_\_c_o_m_m_o_n_\_s_e_r_v_i_c_e_\_i_m_p_l_\_s_e_r_v_i_c_e___i_m_p_l_._p_y              47         22      0        53%
+_f_s_s_\_c_o_m_m_o_n_\_s_e_r_v_i_c_e_\_i_m_p_l_\_s_e_r_v_i_c_e___i_m_p_l_._p_y              47         20      0        57%
 _f_s_s_\_c_o_m_m_o_n_\_s_e_r_v_i_c_e_\_s_e_r_v_i_c_e_._p_y                        50         15      0        70%
 _f_s_s_\_c_o_m_m_o_n_\_u_t_i_l_\_____i_n_i_t_____._p_y                          0          0       0        100%
-_f_s_s_\_c_o_m_m_o_n_\_u_t_i_l_\_s_e_c_u_r_i_t_y_._p_y                          28         2       0        93%
+_f_s_s_\_c_o_m_m_o_n_\_u_t_i_l_\_s_e_c_u_r_i_t_y_._p_y                          31         2       0        94%
 _f_s_s_\_c_o_m_m_o_n_\_u_t_i_l_\_s_n_o_w_f_l_a_k_e_._p_y                         39         11      0        72%
 _f_s_s_\_m_i_d_d_l_e_w_a_r_e_\_____i_n_i_t_____._p_y                           0          0       0        100%
 _f_s_s_\_m_i_d_d_l_e_w_a_r_e_\_d_b___s_e_s_s_i_o_n___m_i_d_d_l_e_w_a_r_e_._p_y              68         12      0        82%
 _f_s_s_\_s_t_a_r_t_e_r_\_____i_n_i_t_____._p_y                              6          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_e_r_v_e_r_._p_y                                71         21      0        70%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_____i_n_i_t_____._p_y                       0          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_a_p_i_\_____i_n_i_t_____._p_y                   0          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_a_p_i_\_v_1_\_____i_n_i_t_____._p_y                0          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_a_p_i_\_v_1_\_p_r_o_b_e___c_o_n_t_r_o_l_l_e_r_._p_y        20         4       0        80%
-_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_a_p_i_\_v_1_\_u_s_e_r___c_o_n_t_r_o_l_l_e_r_._p_y         25         1       0        96%
+_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_a_p_i_\_v_1_\_u_s_e_r___c_o_n_t_r_o_l_l_e_r_._p_y         45         4       0        91%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_e_n_u_m_\_____i_n_i_t_____._p_y                  0          0       0        100%
-_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_e_n_u_m_\_s_y_s_t_e_m_._p_y                    13         0       0        100%
+_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_e_n_u_m_\_s_y_s_t_e_m_._p_y                    14         0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_e_x_c_e_p_t_i_o_n_\_____i_n_i_t_____._p_y             0          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_e_x_c_e_p_t_i_o_n_\_s_y_s_t_e_m_._p_y               5          1       0        80%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_m_a_p_p_e_r_\_____i_n_i_t_____._p_y                0          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_m_a_p_p_e_r_\_u_s_e_r___m_a_p_p_e_r_._p_y             11         1       0        91%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_m_o_d_e_l_\_____i_n_i_t_____._p_y                 0          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_m_o_d_e_l_\_u_s_e_r___d_o_._p_y                  10         0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_r_o_u_t_e_r_\_____i_n_i_t_____._p_y                0          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_r_o_u_t_e_r_\_s_y_s_t_e_m_._p_y                  6          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_c_h_e_m_a_\_____i_n_i_t_____._p_y                0          0       0        100%
-_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_c_h_e_m_a_\_u_s_e_r___s_c_h_e_m_a_._p_y             12         0       0        100%
+_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_c_h_e_m_a_\_u_s_e_r___s_c_h_e_m_a_._p_y             19         0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_e_r_v_i_c_e_\_____i_n_i_t_____._p_y               0          0       0        100%
 _f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_e_r_v_i_c_e_\_i_m_p_l_\_____i_n_i_t_____._p_y          0          0       0        100%
-_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_e_r_v_i_c_e_\_i_m_p_l_\_u_s_e_r___s_e_r_v_i_c_e___i_m_p_l_._p_y 38         13      0        66%
-_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_e_r_v_i_c_e_\_u_s_e_r___s_e_r_v_i_c_e_._p_y           12         2       0        83%
+_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_e_r_v_i_c_e_\_i_m_p_l_\_u_s_e_r___s_e_r_v_i_c_e___i_m_p_l_._p_y 93         35      0        62%
+_f_s_s_\_s_t_a_r_t_e_r_\_s_y_s_t_e_m_\_s_e_r_v_i_c_e_\_u_s_e_r___s_e_r_v_i_c_e_._p_y           24         5       0        79%
 _t_e_s_t_s_\_____i_n_i_t_____._p_y                                    0          0       0        100%
 _t_e_s_t_s_\_s_y_s_t_e_m_\_____i_n_i_t_____._p_y                             0          0       0        100%
 _t_e_s_t_s_\_s_y_s_t_e_m_\_v_1_\_____i_n_i_t_____._p_y                          0          0       0        100%
 _t_e_s_t_s_\_s_y_s_t_e_m_\_v_1_\_p_r_o_b_e___t_e_s_t_._p_y                        12         0       0        100%
-_t_e_s_t_s_\_s_y_s_t_e_m_\_v_1_\_u_s_e_r___t_e_s_t_._p_y                         21         0       0        100%
-Total                                                855        243     0        72%
+_t_e_s_t_s_\_s_y_s_t_e_m_\_v_1_\_u_s_e_r___t_e_s_t_._p_y                         69         0       0        100%
+Total                                                1006       253     0        75%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-11 19:09 +0800
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-13 15:26 +0800
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/keybd_closed.png` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/keybd_open.png` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/status.json` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/status.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977394636015327%*

 * *Differences: {"'files'": "{'d_bbb369617a9e5695_sqlmodel_impl_py': {'hash': 'e602d434b46cdd2b7815f28bd99f9438', "*

 * *            "'index': {'nums': {insert: [(2, 114), (4, 56)], delete: [4, 2]}}}, "*

 * *            "'d_0e53216603666de3_result_py': {'hash': '8879326b8fa2a5faa663cd6041b505ee', 'index': "*

 * *            "{'nums': {insert: [(4, 5)], delete: [4]}}}, 'd_9373b28d605cd29a_service_impl_py': "*

 * *            "{'hash': '8f8f4e14207e6ece19a7b41d2f726734', 'index': {'nums': {insert: [(4, 20)], "*

 * *            "delete: [4]}}}, 'd_39 […]*

```diff
@@ -48,23 +48,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\common\\result\\__init__.py"
             }
         },
         "d_0e53216603666de3_result_py": {
-            "hash": "590f931d28e7d125ea7050cdb27a199d",
+            "hash": "8879326b8fa2a5faa663cd6041b505ee",
             "index": {
                 "html_filename": "d_0e53216603666de3_result_py.html",
                 "nums": [
                     0,
                     1,
                     34,
                     0,
-                    6,
+                    5,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\common\\result\\result.py"
             }
         },
@@ -286,21 +286,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "tests\\system\\v1\\probe_test.py"
             }
         },
         "d_2ddb7f614afd77c0_user_test_py": {
-            "hash": "0d30e2060c8df91ad8b74c4ed70412a3",
+            "hash": "d391d5964571f225e5c0dacfbbbb4c0b",
             "index": {
                 "html_filename": "d_2ddb7f614afd77c0_user_test_py.html",
                 "nums": [
                     0,
                     1,
-                    21,
+                    69,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "tests\\system\\v1\\user_test.py"
@@ -320,21 +320,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\common\\util\\__init__.py"
             }
         },
         "d_392b9405ba6460b0_security_py": {
-            "hash": "97b39eb4da82d75674438a9069638300",
+            "hash": "82d80f808a046198a5f4a62e6e43f35c",
             "index": {
                 "html_filename": "d_392b9405ba6460b0_security_py.html",
                 "nums": [
                     0,
                     1,
-                    28,
+                    31,
                     0,
                     2,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\common\\util\\security.py"
@@ -439,21 +439,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\enum\\__init__.py"
             }
         },
         "d_4c5c7dd0d2e26036_system_py": {
-            "hash": "518cf5198a076cc2b965900b1dd3aab7",
+            "hash": "3f6c27a55cce060e62e039eaf765dfd4",
             "index": {
                 "html_filename": "d_4c5c7dd0d2e26036_system_py.html",
                 "nums": [
                     0,
                     1,
-                    13,
+                    14,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\enum\\system.py"
@@ -609,23 +609,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\common\\service\\impl\\__init__.py"
             }
         },
         "d_9373b28d605cd29a_service_impl_py": {
-            "hash": "9909f0cf5c899b8c68db9dfff8fd7217",
+            "hash": "8f8f4e14207e6ece19a7b41d2f726734",
             "index": {
                 "html_filename": "d_9373b28d605cd29a_service_impl_py.html",
                 "nums": [
                     0,
                     1,
                     47,
                     0,
-                    22,
+                    20,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\common\\service\\impl\\service_impl.py"
             }
         },
@@ -660,23 +660,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\api\\v1\\probe_controller.py"
             }
         },
         "d_9c41cf131237e8e8_user_controller_py": {
-            "hash": "3468454e7a830964272dca1e945e40a2",
+            "hash": "2ef3c74f8159c4adf932ee17a4245b80",
             "index": {
                 "html_filename": "d_9c41cf131237e8e8_user_controller_py.html",
                 "nums": [
                     0,
                     1,
-                    25,
+                    45,
                     0,
-                    1,
+                    4,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\api\\v1\\user_controller.py"
             }
         },
@@ -796,23 +796,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\common\\persistence\\mapper.py"
             }
         },
         "d_bbb369617a9e5695_sqlmodel_impl_py": {
-            "hash": "e57ab87ec814b5b17a5f449497f0393c",
+            "hash": "e602d434b46cdd2b7815f28bd99f9438",
             "index": {
                 "html_filename": "d_bbb369617a9e5695_sqlmodel_impl_py.html",
                 "nums": [
                     0,
                     1,
-                    109,
+                    114,
                     0,
-                    71,
+                    56,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\common\\persistence\\sqlmodel_impl.py"
             }
         },
@@ -830,21 +830,21 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\schema\\__init__.py"
             }
         },
         "d_dab9b2a1903716f2_user_schema_py": {
-            "hash": "47f6712635e9ce3dd94bf48cb420264f",
+            "hash": "09d706bfde2a1c93ef9c71714202fe02",
             "index": {
                 "html_filename": "d_dab9b2a1903716f2_user_schema_py.html",
                 "nums": [
                     0,
                     1,
-                    12,
+                    19,
                     0,
                     0,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\schema\\user_schema.py"
@@ -932,23 +932,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\service\\impl\\__init__.py"
             }
         },
         "d_f83affef05b47916_user_service_impl_py": {
-            "hash": "78a013b84ee4313a9f88b4b853bb546b",
+            "hash": "a67c4e53fcb66a7f65f415fd8f114847",
             "index": {
                 "html_filename": "d_f83affef05b47916_user_service_impl_py.html",
                 "nums": [
                     0,
                     1,
-                    38,
+                    93,
                     0,
-                    13,
+                    35,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\service\\impl\\user_service_impl.py"
             }
         },
@@ -966,23 +966,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\service\\__init__.py"
             }
         },
         "d_fc0d8786bb154269_user_service_py": {
-            "hash": "1619a2056b8f8eecd59d0fcd3730f6b0",
+            "hash": "24127a9552ab9a916bbead8eb4d7c2cf",
             "index": {
                 "html_filename": "d_fc0d8786bb154269_user_service_py.html",
                 "nums": [
                     0,
                     1,
-                    12,
+                    24,
                     0,
-                    2,
+                    5,
                     0,
                     0,
                     0
                 ],
                 "relative_filename": "fss\\starter\\system\\service\\user_service.py"
             }
         }
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/htmlcov/style.css` & `fastapi_sqlmodel_starter-1.0.0b1/src/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/migrations/__pycache__/env.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/__pycache__/env.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xf9c31766 (Thu Apr 11 11:05:29 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 2714
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/migrations/env.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/migrations/script.py.mako` & `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/migrations/versions/947dad7dbfdb_init_project.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/947dad7dbfdb_init_project.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-311.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/migrations/versions/__pycache__/947dad7dbfdb_init_project.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xde4b1566 (Tue Apr  9 14:08:30 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 1516
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/v1/__pycache__/probe_test.cpython-311-pytest-8.1.1.pyc` & `fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/__pycache__/probe_test.cpython-311-pytest-8.1.1.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x33c01766 (Thu Apr 11 10:49:23 2024 UTC)
+moddate:  0x31201966 (Fri Apr 12 11:51:13 2024 UTC)
 files sz: 527
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
```

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/src/tests/system/v1/probe_test.py` & `fastapi_sqlmodel_starter-1.0.0b1/src/tests/system/v1/probe_test.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlmodel_starter-1.0.0b0/PKG-INFO` & `fastapi_sqlmodel_starter-1.0.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: fastapi-sqlmodel-starter
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: Fss aims to be one of top scaffold in PyWeb.
 Home-page: https://github.com/tyvekzhang/fastapi-sqlmodel-starter
 License: MIT
 Keywords: fastapi,sqlmodel,tools,web,scaffold
 Author: tyvekZhang
 Author-email: tyvekzhang@gmail.com
 Maintainer: tyvekZhang
 Maintainer-email: tyvekzhang@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -30,37 +29,40 @@
 Requires-Dist: diskcache (>=5.6.3,<6.0.0)
 Requires-Dist: eval-type-backport (>=0.1.3,<0.2.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: fastapi-async-sqlalchemy (>=0.6.1,<0.7.0)
 Requires-Dist: fastapi-offline (>=1.7.1,<2.0.0)
 Requires-Dist: fastapi-pagination (>=0.12.21,<0.13.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: redis[hiredis] (>=5.0.3,<6.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0)
 Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
+Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0)
 Project-URL: Documentation, https://github.com/tyvekzhang/fastapi-sqlmodel-starter/wiki
 Project-URL: Repository, https://github.com/tyvekzhang/fastapi-sqlmodel-starter
 Description-Content-Type: text/markdown
 
 <div  align="center" style="margin-top: 3%">
    <h1>
      FastAPI Sqlmodel Starter (Fss)
    </h1>
    <p>
      <img src="https://raw.githubusercontent.com/tyvekzhang/fastapi-sqlmodel-starter/main/docs/img/logo.png" alt="logo" style="vertical-align:middle; margin: 0.5%"/>
    </p>
    <p>
      <img alt="GitHub License" src="https://img.shields.io/github/license/tyvekzhang/fastapi-sqlmodel-starter">
      <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/fastapi-sqlmodel-starter">
-     <img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/tyvekzhang/fastapi-sqlmodel-starter/ci.yaml">
+     <img alt="CI" src="https://github.com/tyvekzhang/fastapi-sqlmodel-starter/actions/workflows/ci.yaml/badge.svg">
      <img alt="Codecov" src="https://img.shields.io/codecov/c/github/tyvekzhang/fastapi-sqlmodel-starter">
      <img alt="Read the Docs" src="https://img.shields.io/readthedocs/fastapi-sqlmodel-starter">
    </p>
    <h4>
       <p>
         <b>简体中文</b> |
         <a href="https://github.com/tyvekzhang/fastapi-sqlmodel-starter/blob/main/docs/README_en.md">English</a>
@@ -75,15 +77,15 @@
 ## 特性
 
 - 开箱即用, 内置常见数据库、缓存([默认]Sqlite, PostgreSQL, MySQL, [默认]文件缓存, Redis)
 - 自带单表的几乎所有操作
 - 数据库迁移, 静态代码扫描, 接口文档等一众特性
 
 ## 快速开始
-1. 首先确保python的版本是3.8及以上的
+1. 首先确保python的版本是3.9及以上的
 2. 克隆代码
 ```shell
 git clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter
 cd fastapi-sqlmodel-starter/src
 ```
 3. [可选]创建虚拟环境, 本篇以venv为例, 类似的工具还有conda, virtualenv等
 ```shell
@@ -101,14 +103,15 @@
 ```shell
 alembic upgrade head
 ```
 7. 启动
    - Windows: python3 fss\apiserver.py
    - macOS 或 Linux: python3 fss/apiserver.py
 8. 访问: http://127.0.0.1:9010/docs
+9. 首先通过注册接口新建用户, 接着进行认证, 一切Ok.
 ## 文档
 - https://fastapi-sqlmodel-starter.readthedocs.io/en/latest/
 ## 贡献
 
 欢迎为 FastapiSqlmodelStarter 做出贡献！你可以通过以下方式参与：
 
 - 提交 Bug 或功能需求到 [Issue 追踪器](https://github.com/tyvekzhang/fastapi-sqlmodel-starter/issues)
```

#### html2text {}

```diff
@@ -1,57 +1,58 @@
-Metadata-Version: 2.1 Name: fastapi-sqlmodel-starter Version: 1.0.0b0 Summary:
+Metadata-Version: 2.1 Name: fastapi-sqlmodel-starter Version: 1.0.0b1 Summary:
 Fss aims to be one of top scaffold in PyWeb. Home-page: https://github.com/
 tyvekzhang/fastapi-sqlmodel-starter License: MIT Keywords:
 fastapi,sqlmodel,tools,web,scaffold Author: tyvekZhang Author-email:
 tyvekzhang@gmail.com Maintainer: tyvekZhang Maintainer-email:
-tyvekzhang@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
+tyvekzhang@gmail.com Requires-Python: >=3.9,<4.0 Classifier: Development Status
 :: 4 - Beta Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Dist: aiomysql (>=0.2.0,<0.3.0) Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
-Requires-Dist: alembic (>=1.13.1,<2.0.0) Requires-Dist: asyncpg
-(>=0.29.0,<0.30.0) Requires-Dist: bcrypt (==4.0.1) Requires-Dist: diskcache
-(>=5.6.3,<6.0.0) Requires-Dist: eval-type-backport (>=0.1.3,<0.2.0) Requires-
-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: fastapi-async-sqlalchemy
-(>=0.6.1,<0.7.0) Requires-Dist: fastapi-offline (>=1.7.1,<2.0.0) Requires-Dist:
-fastapi-pagination (>=0.12.21,<0.13.0) Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: passlib (>=1.7.4,<2.0.0) Requires-Dist: python-dotenv
-(>=1.0.1,<2.0.0) Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
-Requires-Dist: python-multipart (>=0.0.9,<0.0.10) Requires-Dist: redis[hiredis]
-(>=5.0.3,<6.0.0) Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0) Requires-
-Dist: sqlmodel (>=0.0.16,<0.0.17) Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
-Project-URL: Documentation, https://github.com/tyvekzhang/fastapi-sqlmodel-
-starter/wiki Project-URL: Repository, https://github.com/tyvekzhang/fastapi-
-sqlmodel-starter Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Requires-Dist: aiomysql (>=0.2.0,<0.3.0) Requires-Dist:
+aiosqlite (>=0.20.0,<0.21.0) Requires-Dist: alembic (>=1.13.1,<2.0.0) Requires-
+Dist: asyncpg (>=0.29.0,<0.30.0) Requires-Dist: bcrypt (==4.0.1) Requires-Dist:
+diskcache (>=5.6.3,<6.0.0) Requires-Dist: eval-type-backport (>=0.1.3,<0.2.0)
+Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: fastapi-async-
+sqlalchemy (>=0.6.1,<0.7.0) Requires-Dist: fastapi-offline (>=1.7.1,<2.0.0)
+Requires-Dist: fastapi-pagination (>=0.12.21,<0.13.0) Requires-Dist: loguru
+(>=0.7.2,<0.8.0) Requires-Dist: openpyxl (>=3.1.2,<4.0.0) Requires-Dist: pandas
+(>=2.2.2,<3.0.0) Requires-Dist: passlib (>=1.7.4,<2.0.0) Requires-Dist: python-
+dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-jose[cryptography]
+(>=3.3.0,<4.0.0) Requires-Dist: python-multipart (>=0.0.9,<0.0.10) Requires-
+Dist: redis[hiredis] (>=5.0.3,<6.0.0) Requires-Dist: sqlalchemy-utils
+(>=0.41.2,<0.42.0) Requires-Dist: sqlmodel (>=0.0.16,<0.0.17) Requires-Dist:
+uvicorn (>=0.29.0,<0.30.0) Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0) Project-
+URL: Documentation, https://github.com/tyvekzhang/fastapi-sqlmodel-starter/wiki
+Project-URL: Repository, https://github.com/tyvekzhang/fastapi-sqlmodel-starter
+Description-Content-Type: text/markdown
                  ************ FFaassttAAPPII SSqqllmmooddeell SSttaarrtteerr ((FFssss)) ************
                                     [logo]
-    [GitHub License][PyPI - Python Version][GitHub Actions Workflow Status]
-                           [Codecov][Read the Docs]
+      [GitHub License][PyPI - Python Version][CI][Codecov][Read the Docs]
                         ****** ?ç?®??ä?½??ä?¸?­?æ?? || _EE_nn_gg_ll_ii_ss_hh ******
               ******** PPyyWWeebb?é?¢??å???æ???å?¥?½?ç??¨?ç???è???æ???æ??¶?ä?¹??ä?¸??ã?? ********
 ## ç¹æ§ - å¼ç®±å³ç¨, åç½®å¸¸è§æ°æ®åºãç¼å­([é»è®¤]Sqlite,
 PostgreSQL, MySQL, [é»è®¤]æä»¶ç¼å­, Redis) -
 èªå¸¦åè¡¨çå ä¹æææä½ - æ°æ®åºè¿ç§», éæä»£ç æ«æ,
 æ¥å£ææ¡£ç­ä¸ä¼ç¹æ§ ## å¿«éå¼å§ 1.
-é¦åç¡®ä¿pythonççæ¬æ¯3.8åä»¥ä¸ç 2. åéä»£ç  ```shell git
+é¦åç¡®ä¿pythonççæ¬æ¯3.9åä»¥ä¸ç 2. åéä»£ç  ```shell git
 clone https://github.com/tyvekzhang/fastapi-sqlmodel-starter cd fastapi-
 sqlmodel-starter/src ``` 3. [å¯é]åå»ºèæç¯å¢, æ¬ç¯ä»¥venvä¸ºä¾,
 ç±»ä¼¼çå·¥å·è¿æconda, virtualenvç­ ```shell python3 -m venv .env_fss ```
 4. [å¯é]æ¿æ´»èæç¯å¢ - Windows: .env_fss\Scripts\activate - macOS æ
 Linux: source .env_fss/bin/activate 5. å®è£ Poetryå¹¶ä¸è½½ä¾èµ ```shell
 pip install poetry --trusted-host=mirrors.tuna.tsinghua.edu.cn --index-
 url=https://mirrors.tuna.tsinghua.edu.cn/pypi/web/simple poetry install ``` 6.
 æ°æ®åºè¿ç§» ```shell alembic upgrade head ``` 7. å¯å¨ - Windows: python3
 fss\apiserver.py - macOS æ Linux: python3 fss/apiserver.py 8. è®¿é®: http://
-127.0.0.1:9010/docs ## ææ¡£ - https://fastapi-sqlmodel-
+127.0.0.1:9010/docs 9. é¦åéè¿æ³¨åæ¥å£æ°å»ºç¨æ·,
+æ¥çè¿è¡è®¤è¯, ä¸åOk. ## ææ¡£ - https://fastapi-sqlmodel-
 starter.readthedocs.io/en/latest/ ## è´¡ç® æ¬¢è¿ä¸º FastapiSqlmodelStarter
 ååºè´¡ç®ï¼ä½ å¯ä»¥éè¿ä»¥ä¸æ¹å¼åä¸ï¼ - æäº¤ Bug
 æåè½éæ±å° [Issue è¿½è¸ªå¨](https://github.com/tyvekzhang/fastapi-
 sqlmodel-starter/issues) - æäº¤ä»£ç æ¹è¿ç Pull Request -
 ç¼ååæ¹è¿ææ¡£ - åäº«ä½ ä½¿ç¨ FastapiSqlmodelStarter
 çç»éªåæ³æ³ ## è®¸å¯è¯ FastapiSqlmodelStarter éç¨ [MIT è®¸å¯è¯]
 (https://opensource.org/licenses/MIT)å¼æºã
```

