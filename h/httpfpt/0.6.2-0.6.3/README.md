# Comparing `tmp/httpfpt-0.6.2.tar.gz` & `tmp/httpfpt-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpfpt-0.6.2.tar", last modified: Wed Mar 20 10:56:23 2024, max compression
+gzip compressed data, was "httpfpt-0.6.3.tar", last modified: Sat Apr 13 05:43:04 2024, max compression
```

## Comparing `httpfpt-0.6.2.tar` & `httpfpt-0.6.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1084 2024-03-19 04:02:01.709207 httpfpt-0.6.2/LICENSE
--rw-r--r--   0        0        0     3912 2024-03-20 10:36:09.414602 httpfpt-0.6.2/README.md
--rw-r--r--   0        0        0       75 2024-03-20 10:37:02.735034 httpfpt-0.6.2/httpfpt/__init__.py
--rw-r--r--   0        0        0     4868 2024-03-20 10:36:09.415602 httpfpt-0.6.2/httpfpt/cli.py
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.710205 httpfpt-0.6.2/httpfpt/common/__init__.py
--rw-r--r--   0        0        0      965 2024-03-19 04:02:01.710205 httpfpt-0.6.2/httpfpt/common/env_handler.py
--rw-r--r--   0        0        0     1896 2024-03-19 04:02:01.711206 httpfpt-0.6.2/httpfpt/common/errors.py
--rw-r--r--   0        0        0     1454 2024-03-19 04:02:01.711206 httpfpt-0.6.2/httpfpt/common/excel_handler.py
--rw-r--r--   0        0        0     1921 2024-03-19 04:02:01.711206 httpfpt-0.6.2/httpfpt/common/json_handler.py
--rw-r--r--   0        0        0     1659 2024-03-19 04:02:01.711206 httpfpt-0.6.2/httpfpt/common/log.py
--rw-r--r--   0        0        0    17711 2024-03-19 04:02:01.712208 httpfpt-0.6.2/httpfpt/common/send_request.py
--rw-r--r--   0        0        0     1554 2024-03-19 04:02:01.713209 httpfpt-0.6.2/httpfpt/common/toml_handler.py
--rw-r--r--   0        0        0     2238 2024-03-19 04:02:01.713209 httpfpt-0.6.2/httpfpt/common/variable_cache.py
--rw-r--r--   0        0        0     3440 2024-03-19 04:02:01.713209 httpfpt-0.6.2/httpfpt/common/yaml_handler.py
--rw-r--r--   0        0        0     4593 2024-03-19 04:02:01.713209 httpfpt-0.6.2/httpfpt/conftest.py
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.714207 httpfpt-0.6.2/httpfpt/core/__init__.py
--rw-r--r--   0        0        0       42 2024-03-19 04:02:01.714207 httpfpt-0.6.2/httpfpt/core/allure_env/environment.properties
--rw-r--r--   0        0        0      997 2024-03-19 04:02:01.714207 httpfpt-0.6.2/httpfpt/core/auth.yaml
--rw-r--r--   0        0        0      964 2024-03-19 04:02:01.714207 httpfpt-0.6.2/httpfpt/core/conf.toml
--rw-r--r--   0        0        0     5161 2024-03-20 10:36:09.415602 httpfpt-0.6.2/httpfpt/core/get_conf.py
--rw-r--r--   0        0        0     3537 2024-03-20 10:36:09.416602 httpfpt-0.6.2/httpfpt/core/path_conf.py
--rw-r--r--   0        0        0       59 2024-03-20 09:52:18.135413 httpfpt-0.6.2/httpfpt/core/run_env/dev.env
--rw-r--r--   0        0        0       32 2024-03-19 04:02:01.715206 httpfpt-0.6.2/httpfpt/core/run_env/pro.env
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.716208 httpfpt-0.6.2/httpfpt/data/__init__.py
--rw-r--r--   0        0        0      400 2024-03-20 09:52:18.153003 httpfpt-0.6.2/httpfpt/data/global_vars.yaml
--rw-r--r--   0        0        0      461 2024-03-19 04:02:01.716208 httpfpt-0.6.2/httpfpt/data/hooks.py
--rw-r--r--   0        0        0     3704 2024-03-19 04:02:01.717208 httpfpt-0.6.2/httpfpt/data/test_data/test_project/api_testcase_template.yaml
--rw-r--r--   0        0        0     1202 2024-03-20 10:37:02.735034 httpfpt-0.6.2/httpfpt/data/test_data/test_project/only_skip.yml
--rw-r--r--   0        0        0      961 2024-03-19 04:02:01.717208 httpfpt-0.6.2/httpfpt/data/test_data/test_project/upload_file.json
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.717208 httpfpt-0.6.2/httpfpt/db/__init__.py
--rw-r--r--   0        0        0     5475 2024-03-19 04:02:01.718209 httpfpt-0.6.2/httpfpt/db/mysql_db.py
--rw-r--r--   0        0        0     2883 2024-03-19 04:02:01.718209 httpfpt-0.6.2/httpfpt/db/redis_db.py
--rw-r--r--   0        0        0      209 2024-03-19 04:02:01.718209 httpfpt-0.6.2/httpfpt/enums/__init__.py
--rw-r--r--   0        0        0      239 2024-03-19 04:02:01.719212 httpfpt-0.6.2/httpfpt/enums/allure_severity_type.py
--rw-r--r--   0        0        0      711 2024-03-19 04:02:01.719212 httpfpt-0.6.2/httpfpt/enums/assert_type.py
--rw-r--r--   0        0        0      173 2024-03-19 04:02:01.719212 httpfpt-0.6.2/httpfpt/enums/case_data_type.py
--rw-r--r--   0        0        0      146 2024-03-19 04:02:01.719212 httpfpt-0.6.2/httpfpt/enums/email_type.py
--rw-r--r--   0        0        0      154 2024-03-19 04:02:01.720208 httpfpt-0.6.2/httpfpt/enums/query_fetch_type.py
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.720208 httpfpt-0.6.2/httpfpt/enums/request/__init__.py
--rw-r--r--   0        0        0      214 2024-03-19 04:02:01.720208 httpfpt-0.6.2/httpfpt/enums/request/auth.py
--rw-r--r--   0        0        0      321 2024-03-19 04:02:01.720208 httpfpt-0.6.2/httpfpt/enums/request/body.py
--rw-r--r--   0        0        0      163 2024-03-19 04:02:01.720208 httpfpt-0.6.2/httpfpt/enums/request/engin.py
--rw-r--r--   0        0        0      249 2024-03-19 04:02:01.720208 httpfpt-0.6.2/httpfpt/enums/request/method.py
--rw-r--r--   0        0        0      207 2024-03-19 04:02:01.721212 httpfpt-0.6.2/httpfpt/enums/setup_type.py
--rw-r--r--   0        0        0      241 2024-03-19 04:02:01.721212 httpfpt-0.6.2/httpfpt/enums/sql_type.py
--rw-r--r--   0        0        0      231 2024-03-19 04:02:01.721212 httpfpt-0.6.2/httpfpt/enums/teardown_type.py
--rw-r--r--   0        0        0      210 2024-03-19 04:02:01.721212 httpfpt-0.6.2/httpfpt/enums/var_type.py
--rw-r--r--   0        0        0        0 2024-03-20 10:36:09.416602 httpfpt-0.6.2/httpfpt/py.typed
--rw-r--r--   0        0        0      981 2024-03-19 04:02:01.721212 httpfpt-0.6.2/httpfpt/pytest.ini
--rw-r--r--   0        0        0     8926 2024-03-20 10:37:02.736010 httpfpt-0.6.2/httpfpt/run.py
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.722224 httpfpt-0.6.2/httpfpt/schemas/__init__.py
--rw-r--r--   0        0        0     3840 2024-03-20 10:37:02.736010 httpfpt-0.6.2/httpfpt/schemas/case_data.py
--rw-r--r--   0        0        0     1031 2024-03-19 04:02:01.722224 httpfpt-0.6.2/httpfpt/templates/email_notification.html
--rw-r--r--   0        0        0     2548 2024-03-19 04:02:01.723206 httpfpt-0.6.2/httpfpt/templates/email_report.html
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.724207 httpfpt-0.6.2/httpfpt/utils/__init__.py
--rw-r--r--   0        0        0     1904 2024-03-19 04:02:01.724207 httpfpt-0.6.2/httpfpt/utils/allure_control.py
--rw-r--r--   0        0        0    20341 2024-03-19 04:02:01.725208 httpfpt-0.6.2/httpfpt/utils/assert_control.py
--rw-r--r--   0        0        0     4080 2024-03-19 04:02:01.725208 httpfpt-0.6.2/httpfpt/utils/auth_plugins.py
--rw-r--r--   0        0        0     4271 2024-03-20 10:37:02.737009 httpfpt-0.6.2/httpfpt/utils/case_auto_generator.py
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.726208 httpfpt-0.6.2/httpfpt/utils/cli/__init__.py
--rw-r--r--   0        0        0     3458 2024-03-19 04:02:01.726208 httpfpt-0.6.2/httpfpt/utils/cli/about_testcase.py
--rw-r--r--   0        0        0     2569 2024-03-19 04:02:01.726208 httpfpt-0.6.2/httpfpt/utils/cli/import_case_data.py
--rw-r--r--   0        0        0     3510 2024-03-20 10:36:09.417600 httpfpt-0.6.2/httpfpt/utils/cli/new_project.py
--rw-r--r--   0        0        0      511 2024-03-19 04:02:01.726208 httpfpt-0.6.2/httpfpt/utils/cli/version.py
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.726208 httpfpt-0.6.2/httpfpt/utils/data_manage/__init__.py
--rw-r--r--   0        0        0     6559 2024-03-19 04:02:01.727206 httpfpt-0.6.2/httpfpt/utils/data_manage/apifox.py
--rw-r--r--   0        0        0      731 2024-03-19 04:02:01.727206 httpfpt-0.6.2/httpfpt/utils/data_manage/base_format.py
--rw-r--r--   0        0        0     2641 2024-03-19 04:02:01.727206 httpfpt-0.6.2/httpfpt/utils/data_manage/git_repo.py
--rw-r--r--   0        0        0      106 2024-03-19 04:02:01.727206 httpfpt-0.6.2/httpfpt/utils/data_manage/har.py
--rw-r--r--   0        0        0      109 2024-03-19 04:02:01.727206 httpfpt-0.6.2/httpfpt/utils/data_manage/jmeter.py
--rw-r--r--   0        0        0    19137 2024-03-19 04:02:01.728207 httpfpt-0.6.2/httpfpt/utils/data_manage/openapi.py
--rw-r--r--   0        0        0      110 2024-03-19 04:02:01.728207 httpfpt-0.6.2/httpfpt/utils/data_manage/postman.py
--rw-r--r--   0        0        0      282 2024-03-19 04:02:01.728207 httpfpt-0.6.2/httpfpt/utils/enum_control.py
--rw-r--r--   0        0        0     1823 2024-03-19 04:02:01.728207 httpfpt-0.6.2/httpfpt/utils/file_control.py
--rw-r--r--   0        0        0      382 2024-03-19 04:02:01.728207 httpfpt-0.6.2/httpfpt/utils/pydantic_parser.py
--rw-r--r--   0        0        0    10113 2024-03-19 04:02:01.729206 httpfpt-0.6.2/httpfpt/utils/relate_testcase_executor.py
--rw-r--r--   0        0        0       49 2024-03-19 04:02:01.729206 httpfpt-0.6.2/httpfpt/utils/request/__init__.py
--rw-r--r--   0        0        0     7759 2024-03-20 10:37:02.737009 httpfpt-0.6.2/httpfpt/utils/request/case_data_parse.py
--rw-r--r--   0        0        0     3796 2024-03-19 04:02:01.729206 httpfpt-0.6.2/httpfpt/utils/request/hook_executor.py
--rw-r--r--   0        0        0      980 2024-03-20 10:37:02.737009 httpfpt-0.6.2/httpfpt/utils/request/ids_extract.py
--rw-r--r--   0        0        0    35232 2024-03-20 10:37:02.738010 httpfpt-0.6.2/httpfpt/utils/request/request_data_parse.py
--rw-r--r--   0        0        0     5709 2024-03-19 04:02:01.730208 httpfpt-0.6.2/httpfpt/utils/request/vars_extractor.py
--rw-r--r--   0        0        0     1236 2024-03-19 04:02:01.731207 httpfpt-0.6.2/httpfpt/utils/request/vars_recorder.py
--rw-r--r--   0        0        0      106 2024-03-19 04:02:01.731207 httpfpt-0.6.2/httpfpt/utils/rich_console.py
--rw-r--r--   0        0        0        0 2024-03-19 04:02:01.731207 httpfpt-0.6.2/httpfpt/utils/send_report/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-19 04:02:01.731207 httpfpt-0.6.2/httpfpt/utils/send_report/dingding.py
--rw-r--r--   0        0        0     3702 2024-03-20 10:36:09.417600 httpfpt-0.6.2/httpfpt/utils/send_report/email.py
--rw-r--r--   0        0        0     2250 2024-03-19 04:02:01.732206 httpfpt-0.6.2/httpfpt/utils/send_report/feishu.py
--rw-r--r--   0        0        0     1818 2024-03-19 04:02:01.732206 httpfpt-0.6.2/httpfpt/utils/send_report/wechat.py
--rw-r--r--   0        0        0      398 2024-03-19 04:02:01.732206 httpfpt-0.6.2/httpfpt/utils/time_control.py
--rw-r--r--   0        0        0     2067 2024-03-20 10:56:23.476297 httpfpt-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 httpfpt-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-28 08:25:55.678626 httpfpt-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3827 2024-04-13 05:35:32.869033 httpfpt-0.6.3/README.md
+-rw-r--r--   0        0        0       71 2024-04-13 05:32:13.201290 httpfpt-0.6.3/httpfpt/__init__.py
+-rw-r--r--   0        0        0     4691 2024-04-13 05:35:32.869738 httpfpt-0.6.3/httpfpt/cli.py
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.679366 httpfpt-0.6.3/httpfpt/common/__init__.py
+-rw-r--r--   0        0        0      925 2024-03-28 08:25:55.679559 httpfpt-0.6.3/httpfpt/common/env_handler.py
+-rw-r--r--   0        0        0     1814 2024-03-28 08:25:55.679794 httpfpt-0.6.3/httpfpt/common/errors.py
+-rw-r--r--   0        0        0     1407 2024-03-28 08:25:55.680005 httpfpt-0.6.3/httpfpt/common/excel_handler.py
+-rw-r--r--   0        0        0     1848 2024-03-28 08:25:55.680173 httpfpt-0.6.3/httpfpt/common/json_handler.py
+-rw-r--r--   0        0        0     1592 2024-03-28 08:25:55.680698 httpfpt-0.6.3/httpfpt/common/log.py
+-rw-r--r--   0        0        0    17833 2024-04-13 05:32:13.202285 httpfpt-0.6.3/httpfpt/common/send_request.py
+-rw-r--r--   0        0        0     1498 2024-03-28 08:25:55.681156 httpfpt-0.6.3/httpfpt/common/toml_handler.py
+-rw-r--r--   0        0        0     2144 2024-03-28 08:25:55.681696 httpfpt-0.6.3/httpfpt/common/variable_cache.py
+-rw-r--r--   0        0        0     3329 2024-03-28 08:25:55.682112 httpfpt-0.6.3/httpfpt/common/yaml_handler.py
+-rw-r--r--   0        0        0     4418 2024-03-28 08:25:55.682307 httpfpt-0.6.3/httpfpt/conftest.py
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.682725 httpfpt-0.6.3/httpfpt/core/__init__.py
+-rw-r--r--   0        0        0       39 2024-03-28 08:25:55.682920 httpfpt-0.6.3/httpfpt/core/allure_env/environment.properties
+-rw-r--r--   0        0        0      962 2024-03-28 08:25:55.683242 httpfpt-0.6.3/httpfpt/core/auth.yaml
+-rw-r--r--   0        0        0      898 2024-03-28 08:25:55.683370 httpfpt-0.6.3/httpfpt/core/conf.toml
+-rw-r--r--   0        0        0     5044 2024-04-13 05:35:32.870402 httpfpt-0.6.3/httpfpt/core/get_conf.py
+-rw-r--r--   0        0        0     3428 2024-04-13 05:35:32.870869 httpfpt-0.6.3/httpfpt/core/path_conf.py
+-rw-r--r--   0        0        0       57 2024-03-28 08:25:55.684204 httpfpt-0.6.3/httpfpt/core/run_env/dev.env
+-rw-r--r--   0        0        0       31 2024-03-28 08:25:55.684331 httpfpt-0.6.3/httpfpt/core/run_env/pro.env
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.684640 httpfpt-0.6.3/httpfpt/data/__init__.py
+-rw-r--r--   0        0        0      386 2024-03-28 08:25:55.684797 httpfpt-0.6.3/httpfpt/data/global_vars.yaml
+-rw-r--r--   0        0        0      435 2024-03-28 08:25:55.684925 httpfpt-0.6.3/httpfpt/data/hooks.py
+-rw-r--r--   0        0        0     3544 2024-03-28 08:25:55.685383 httpfpt-0.6.3/httpfpt/data/test_data/test_project/api_testcase_template.yaml
+-rw-r--r--   0        0        0     1143 2024-03-28 08:25:55.685589 httpfpt-0.6.3/httpfpt/data/test_data/test_project/only_skip.yml
+-rw-r--r--   0        0        0      917 2024-03-28 08:25:55.686034 httpfpt-0.6.3/httpfpt/data/test_data/test_project/upload_file.json
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.686507 httpfpt-0.6.3/httpfpt/db/__init__.py
+-rw-r--r--   0        0        0     5449 2024-04-13 05:32:13.203301 httpfpt-0.6.3/httpfpt/db/mysql_db.py
+-rw-r--r--   0        0        0     2785 2024-03-28 08:25:55.686937 httpfpt-0.6.3/httpfpt/db/redis_db.py
+-rw-r--r--   0        0        0      194 2024-03-28 08:25:55.687181 httpfpt-0.6.3/httpfpt/enums/__init__.py
+-rw-r--r--   0        0        0      228 2024-03-28 08:25:55.687448 httpfpt-0.6.3/httpfpt/enums/allure_severity_type.py
+-rw-r--r--   0        0        0      685 2024-03-28 08:25:55.687730 httpfpt-0.6.3/httpfpt/enums/assert_type.py
+-rw-r--r--   0        0        0      164 2024-03-28 08:25:55.688166 httpfpt-0.6.3/httpfpt/enums/case_data_type.py
+-rw-r--r--   0        0        0      138 2024-03-28 08:25:55.688354 httpfpt-0.6.3/httpfpt/enums/email_type.py
+-rw-r--r--   0        0        0      146 2024-03-28 08:25:55.688802 httpfpt-0.6.3/httpfpt/enums/query_fetch_type.py
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.689082 httpfpt-0.6.3/httpfpt/enums/request/__init__.py
+-rw-r--r--   0        0        0      205 2024-03-28 08:25:55.689262 httpfpt-0.6.3/httpfpt/enums/request/auth.py
+-rw-r--r--   0        0        0      306 2024-03-28 08:25:55.689440 httpfpt-0.6.3/httpfpt/enums/request/body.py
+-rw-r--r--   0        0        0      155 2024-03-28 08:25:55.689681 httpfpt-0.6.3/httpfpt/enums/request/engin.py
+-rw-r--r--   0        0        0      235 2024-03-28 08:25:55.689858 httpfpt-0.6.3/httpfpt/enums/request/method.py
+-rw-r--r--   0        0        0      197 2024-03-28 08:25:55.690037 httpfpt-0.6.3/httpfpt/enums/setup_type.py
+-rw-r--r--   0        0        0      228 2024-03-28 08:25:55.690206 httpfpt-0.6.3/httpfpt/enums/sql_type.py
+-rw-r--r--   0        0        0      220 2024-03-28 08:25:55.690359 httpfpt-0.6.3/httpfpt/enums/teardown_type.py
+-rw-r--r--   0        0        0      198 2024-03-28 08:25:55.690507 httpfpt-0.6.3/httpfpt/enums/var_type.py
+-rw-r--r--   0        0        0        0 2024-04-13 05:35:32.871003 httpfpt-0.6.3/httpfpt/py.typed
+-rw-r--r--   0        0        0      953 2024-03-28 08:25:55.690688 httpfpt-0.6.3/httpfpt/pytest.ini
+-rw-r--r--   0        0        0     8686 2024-04-13 05:35:32.871696 httpfpt-0.6.3/httpfpt/run.py
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.691182 httpfpt-0.6.3/httpfpt/schemas/__init__.py
+-rw-r--r--   0        0        0     3831 2024-04-13 05:32:13.204061 httpfpt-0.6.3/httpfpt/schemas/case_data.py
+-rw-r--r--   0        0        0      998 2024-03-28 08:25:55.691644 httpfpt-0.6.3/httpfpt/templates/email_notification.html
+-rw-r--r--   0        0        0     2475 2024-03-28 08:25:55.691819 httpfpt-0.6.3/httpfpt/templates/email_report.html
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.693256 httpfpt-0.6.3/httpfpt/utils/__init__.py
+-rw-r--r--   0        0        0     1832 2024-03-28 08:25:55.693472 httpfpt-0.6.3/httpfpt/utils/allure_control.py
+-rw-r--r--   0        0        0    19972 2024-04-13 05:32:13.205029 httpfpt-0.6.3/httpfpt/utils/assert_control.py
+-rw-r--r--   0        0        0     3980 2024-03-28 08:25:55.694573 httpfpt-0.6.3/httpfpt/utils/auth_plugins.py
+-rw-r--r--   0        0        0     4166 2024-03-28 08:25:55.694808 httpfpt-0.6.3/httpfpt/utils/case_auto_generator.py
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.695138 httpfpt-0.6.3/httpfpt/utils/cli/__init__.py
+-rw-r--r--   0        0        0     3375 2024-03-28 08:25:55.695478 httpfpt-0.6.3/httpfpt/utils/cli/about_testcase.py
+-rw-r--r--   0        0        0     2502 2024-03-28 08:25:55.696079 httpfpt-0.6.3/httpfpt/utils/cli/import_case_data.py
+-rw-r--r--   0        0        0     3415 2024-04-13 05:35:32.872947 httpfpt-0.6.3/httpfpt/utils/cli/new_project.py
+-rw-r--r--   0        0        0      492 2024-03-28 08:25:55.696532 httpfpt-0.6.3/httpfpt/utils/cli/version.py
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.696846 httpfpt-0.6.3/httpfpt/utils/data_manage/__init__.py
+-rw-r--r--   0        0        0     6381 2024-03-28 08:25:55.697089 httpfpt-0.6.3/httpfpt/utils/data_manage/apifox.py
+-rw-r--r--   0        0        0      702 2024-03-28 08:25:55.697259 httpfpt-0.6.3/httpfpt/utils/data_manage/base_format.py
+-rw-r--r--   0        0        0     2577 2024-03-28 08:25:55.697445 httpfpt-0.6.3/httpfpt/utils/data_manage/git_repo.py
+-rw-r--r--   0        0        0       99 2024-03-28 08:25:55.697640 httpfpt-0.6.3/httpfpt/utils/data_manage/har.py
+-rw-r--r--   0        0        0      102 2024-03-28 08:25:55.697827 httpfpt-0.6.3/httpfpt/utils/data_manage/jmeter.py
+-rw-r--r--   0        0        0    18727 2024-03-28 08:25:55.698062 httpfpt-0.6.3/httpfpt/utils/data_manage/openapi.py
+-rw-r--r--   0        0        0      103 2024-03-28 08:25:55.698281 httpfpt-0.6.3/httpfpt/utils/data_manage/postman.py
+-rw-r--r--   0        0        0      270 2024-03-28 08:25:55.698446 httpfpt-0.6.3/httpfpt/utils/enum_control.py
+-rw-r--r--   0        0        0     1754 2024-03-28 08:25:55.698904 httpfpt-0.6.3/httpfpt/utils/file_control.py
+-rw-r--r--   0        0        0      364 2024-03-28 08:25:55.699228 httpfpt-0.6.3/httpfpt/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     9886 2024-03-28 08:25:55.699635 httpfpt-0.6.3/httpfpt/utils/relate_testcase_executor.py
+-rw-r--r--   0        0        0       47 2024-03-28 08:25:55.700008 httpfpt-0.6.3/httpfpt/utils/request/__init__.py
+-rw-r--r--   0        0        0     7570 2024-03-28 08:25:55.700274 httpfpt-0.6.3/httpfpt/utils/request/case_data_parse.py
+-rw-r--r--   0        0        0     3683 2024-03-28 08:25:55.700633 httpfpt-0.6.3/httpfpt/utils/request/hook_executor.py
+-rw-r--r--   0        0        0      952 2024-03-28 08:25:55.700855 httpfpt-0.6.3/httpfpt/utils/request/ids_extract.py
+-rw-r--r--   0        0        0    34270 2024-04-13 05:32:13.206154 httpfpt-0.6.3/httpfpt/utils/request/request_data_parse.py
+-rw-r--r--   0        0        0     5568 2024-03-28 08:25:55.701597 httpfpt-0.6.3/httpfpt/utils/request/vars_extractor.py
+-rw-r--r--   0        0        0     1201 2024-03-28 08:25:55.701910 httpfpt-0.6.3/httpfpt/utils/request/vars_recorder.py
+-rw-r--r--   0        0        0      101 2024-03-28 08:25:55.702144 httpfpt-0.6.3/httpfpt/utils/rich_console.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:25:55.702356 httpfpt-0.6.3/httpfpt/utils/send_report/__init__.py
+-rw-r--r--   0        0        0     1769 2024-03-28 08:25:55.702674 httpfpt-0.6.3/httpfpt/utils/send_report/dingding.py
+-rw-r--r--   0        0        0     3597 2024-04-13 05:35:32.894997 httpfpt-0.6.3/httpfpt/utils/send_report/email.py
+-rw-r--r--   0        0        0     2202 2024-03-28 08:25:55.703055 httpfpt-0.6.3/httpfpt/utils/send_report/feishu.py
+-rw-r--r--   0        0        0     1776 2024-03-28 08:25:55.703232 httpfpt-0.6.3/httpfpt/utils/send_report/wechat.py
+-rw-r--r--   0        0        0      380 2024-03-28 08:25:55.703412 httpfpt-0.6.3/httpfpt/utils/time_control.py
+-rw-r--r--   0        0        0     2067 2024-04-13 05:43:04.332148 httpfpt-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5666 1970-01-01 00:00:00.000000 httpfpt-0.6.3/PKG-INFO
```

### Comparing `httpfpt-0.6.2/README.md` & `httpfpt-0.6.3/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# HttpFpt
-
-![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/wu-clan/httpfpt/ci.yml?logo=github)
-[![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
-[![GitHub](https://img.shields.io/github/license/wu-clan/httpfpt)](https://github.com/wu-clan/httpfpt/blob/master/LICENSE)
-![Static Badge](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
-![GitHub release (with filter)](https://img.shields.io/github/v/release/wu-clan/httpfpt)
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-
-> [!IMPORTANT]  
-> 当前分支为 SDK 版本，如需修改源码进行功能定制，建议切换到 [master](https://github.com/wu-clan/httpfpt) 分支
-
-基于 HTTP 请求的快速数据驱动 pytest 接口自动化测试框架
-
-我在掘金发表了关于 `HttpFpt` 的前身和由来，包括部分功能点的说明， 感兴趣
-
-的小伙伴可以一睹为快，[点击跳转](https://juejin.cn/post/7224314619867136037)
-
-## 功能点
-
-- 多项目分级，自由切换，互不干扰
-- 测试数据隔离，自动解析与验证
-- 测试数据错误定位（参数错误，重复测试用例ID...）
-- 多环境自定义配置，不同用例可以选择不同的运行环境
-- 动态环境配置，自动识别和应用当前请求所需的基础环境配置
-- 动态参数化，可通过全局变量，局部变量，缓存变量，关联变量等方式进行参数化
-- 数据依赖，支持接口返回数据共享，轻松实现接口依赖
-- 钩子函数，支持调用自定义钩子函数，实现更多的自定义功能
-- 日志记录，自动记录测试过程中的请求数据日志
-- 多元化断言，json 断言，sql 断言，json-schema 断言，正则断言，原生 python assert 断言
-- 兼容 yaml / json 两种文件格式编写测试数据
-- 测试用例自动生成，可以根据测试数据文件自动生成测试用例
-- 自动测试报告，html, allure
-- 自动测试结果通知，飞书，钉钉，企业微信，邮箱
-- ......
-
-## 流程图
-
-![httpfpt_flowchart](https://github.com/wu-clan/image/blob/master/httpfpt_flowchart.png?raw=true)
-
-## ⬇️ 下载
-
-```shell
-pip install httpfpt
-```
-
-## 🧑‍💻 Use
-
-1. 安装 redis 数据库并启动服务
-
-   [Redis Windows](https://github.com/redis-windows/redis-windows)
-
-   [Linux / macOS](https://redis.io/download/)
-
-   [Docker](https://hub.docker.com/_/redis)
-
-2. 安装 mysql 数据库（可选，如果你需要本地数据库）
-
-   [Windows / Linux / macOS](https://dev.mysql.com/downloads/installer/)
-
-   [Docker](https://hub.docker.com/_/mysql)
-
-> [!WARNING]
-> allure 测试报告默认使用 allure-pytest 生成，但是不能直接访问，有以下选择
-> 1. 本地访问：你必须安装 [allure](https://www.yuque.com/poloyy/python/aiqlmi)
-     程序和 [Java JDK](https://adoptopenjdk.net/archive.html?variant=openjdk8&jvmVariant=hotspot) 才能进行本地可视化浏览
-> 2. Jenkins（文档内包含集成教程）: 将 allure 测试报告集成到到 Jenkins 中，通过 Jenkins 进行浏览
-
-## 帮助
-
-有关更多详细信息，请参阅 [文档](https://wu-clan.github.io/httpfpt_docs)
-
-## 互动
-
-[WeChat / QQ](https://github.com/wu-clan)
-
-## 状态
-
-![Alt](https://repobeats.axiom.co/api/embed/98343c7bb6875c60a529fff021611eceecb296f1.svg "Repo beats analytics image")
-
-## 赞助
-
-如果此项目能够帮助到你，你可以赞助作者一些咖啡豆表示鼓励：[:coffee: Sponsor :coffee:](https://wu-clan.github.io/sponsor/)
-
-[![Stargazers over time](https://starchart.cc/wu-clan/httpfpt.svg?variant=adaptive)](https://starchart.cc/wu-clan/httpfpt)
+# HttpFpt
+
+![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/wu-clan/httpfpt/ci.yml?logo=github)
+[![Checked with pyright](https://microsoft.github.io/pyright/img/pyright_badge.svg)](https://microsoft.github.io/pyright/)
+[![GitHub](https://img.shields.io/github/license/wu-clan/httpfpt)](https://github.com/wu-clan/httpfpt/blob/master/LICENSE)
+![Static Badge](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue)
+![GitHub release (with filter)](https://img.shields.io/github/v/release/wu-clan/httpfpt)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+
+> [!IMPORTANT]  
+> 当前分支为 SDK 版本，如需修改源码进行功能定制，建议切换到 [master](https://github.com/wu-clan/httpfpt) 分支
+
+基于 HTTP 请求的快速数据驱动 pytest 接口自动化测试框架
+
+我在掘金发表了关于 `HttpFpt` 的前身和由来，包括部分功能点的说明， 感兴趣
+
+的小伙伴可以一睹为快，[点击跳转](https://juejin.cn/post/7224314619867136037)
+
+## 功能点
+
+- 多项目分级，自由切换，互不干扰
+- 测试数据隔离，自动解析与验证
+- 测试数据错误定位（参数错误，重复测试用例ID...）
+- 多环境自定义配置，不同用例可以选择不同的运行环境
+- 动态环境配置，自动识别和应用当前请求所需的基础环境配置
+- 动态参数化，可通过全局变量，局部变量，缓存变量，关联变量等方式进行参数化
+- 数据依赖，支持接口返回数据共享，轻松实现接口依赖
+- 钩子函数，支持调用自定义钩子函数，实现更多的自定义功能
+- 日志记录，自动记录测试过程中的请求数据日志
+- 多元化断言，json 断言，sql 断言，json-schema 断言，正则断言，原生 python assert 断言
+- 兼容 yaml / json 两种文件格式编写测试数据
+- 测试用例自动生成，可以根据测试数据文件自动生成测试用例
+- 自动测试报告，html, allure
+- 自动测试结果通知，飞书，钉钉，企业微信，邮箱
+- ......
+
+## 流程图
+
+![httpfpt_flowchart](https://github.com/wu-clan/image/blob/master/httpfpt_flowchart.png?raw=true)
+
+## ⬇️ 下载
+
+```shell
+pip install httpfpt
+```
+
+## 🧑‍💻 Use
+
+1. 安装 redis 数据库并启动服务
+
+   [Redis Windows](https://github.com/redis-windows/redis-windows)
+
+   [Linux / macOS](https://redis.io/download/)
+
+   [Docker](https://hub.docker.com/_/redis)
+
+2. 安装 mysql 数据库（可选，如果你需要本地数据库）
+
+   [Windows / Linux / macOS](https://dev.mysql.com/downloads/installer/)
+
+   [Docker](https://hub.docker.com/_/mysql)
+
+> [!WARNING]
+> allure 测试报告默认使用 allure-pytest 生成，但是不能直接访问，有以下选择
+> 1. 本地访问：你必须安装 [allure](https://www.yuque.com/poloyy/python/aiqlmi)
+     程序和 [Java JDK](https://adoptopenjdk.net/archive.html?variant=openjdk8&jvmVariant=hotspot) 才能进行本地可视化浏览
+> 2. Jenkins（文档内包含集成教程）: 将 allure 测试报告集成到到 Jenkins 中，通过 Jenkins 进行浏览
+
+## 帮助
+
+有关更多详细信息，请参阅 [文档](https://wu-clan.github.io/httpfpt_docs)
+
+## 互动
+
+[WeChat / QQ](https://github.com/wu-clan)
+
+## 状态
+
+![Alt](https://repobeats.axiom.co/api/embed/98343c7bb6875c60a529fff021611eceecb296f1.svg "Repo beats analytics image")
+
+## 赞助
+
+如果此项目能够帮助到你，你可以赞助作者一些咖啡豆表示鼓励：[:coffee: Sponsor :coffee:](https://wu-clan.github.io/sponsor/)
+
+[![Stargazers over time](https://starchart.cc/wu-clan/httpfpt.svg?variant=adaptive)](https://starchart.cc/wu-clan/httpfpt)
```

### Comparing `httpfpt-0.6.2/httpfpt/cli.py` & `httpfpt-0.6.3/httpfpt/cli.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-from dataclasses import dataclass
-
-import cappa
-
-from cappa import Subcommands
-from typing_extensions import Annotated
-
-from httpfpt.utils.cli.new_project import create_new_project
-from httpfpt.utils.cli.version import get_version
-
-
-@cappa.command(name='httpfpt-cli')
-@dataclass
-class HttpFptCLI:
-    version: Annotated[
-        bool,
-        cappa.Arg(
-            short='-V',
-            long=True,
-            default=False,
-            help='Print version information.',
-        ),
-    ]
-    start_project: Annotated[
-        bool,
-        cappa.Arg(
-            value_name='<PROJECT NAME, PROJECT PATH>',
-            long='--startproject',
-            default=False,
-            help='Create a new project.',
-            required=False,
-        ),
-    ]
-    subcmd: Subcommands[TestCaseCLI | ImportCLI | None] = None
-
-    def __call__(self) -> None:
-        if self.version:
-            get_version()
-        if self.start_project:
-            create_new_project()
-
-
-@cappa.command(name='testcase', help='Test case tools.')
-@dataclass
-class TestCaseCLI:
-    data_verify: Annotated[
-        str,
-        cappa.Arg(
-            value_name='<FILENAME / ALL>',
-            short='-c',
-            long=True,
-            default='',
-            help='验证测试数据结构；当指定文件（文件名/绝对路径）时, 仅验证指定文件, 当指定 "all" 时, 验证所有文件.',
-            required=False,
-        ),
-    ]
-    generate: Annotated[
-        bool,
-        cappa.Arg(
-            short='-g',
-            long=True,
-            default=False,
-            help='自动生成测试用例.',
-            required=False,
-        ),
-    ]
-
-    def __call__(self) -> None:
-        from httpfpt.utils.cli.about_testcase import generate_testcases, testcase_data_verify
-
-        if self.data_verify:
-            testcase_data_verify(self.data_verify)
-        if self.generate:
-            generate_testcases()
-
-
-@cappa.command(name='import', help='Import testcase data.')
-@dataclass
-class ImportCLI:
-    openai: Annotated[
-        tuple[str, str],
-        cappa.Arg(
-            value_name='<JSONFILE / URL> <PROJECT>',
-            short='-o',
-            long='--import-openapi',
-            default=(),
-            help='导入 openapi 数据到 yaml 数据文件; 支持 json 文件 / url 导入, 需要指定 project 项目名.',
-            required=False,
-        ),
-    ]
-    apifox: Annotated[
-        tuple[str, str],
-        cappa.Arg(
-            value_name='<JSONFILE> <PROJECT>',
-            short='-a',
-            long='--import-apifox',
-            default=(),
-            help='Beta: 导入 apifox 数据到 yaml 数据文件; 支持 json 文件导入, 需要指定 project 项目名.',
-            required=False,
-        ),
-    ]
-    har: Annotated[
-        tuple[str, str],
-        cappa.Arg(
-            short='-h',
-            long='--import-har',
-            default=(),
-            help='TODO: Not started yet.',
-            required=False,
-        ),
-    ]
-    jmeter: Annotated[
-        tuple[str, str],
-        cappa.Arg(
-            short='-j',
-            long='--import-jmeter',
-            default=(),
-            help='TODO: Not started yet.',
-            required=False,
-        ),
-    ]
-    postman: Annotated[
-        tuple[str, str],
-        cappa.Arg(
-            short='-p',
-            long='--import-postman',
-            default=(),
-            help='TODO: Not started yet.',
-            required=False,
-        ),
-    ]
-    git: Annotated[
-        str,
-        cappa.Arg(
-            value_name='<GIT HTTPS>',
-            long='--import-git',
-            default='',
-            help='导入 git 仓库测试数据到本地.',
-            required=False,
-        ),
-    ]
-
-    def __call__(self) -> None:
-        from httpfpt.utils.cli.import_case_data import (
-            import_apifox_case_data,
-            import_git_case_data,
-            import_har_case_data,
-            import_jmeter_case_data,
-            import_openapi_case_data,
-            import_postman_case_data,
-        )
-
-        if self.openai:
-            import_openapi_case_data(self.openai)
-        if self.apifox:
-            import_apifox_case_data(self.apifox)
-        if self.har:
-            import_har_case_data(self.har)
-        if self.jmeter:
-            import_jmeter_case_data(self.jmeter)
-        if self.postman:
-            import_postman_case_data(self.postman)
-        if self.git:
-            import_git_case_data(self.git)
-
-
-def cappa_invoke() -> None:
-    """cli 执行程序"""
-    cappa.invoke(HttpFptCLI)
-
-
-if __name__ == '__main__':
-    cappa_invoke()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from dataclasses import dataclass
+
+import cappa
+
+from cappa import Subcommands
+from typing_extensions import Annotated
+
+from httpfpt.utils.cli.new_project import create_new_project
+from httpfpt.utils.cli.version import get_version
+
+
+@cappa.command(name='httpfpt-cli')
+@dataclass
+class HttpFptCLI:
+    version: Annotated[
+        bool,
+        cappa.Arg(
+            short='-V',
+            long=True,
+            default=False,
+            help='Print version information.',
+        ),
+    ]
+    start_project: Annotated[
+        bool,
+        cappa.Arg(
+            value_name='<PROJECT NAME, PROJECT PATH>',
+            long='--startproject',
+            default=False,
+            help='Create a new project.',
+            required=False,
+        ),
+    ]
+    subcmd: Subcommands[TestCaseCLI | ImportCLI | None] = None
+
+    def __call__(self) -> None:
+        if self.version:
+            get_version()
+        if self.start_project:
+            create_new_project()
+
+
+@cappa.command(name='testcase', help='Test case tools.')
+@dataclass
+class TestCaseCLI:
+    data_verify: Annotated[
+        str,
+        cappa.Arg(
+            value_name='<FILENAME / ALL>',
+            short='-c',
+            long=True,
+            default='',
+            help='验证测试数据结构；当指定文件（文件名/绝对路径）时, 仅验证指定文件, 当指定 "all" 时, 验证所有文件.',
+            required=False,
+        ),
+    ]
+    generate: Annotated[
+        bool,
+        cappa.Arg(
+            short='-g',
+            long=True,
+            default=False,
+            help='自动生成测试用例.',
+            required=False,
+        ),
+    ]
+
+    def __call__(self) -> None:
+        from httpfpt.utils.cli.about_testcase import generate_testcases, testcase_data_verify
+
+        if self.data_verify:
+            testcase_data_verify(self.data_verify)
+        if self.generate:
+            generate_testcases()
+
+
+@cappa.command(name='import', help='Import testcase data.')
+@dataclass
+class ImportCLI:
+    openai: Annotated[
+        tuple[str, str],
+        cappa.Arg(
+            value_name='<JSONFILE / URL> <PROJECT>',
+            short='-o',
+            long='--import-openapi',
+            default=(),
+            help='导入 openapi 数据到 yaml 数据文件; 支持 json 文件 / url 导入, 需要指定 project 项目名.',
+            required=False,
+        ),
+    ]
+    apifox: Annotated[
+        tuple[str, str],
+        cappa.Arg(
+            value_name='<JSONFILE> <PROJECT>',
+            short='-a',
+            long='--import-apifox',
+            default=(),
+            help='Beta: 导入 apifox 数据到 yaml 数据文件; 支持 json 文件导入, 需要指定 project 项目名.',
+            required=False,
+        ),
+    ]
+    har: Annotated[
+        tuple[str, str],
+        cappa.Arg(
+            short='-h',
+            long='--import-har',
+            default=(),
+            help='TODO: Not started yet.',
+            required=False,
+        ),
+    ]
+    jmeter: Annotated[
+        tuple[str, str],
+        cappa.Arg(
+            short='-j',
+            long='--import-jmeter',
+            default=(),
+            help='TODO: Not started yet.',
+            required=False,
+        ),
+    ]
+    postman: Annotated[
+        tuple[str, str],
+        cappa.Arg(
+            short='-p',
+            long='--import-postman',
+            default=(),
+            help='TODO: Not started yet.',
+            required=False,
+        ),
+    ]
+    git: Annotated[
+        str,
+        cappa.Arg(
+            value_name='<GIT HTTPS>',
+            long='--import-git',
+            default='',
+            help='导入 git 仓库测试数据到本地.',
+            required=False,
+        ),
+    ]
+
+    def __call__(self) -> None:
+        from httpfpt.utils.cli.import_case_data import (
+            import_apifox_case_data,
+            import_git_case_data,
+            import_har_case_data,
+            import_jmeter_case_data,
+            import_openapi_case_data,
+            import_postman_case_data,
+        )
+
+        if self.openai:
+            import_openapi_case_data(self.openai)
+        if self.apifox:
+            import_apifox_case_data(self.apifox)
+        if self.har:
+            import_har_case_data(self.har)
+        if self.jmeter:
+            import_jmeter_case_data(self.jmeter)
+        if self.postman:
+            import_postman_case_data(self.postman)
+        if self.git:
+            import_git_case_data(self.git)
+
+
+def cappa_invoke() -> None:
+    """cli 执行程序"""
+    cappa.invoke(HttpFptCLI)
+
+
+if __name__ == '__main__':
+    cappa_invoke()
```

### Comparing `httpfpt-0.6.2/httpfpt/common/env_handler.py` & `httpfpt-0.6.3/httpfpt/common/env_handler.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import os
-
-import dotenv
-
-from httpfpt.common.log import log
-
-
-def get_env_dict(filepath: str) -> dict:
-    """
-    获取 env 字典信息
-
-    :param filepath:
-    :return:
-    """
-    dotenv.find_dotenv(filepath, raise_error_if_not_found=True)
-    env_dict = dict(dotenv.dotenv_values(filepath))
-    return env_dict
-
-
-def write_env_vars(filepath: str, filename: str, key: str, value: str) -> None:
-    """
-    写入 env 信息
-
-    :param filepath:
-    :param filename:
-    :param key:
-    :param value:
-    :return:
-    """
-    _file = os.path.join(filepath, filename)
-    key_upper = key.upper()
-    try:
-        dotenv.set_key(_file, key_upper, value)
-    except Exception as e:
-        log.error(f'写入 {filename} 环境变量 {key_upper}={value} 错误: {e}')
-        raise e
-    else:
-        log.info(f'写入环境变量成功: {filename} -> {key_upper}={value}')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+import os
+
+import dotenv
+
+from httpfpt.common.log import log
+
+
+def get_env_dict(filepath: str) -> dict:
+    """
+    获取 env 字典信息
+
+    :param filepath:
+    :return:
+    """
+    dotenv.find_dotenv(filepath, raise_error_if_not_found=True)
+    env_dict = dict(dotenv.dotenv_values(filepath))
+    return env_dict
+
+
+def write_env_vars(filepath: str, filename: str, key: str, value: str) -> None:
+    """
+    写入 env 信息
+
+    :param filepath:
+    :param filename:
+    :param key:
+    :param value:
+    :return:
+    """
+    _file = os.path.join(filepath, filename)
+    key_upper = key.upper()
+    try:
+        dotenv.set_key(_file, key_upper, value)
+    except Exception as e:
+        log.error(f'写入 {filename} 环境变量 {key_upper}={value} 错误: {e}')
+        raise e
+    else:
+        log.info(f'写入环境变量成功: {filename} -> {key_upper}={value}')
```

### Comparing `httpfpt-0.6.2/httpfpt/common/errors.py` & `httpfpt-0.6.3/httpfpt/common/errors.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-
-class HttpFptErrorMixin:
-    """HttpFpt错误基类"""
-
-    def __init__(self, msg: str) -> None:
-        self.msg = msg
-
-    def __str__(self) -> str:
-        return self.msg
-
-
-class ConfigInitError(HttpFptErrorMixin, RuntimeError):
-    """配置初始化错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class AuthError(HttpFptErrorMixin, ValueError):
-    """认证错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class RequestDataParseError(HttpFptErrorMixin, ValueError):
-    """请求数据解析错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class CorrelateTestCaseError(HttpFptErrorMixin, ValueError):
-    """关联测试用例错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class SendRequestError(HttpFptErrorMixin, RuntimeError):
-    """发送请求错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class JsonPathFindError(HttpFptErrorMixin, ValueError):
-    """JsonPath查找错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class VariableError(HttpFptErrorMixin, ValueError):
-    """变量错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class SQLSyntaxError(HttpFptErrorMixin, ValueError):
-    """SQL语法错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class AssertSyntaxError(HttpFptErrorMixin, ValueError):
-    """断言格式错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
-
-
-class AssertError(HttpFptErrorMixin, AssertionError):
-    """断言错误"""
-
-    def __init__(self, msg: str) -> None:
-        super().__init__(msg)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+
+class HttpFptErrorMixin:
+    """HttpFpt错误基类"""
+
+    def __init__(self, msg: str) -> None:
+        self.msg = msg
+
+    def __str__(self) -> str:
+        return self.msg
+
+
+class ConfigInitError(HttpFptErrorMixin, RuntimeError):
+    """配置初始化错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class AuthError(HttpFptErrorMixin, ValueError):
+    """认证错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class RequestDataParseError(HttpFptErrorMixin, ValueError):
+    """请求数据解析错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class CorrelateTestCaseError(HttpFptErrorMixin, ValueError):
+    """关联测试用例错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class SendRequestError(HttpFptErrorMixin, RuntimeError):
+    """发送请求错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class JsonPathFindError(HttpFptErrorMixin, ValueError):
+    """JsonPath查找错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class VariableError(HttpFptErrorMixin, ValueError):
+    """变量错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class SQLSyntaxError(HttpFptErrorMixin, ValueError):
+    """SQL语法错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class AssertSyntaxError(HttpFptErrorMixin, ValueError):
+    """断言格式错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
+
+
+class AssertError(HttpFptErrorMixin, AssertionError):
+    """断言错误"""
+
+    def __init__(self, msg: str) -> None:
+        super().__init__(msg)
```

### Comparing `httpfpt-0.6.2/httpfpt/common/excel_handler.py` & `httpfpt-0.6.3/httpfpt/common/excel_handler.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import os
-
-from typing import Any
-
-import xlrd
-
-from httpfpt.common.log import log
-
-
-def read_excel(filepath: str, *, filename: str, sheet: str) -> list[dict[str, Any | None] | None]:
-    """
-    读取 xlsx 文件
-
-    :param filepath: 文件路径
-    :param filename: 文件名
-    :param sheet: 工作表
-    :return:
-    """
-    file = os.path.join(filepath, filename)
-    data = xlrd.open_workbook(file)
-    table = data.sheet_by_name(sheet)
-    # 获取总行,列数
-    rows = table.nrows
-    cols = table.ncols  # noqa: F841
-    if rows > 1:
-        # 获取第一行内容, 通常为列说明
-        keys = table.row_values(0)
-        data_list = []
-        # 获取文档剩下所有内容
-        for col in range(1, rows):
-            values = table.row_values(col)
-            # key, value组合为字典
-            data = dict(zip(keys, values))
-            # 数据整理
-            for value in data:
-                # 替换空字符串为 None, 保证与 yaml 数据返回格式一致
-                if data[value] == '':
-                    data[value] = None
-            data_list.append(data)
-        return data_list
-    else:
-        log.warning(f'数据表格 {filename} 没有数据!')
-        raise ValueError(f'数据表格 {filename} 没有数据! 请检查数据文件内容是否正确!')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import os
+
+from typing import Any
+
+import xlrd
+
+from httpfpt.common.log import log
+
+
+def read_excel(filepath: str, *, filename: str, sheet: str) -> list[dict[str, Any | None] | None]:
+    """
+    读取 xlsx 文件
+
+    :param filepath: 文件路径
+    :param filename: 文件名
+    :param sheet: 工作表
+    :return:
+    """
+    file = os.path.join(filepath, filename)
+    data = xlrd.open_workbook(file)
+    table = data.sheet_by_name(sheet)
+    # 获取总行,列数
+    rows = table.nrows
+    cols = table.ncols  # noqa: F841
+    if rows > 1:
+        # 获取第一行内容, 通常为列说明
+        keys = table.row_values(0)
+        data_list = []
+        # 获取文档剩下所有内容
+        for col in range(1, rows):
+            values = table.row_values(col)
+            # key, value组合为字典
+            data = dict(zip(keys, values))
+            # 数据整理
+            for value in data:
+                # 替换空字符串为 None, 保证与 yaml 数据返回格式一致
+                if data[value] == '':
+                    data[value] = None
+            data_list.append(data)
+        return data_list
+    else:
+        log.warning(f'数据表格 {filename} 没有数据!')
+        raise ValueError(f'数据表格 {filename} 没有数据! 请检查数据文件内容是否正确!')
```

### Comparing `httpfpt-0.6.2/httpfpt/common/log.py` & `httpfpt-0.6.3/httpfpt/common/log.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import logging
-import os
-
-from typing import TYPE_CHECKING
-
-from loguru import logger
-
-from httpfpt.core.path_conf import httpfpt_path
-
-if TYPE_CHECKING:
-    import loguru
-
-
-class PropagateHandler(logging.Handler):
-    def emit(self, record) -> None:  # noqa: ANN001
-        logging.getLogger(record.name).handle(record)
-
-
-class Logger:
-    @staticmethod
-    def log() -> loguru.Logger:
-        """
-        日志记录器
-
-        :return:
-        """
-        log_path = httpfpt_path.log_dir
-
-        if not os.path.join(log_path):
-            os.makedirs(log_path)
-
-        log_file = os.path.join(log_path, 'httpfpt.log')
-
-        # 清除 logger 配置
-        logger.remove()
-
-        # 控制台输出，建议通过 pytest.ini 配置
-        # logger.add(
-        #     sys.stdout,
-        #     format='{time:YYYYMMDD HH:mm:ss.SSS} | <level>{level: <8}</level> | <level>{message}</level>',
-        # )
-
-        # 将 logging message 替换为 loguru message
-        logger.add(PropagateHandler(), format='<level>{message}</level>')
-
-        # 输出到文件
-        logger.add(
-            log_file,
-            format='<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | <level>{message}</level>',
-            level='DEBUG',
-            rotation='00:00',
-            retention='7 days',
-            encoding='utf8',
-            enqueue=True,
-            backtrace=True,
-            diagnose=False,
-            catch=True,
-        )
-
-        return logger
-
-
-log = Logger().log()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import logging
+import os
+
+from typing import TYPE_CHECKING
+
+from loguru import logger
+
+from httpfpt.core.path_conf import httpfpt_path
+
+if TYPE_CHECKING:
+    import loguru
+
+
+class PropagateHandler(logging.Handler):
+    def emit(self, record) -> None:  # noqa: ANN001
+        logging.getLogger(record.name).handle(record)
+
+
+class Logger:
+    @staticmethod
+    def log() -> loguru.Logger:
+        """
+        日志记录器
+
+        :return:
+        """
+        log_path = httpfpt_path.log_dir
+
+        if not os.path.join(log_path):
+            os.makedirs(log_path)
+
+        log_file = os.path.join(log_path, 'httpfpt.log')
+
+        # 清除 logger 配置
+        logger.remove()
+
+        # 控制台输出，建议通过 pytest.ini 配置
+        # logger.add(
+        #     sys.stdout,
+        #     format='{time:YYYYMMDD HH:mm:ss.SSS} | <level>{level: <8}</level> | <level>{message}</level>',
+        # )
+
+        # 将 logging message 替换为 loguru message
+        logger.add(PropagateHandler(), format='<level>{message}</level>')
+
+        # 输出到文件
+        logger.add(
+            log_file,
+            format='<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | <level>{message}</level>',
+            level='DEBUG',
+            rotation='00:00',
+            retention='7 days',
+            encoding='utf8',
+            enqueue=True,
+            backtrace=True,
+            diagnose=False,
+            catch=True,
+        )
+
+        return logger
+
+
+log = Logger().log()
```

### Comparing `httpfpt-0.6.2/httpfpt/common/send_request.py` & `httpfpt-0.6.3/httpfpt/common/send_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,404 +1,414 @@
-#!/usr/bin/env python
-# _*_ coding:utf-8 _*_
-import time
-
-from json import JSONDecodeError
-
-import allure
-import httpx
-import requests
-import stamina
-
-from _pytest.outcomes import Skipped
-from httpx import Response as HttpxResponse
-from requests import Response as RequestsResponse
-
-from httpfpt.common.errors import AssertError, SendRequestError
-from httpfpt.common.log import log
-from httpfpt.core.get_conf import httpfpt_config
-from httpfpt.db.mysql_db import mysql_client
-from httpfpt.enums.request.body import BodyType
-from httpfpt.enums.request.engin import EnginType
-from httpfpt.enums.setup_type import SetupType
-from httpfpt.enums.teardown_type import TeardownType
-from httpfpt.utils.allure_control import allure_attach_file, allure_step
-from httpfpt.utils.assert_control import asserter
-from httpfpt.utils.enum_control import get_enum_values
-from httpfpt.utils.relate_testcase_executor import exec_setup_testcase
-from httpfpt.utils.request.hook_executor import hook_executor
-from httpfpt.utils.request.request_data_parse import RequestDataParse
-from httpfpt.utils.request.vars_extractor import var_extractor
-from httpfpt.utils.time_control import get_current_time
-
-
-class SendRequests:
-    """发送请求"""
-
-    @property
-    def init_response_metadata(self) -> dict:
-        """
-        :return: 响应元数据
-        """
-        response_metadata = {
-            'url': None,
-            'status_code': 200,
-            'elapsed': 0,
-            'headers': None,
-            'cookies': None,
-            'json': None,
-            'content': None,
-            'text': None,
-            'stat': {
-                'execute_time': None,
-            },
-            'request': None,
-        }
-        return response_metadata
-
-    @staticmethod
-    def _requests_engin(**kwargs) -> RequestsResponse:
-        """
-        requests 引擎
-
-        :param kwargs:
-        :return:
-        """
-        kwargs['timeout'] = kwargs['timeout'] or httpfpt_config.REQUEST_TIMEOUT
-        kwargs['verify'] = kwargs['verify'] or httpfpt_config.REQUEST_VERIFY
-        kwargs['proxies'] = kwargs['proxies'] or httpfpt_config.REQUEST_PROXIES_REQUESTS
-        kwargs['allow_redirects'] = kwargs['allow_redirects'] or httpfpt_config.REQUEST_REDIRECTS
-        request_retry = kwargs['retry'] or httpfpt_config.REQUEST_RETRY
-        del kwargs['retry']
-        # 消除安全警告
-        requests.packages.urllib3.disable_warnings()  # type: ignore
-        log.info('开始发送请求...')
-        try:
-            for attempt in stamina.retry_context(on=requests.HTTPError, attempts=request_retry):
-                with attempt:
-                    if attempt.num > 1:
-                        log.warning('请求响应异常重试...')
-                    response = requests.session().request(**kwargs)
-                    response.raise_for_status()
-        except Exception as e:
-            log.error(f'发送 requests 请求响应异常: {e}')
-            raise SendRequestError(e.__str__())
-        else:
-            return response  # type: ignore
-
-    @staticmethod
-    def _httpx_engin(**kwargs) -> HttpxResponse:
-        """
-        httpx 引擎
-
-        :param kwargs:
-        :return:
-        """
-        kwargs['timeout'] = kwargs['timeout'] or httpfpt_config.REQUEST_TIMEOUT
-        verify = kwargs['verify'] or httpfpt_config.REQUEST_VERIFY
-        proxies = kwargs['proxies'] or httpfpt_config.REQUEST_PROXIES_HTTPX
-        redirects = kwargs['allow_redirects'] or httpfpt_config.REQUEST_REDIRECTS
-        request_retry = kwargs['retry'] or httpfpt_config.REQUEST_RETRY
-        del kwargs['verify']
-        del kwargs['proxies']
-        del kwargs['allow_redirects']
-        del kwargs['retry']
-        log.info('开始发送请求...')
-        try:
-            with httpx.Client(verify=verify, proxies=proxies, follow_redirects=redirects) as client:  # type: ignore
-                for attempt in stamina.retry_context(on=httpx.HTTPError, attempts=request_retry):
-                    with attempt:
-                        if attempt.num > 1:
-                            log.warning('请求响应异常重试...')
-                        response = client.request(**kwargs)
-                        response.raise_for_status()
-        except Exception as e:
-            log.error(f'发送 httpx 请求响应异常: {e}')
-            raise SendRequestError(e.__str__())
-        else:
-            return response  # type: ignore
-
-    def send_request(
-        self,
-        request_data: dict,
-        *,
-        request_engin: EnginType = EnginType.requests,
-        log_data: bool = True,
-        relate_log: bool = False,
-        **kwargs,
-    ) -> dict:
-        """
-        发送请求
-
-        :param request_data: 请求数据
-        :param request_engin: 请求引擎
-        :param log_data: 日志记录数据
-        :param relate_log: 关联测试用例
-        :return: response
-        """
-        if request_engin not in get_enum_values(EnginType):
-            raise SendRequestError('请求发起失败，请使用合法的请求引擎')
-
-        # 获取解析后的请求数据
-        log.info('开始解析用例数据...' if not relate_log else '开始解析关联用例数据...')
-        try:
-            request_data_parse = RequestDataParse(request_data, request_engin)
-            parsed_data = request_data_parse.get_request_data_parsed(relate_log)
-        except Skipped as e:
-            raise e
-        except Exception as e:
-            if not relate_log:
-                log.error(f'用例数据解析失败: {e}')
-            raise e
-        log.info('用例数据解析完成' if not relate_log else '关联用例数据解析完成')
-
-        # 记录请求前置数据; 此处数据中如果包含关联用例变量, 不会被替换为结果记录, 因为替换动作还未发生
-        setup = parsed_data['setup']
-        if log_data:
-            if setup:
-                self.log_request_setup(setup)
-
-        # 前置处理
-        if parsed_data['is_setup']:
-            log.info('开始处理请求前置...')
-            try:
-                for item in setup:
-                    for key, value in item.items():
-                        if value is not None:
-                            if key == SetupType.TESTCASE:
-                                relate_parsed_data = exec_setup_testcase(parsed_data, value)
-                                if relate_parsed_data:
-                                    parsed_data = relate_parsed_data
-                            elif key == SetupType.SQL:
-                                sql = var_extractor.vars_replace({'sql': value}, parsed_data['env'])['sql']
-                                mysql_client.exec_case_sql(sql, parsed_data['env'])
-                            elif key == SetupType.HOOK:
-                                hook_executor.exec_hook_func(value)
-                            elif key == SetupType.WAIT_TIME:
-                                time.sleep(value)
-                                log.info(f'执行请求前等待：{value} s')
-            except Exception as e:
-                log.error(f'请求前置处理异常: {e}')
-                raise e
-            log.info('请求前置处理完成')
-
-        # 日志记录请求数据
-        if log_data:
-            self.log_request_up(parsed_data)
-            self.allure_request_up(parsed_data)
-
-        # allure 记录动态数据
-        self.allure_dynamic_data(parsed_data)
-
-        # 整理请求参数
-        request_conf = {
-            'timeout': parsed_data['timeout'],
-            'verify': parsed_data['verify'],
-            'proxies': parsed_data['proxies'],
-            'allow_redirects': parsed_data['redirects'],
-            'retry': parsed_data['retry'],
-        }
-        request_data_parsed = {
-            'method': parsed_data['method'],
-            'url': parsed_data['url'],
-            'params': parsed_data['params'],
-            'headers': parsed_data['headers'],
-            'cookies': parsed_data['cookies'],
-            'body': parsed_data['body'],
-            'files': parsed_data['files'],
-        }
-        if parsed_data['body_type'] == BodyType.JSON or parsed_data['body_type'] == BodyType.GraphQL:
-            request_data_parsed.update({'json': request_data_parsed.pop('body')})
-        elif parsed_data['body_type'] == BodyType.binary:
-            if request_engin == EnginType.httpx:
-                request_data_parsed.update({'content': request_data_parsed.pop('body')})
-        else:
-            request_data_parsed.update({'data': request_data_parsed.pop('body')})
-        try:
-            request_data_parsed = var_extractor.vars_replace(request_data_parsed, parsed_data['env'])
-        except Exception as e:
-            log.error(e)
-            raise e
-
-        # 发送请求
-        response_data = self.init_response_metadata
-        response_data['stat']['execute_time'] = get_current_time()
-        if request_engin == EnginType.requests:
-            response = self._requests_engin(**request_conf, **request_data_parsed, **kwargs)
-        elif request_engin == EnginType.httpx:
-            response = self._httpx_engin(**request_conf, **request_data_parsed, **kwargs)
-        else:
-            raise SendRequestError('请求发起失败，请使用合法的请求引擎：requests / httpx')
-
-        # 记录响应数据
-        response_data['url'] = str(response.url)
-        response_data['status_code'] = int(response.status_code)
-        response_data['elapsed'] = response.elapsed.microseconds / 1000.0
-        response_data['headers'] = dict(response.headers)
-        response_data['cookies'] = dict(response.cookies)
-        try:
-            json_data = response.json()
-        except JSONDecodeError:
-            log.warning('响应数据解析失败，响应数据不是有效的 json 格式')
-            json_data = {}
-        response_data['json'] = json_data
-        response_data['content'] = response.content.decode('utf-8')
-        response_data['text'] = response.text
-        response_data['request'] = request_data_parsed
-
-        # 日志记录响应数据
-        teardown = parsed_data['teardown']
-        if log_data:
-            self.log_request_down(response_data)
-            self.allure_request_down(response_data)
-            if teardown:
-                self.log_request_teardown(teardown)
-
-        # 后置处理
-        if parsed_data['is_teardown']:
-            log.info('开始处理请求后置...')
-            try:
-                for item in teardown:
-                    for key, value in item.items():
-                        if value is not None:
-                            if key == TeardownType.SQL:
-                                sql = var_extractor.vars_replace({'sql': value}, parsed_data['env'])['sql']
-                                mysql_client.exec_case_sql(sql, parsed_data['env'])
-                            if key == TeardownType.HOOK:
-                                hook_executor.exec_hook_func(value)
-                            if key == TeardownType.EXTRACT:
-                                var_extractor.teardown_var_extract(response_data, value, parsed_data['env'])
-                            if key == TeardownType.ASSERT:
-                                assert_text = var_extractor.vars_replace(
-                                    target={'assert_text': value}, env=parsed_data['env']
-                                )['assert_text']
-                                asserter.exec_asserter(response_data, assert_text)
-                            elif key == TeardownType.WAIT_TIME:
-                                log.info(f'执行请求后等待：{value} s')
-                                time.sleep(value)
-            except AssertionError as e:
-                log.error(f'断言失败: {e}')
-                raise AssertError(f'断言失败: {e}')
-            except Exception as e:
-                log.error(f'请求后置处理异常: {e}')
-                raise e
-            log.info('请求后置处理完成')
-
-        return response_data
-
-    def log_request_setup(self, setup: list) -> None:
-        for item in setup:
-            for key, value in item.items():
-                if key == SetupType.TESTCASE:
-                    log.info(f'前置 setup_testcase: {value}')
-                    self.allure_request_setup({'setup_testcase': value})
-                elif key == SetupType.SQL:
-                    log.info(f'前置 setup_sql: {value}')
-                    self.allure_request_setup({'setup_sql': value})
-                elif key == SetupType.HOOK:
-                    log.info(f'前置 setup_hook: {value}')
-                    self.allure_request_setup({'setup_hook': value})
-                elif key == SetupType.WAIT_TIME:
-                    log.info(f'前置 setup_wait_time: {value}')
-                    self.allure_request_setup({'setup_wait_time': value})
-
-    @staticmethod
-    def log_request_up(parsed_data: dict) -> None:
-        log.info(f"用例 env: {parsed_data['env']}")
-        log.info(f"用例 module: {parsed_data['module']}")
-        log.info(f"用例 name: {parsed_data['name']}")
-        log.info(f"用例 description: {parsed_data['description']}")
-        log.info(f"请求 method: {parsed_data['method']}")
-        log.info(f"请求 url: {parsed_data['url']}")
-        log.info(f"请求 params: {parsed_data['params']}")
-        log.info(f"请求 headers: {parsed_data['headers']}")
-        log.info(f"请求 data_type：{parsed_data['body_type']}")
-        if parsed_data['body_type'] != BodyType.JSON:
-            log.info(f"请求 data：{parsed_data['body']}")
-        else:
-            log.info(f"请求 json: {parsed_data['body']}")
-        log.info(f"请求 files: {parsed_data['files_no_parse']}")
-
-    def log_request_teardown(self, teardown: list) -> None:
-        for item in teardown:
-            for key, value in item.items():
-                if key == TeardownType.SQL:
-                    log.info(f'后置 teardown_sql: {value}')
-                    self.allure_request_teardown({'teardown_sql': value})
-                elif key == TeardownType.HOOK:
-                    log.info(f'后置 teardown_hook: {value}')
-                    self.allure_request_teardown({'teardown_hook': value})
-                elif key == TeardownType.EXTRACT:
-                    log.info(f'后置 teardown_extract: {value}')
-                    self.allure_request_teardown({'teardown_extract': value})
-                elif key == TeardownType.ASSERT:
-                    log.info(f'后置 teardown_assert: {value}')
-                    self.allure_request_teardown({'teardown_assert': value})
-                elif key == TeardownType.WAIT_TIME:
-                    log.info(f'后置 teardown_wait_time: {value}')
-                    self.allure_request_teardown({'teardown_wait_time': value})
-
-    @staticmethod
-    def log_request_down(response_data: dict) -> None:
-        log.info(f"请求发送时间: {response_data['stat']['execute_time']}")
-        str_status_code = str(response_data['status_code'])
-        if str_status_code.startswith(('4', '5')):
-            log.error(f"响应状态码: {response_data['status_code']}")
-        else:
-            log.info(f"响应状态码: {response_data['status_code']}")
-        log.info(f"响应时间: {response_data['elapsed']} ms")
-
-    @staticmethod
-    def allure_request_setup(setup_log: dict) -> None:
-        allure_step('请求前置', setup_log)
-
-    @staticmethod
-    def allure_request_up(parsed_data: dict) -> None:
-        allure_step(
-            '请求数据',
-            {
-                'env': parsed_data['env'],
-                'module': parsed_data['module'],
-                'name': parsed_data['name'],
-                'case_id': parsed_data['case_id'],
-                'description': parsed_data['description'],
-                'method': parsed_data['method'],
-                'url': parsed_data['url'],
-                'params': parsed_data['params'],
-                'headers': parsed_data['headers'],
-                'data_type': parsed_data['body_type'],
-                'data': parsed_data['body'],
-                'files': parsed_data['files_no_parse'],
-            },
-        )
-
-    @staticmethod
-    def allure_request_teardown(teardown_log: dict) -> None:
-        allure_step('请求后置', teardown_log)
-
-    @staticmethod
-    def allure_request_down(response_data: dict) -> None:
-        allure_step(
-            '响应数据',
-            {
-                'status_code': response_data['status_code'],
-                'elapsed': response_data['elapsed'],
-            },
-        )
-
-    @staticmethod
-    def allure_dynamic_data(parsed_data: dict) -> None:
-        allure.dynamic.title(parsed_data['name'])
-        allure.dynamic.description(parsed_data['description'])
-        allure.dynamic.link(parsed_data['url'])
-        if parsed_data['allure_severity'] is not None:
-            allure.dynamic.severity(parsed_data['allure_severity'])
-        if parsed_data['files_no_parse'] is not None:
-            for v in parsed_data['files_no_parse'].values():
-                if isinstance(v, list):
-                    for path in v:
-                        allure_attach_file(path)
-                else:
-                    allure_attach_file(v)
-
-
-send_request = SendRequests()
+#!/usr/bin/env python
+# _*_ coding:utf-8 _*_
+import time
+
+from json import JSONDecodeError
+
+import allure
+import httpx
+import requests
+import stamina
+
+from _pytest.outcomes import Skipped
+from httpx import Response as HttpxResponse
+from requests import Response as RequestsResponse
+
+from httpfpt.common.errors import AssertError, SendRequestError
+from httpfpt.common.log import log
+from httpfpt.core.get_conf import httpfpt_config
+from httpfpt.db.mysql_db import mysql_client
+from httpfpt.enums.request.body import BodyType
+from httpfpt.enums.request.engin import EnginType
+from httpfpt.enums.setup_type import SetupType
+from httpfpt.enums.teardown_type import TeardownType
+from httpfpt.utils.allure_control import allure_attach_file, allure_step
+from httpfpt.utils.assert_control import asserter
+from httpfpt.utils.enum_control import get_enum_values
+from httpfpt.utils.relate_testcase_executor import exec_setup_testcase
+from httpfpt.utils.request.hook_executor import hook_executor
+from httpfpt.utils.request.request_data_parse import RequestDataParse
+from httpfpt.utils.request.vars_extractor import var_extractor
+from httpfpt.utils.time_control import get_current_time
+
+
+class SendRequests:
+    """发送请求"""
+
+    @property
+    def init_response_metadata(self) -> dict:
+        """
+        :return: 响应元数据
+        """
+        response_metadata = {
+            'url': None,
+            'status_code': 200,
+            'elapsed': 0,
+            'headers': None,
+            'cookies': None,
+            'json': None,
+            'content': None,
+            'text': None,
+            'stat': {
+                'execute_time': None,
+            },
+            'request': None,
+        }
+        return response_metadata
+
+    @staticmethod
+    def _requests_engin(**kwargs) -> RequestsResponse:
+        """
+        requests 引擎
+
+        :param kwargs:
+        :return:
+        """
+        kwargs['timeout'] = kwargs['timeout'] or httpfpt_config.REQUEST_TIMEOUT
+        kwargs['verify'] = kwargs['verify'] or httpfpt_config.REQUEST_VERIFY
+        kwargs['proxies'] = kwargs['proxies'] or httpfpt_config.REQUEST_PROXIES_REQUESTS
+        kwargs['allow_redirects'] = kwargs['allow_redirects'] or httpfpt_config.REQUEST_REDIRECTS
+        request_retry = kwargs['retry'] or httpfpt_config.REQUEST_RETRY
+        del kwargs['retry']
+        # 消除安全警告
+        requests.packages.urllib3.disable_warnings()  # type: ignore
+        log.info('开始发送请求...')
+        try:
+            for attempt in stamina.retry_context(on=requests.HTTPError, attempts=request_retry):
+                with attempt:
+                    if attempt.num > 1:
+                        log.warning('请求响应异常重试...')
+                    response = requests.session().request(**kwargs)
+                    response.raise_for_status()
+        except Exception as e:
+            log.error(f'发送 requests 请求响应异常: {e}')
+            raise SendRequestError(e.__str__())
+        else:
+            return response  # type: ignore
+
+    @staticmethod
+    def _httpx_engin(**kwargs) -> HttpxResponse:
+        """
+        httpx 引擎
+
+        :param kwargs:
+        :return:
+        """
+        kwargs['timeout'] = kwargs['timeout'] or httpfpt_config.REQUEST_TIMEOUT
+        verify = kwargs['verify'] or httpfpt_config.REQUEST_VERIFY
+        proxies = kwargs['proxies'] or httpfpt_config.REQUEST_PROXIES_HTTPX
+        redirects = kwargs['allow_redirects'] or httpfpt_config.REQUEST_REDIRECTS
+        request_retry = kwargs['retry'] or httpfpt_config.REQUEST_RETRY
+        del kwargs['verify']
+        del kwargs['proxies']
+        del kwargs['allow_redirects']
+        del kwargs['retry']
+        log.info('开始发送请求...')
+        try:
+            with httpx.Client(verify=verify, proxies=proxies, follow_redirects=redirects) as client:  # type: ignore
+                for attempt in stamina.retry_context(on=httpx.HTTPError, attempts=request_retry):
+                    with attempt:
+                        if attempt.num > 1:
+                            log.warning('请求响应异常重试...')
+                        response = client.request(**kwargs)
+                        response.raise_for_status()
+        except Exception as e:
+            log.error(f'发送 httpx 请求响应异常: {e}')
+            raise SendRequestError(e.__str__())
+        else:
+            return response  # type: ignore
+
+    def send_request(
+        self,
+        request_data: dict,
+        *,
+        request_engin: EnginType = EnginType.requests,
+        log_data: bool = True,
+        relate_log: bool = False,
+        **kwargs,
+    ) -> dict:
+        """
+        发送请求
+
+        :param request_data: 请求数据
+        :param request_engin: 请求引擎
+        :param log_data: 日志记录数据
+        :param relate_log: 关联测试用例
+        :return: response
+        """
+        if request_engin not in get_enum_values(EnginType):
+            raise SendRequestError('请求发起失败，请使用合法的请求引擎')
+
+        # 获取解析后的请求数据
+        log.info('开始解析用例数据...' if not relate_log else '开始解析关联用例数据...')
+        try:
+            request_data_parse = RequestDataParse(request_data, request_engin)
+            parsed_data = request_data_parse.get_request_data_parsed(relate_log)
+        except Skipped as e:
+            raise e
+        except Exception as e:
+            if not relate_log:
+                log.error(f'用例数据解析失败: {e}')
+            raise e
+        log.info('用例数据解析完成' if not relate_log else '关联用例数据解析完成')
+
+        # 记录请求前置数据; 此处数据中如果包含关联用例变量, 不会被替换为结果记录, 因为替换动作还未发生
+        setup = parsed_data['setup']
+        if log_data:
+            if setup:
+                self.log_request_setup(setup)
+
+        # 前置处理
+        if parsed_data['is_setup']:
+            log.info('开始处理请求前置...')
+            try:
+                for item in setup:
+                    for key, value in item.items():
+                        if value is not None:
+                            if key == SetupType.TESTCASE:
+                                relate_parsed_data = exec_setup_testcase(parsed_data, value)
+                                if relate_parsed_data:
+                                    parsed_data = relate_parsed_data
+                            elif key == SetupType.SQL:
+                                setup_sql = var_extractor.vars_replace({'sql': value}, parsed_data['env'])
+                                sql = setup_sql['sql']
+                                sql_fetch = setup_sql.get('fetch')
+                                mysql_client.exec_case_sql(sql, sql_fetch, parsed_data['env'])
+                            elif key == SetupType.HOOK:
+                                hook_executor.exec_hook_func(value)
+                            elif key == SetupType.WAIT_TIME:
+                                time.sleep(value)
+                                log.info(f'执行请求前等待：{value} s')
+            except Exception as e:
+                log.error(f'请求前置处理异常: {e}')
+                raise e
+            log.info('请求前置处理完成')
+
+        # 日志记录请求数据
+        if log_data:
+            self.log_request_up(parsed_data)
+            self.allure_request_up(parsed_data)
+
+        # allure 记录动态数据
+        self.allure_dynamic_data(parsed_data)
+
+        # 整理请求参数
+        request_conf = {
+            'timeout': parsed_data['timeout'],
+            'verify': parsed_data['verify'],
+            'proxies': parsed_data['proxies'],
+            'allow_redirects': parsed_data['redirects'],
+            'retry': parsed_data['retry'],
+        }
+        request_data_parsed = {
+            'method': parsed_data['method'],
+            'url': parsed_data['url'],
+            'params': parsed_data['params'],
+            'headers': parsed_data['headers'],
+            'cookies': parsed_data['cookies'],
+            'body': parsed_data['body'],
+            'files': parsed_data['files'],
+        }
+        if parsed_data['body_type'] == BodyType.JSON or parsed_data['body_type'] == BodyType.GraphQL:
+            request_data_parsed.update({'json': request_data_parsed.pop('body')})
+        elif parsed_data['body_type'] == BodyType.binary:
+            if request_engin == EnginType.httpx:
+                request_data_parsed.update({'content': request_data_parsed.pop('body')})
+        else:
+            request_data_parsed.update({'data': request_data_parsed.pop('body')})
+        try:
+            request_data_parsed = var_extractor.vars_replace(request_data_parsed, parsed_data['env'])
+        except Exception as e:
+            log.error(e)
+            raise e
+
+        # 发送请求
+        response_data = self.init_response_metadata
+        response_data['stat']['execute_time'] = get_current_time()
+        if request_engin == EnginType.requests:
+            response = self._requests_engin(**request_conf, **request_data_parsed, **kwargs)
+        elif request_engin == EnginType.httpx:
+            response = self._httpx_engin(**request_conf, **request_data_parsed, **kwargs)
+        else:
+            raise SendRequestError('请求发起失败，请使用合法的请求引擎：requests / httpx')
+
+        # 记录响应数据
+        response_data['url'] = str(response.url)
+        response_data['status_code'] = int(response.status_code)
+        response_data['elapsed'] = response.elapsed.microseconds / 1000.0
+        res_headers = dict(response.headers)
+        response_data['headers'] = res_headers
+        response_data['cookies'] = dict(response.cookies)
+        res_content_type = res_headers.get('Content-Type')
+        try:
+            if res_content_type and 'application/json' in res_content_type:
+                json_data = response.json()
+            else:
+                json_data = {}
+        except JSONDecodeError:
+            err_msg = '响应数据解析失败，响应数据不是有效的 json 格式'
+            log.warning(err_msg)
+            raise SendRequestError(err_msg)
+        response_data['json'] = json_data
+        response_data['content'] = response.content
+        response_data['text'] = response.text
+        response_data['request'] = request_data_parsed
+
+        # 日志记录响应数据
+        teardown = parsed_data['teardown']
+        if log_data:
+            self.log_request_down(response_data)
+            self.allure_request_down(response_data)
+            if teardown:
+                self.log_request_teardown(teardown)
+
+        # 后置处理
+        if parsed_data['is_teardown']:
+            log.info('开始处理请求后置...')
+            try:
+                for item in teardown:
+                    for key, value in item.items():
+                        if value is not None:
+                            if key == TeardownType.SQL:
+                                teardown_sql = var_extractor.vars_replace({'sql': value}, parsed_data['env'])
+                                sql = teardown_sql['sql']
+                                sql_fetch = teardown_sql.get('fetch')
+                                mysql_client.exec_case_sql(sql, sql_fetch, parsed_data['env'])
+                            if key == TeardownType.HOOK:
+                                hook_executor.exec_hook_func(value)
+                            if key == TeardownType.EXTRACT:
+                                var_extractor.teardown_var_extract(response_data, value, parsed_data['env'])
+                            if key == TeardownType.ASSERT:
+                                assert_text = var_extractor.vars_replace(
+                                    target={'assert_text': value}, env=parsed_data['env']
+                                )['assert_text']
+                                asserter.exec_asserter(response_data, assert_text)
+                            elif key == TeardownType.WAIT_TIME:
+                                log.info(f'执行请求后等待：{value} s')
+                                time.sleep(value)
+            except AssertionError as e:
+                log.error(f'断言失败: {e}')
+                raise AssertError(f'断言失败: {e}')
+            except Exception as e:
+                log.error(f'请求后置处理异常: {e}')
+                raise e
+            log.info('请求后置处理完成')
+
+        return response_data
+
+    def log_request_setup(self, setup: list) -> None:
+        for item in setup:
+            for key, value in item.items():
+                if key == SetupType.TESTCASE:
+                    log.info(f'前置 setup_testcase: {value}')
+                    self.allure_request_setup({'setup_testcase': value})
+                elif key == SetupType.SQL:
+                    log.info(f'前置 setup_sql: {value}')
+                    self.allure_request_setup({'setup_sql': value})
+                elif key == SetupType.HOOK:
+                    log.info(f'前置 setup_hook: {value}')
+                    self.allure_request_setup({'setup_hook': value})
+                elif key == SetupType.WAIT_TIME:
+                    log.info(f'前置 setup_wait_time: {value}')
+                    self.allure_request_setup({'setup_wait_time': value})
+
+    @staticmethod
+    def log_request_up(parsed_data: dict) -> None:
+        log.info(f"用例 env: {parsed_data['env']}")
+        log.info(f"用例 module: {parsed_data['module']}")
+        log.info(f"用例 name: {parsed_data['name']}")
+        log.info(f"用例 description: {parsed_data['description']}")
+        log.info(f"请求 method: {parsed_data['method']}")
+        log.info(f"请求 url: {parsed_data['url']}")
+        log.info(f"请求 params: {parsed_data['params']}")
+        log.info(f"请求 headers: {parsed_data['headers']}")
+        log.info(f"请求 data_type：{parsed_data['body_type']}")
+        if parsed_data['body_type'] != BodyType.JSON:
+            log.info(f"请求 data：{parsed_data['body']}")
+        else:
+            log.info(f"请求 json: {parsed_data['body']}")
+        log.info(f"请求 files: {parsed_data['files_no_parse']}")
+
+    def log_request_teardown(self, teardown: list) -> None:
+        for item in teardown:
+            for key, value in item.items():
+                if key == TeardownType.SQL:
+                    log.info(f'后置 teardown_sql: {value}')
+                    self.allure_request_teardown({'teardown_sql': value})
+                elif key == TeardownType.HOOK:
+                    log.info(f'后置 teardown_hook: {value}')
+                    self.allure_request_teardown({'teardown_hook': value})
+                elif key == TeardownType.EXTRACT:
+                    log.info(f'后置 teardown_extract: {value}')
+                    self.allure_request_teardown({'teardown_extract': value})
+                elif key == TeardownType.ASSERT:
+                    log.info(f'后置 teardown_assert: {value}')
+                    self.allure_request_teardown({'teardown_assert': value})
+                elif key == TeardownType.WAIT_TIME:
+                    log.info(f'后置 teardown_wait_time: {value}')
+                    self.allure_request_teardown({'teardown_wait_time': value})
+
+    @staticmethod
+    def log_request_down(response_data: dict) -> None:
+        log.info(f"请求发送时间: {response_data['stat']['execute_time']}")
+        str_status_code = str(response_data['status_code'])
+        if str_status_code.startswith(('4', '5')):
+            log.error(f"响应状态码: {response_data['status_code']}")
+        else:
+            log.info(f"响应状态码: {response_data['status_code']}")
+        log.info(f"响应时间: {response_data['elapsed']} ms")
+
+    @staticmethod
+    def allure_request_setup(setup_log: dict) -> None:
+        allure_step('请求前置', setup_log)
+
+    @staticmethod
+    def allure_request_up(parsed_data: dict) -> None:
+        allure_step(
+            '请求数据',
+            {
+                'env': parsed_data['env'],
+                'module': parsed_data['module'],
+                'name': parsed_data['name'],
+                'case_id': parsed_data['case_id'],
+                'description': parsed_data['description'],
+                'method': parsed_data['method'],
+                'url': parsed_data['url'],
+                'params': parsed_data['params'],
+                'headers': parsed_data['headers'],
+                'data_type': parsed_data['body_type'],
+                'data': parsed_data['body'],
+                'files': parsed_data['files_no_parse'],
+            },
+        )
+
+    @staticmethod
+    def allure_request_teardown(teardown_log: dict) -> None:
+        allure_step('请求后置', teardown_log)
+
+    @staticmethod
+    def allure_request_down(response_data: dict) -> None:
+        allure_step(
+            '响应数据',
+            {
+                'status_code': response_data['status_code'],
+                'elapsed': response_data['elapsed'],
+            },
+        )
+
+    @staticmethod
+    def allure_dynamic_data(parsed_data: dict) -> None:
+        allure.dynamic.title(parsed_data['name'])
+        allure.dynamic.description(parsed_data['description'])
+        allure.dynamic.link(parsed_data['url'])
+        if parsed_data['allure_severity'] is not None:
+            allure.dynamic.severity(parsed_data['allure_severity'])
+        if parsed_data['files_no_parse'] is not None:
+            for v in parsed_data['files_no_parse'].values():
+                if isinstance(v, list):
+                    for path in v:
+                        allure_attach_file(path)
+                else:
+                    allure_attach_file(v)
+
+
+send_request = SendRequests()
```

### Comparing `httpfpt-0.6.2/httpfpt/common/toml_handler.py` & `httpfpt-0.6.3/httpfpt/common/json_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,73 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import os
-
-import rtoml
-
-from httpfpt.common.log import log
-
-
-def read_toml(filepath: str, filename: str | None = None, encoding: str = 'utf-8') -> dict:
-    """
-    读取 toml 文件
-
-    :param filepath: 文件路径
-    :param filename: 文件名
-    :param encoding: 文件内容编码格式
-    :return:
-    """
-    if filename:
-        filepath = os.path.join(filepath, filename)
-    try:
-        with open(filepath, encoding=encoding) as f:
-            data = rtoml.load(f)
-    except Exception as e:
-        log.error(f'文件 {filename} 读取错误: {e}')
-        raise e
-    else:
-        return data
-
-
-def write_toml(filepath: str, filename: str, data: dict, encoding: str = 'utf-8', mode: str = 'a') -> int:
-    """
-    将字典写入包含 TOML 格式数据的文件
-
-    :param filepath: 文件路径
-    :param filename: 文件名称
-    :param data: 写入内容
-    :param encoding: 文件内容编码格式
-    :param mode: 文件写入模式
-    :return:
-    """
-    if not os.path.exists(filepath):
-        os.makedirs(filepath)
-
-    _file = os.path.join(filepath, filename)
-    try:
-        with open(_file, encoding=encoding, mode=mode) as f:
-            result = rtoml.dump(data, f)  # type: ignore
-    except ValueError as e:
-        log.error(f'写入文件 "{filename}" 错误 \n {e}')
-        raise e
-    else:
-        log.info(f'写入文件 {filename} 成功')
-        return result
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import json
+import os
+
+from typing import Any
+
+from httpfpt.common.log import log
+
+
+def read_json_file(filepath: str, filename: str | None = None, **kwargs) -> dict:
+    """
+    读取 json 文件
+
+    :param filepath:
+    :param filename:
+    :param kwargs:
+    :return:
+    """
+    if filename:
+        filepath = os.path.join(filepath, filename)
+    try:
+        with open(filepath, encoding='utf-8') as f:
+            data = json.load(f, **kwargs)
+    except Exception as e:
+        log.error(f'文件 {filename} 读取错误: {e}')
+        raise e
+    if data is not None:
+        return data
+    else:
+        log.warning(f'数据文件 {filename} 没有数据!')
+        raise ValueError(f'数据文件 {filename} 没有数据! 请检查数据文件内容是否正确!')
+
+
+def write_json_file(
+    filepath: str | None = None,
+    *,
+    filename: str,
+    data: Any = None,
+    encoding: str = 'utf-8',
+    mode: str = 'a',
+    **kwargs,
+) -> None:
+    """
+    写入 json 文件
+
+    :param filepath:
+    :param filename:
+    :param data:
+    :param encoding:
+    :param mode:
+    :param kwargs:
+    :return:
+    """
+    if filepath is not None:
+        if not os.path.exists(filepath):
+            os.makedirs(filepath)
+        _file = os.path.join(filepath, filename)
+    else:
+        _file = filename
+    if not _file:
+        log.warning('写入 json 文件失败，文件名为空')
+        raise ValueError('写入 json 文件失败，文件名为空')
+    try:
+        with open(_file, encoding=encoding, mode=mode) as f:
+            json.dump(data, f, ensure_ascii=False, **kwargs)
+    except Exception as e:
+        log.error(f'写入文件 "{filename}" 错误: {e}')
+        raise e
+    else:
+        log.info(f'写入文件 {filename} 成功')
```

### Comparing `httpfpt-0.6.2/httpfpt/common/yaml_handler.py` & `httpfpt-0.6.3/httpfpt/common/yaml_handler.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import os
-
-from pathlib import Path
-from typing import Any
-
-import yaml
-
-from httpfpt.common.log import log
-from httpfpt.core.path_conf import httpfpt_path
-from httpfpt.utils.time_control import get_current_time
-
-
-def read_yaml(filepath: str, filename: str | None = None) -> dict[str, Any]:
-    """
-    读取 yaml 文件
-
-    :param filepath: 文件路径
-    :param filename: 文件名
-    :return:
-    """
-    if filename:
-        filepath = os.path.join(filepath, filename)
-    try:
-        with open(filepath, encoding='utf-8') as f:
-            data = yaml.load(f, Loader=yaml.FullLoader)
-    except Exception as e:
-        log.error(f'文件 {filename} 读取错误: {e}')
-        raise e
-    if data is not None:
-        return data
-    else:
-        log.warning(f'数据文件 {filename} 没有数据!')
-        raise ValueError(f'数据文件 {filename} 没有数据! 请检查数据文件内容是否正确!')
-
-
-def write_yaml(filepath: str, filename: str, data: Any = None, *, encoding: str = 'utf-8', mode: str = 'a') -> None:
-    """
-    将数据写入包含 yaml 格式数据的文件
-
-    :param filepath: 文件路径
-    :param filename: 文件名
-    :param data: 数据
-    :param encoding: 文件内容编码格式
-    :param mode: 文件写入模式
-    :return:
-    """
-    _file = os.path.join(filepath, filename)
-    if not Path(_file).parent.exists():
-        Path(_file).parent.mkdir(parents=True, exist_ok=True)
-    try:
-        with open(_file, encoding=encoding, mode=mode) as f:
-            result = yaml.dump(data, f, allow_unicode=True)
-    except Exception as e:
-        log.error(f'写入文件 "{filename}" 错误: {e}')
-        raise e
-    else:
-        log.info(f'写入文件成功: {filename} ')
-        return result
-
-
-def write_yaml_report(
-    filename: str = f'APITestResult_{get_current_time("%Y-%m-%d %H_%M_%S")}.yaml',
-    *,
-    data: Any,
-    encoding: str = 'utf-8',
-    mode: str = 'a',
-) -> None:
-    """
-    写入 yaml 测试报告
-
-    :param filename: 测试报告文件名
-    :param data: 写入数据
-    :param encoding: 文件编码格式
-    :param mode: 文件写入模式
-    :return
-    """
-    _yaml_report_path = httpfpt_path.yaml_report_dir
-    if not os.path.exists(_yaml_report_path):
-        os.makedirs(_yaml_report_path)
-    _file = os.path.join(_yaml_report_path, filename)
-    try:
-        with open(_file, encoding=encoding, mode=mode) as f:
-            yaml.dump(data, f, allow_unicode=True)
-    except Exception as e:
-        log.error(f'写入 {filename} 测试报告失败: {e}')
-        raise e
-    else:
-        log.info(f'写入测试报告成功: {filename}')
-
-
-def write_yaml_vars(data: dict) -> None:
-    """
-    写入 yaml 全部变量
-
-    :param data:
-    :return:
-    """
-    _file = os.path.join(httpfpt_path.data_dir, 'global_vars.yaml')
-    try:
-        _vars = read_yaml(httpfpt_path.data_dir, filename='global_vars.yaml')
-        _vars.update(data)
-        with open(_file, encoding='utf-8', mode='w') as f:
-            yaml.dump(_vars, f, allow_unicode=True)
-    except Exception as e:
-        log.error(f'写入 global_vars.yaml 全局变量 {data} 错误: {e}')
-    else:
-        log.info(f'写入全局变量成功: global_vars.yaml -> {data}')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import os
+
+from pathlib import Path
+from typing import Any
+
+import yaml
+
+from httpfpt.common.log import log
+from httpfpt.core.path_conf import httpfpt_path
+from httpfpt.utils.time_control import get_current_time
+
+
+def read_yaml(filepath: str, filename: str | None = None) -> dict[str, Any]:
+    """
+    读取 yaml 文件
+
+    :param filepath: 文件路径
+    :param filename: 文件名
+    :return:
+    """
+    if filename:
+        filepath = os.path.join(filepath, filename)
+    try:
+        with open(filepath, encoding='utf-8') as f:
+            data = yaml.load(f, Loader=yaml.FullLoader)
+    except Exception as e:
+        log.error(f'文件 {filename} 读取错误: {e}')
+        raise e
+    if data is not None:
+        return data
+    else:
+        log.warning(f'数据文件 {filename} 没有数据!')
+        raise ValueError(f'数据文件 {filename} 没有数据! 请检查数据文件内容是否正确!')
+
+
+def write_yaml(filepath: str, filename: str, data: Any = None, *, encoding: str = 'utf-8', mode: str = 'a') -> None:
+    """
+    将数据写入包含 yaml 格式数据的文件
+
+    :param filepath: 文件路径
+    :param filename: 文件名
+    :param data: 数据
+    :param encoding: 文件内容编码格式
+    :param mode: 文件写入模式
+    :return:
+    """
+    _file = os.path.join(filepath, filename)
+    if not Path(_file).parent.exists():
+        Path(_file).parent.mkdir(parents=True, exist_ok=True)
+    try:
+        with open(_file, encoding=encoding, mode=mode) as f:
+            result = yaml.dump(data, f, allow_unicode=True)
+    except Exception as e:
+        log.error(f'写入文件 "{filename}" 错误: {e}')
+        raise e
+    else:
+        log.info(f'写入文件成功: {filename} ')
+        return result
+
+
+def write_yaml_report(
+    filename: str = f'APITestResult_{get_current_time("%Y-%m-%d %H_%M_%S")}.yaml',
+    *,
+    data: Any,
+    encoding: str = 'utf-8',
+    mode: str = 'a',
+) -> None:
+    """
+    写入 yaml 测试报告
+
+    :param filename: 测试报告文件名
+    :param data: 写入数据
+    :param encoding: 文件编码格式
+    :param mode: 文件写入模式
+    :return
+    """
+    _yaml_report_path = httpfpt_path.yaml_report_dir
+    if not os.path.exists(_yaml_report_path):
+        os.makedirs(_yaml_report_path)
+    _file = os.path.join(_yaml_report_path, filename)
+    try:
+        with open(_file, encoding=encoding, mode=mode) as f:
+            yaml.dump(data, f, allow_unicode=True)
+    except Exception as e:
+        log.error(f'写入 {filename} 测试报告失败: {e}')
+        raise e
+    else:
+        log.info(f'写入测试报告成功: {filename}')
+
+
+def write_yaml_vars(data: dict) -> None:
+    """
+    写入 yaml 全部变量
+
+    :param data:
+    :return:
+    """
+    _file = os.path.join(httpfpt_path.data_dir, 'global_vars.yaml')
+    try:
+        _vars = read_yaml(httpfpt_path.data_dir, filename='global_vars.yaml')
+        _vars.update(data)
+        with open(_file, encoding='utf-8', mode='w') as f:
+            yaml.dump(_vars, f, allow_unicode=True)
+    except Exception as e:
+        log.error(f'写入 global_vars.yaml 全局变量 {data} 错误: {e}')
+    else:
+        log.info(f'写入全局变量成功: global_vars.yaml -> {data}')
```

### Comparing `httpfpt-0.6.2/httpfpt/conftest.py` & `httpfpt-0.6.3/httpfpt/conftest.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import time
-
-from datetime import datetime
-
-import pytest
-
-from py._xmlgen import html
-
-from httpfpt.common.log import log
-from httpfpt.common.variable_cache import variable_cache
-from httpfpt.common.yaml_handler import write_yaml_report
-from httpfpt.core.get_conf import httpfpt_config
-
-
-@pytest.fixture(scope='session', autouse=True)
-def session_fixture(tmp_path_factory):
-    pass
-
-
-@pytest.fixture(scope='package', autouse=True)
-def package_fixture():
-    yield
-    # 预留空行
-    log.info('')
-    # 清理临时变量
-    variable_cache.clear()
-
-
-@pytest.fixture(scope='module', autouse=True)
-def module_fixture():
-    pass
-
-
-@pytest.fixture(scope='class', autouse=True)
-def class_fixture():
-    pass
-
-
-@pytest.fixture(scope='function', autouse=True)
-def function_fixture(request):
-    log.info('')  # 预留空行
-    log.info(f'🔥 Running: {request.function.__name__}')
-
-    def testcase_end():
-        log.info('🔚 End')
-
-    # teardown终结函数 == yield后的代码
-    request.addfinalizer(testcase_end)
-
-
-def pytest_configure(config):
-    """
-    pytest配置
-
-    :param config:
-    :return:
-    """
-    # 元信息配置
-    metadata = config.pluginmanager.getplugin('metadata')
-    if metadata:
-        from pytest_metadata.plugin import metadata_key
-
-        config.stash[metadata_key]['Project Name'] = httpfpt_config.PROJECT_NAME
-        del config.stash[metadata_key]['Packages']
-        del config.stash[metadata_key]['Platform']
-        del config.stash[metadata_key]['Plugins']
-
-
-def pytest_html_results_summary(prefix):
-    """
-    html报告摘要信息配置
-
-    :param prefix:
-    :return:
-    """
-    # 向 html 报告中的 summary 添加额外信息
-    prefix.extend([html.p(f'Tester: {httpfpt_config.TESTER_NAME}')])
-
-
-@pytest.mark.optionalhook
-def pytest_html_report_title(report):
-    """
-    html报告标题配置
-
-    :param report:
-    :return:
-    """
-    report.title = f'{httpfpt_config.TEST_REPORT_TITLE}'
-
-
-@pytest.mark.optionalhook
-def pytest_html_results_table_header(cells):
-    """
-    html报告表格列配置
-
-    :param cells:
-    :return:
-    """
-    cells.insert(1, html.th('Description'))
-    cells.insert(3, html.th('Start Time', class_='sortable time', col='time'))
-    cells.pop()
-
-
-@pytest.mark.optionalhook
-def pytest_html_results_table_row(report, cells):
-    """
-    html报告表格列值配置
-
-    :param report:
-    :param cells:
-    :return:
-    """
-    cells.insert(1, html.td(getattr(report, 'description', None)))
-    cells.insert(3, html.td(datetime.now(), class_='col-time'))
-    cells.pop()
-
-
-@pytest.mark.hookwrapper
-def pytest_runtest_makereport(item, call):
-    """
-    自动化获取用例描述, 解决测试用例参数包含中文问题
-
-    :param item:
-    :param call:
-    :return:
-    """
-    outcome = yield
-    report = outcome.get_result()
-    # 获取用例描述
-    if getattr(item.function, '__doc__', None) is None:
-        report.description = str(item.function.__name__)
-    else:
-        report.description = str(item.function.__doc__)
-
-
-def pytest_collection_modifyitems(items):
-    """
-    解决数据驱动ids参数为中文时,控制台输出乱码问题
-
-    :param items:
-    :return:
-    """
-    # item表示每个用例
-    for item in items:
-        item.name = item.name.encode('utf-8').decode('unicode_escape')
-        item._nodeid = item.nodeid.encode('utf-8').decode('unicode_escape')
-
-
-def pytest_terminal_summary(terminalreporter, exitstatus, config):
-    """
-    收集测试结果
-    """
-    started_time = terminalreporter._sessionstarttime
-    elapsed_seconds = float(time.time() - started_time)
-    hours, remainder = divmod(elapsed_seconds, 3600)
-    minutes, seconds = divmod(remainder, 60)
-    total = terminalreporter._numcollected
-    stats = terminalreporter.stats
-    passed = len(stats.get('passed', []))
-    failed = len(stats.get('failed', []))
-    error = len(stats.get('error', []))
-    skipped = len(stats.get('skipped', []))
-    data = {
-        'result': 'Success' if failed == 0 else 'Failed',
-        'total': total,
-        'passed': passed,
-        'failed': failed,
-        'error': error,
-        'skipped': skipped,
-        'started_time': datetime.fromtimestamp(started_time).strftime('%Y-%m-%d %H:%M:%S'),
-        'elapsed': f'{int(hours):02}:{int(minutes):02}:{int(seconds):02}',
-    }
-    write_yaml_report(data=data)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+import time
+
+from datetime import datetime
+
+import pytest
+
+from py._xmlgen import html
+
+from httpfpt.common.log import log
+from httpfpt.common.variable_cache import variable_cache
+from httpfpt.common.yaml_handler import write_yaml_report
+from httpfpt.core.get_conf import httpfpt_config
+
+
+@pytest.fixture(scope='session', autouse=True)
+def session_fixture(tmp_path_factory):
+    pass
+
+
+@pytest.fixture(scope='package', autouse=True)
+def package_fixture():
+    yield
+    # 预留空行
+    log.info('')
+    # 清理临时变量
+    variable_cache.clear()
+
+
+@pytest.fixture(scope='module', autouse=True)
+def module_fixture():
+    pass
+
+
+@pytest.fixture(scope='class', autouse=True)
+def class_fixture():
+    pass
+
+
+@pytest.fixture(scope='function', autouse=True)
+def function_fixture(request):
+    log.info('')  # 预留空行
+    log.info(f'🔥 Running: {request.function.__name__}')
+
+    def testcase_end():
+        log.info('🔚 End')
+
+    # teardown终结函数 == yield后的代码
+    request.addfinalizer(testcase_end)
+
+
+def pytest_configure(config):
+    """
+    pytest配置
+
+    :param config:
+    :return:
+    """
+    # 元信息配置
+    metadata = config.pluginmanager.getplugin('metadata')
+    if metadata:
+        from pytest_metadata.plugin import metadata_key
+
+        config.stash[metadata_key]['Project Name'] = httpfpt_config.PROJECT_NAME
+        del config.stash[metadata_key]['Packages']
+        del config.stash[metadata_key]['Platform']
+        del config.stash[metadata_key]['Plugins']
+
+
+def pytest_html_results_summary(prefix):
+    """
+    html报告摘要信息配置
+
+    :param prefix:
+    :return:
+    """
+    # 向 html 报告中的 summary 添加额外信息
+    prefix.extend([html.p(f'Tester: {httpfpt_config.TESTER_NAME}')])
+
+
+@pytest.mark.optionalhook
+def pytest_html_report_title(report):
+    """
+    html报告标题配置
+
+    :param report:
+    :return:
+    """
+    report.title = f'{httpfpt_config.TEST_REPORT_TITLE}'
+
+
+@pytest.mark.optionalhook
+def pytest_html_results_table_header(cells):
+    """
+    html报告表格列配置
+
+    :param cells:
+    :return:
+    """
+    cells.insert(1, html.th('Description'))
+    cells.insert(3, html.th('Start Time', class_='sortable time', col='time'))
+    cells.pop()
+
+
+@pytest.mark.optionalhook
+def pytest_html_results_table_row(report, cells):
+    """
+    html报告表格列值配置
+
+    :param report:
+    :param cells:
+    :return:
+    """
+    cells.insert(1, html.td(getattr(report, 'description', None)))
+    cells.insert(3, html.td(datetime.now(), class_='col-time'))
+    cells.pop()
+
+
+@pytest.mark.hookwrapper
+def pytest_runtest_makereport(item, call):
+    """
+    自动化获取用例描述, 解决测试用例参数包含中文问题
+
+    :param item:
+    :param call:
+    :return:
+    """
+    outcome = yield
+    report = outcome.get_result()
+    # 获取用例描述
+    if getattr(item.function, '__doc__', None) is None:
+        report.description = str(item.function.__name__)
+    else:
+        report.description = str(item.function.__doc__)
+
+
+def pytest_collection_modifyitems(items):
+    """
+    解决数据驱动ids参数为中文时,控制台输出乱码问题
+
+    :param items:
+    :return:
+    """
+    # item表示每个用例
+    for item in items:
+        item.name = item.name.encode('utf-8').decode('unicode_escape')
+        item._nodeid = item.nodeid.encode('utf-8').decode('unicode_escape')
+
+
+def pytest_terminal_summary(terminalreporter, exitstatus, config):
+    """
+    收集测试结果
+    """
+    started_time = terminalreporter._sessionstarttime
+    elapsed_seconds = float(time.time() - started_time)
+    hours, remainder = divmod(elapsed_seconds, 3600)
+    minutes, seconds = divmod(remainder, 60)
+    total = terminalreporter._numcollected
+    stats = terminalreporter.stats
+    passed = len(stats.get('passed', []))
+    failed = len(stats.get('failed', []))
+    error = len(stats.get('error', []))
+    skipped = len(stats.get('skipped', []))
+    data = {
+        'result': 'Success' if failed == 0 else 'Failed',
+        'total': total,
+        'passed': passed,
+        'failed': failed,
+        'error': error,
+        'skipped': skipped,
+        'started_time': datetime.fromtimestamp(started_time).strftime('%Y-%m-%d %H:%M:%S'),
+        'elapsed': f'{int(hours):02}:{int(minutes):02}:{int(seconds):02}',
+    }
+    write_yaml_report(data=data)
```

### Comparing `httpfpt-0.6.2/httpfpt/core/get_conf.py` & `httpfpt-0.6.3/httpfpt/core/get_conf.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-from functools import lru_cache
-
-from glom import glom
-
-from httpfpt.common.errors import ConfigInitError
-from httpfpt.common.toml_handler import read_toml
-from httpfpt.core.path_conf import httpfpt_path
-
-__all__ = ['httpfpt_config']
-
-
-class HttpFptConfig:
-    def __init__(self) -> None:
-        self.settings = read_toml(httpfpt_path.settings_dir, 'conf.toml')
-        try:
-            # 项目目录名
-            self.PROJECT_NAME = glom(self.settings, 'project.name')
-
-            # 测试报告
-            self.TEST_REPORT_TITLE = glom(self.settings, 'report.title')
-            self.TESTER_NAME = glom(self.settings, 'report.tester_name')
-
-            # mysql 数据库
-            self.MYSQL_HOST = glom(self.settings, 'mysql.host')
-            self.MYSQL_PORT = glom(self.settings, 'mysql.port')
-            self.MYSQL_USER = glom(self.settings, 'mysql.user')
-            self.MYSQL_PASSWORD = glom(self.settings, 'mysql.password')
-            self.MYSQL_DATABASE = glom(self.settings, 'mysql.database')
-            self.MYSQL_CHARSET = glom(self.settings, 'mysql.charset')
-
-            # redis 数据库
-            self.REDIS_HOST = glom(self.settings, 'redis.host')
-            self.REDIS_PORT = glom(self.settings, 'redis.port')
-            self.REDIS_PASSWORD = glom(self.settings, 'redis.password')
-            self.REDIS_DATABASE = glom(self.settings, 'redis.database')
-            self.REDIS_TIMEOUT = glom(self.settings, 'redis.timeout')
-
-            # 邮件
-            self.EMAIL_SERVER = glom(self.settings, 'email.host')
-            self.EMAIL_PORT = glom(self.settings, 'email.port')
-            self.EMAIL_USER = glom(self.settings, 'email.user')
-            self.EMAIL_PASSWORD = glom(self.settings, 'email.password')
-            self.EMAIL_SEND_TO = glom(self.settings, 'email.receiver')
-            self.EMAIL_SSL = glom(self.settings, 'email.ssl')
-            self.EMAIL_SEND = glom(self.settings, 'email.send')
-
-            # 钉钉
-            self.DINGDING_WEBHOOK = glom(self.settings, 'dingding.webhook')
-            self.DINGDING_PROXY = {
-                'http': glom(self.settings, 'dingding.proxies.http')
-                if glom(self.settings, 'dingding.proxies.http') != ''
-                else None,
-                'https': glom(self.settings, 'dingding.proxies.https')
-                if glom(self.settings, 'dingding.proxies.https') != ''
-                else None,
-            }
-            self.DINGDING_SEND = glom(self.settings, 'dingding.send')
-
-            # 飞书
-            self.FEISHU_WEBHOOK = glom(self.settings, 'feishu.webhook')
-            self.FEISHU_PROXY = {
-                'http': glom(self.settings, 'feishu.proxies.http')
-                if glom(self.settings, 'feishu.proxies.http') != ''
-                else None,
-                'https': glom(self.settings, 'feishu.proxies.https')
-                if glom(self.settings, 'feishu.proxies.https') != ''
-                else None,
-            }
-            self.FEISHU_SEND = glom(self.settings, 'feishu.send')
-
-            # 企业微信
-            self.WECHAT_WEBHOOK = glom(self.settings, 'wechat.webhook')
-            self.WECHAT_PROXY = {
-                'http': glom(self.settings, 'wechat.proxies.http')
-                if glom(self.settings, 'wechat.proxies.http') != ''
-                else None,
-                'https': glom(self.settings, 'wechat.proxies.https')
-                if glom(self.settings, 'wechat.proxies.https') != ''
-                else None,
-            }
-            self.WECHAT_SEND = glom(self.settings, 'wechat.send')
-
-            # 请求发送
-            self.REQUEST_TIMEOUT = glom(self.settings, 'request.timeout')
-            self.REQUEST_VERIFY = glom(self.settings, 'request.verify')
-            self.REQUEST_REDIRECTS = glom(self.settings, 'request.redirects')
-            self.REQUEST_PROXIES_REQUESTS = {
-                'http': glom(self.settings, 'request.proxies.http')
-                if glom(self.settings, 'request.proxies.http') != ''
-                else None,
-                'https': glom(self.settings, 'request.proxies.https')
-                if glom(self.settings, 'request.proxies.https') != ''
-                else None,
-            }
-            self.REQUEST_PROXIES_HTTPX = {
-                'http://': glom(self.settings, 'request.proxies.http')
-                if glom(self.settings, 'request.proxies.http') != ''
-                else None,
-                'https://': glom(self.settings, 'request.proxies.https')
-                if glom(self.settings, 'request.proxies.https') != ''
-                else None,
-            }
-            self.REQUEST_RETRY = glom(self.settings, 'request.retry')
-        except KeyError as e:
-            raise ConfigInitError(f'配置解析失败：缺失参数 {str(e)}，请核对项目配置文件')
-
-
-@lru_cache(maxsize=None)
-def cache_httpfpt_config() -> HttpFptConfig:
-    return HttpFptConfig()
-
-
-httpfpt_config = cache_httpfpt_config()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from functools import lru_cache
+
+from glom import glom
+
+from httpfpt.common.errors import ConfigInitError
+from httpfpt.common.toml_handler import read_toml
+from httpfpt.core.path_conf import httpfpt_path
+
+__all__ = ['httpfpt_config']
+
+
+class HttpFptConfig:
+    def __init__(self) -> None:
+        self.settings = read_toml(httpfpt_path.settings_dir, 'conf.toml')
+        try:
+            # 项目目录名
+            self.PROJECT_NAME = glom(self.settings, 'project.name')
+
+            # 测试报告
+            self.TEST_REPORT_TITLE = glom(self.settings, 'report.title')
+            self.TESTER_NAME = glom(self.settings, 'report.tester_name')
+
+            # mysql 数据库
+            self.MYSQL_HOST = glom(self.settings, 'mysql.host')
+            self.MYSQL_PORT = glom(self.settings, 'mysql.port')
+            self.MYSQL_USER = glom(self.settings, 'mysql.user')
+            self.MYSQL_PASSWORD = glom(self.settings, 'mysql.password')
+            self.MYSQL_DATABASE = glom(self.settings, 'mysql.database')
+            self.MYSQL_CHARSET = glom(self.settings, 'mysql.charset')
+
+            # redis 数据库
+            self.REDIS_HOST = glom(self.settings, 'redis.host')
+            self.REDIS_PORT = glom(self.settings, 'redis.port')
+            self.REDIS_PASSWORD = glom(self.settings, 'redis.password')
+            self.REDIS_DATABASE = glom(self.settings, 'redis.database')
+            self.REDIS_TIMEOUT = glom(self.settings, 'redis.timeout')
+
+            # 邮件
+            self.EMAIL_SERVER = glom(self.settings, 'email.host')
+            self.EMAIL_PORT = glom(self.settings, 'email.port')
+            self.EMAIL_USER = glom(self.settings, 'email.user')
+            self.EMAIL_PASSWORD = glom(self.settings, 'email.password')
+            self.EMAIL_SEND_TO = glom(self.settings, 'email.receiver')
+            self.EMAIL_SSL = glom(self.settings, 'email.ssl')
+            self.EMAIL_SEND = glom(self.settings, 'email.send')
+
+            # 钉钉
+            self.DINGDING_WEBHOOK = glom(self.settings, 'dingding.webhook')
+            self.DINGDING_PROXY = {
+                'http': glom(self.settings, 'dingding.proxies.http')
+                if glom(self.settings, 'dingding.proxies.http') != ''
+                else None,
+                'https': glom(self.settings, 'dingding.proxies.https')
+                if glom(self.settings, 'dingding.proxies.https') != ''
+                else None,
+            }
+            self.DINGDING_SEND = glom(self.settings, 'dingding.send')
+
+            # 飞书
+            self.FEISHU_WEBHOOK = glom(self.settings, 'feishu.webhook')
+            self.FEISHU_PROXY = {
+                'http': glom(self.settings, 'feishu.proxies.http')
+                if glom(self.settings, 'feishu.proxies.http') != ''
+                else None,
+                'https': glom(self.settings, 'feishu.proxies.https')
+                if glom(self.settings, 'feishu.proxies.https') != ''
+                else None,
+            }
+            self.FEISHU_SEND = glom(self.settings, 'feishu.send')
+
+            # 企业微信
+            self.WECHAT_WEBHOOK = glom(self.settings, 'wechat.webhook')
+            self.WECHAT_PROXY = {
+                'http': glom(self.settings, 'wechat.proxies.http')
+                if glom(self.settings, 'wechat.proxies.http') != ''
+                else None,
+                'https': glom(self.settings, 'wechat.proxies.https')
+                if glom(self.settings, 'wechat.proxies.https') != ''
+                else None,
+            }
+            self.WECHAT_SEND = glom(self.settings, 'wechat.send')
+
+            # 请求发送
+            self.REQUEST_TIMEOUT = glom(self.settings, 'request.timeout')
+            self.REQUEST_VERIFY = glom(self.settings, 'request.verify')
+            self.REQUEST_REDIRECTS = glom(self.settings, 'request.redirects')
+            self.REQUEST_PROXIES_REQUESTS = {
+                'http': glom(self.settings, 'request.proxies.http')
+                if glom(self.settings, 'request.proxies.http') != ''
+                else None,
+                'https': glom(self.settings, 'request.proxies.https')
+                if glom(self.settings, 'request.proxies.https') != ''
+                else None,
+            }
+            self.REQUEST_PROXIES_HTTPX = {
+                'http://': glom(self.settings, 'request.proxies.http')
+                if glom(self.settings, 'request.proxies.http') != ''
+                else None,
+                'https://': glom(self.settings, 'request.proxies.https')
+                if glom(self.settings, 'request.proxies.https') != ''
+                else None,
+            }
+            self.REQUEST_RETRY = glom(self.settings, 'request.retry')
+        except KeyError as e:
+            raise ConfigInitError(f'配置解析失败：缺失参数 {str(e)}，请核对项目配置文件')
+
+
+@lru_cache(maxsize=None)
+def cache_httpfpt_config() -> HttpFptConfig:
+    return HttpFptConfig()
+
+
+httpfpt_config = cache_httpfpt_config()
```

### Comparing `httpfpt-0.6.2/httpfpt/core/path_conf.py` & `httpfpt-0.6.3/httpfpt/core/path_conf.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import os
-
-from functools import lru_cache
-
-from httpfpt.common.errors import ConfigInitError
-
-__all__ = ['httpfpt_path']
-
-
-class HttpFptPathConfig:
-    @property
-    def project_dir(self) -> str:
-        """项目根路径"""
-        _base_dir = os.getenv('HTTPFPT_PROJECT_PATH')
-        if not _base_dir:
-            raise ConfigInitError(
-                '运行失败：在访问 HTTPFPT API 前，请先通过 `httpfpt` 命令创建新项目；'
-                '如果已经创建，请确保配置了 `HTTPFPT_PROJECT_PATH` 环境变量为项目目录'
-            )
-        else:
-            if not os.path.exists(_base_dir):
-                raise ConfigInitError(
-                    f"操作失败 - 未找到项目路径 '{_base_dir}'。请确保以下几点："
-                    f'1. 环境变量是否已正确配置；2. 检查指定的项目路径是否存在。'
-                    f'如果项目还未创建，你需要先创建一个新项目；完成上述检查后，请重新尝试执行此操作'
-                )
-        return _base_dir
-
-    @property
-    def log_dir(self) -> str:
-        """日志路径"""
-        return os.path.join(self.project_dir, 'log')
-
-    @property
-    def data_dir(self) -> str:
-        """数据路径"""
-        return os.path.join(self.project_dir, 'data')
-
-    @property
-    def case_data_dir(self) -> str:
-        """用例数据路径"""
-        return os.path.join(self.data_dir, 'test_data')
-
-    @property
-    def report_dir(self) -> str:
-        """测试报告路径"""
-        return os.path.join(self.project_dir, 'report')
-
-    @property
-    def allure_report_dir(self) -> str:
-        """allure测试报告路径"""
-        return os.path.join(self.report_dir, 'allure_report')
-
-    @property
-    def allure_html_report_dir(self) -> str:
-        """allure html测试报告路径"""
-        return os.path.join(self.allure_report_dir, 'html')
-
-    @property
-    def html_report_dir(self) -> str:
-        """HTML测试报告路径"""
-        return os.path.join(self.report_dir, 'html_report')
-
-    @property
-    def yaml_report_dir(self) -> str:
-        """YAML测试报告路径"""
-        return os.path.join(self.report_dir, 'yaml_report')
-
-    @property
-    def allure_env_file(self) -> str:
-        """allure环境文件"""
-        return os.path.join(self.project_dir, 'core', 'allure_env', 'environment.properties')
-
-    @property
-    def allure_report_env_file(self) -> str:
-        """allure报告环境文件，用作copy，避免allure开启清理缓存导致环境文件丢失"""
-        return os.path.join(self.allure_report_dir, 'environment.properties')
-
-    @property
-    def run_env_dir(self) -> str:
-        """运行环境文件路径"""
-        return os.path.join(self.project_dir, 'core', 'run_env')
-
-    @property
-    def testcase_dir(self) -> str:
-        """测试用例路径"""
-        return os.path.join(self.project_dir, 'testcases')
-
-    @property
-    def auth_conf_dir(self) -> str:
-        """AUTH配置文件路径"""
-        return os.path.join(self.project_dir, 'core')
-
-    @property
-    def settings_dir(self) -> str:
-        """核心配置文件路径"""
-        return self.auth_conf_dir
-
-
-@lru_cache(maxsize=None)
-def cache_httpfpt_path() -> HttpFptPathConfig:
-    return HttpFptPathConfig()
-
-
-httpfpt_path = cache_httpfpt_path()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import os
+
+from functools import lru_cache
+
+from httpfpt.common.errors import ConfigInitError
+
+__all__ = ['httpfpt_path']
+
+
+class HttpFptPathConfig:
+    @property
+    def project_dir(self) -> str:
+        """项目根路径"""
+        _base_dir = os.getenv('HTTPFPT_PROJECT_PATH')
+        if not _base_dir:
+            raise ConfigInitError(
+                '运行失败：在访问 HTTPFPT API 前，请先通过 `httpfpt` 命令创建新项目；'
+                '如果已经创建，请确保配置了 `HTTPFPT_PROJECT_PATH` 环境变量为项目目录'
+            )
+        else:
+            if not os.path.exists(_base_dir):
+                raise ConfigInitError(
+                    f"操作失败 - 未找到项目路径 '{_base_dir}'。请确保以下几点："
+                    f'1. 环境变量是否已正确配置；2. 检查指定的项目路径是否存在。'
+                    f'如果项目还未创建，你需要先创建一个新项目；完成上述检查后，请重新尝试执行此操作'
+                )
+        return _base_dir
+
+    @property
+    def log_dir(self) -> str:
+        """日志路径"""
+        return os.path.join(self.project_dir, 'log')
+
+    @property
+    def data_dir(self) -> str:
+        """数据路径"""
+        return os.path.join(self.project_dir, 'data')
+
+    @property
+    def case_data_dir(self) -> str:
+        """用例数据路径"""
+        return os.path.join(self.data_dir, 'test_data')
+
+    @property
+    def report_dir(self) -> str:
+        """测试报告路径"""
+        return os.path.join(self.project_dir, 'report')
+
+    @property
+    def allure_report_dir(self) -> str:
+        """allure测试报告路径"""
+        return os.path.join(self.report_dir, 'allure_report')
+
+    @property
+    def allure_html_report_dir(self) -> str:
+        """allure html测试报告路径"""
+        return os.path.join(self.allure_report_dir, 'html')
+
+    @property
+    def html_report_dir(self) -> str:
+        """HTML测试报告路径"""
+        return os.path.join(self.report_dir, 'html_report')
+
+    @property
+    def yaml_report_dir(self) -> str:
+        """YAML测试报告路径"""
+        return os.path.join(self.report_dir, 'yaml_report')
+
+    @property
+    def allure_env_file(self) -> str:
+        """allure环境文件"""
+        return os.path.join(self.project_dir, 'core', 'allure_env', 'environment.properties')
+
+    @property
+    def allure_report_env_file(self) -> str:
+        """allure报告环境文件，用作copy，避免allure开启清理缓存导致环境文件丢失"""
+        return os.path.join(self.allure_report_dir, 'environment.properties')
+
+    @property
+    def run_env_dir(self) -> str:
+        """运行环境文件路径"""
+        return os.path.join(self.project_dir, 'core', 'run_env')
+
+    @property
+    def testcase_dir(self) -> str:
+        """测试用例路径"""
+        return os.path.join(self.project_dir, 'testcases')
+
+    @property
+    def auth_conf_dir(self) -> str:
+        """AUTH配置文件路径"""
+        return os.path.join(self.project_dir, 'core')
+
+    @property
+    def settings_dir(self) -> str:
+        """核心配置文件路径"""
+        return self.auth_conf_dir
+
+
+@lru_cache(maxsize=None)
+def cache_httpfpt_path() -> HttpFptPathConfig:
+    return HttpFptPathConfig()
+
+
+httpfpt_path = cache_httpfpt_path()
```

### Comparing `httpfpt-0.6.2/httpfpt/data/test_data/test_project/api_testcase_template.yaml` & `httpfpt-0.6.3/httpfpt/data/test_data/test_project/api_testcase_template.yaml`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-config:
-  allure:
-    epic: demo接口
-    feature: demo模块
-    story: yaml数据测试输出
-  request:
-    env: dev.env
-    headers:
-    timeout: 10
-    verify: False
-    redirects: True
-    proxies:
-      http:
-      https:
-    retry:
-  module: test
-
-test_steps:
-  - name: 查询
-    case_id: event_query_001
-    description: 测试关联变量
-    is_run:
-    request:
-      method: GET
-      url: /posts/1
-      params:
-      headers:
-      body_type:
-      body:
-      files:
-    setup:
-      - testcase:
-          case_id: event_linked_001
-          request:
-            - value: 2
-              jsonpath: $.params.postId
-          response:
-            - key: rcode
-              jsonpath: $.status_code
-      - testcase:
-          case_id: event_linked_001
-          response:
-              - key: rcode
-                jsonpath: $.status_code
-      - testcase: event_linked_001
-      - hook:
-      - wait_time: 0
-    teardown:
-      - sql:
-      - hook:
-      - extract:
-          key: test_cache
-          type: cache
-          jsonpath: $.status_code
-      - assert:
-          check:
-          type: str_eq
-          value: ^{rcode}
-          jsonpath: $.status_code
-      - wait_time: 0
-
-  - name: 断言
-    case_id: event_query_002
-    description: 测试高级断言
-    is_run:
-    request:
-      method: GET
-      url: /albums/1
-      params:
-      headers:
-      body_type:
-      body:
-      files:
-    setup:
-      - wait_time: 0
-    teardown:
-      - extract:
-          key: test_env
-          type: env
-          jsonpath: $.status_code
-      - extract:
-          key: test_global
-          type: global
-          jsonpath: $.status_code
-      - assert: assert 200 == pm.response.get('status_code')
-      - assert: assert pm.response.get('status_code') == IsInt(exactly=200), '响应状态码非200'
-      - assert: assert int(pm.response.get('status_code')) == IsInt, '响应状态码错误'
-      - assert: assert 'postId' not in str(pm.response.get('content')), '没有返回content'
-      - assert:
-          check:
-          type: jsonschema
-          jsonschema:
-            type: object
-            properties:
-              userId:
-                type: integer
-              id:
-                type: integer
-              title:
-                type: string
-            required:
-              - userId
-              - id
-              - title
-      - assert:
-          check:
-          type: re
-          pattern: '^\b200\b'
-          jsonpath: $.status_code
-
-  - name: hook
-    case_id: event_create_001
-    description: 测试hook
-    is_run:
-    retry: 2
-    request:
-      method: POST
-      url: /users/1
-      params:
-      headers:
-      body_type: json
-      body:
-        title: foo
-        body: sum(a+b)=${sum_a_b(1,2)}; $test_cache ; $test_env ; ${test_global}.
-        userId: 1
-      files:
-    setup:
-      - hook: ${current_time()}
-    teardown:
-      - hook: ${random_phone()}
-      - assert: assert 200 == pm.response.get('status_code')
-
-  - name: 被关联用例
-    case_id: event_linked_001
-    description: 作为被关联简易用例而存在
-    is_run:
-    request:
-      method: GET
-      url: /comments
-      params:
-        postId: 1
-      headers:
-      body_type:
-      body:
-      files:
-
-  - name: 跨文件关联用例
-    case_id: event_relate_001
-    description: 测试跨文件关联用例
-    is_run:
-    request:
-      method: GET
-      url: /albums/1
-      params:
-      headers:
-      body_type:
-      body:
-      files:
-    setup:
-      - testcase: event_upload_004
+config:
+  allure:
+    epic: demo接口
+    feature: demo模块
+    story: yaml数据测试输出
+  request:
+    env: dev.env
+    headers:
+    timeout: 10
+    verify: False
+    redirects: True
+    proxies:
+      http:
+      https:
+    retry:
+  module: test
+
+test_steps:
+  - name: 查询
+    case_id: event_query_001
+    description: 测试关联变量
+    is_run:
+    request:
+      method: GET
+      url: /posts/1
+      params:
+      headers:
+      body_type:
+      body:
+      files:
+    setup:
+      - testcase:
+          case_id: event_linked_001
+          request:
+            - value: 2
+              jsonpath: $.params.postId
+          response:
+            - key: rcode
+              jsonpath: $.status_code
+      - testcase:
+          case_id: event_linked_001
+          response:
+              - key: rcode
+                jsonpath: $.status_code
+      - testcase: event_linked_001
+      - hook:
+      - wait_time: 0
+    teardown:
+      - sql:
+      - hook:
+      - extract:
+          key: test_cache
+          type: cache
+          jsonpath: $.status_code
+      - assert:
+          check:
+          type: str_eq
+          value: ^{rcode}
+          jsonpath: $.status_code
+      - wait_time: 0
+
+  - name: 断言
+    case_id: event_query_002
+    description: 测试高级断言
+    is_run:
+    request:
+      method: GET
+      url: /albums/1
+      params:
+      headers:
+      body_type:
+      body:
+      files:
+    setup:
+      - wait_time: 0
+    teardown:
+      - extract:
+          key: test_env
+          type: env
+          jsonpath: $.status_code
+      - extract:
+          key: test_global
+          type: global
+          jsonpath: $.status_code
+      - assert: assert 200 == pm.response.get('status_code')
+      - assert: assert pm.response.get('status_code') == IsInt(exactly=200), '响应状态码非200'
+      - assert: assert int(pm.response.get('status_code')) == IsInt, '响应状态码错误'
+      - assert: assert 'postId' not in str(pm.response.get('content')), '没有返回content'
+      - assert:
+          check:
+          type: jsonschema
+          jsonschema:
+            type: object
+            properties:
+              userId:
+                type: integer
+              id:
+                type: integer
+              title:
+                type: string
+            required:
+              - userId
+              - id
+              - title
+      - assert:
+          check:
+          type: re
+          pattern: '^\b200\b'
+          jsonpath: $.status_code
+
+  - name: hook
+    case_id: event_create_001
+    description: 测试hook
+    is_run:
+    retry: 2
+    request:
+      method: POST
+      url: /users/1
+      params:
+      headers:
+      body_type: json
+      body:
+        title: foo
+        body: sum(a+b)=${sum_a_b(1,2)}; $test_cache ; $test_env ; ${test_global}.
+        userId: 1
+      files:
+    setup:
+      - hook: ${current_time()}
+    teardown:
+      - hook: ${random_phone()}
+      - assert: assert 200 == pm.response.get('status_code')
+
+  - name: 被关联用例
+    case_id: event_linked_001
+    description: 作为被关联简易用例而存在
+    is_run:
+    request:
+      method: GET
+      url: /comments
+      params:
+        postId: 1
+      headers:
+      body_type:
+      body:
+      files:
+
+  - name: 跨文件关联用例
+    case_id: event_relate_001
+    description: 测试跨文件关联用例
+    is_run:
+    request:
+      method: GET
+      url: /albums/1
+      params:
+      headers:
+      body_type:
+      body:
+      files:
+    setup:
+      - testcase: event_upload_004
```

### Comparing `httpfpt-0.6.2/httpfpt/enums/assert_type.py` & `httpfpt-0.6.3/httpfpt/enums/assert_type.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from enum import unique
-
-from httpfpt.enums import StrEnum
-
-
-@unique
-class AssertType(StrEnum):
-    equal = 'eq'
-    not_equal = 'not_eq'
-    greater_than = 'gt'
-    greater_than_or_equal = 'ge'
-    less_than = 'lt'
-    less_than_or_equal = 'le'
-    string_equal = 'str_eq'
-    length_equal = 'len_eq'
-    not_length_equal = 'not_len_eq'
-    length_less_than = 'len_lt'
-    length_less_than_or_equal = 'len_le'
-    length_greater_than = 'len_gt'
-    length_greater_than_or_equal = 'len_ge'
-    contains = 'contains'
-    not_contains = 'not_contains'
-    startswith = 'startswith'  # type: ignore
-    endswith = 'endswith'  # type: ignore
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from enum import unique
+
+from httpfpt.enums import StrEnum
+
+
+@unique
+class AssertType(StrEnum):
+    equal = 'eq'
+    not_equal = 'not_eq'
+    greater_than = 'gt'
+    greater_than_or_equal = 'ge'
+    less_than = 'lt'
+    less_than_or_equal = 'le'
+    string_equal = 'str_eq'
+    length_equal = 'len_eq'
+    not_length_equal = 'not_len_eq'
+    length_less_than = 'len_lt'
+    length_less_than_or_equal = 'len_le'
+    length_greater_than = 'len_gt'
+    length_greater_than_or_equal = 'len_ge'
+    contains = 'contains'
+    not_contains = 'not_contains'
+    startswith = 'startswith'  # type: ignore
+    endswith = 'endswith'  # type: ignore
```

### Comparing `httpfpt-0.6.2/httpfpt/pytest.ini` & `httpfpt-0.6.3/httpfpt/pytest.ini`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-; 官方指南: https://docs.pytest.org/en/8.0.x/reference/reference.html#configuration-options
-[pytest]
-; Use cases marked by xfail force the status to fail
-xfail_strict = True
-; Test case format
-python_files = test_*
-python_classes = Test*
-python_functions = test_*
-; Console output style
-console_output_style = progress
-; Mark use case status as xfail if parameter set in parameterization is empty
-empty_parameter_set_mark = xfail
-; Pytest minimum version requirements
-minversion = 8.0.0
-; Pytest plugin requirements
-required_plugins = pytest-html>=4.0.0
-; Collapse all tables of html report
-render_collapsed = all
-; Logging settings
-log_format = %(asctime)s | %(levelname)s | %(message)s
-log_date_format = %Y-%m-%d %H:%M:%S
-log_cli = False
-log_cli_format = %(asctime)s | %(levelname)s | %(message)s
-log_cli_date_format = %Y-%m-%d %H:%M:%S
-; Custom markers registration
-markers =
-    test_mark: this is a test mark
-    test_api: demo's test api mark
+; 官方指南: https://docs.pytest.org/en/8.0.x/reference/reference.html#configuration-options
+[pytest]
+; Use cases marked by xfail force the status to fail
+xfail_strict = True
+; Test case format
+python_files = test_*
+python_classes = Test*
+python_functions = test_*
+; Console output style
+console_output_style = progress
+; Mark use case status as xfail if parameter set in parameterization is empty
+empty_parameter_set_mark = xfail
+; Pytest minimum version requirements
+minversion = 8.0.0
+; Pytest plugin requirements
+required_plugins = pytest-html>=4.0.0
+; Collapse all tables of html report
+render_collapsed = all
+; Logging settings
+log_format = %(asctime)s | %(levelname)s | %(message)s
+log_date_format = %Y-%m-%d %H:%M:%S
+log_cli = False
+log_cli_format = %(asctime)s | %(levelname)s | %(message)s
+log_cli_date_format = %Y-%m-%d %H:%M:%S
+; Custom markers registration
+markers =
+    test_mark: this is a test mark
+    test_api: demo's test api mark
```

### Comparing `httpfpt-0.6.2/httpfpt/run.py` & `httpfpt-0.6.3/httpfpt/run.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,240 +1,240 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import os
-import shutil
-import subprocess
-
-from typing import Literal
-
-import pytest
-
-from httpfpt.common.log import log
-from httpfpt.common.yaml_handler import read_yaml
-from httpfpt.core.get_conf import httpfpt_config
-from httpfpt.core.path_conf import httpfpt_path
-from httpfpt.db.redis_db import redis_client
-from httpfpt.utils.case_auto_generator import auto_generate_testcases
-from httpfpt.utils.request import case_data_parse as case_data
-from httpfpt.utils.send_report.dingding import DingDing
-from httpfpt.utils.send_report.email import SendEmail
-from httpfpt.utils.send_report.feishu import FeiShu
-from httpfpt.utils.send_report.wechat import WeChat
-from httpfpt.utils.time_control import get_current_time
-
-
-def startup(
-    *args,
-    testcase_generate: bool,
-    log_level: Literal['-q', '-s', '-v', '-vv'],
-    case_path: str | None,
-    html_report: bool,
-    allure: bool,
-    allure_clear: bool,
-    allure_serve: bool,
-    maxfail: int,
-    x: bool,
-    strict_markers: bool,
-    capture: bool,
-    disable_warnings: bool,
-    **kwargs,
-) -> None:
-    """运行启动程序"""
-    if testcase_generate:
-        auto_generate_testcases()
-
-    run_args = [log_level]
-
-    default_case_path = os.sep.join([httpfpt_path.testcase_dir, httpfpt_config.PROJECT_NAME])
-    if case_path:
-        if '::' not in case_path:
-            raise ValueError(
-                '用例收集失败, 请检查路径参数 \n'
-                '类用例说明: \n'
-                '\t1. 项目目录下没有多级目录: case_path = "文件名::类名" \n'
-                '\t2. 项目目录下有多级目录: case_path = "目录名/.../文件名::类名" \n'
-                '函数用例说明: \n'
-                '\t1. 项目目录下没有多级目录: case_path = "文件名::类名::函数名" \n'
-                '\t2. 项目目录下有多级目录: case_path = "目录名/.../文件名::函数名"'
-            )
-        sep = os.path.sep
-        case_path = case_path.replace('/', sep)
-        run_path = os.sep.join([default_case_path, case_path])
-    else:
-        run_path = default_case_path
-    run_args.append(run_path)
-
-    html_report_filename = f'{httpfpt_config.PROJECT_NAME}_{get_current_time("%Y-%m-%d %H_%M_%S")}.html'
-    if html_report:
-        if not os.path.exists(httpfpt_path.html_report_dir):
-            os.makedirs(httpfpt_path.html_report_dir)
-        run_args.extend(
-            (
-                f'--html={os.path.join(httpfpt_path.html_report_dir, html_report_filename)}',
-                '--self-contained-html',
-            )
-        )
-
-    if allure:
-        run_args.append(f'--alluredir={httpfpt_path.allure_report_dir}')
-        if allure_clear:
-            run_args.append('--clean-alluredir')
-
-    if maxfail != 0:
-        run_args.append(f'--maxfail {maxfail}')
-
-    if x:
-        run_args.append('-x')
-
-    if strict_markers:
-        run_args.append('--strict-markers')
-
-    if capture:
-        run_args.append('--capture=tee-sys')
-
-    if disable_warnings:
-        run_args.append('--disable-warnings')
-
-    if len(args) > 0:
-        for i in args:
-            if i not in run_args:
-                run_args.append(i)
-    if len(kwargs) > 0:
-        for k, v in kwargs.items():
-            for i in run_args:
-                if '=' in i and k in i:
-                    run_args.remove(i)
-                    run_args.append(f'{k}={v}')
-    format_run_args = []
-    for i in run_args:
-        if '=' in i:
-            i_split = i.split('=')
-            new_i = i.replace(i_split[1], f'"{i_split[1]}"')
-            format_run_args.append(new_i)
-        else:
-            format_run_args.append(i)
-    run_pytest_command_args = ' '.join(
-        i if os.path.isdir(i) or i.startswith('-') else f'"{i}"' for i in format_run_args
-    )
-
-    log.info(
-        f'开始运行项目：{httpfpt_config.PROJECT_NAME}' if run_path == default_case_path else f'开始运行：{run_path}'
-    )
-    log.info(f'Pytest CLI: pytest {run_pytest_command_args}')
-    log.info('🚀 START')
-    pytest.main(run_args)
-    log.info('🏁 FINISH')
-
-    yaml_report_files = os.listdir(httpfpt_path.yaml_report_dir)
-    yaml_report_files.sort()
-    test_result = read_yaml(httpfpt_path.yaml_report_dir, filename=yaml_report_files[-1])
-
-    if html_report and httpfpt_config.EMAIL_SEND:
-        SendEmail(test_result, html_report_filename).send_report()
-
-    if httpfpt_config.DINGDING_SEND:
-        DingDing(test_result).send()
-
-    if httpfpt_config.FEISHU_SEND:
-        FeiShu(test_result).send()
-
-    if httpfpt_config.WECHAT_SEND:
-        WeChat(test_result).send()
-
-    if allure:
-        if not os.path.exists(httpfpt_path.allure_report_env_file):
-            shutil.copyfile(httpfpt_path.allure_env_file, httpfpt_path.allure_report_env_file)
-
-        if allure_serve:
-            subprocess.run(
-                f'allure generate {httpfpt_path.allure_report_dir} -o {httpfpt_path.allure_html_report_dir} --clean'
-            )
-            subprocess.run(f'allure serve {httpfpt_path.allure_report_dir}')
-
-
-def run(
-    *args,
-    # auto testcases
-    testcase_generate: bool = False,
-    # init
-    clean_cache: bool = False,
-    pydantic_verify: bool = True,
-    # log level
-    log_level: Literal['-q', '-s', '-v', '-vv'] = '-s',
-    # case path
-    case_path: str | None = None,
-    # html report
-    html_report: bool = True,
-    # allure
-    allure: bool = True,
-    allure_clear: bool = True,
-    allure_serve: bool = False,
-    # extra
-    maxfail: int = 0,
-    x: bool = False,
-    strict_markers: bool = False,
-    capture: bool = True,
-    disable_warnings: bool = True,
-    **kwargs,
-) -> None:
-    """
-    运行入口
-
-    :param args: pytest 运行参数
-    :param testcase_generate: 自动生成测试用例（跳过同名文件），建议通过 CLI 手动执行，默认关闭
-    :param clean_cache: 清理 redis 缓存数据，对于脏数据，这很有用，默认关闭
-    :param pydantic_verify: 用例数据完整架构 pydantic 快速检测, 默认开启
-    :param args: pytest 运行参数
-    :param log_level: 控制台打印输出级别, 默认"-s"
-    :param case_path: 指定当前项目下的测试用例函数, 默认为空，如果指定，则执行指定用例，否则执行全部
-    :param html_report: 生成 HTML 测试报告, 默认开启
-    :param allure: 生成 allure 测试报告, 默认开启
-    :param allure_clear: 清空 allure 报告历史记录, 默认开启
-    :param allure_serve: 自动打开 allure 测试报告服务， 默认关闭
-    :param maxfail: 用例运行失败数量，到达数量上限后终止运行，默认为 0，即不终止
-    :param x: 用例运行失败, 终止运行, 默认关闭
-    :param strict_markers: markers 严格模式, 对于设置 marker 装饰器的用例, 如果 marker 未在 pytest.ini 注册, 用例将报错
-    :param capture: 避免在使用输出模式为"v"和"s"时，html报告中的表格日志为空的情况, 默认开启
-    :param disable_warnings: 关闭控制台警告信息, 默认开启
-    :param kwargs: pytest 运行关键字参数
-    :return:
-    """
-    try:
-        logo = """\n
-         /$$   /$$ /$$$$$$$$ /$$$$$$$$ /$$$$$$$  /$$$$$$$$ /$$$$$$$  /$$$$$$$$
-        | $$  | $$|__  $$__/|__  $$__/| $$__  $$| $$_____/| $$__  $$|__  $$__/
-        | $$  | $$   | $$      | $$   | $$  | $$| $$      | $$  | $$   | $$
-        | $$$$$$$$   | $$      | $$   | $$$$$$$/| $$$$$$  | $$$$$$$/   | $$
-        | $$__  $$   | $$      | $$   | $$____/ | $$___/  | $$____/    | $$
-        | $$  | $$   | $$      | $$   | $$      | $$      | $$         | $$
-        | $$  | $$   | $$      | $$   | $$      | $$      | $$         | $$
-        |__/  |__/   |__/      |__/   |__/      |__/      |__/         |__/
-
-            """
-        log.info(logo)
-        redis_client.init()
-        case_data.clean_cache_data(clean_cache)
-        case_data.case_data_init(pydantic_verify)
-        case_data.case_id_unique_verify()
-        startup(
-            *args,
-            testcase_generate=testcase_generate,
-            log_level=log_level,
-            case_path=case_path,
-            html_report=html_report,
-            allure=allure,
-            allure_clear=allure_clear,
-            allure_serve=allure_serve,
-            maxfail=maxfail,
-            x=x,
-            strict_markers=strict_markers,
-            capture=capture,
-            disable_warnings=disable_warnings,
-            **kwargs,
-        )
-    except Exception as e:
-        log.error(f'运行异常：{e}')
-        import traceback
-
-        SendEmail({'error': traceback.format_exc()}).send_error()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import os
+import shutil
+import subprocess
+
+from typing import Literal
+
+import pytest
+
+from httpfpt.common.log import log
+from httpfpt.common.yaml_handler import read_yaml
+from httpfpt.core.get_conf import httpfpt_config
+from httpfpt.core.path_conf import httpfpt_path
+from httpfpt.db.redis_db import redis_client
+from httpfpt.utils.case_auto_generator import auto_generate_testcases
+from httpfpt.utils.request import case_data_parse as case_data
+from httpfpt.utils.send_report.dingding import DingDing
+from httpfpt.utils.send_report.email import SendEmail
+from httpfpt.utils.send_report.feishu import FeiShu
+from httpfpt.utils.send_report.wechat import WeChat
+from httpfpt.utils.time_control import get_current_time
+
+
+def startup(
+    *args,
+    testcase_generate: bool,
+    log_level: Literal['-q', '-s', '-v', '-vv'],
+    case_path: str | None,
+    html_report: bool,
+    allure: bool,
+    allure_clear: bool,
+    allure_serve: bool,
+    maxfail: int,
+    x: bool,
+    strict_markers: bool,
+    capture: bool,
+    disable_warnings: bool,
+    **kwargs,
+) -> None:
+    """运行启动程序"""
+    if testcase_generate:
+        auto_generate_testcases()
+
+    run_args = [log_level]
+
+    default_case_path = os.sep.join([httpfpt_path.testcase_dir, httpfpt_config.PROJECT_NAME])
+    if case_path:
+        if '::' not in case_path:
+            raise ValueError(
+                '用例收集失败, 请检查路径参数 \n'
+                '类用例说明: \n'
+                '\t1. 项目目录下没有多级目录: case_path = "文件名::类名" \n'
+                '\t2. 项目目录下有多级目录: case_path = "目录名/.../文件名::类名" \n'
+                '函数用例说明: \n'
+                '\t1. 项目目录下没有多级目录: case_path = "文件名::类名::函数名" \n'
+                '\t2. 项目目录下有多级目录: case_path = "目录名/.../文件名::函数名"'
+            )
+        sep = os.path.sep
+        case_path = case_path.replace('/', sep)
+        run_path = os.sep.join([default_case_path, case_path])
+    else:
+        run_path = default_case_path
+    run_args.append(run_path)
+
+    html_report_filename = f'{httpfpt_config.PROJECT_NAME}_{get_current_time("%Y-%m-%d %H_%M_%S")}.html'
+    if html_report:
+        if not os.path.exists(httpfpt_path.html_report_dir):
+            os.makedirs(httpfpt_path.html_report_dir)
+        run_args.extend(
+            (
+                f'--html={os.path.join(httpfpt_path.html_report_dir, html_report_filename)}',
+                '--self-contained-html',
+            )
+        )
+
+    if allure:
+        run_args.append(f'--alluredir={httpfpt_path.allure_report_dir}')
+        if allure_clear:
+            run_args.append('--clean-alluredir')
+
+    if maxfail != 0:
+        run_args.append(f'--maxfail {maxfail}')
+
+    if x:
+        run_args.append('-x')
+
+    if strict_markers:
+        run_args.append('--strict-markers')
+
+    if capture:
+        run_args.append('--capture=tee-sys')
+
+    if disable_warnings:
+        run_args.append('--disable-warnings')
+
+    if len(args) > 0:
+        for i in args:
+            if i not in run_args:
+                run_args.append(i)
+    if len(kwargs) > 0:
+        for k, v in kwargs.items():
+            for i in run_args:
+                if '=' in i and k in i:
+                    run_args.remove(i)
+                    run_args.append(f'{k}={v}')
+    format_run_args = []
+    for i in run_args:
+        if '=' in i:
+            i_split = i.split('=')
+            new_i = i.replace(i_split[1], f'"{i_split[1]}"')
+            format_run_args.append(new_i)
+        else:
+            format_run_args.append(i)
+    run_pytest_command_args = ' '.join(
+        i if os.path.isdir(i) or i.startswith('-') else f'"{i}"' for i in format_run_args
+    )
+
+    log.info(
+        f'开始运行项目：{httpfpt_config.PROJECT_NAME}' if run_path == default_case_path else f'开始运行：{run_path}'
+    )
+    log.info(f'Pytest CLI: pytest {run_pytest_command_args}')
+    log.info('🚀 START')
+    pytest.main(run_args)
+    log.info('🏁 FINISH')
+
+    yaml_report_files = os.listdir(httpfpt_path.yaml_report_dir)
+    yaml_report_files.sort()
+    test_result = read_yaml(httpfpt_path.yaml_report_dir, filename=yaml_report_files[-1])
+
+    if html_report and httpfpt_config.EMAIL_SEND:
+        SendEmail(test_result, html_report_filename).send_report()
+
+    if httpfpt_config.DINGDING_SEND:
+        DingDing(test_result).send()
+
+    if httpfpt_config.FEISHU_SEND:
+        FeiShu(test_result).send()
+
+    if httpfpt_config.WECHAT_SEND:
+        WeChat(test_result).send()
+
+    if allure:
+        if not os.path.exists(httpfpt_path.allure_report_env_file):
+            shutil.copyfile(httpfpt_path.allure_env_file, httpfpt_path.allure_report_env_file)
+
+        if allure_serve:
+            subprocess.run(
+                f'allure generate {httpfpt_path.allure_report_dir} -o {httpfpt_path.allure_html_report_dir} --clean'
+            )
+            subprocess.run(f'allure serve {httpfpt_path.allure_report_dir}')
+
+
+def run(
+    *args,
+    # auto testcases
+    testcase_generate: bool = False,
+    # init
+    clean_cache: bool = False,
+    pydantic_verify: bool = True,
+    # log level
+    log_level: Literal['-q', '-s', '-v', '-vv'] = '-s',
+    # case path
+    case_path: str | None = None,
+    # html report
+    html_report: bool = True,
+    # allure
+    allure: bool = True,
+    allure_clear: bool = True,
+    allure_serve: bool = False,
+    # extra
+    maxfail: int = 0,
+    x: bool = False,
+    strict_markers: bool = False,
+    capture: bool = True,
+    disable_warnings: bool = True,
+    **kwargs,
+) -> None:
+    """
+    运行入口
+
+    :param args: pytest 运行参数
+    :param testcase_generate: 自动生成测试用例（跳过同名文件），建议通过 CLI 手动执行，默认关闭
+    :param clean_cache: 清理 redis 缓存数据，对于脏数据，这很有用，默认关闭
+    :param pydantic_verify: 用例数据完整架构 pydantic 快速检测, 默认开启
+    :param args: pytest 运行参数
+    :param log_level: 控制台打印输出级别, 默认"-s"
+    :param case_path: 指定当前项目下的测试用例函数, 默认为空，如果指定，则执行指定用例，否则执行全部
+    :param html_report: 生成 HTML 测试报告, 默认开启
+    :param allure: 生成 allure 测试报告, 默认开启
+    :param allure_clear: 清空 allure 报告历史记录, 默认开启
+    :param allure_serve: 自动打开 allure 测试报告服务， 默认关闭
+    :param maxfail: 用例运行失败数量，到达数量上限后终止运行，默认为 0，即不终止
+    :param x: 用例运行失败, 终止运行, 默认关闭
+    :param strict_markers: markers 严格模式, 对于设置 marker 装饰器的用例, 如果 marker 未在 pytest.ini 注册, 用例将报错
+    :param capture: 避免在使用输出模式为"v"和"s"时，html报告中的表格日志为空的情况, 默认开启
+    :param disable_warnings: 关闭控制台警告信息, 默认开启
+    :param kwargs: pytest 运行关键字参数
+    :return:
+    """
+    try:
+        logo = """\n
+         /$$   /$$ /$$$$$$$$ /$$$$$$$$ /$$$$$$$  /$$$$$$$$ /$$$$$$$  /$$$$$$$$
+        | $$  | $$|__  $$__/|__  $$__/| $$__  $$| $$_____/| $$__  $$|__  $$__/
+        | $$  | $$   | $$      | $$   | $$  | $$| $$      | $$  | $$   | $$
+        | $$$$$$$$   | $$      | $$   | $$$$$$$/| $$$$$$  | $$$$$$$/   | $$
+        | $$__  $$   | $$      | $$   | $$____/ | $$___/  | $$____/    | $$
+        | $$  | $$   | $$      | $$   | $$      | $$      | $$         | $$
+        | $$  | $$   | $$      | $$   | $$      | $$      | $$         | $$
+        |__/  |__/   |__/      |__/   |__/      |__/      |__/         |__/
+
+            """
+        log.info(logo)
+        redis_client.init()
+        case_data.clean_cache_data(clean_cache)
+        case_data.case_data_init(pydantic_verify)
+        case_data.case_id_unique_verify()
+        startup(
+            *args,
+            testcase_generate=testcase_generate,
+            log_level=log_level,
+            case_path=case_path,
+            html_report=html_report,
+            allure=allure,
+            allure_clear=allure_clear,
+            allure_serve=allure_serve,
+            maxfail=maxfail,
+            x=x,
+            strict_markers=strict_markers,
+            capture=capture,
+            disable_warnings=disable_warnings,
+            **kwargs,
+        )
+    except Exception as e:
+        log.error(f'运行异常：{e}')
+        import traceback
+
+        SendEmail({'error': traceback.format_exc()}).send_error()
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/allure_control.py` & `httpfpt-0.6.3/httpfpt/utils/allure_control.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-from json import dumps as json_dumps
-from typing import Any
-
-import allure
-
-from allure_commons.types import AttachmentType
-
-from httpfpt.utils.file_control import get_file_property
-
-
-def allure_step(step: str, var: str | dict) -> None:
-    """
-    allure 操作步骤
-
-    :param step: 操作步骤
-    :param var: 操作步骤中的变量
-    :return:
-    """
-    with allure.step(step):
-        allure.attach(
-            body=json_dumps(var, ensure_ascii=False, indent=2) if isinstance(var, dict) else var,
-            name='JSON Serialize',
-            attachment_type=AttachmentType.JSON,
-        )
-
-
-def allure_attach(
-    body: Any = None, name: str | None = None, attachment_type: str = 'JSON', extension: Any = None
-) -> None:
-    """
-    allure 报告上传附件
-
-    :param body: 显示的内容
-    :param name: 附件名称
-    :param attachment_type: 文件类型，默认 JSON
-    :param extension:
-    :return:
-    """
-    allure.attach(
-        body=body,
-        name=name,
-        attachment_type=getattr(AttachmentType, attachment_type.upper(), None),
-        extension=extension,
-    )
-
-
-def allure_attach_file(filepath: str, name: str | None = None, extension: Any = None) -> None:
-    """
-    allure 报告上传附件
-
-    :param filepath: 文件路径
-    :param name:
-    :param extension:
-    :return:
-    """
-    file_property = get_file_property(filepath)
-    filename = file_property[0]
-    filetype = file_property[2]
-    if filetype == 'txt':
-        filetype = 'TEXT'
-    elif filetype == 'uri':
-        filetype = 'URI_LIST'
-    allure.attach.file(
-        source=filepath,
-        name=name or filename,
-        attachment_type=getattr(AttachmentType, filetype.upper(), None),
-        extension=extension,
-    )
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from json import dumps as json_dumps
+from typing import Any
+
+import allure
+
+from allure_commons.types import AttachmentType
+
+from httpfpt.utils.file_control import get_file_property
+
+
+def allure_step(step: str, var: str | dict) -> None:
+    """
+    allure 操作步骤
+
+    :param step: 操作步骤
+    :param var: 操作步骤中的变量
+    :return:
+    """
+    with allure.step(step):
+        allure.attach(
+            body=json_dumps(var, ensure_ascii=False, indent=2) if isinstance(var, dict) else var,
+            name='JSON Serialize',
+            attachment_type=AttachmentType.JSON,
+        )
+
+
+def allure_attach(
+    body: Any = None, name: str | None = None, attachment_type: str = 'JSON', extension: Any = None
+) -> None:
+    """
+    allure 报告上传附件
+
+    :param body: 显示的内容
+    :param name: 附件名称
+    :param attachment_type: 文件类型，默认 JSON
+    :param extension:
+    :return:
+    """
+    allure.attach(
+        body=body,
+        name=name,
+        attachment_type=getattr(AttachmentType, attachment_type.upper(), None),
+        extension=extension,
+    )
+
+
+def allure_attach_file(filepath: str, name: str | None = None, extension: Any = None) -> None:
+    """
+    allure 报告上传附件
+
+    :param filepath: 文件路径
+    :param name:
+    :param extension:
+    :return:
+    """
+    file_property = get_file_property(filepath)
+    filename = file_property[0]
+    filetype = file_property[2]
+    if filetype == 'txt':
+        filetype = 'TEXT'
+    elif filetype == 'uri':
+        filetype = 'URI_LIST'
+    allure.attach.file(
+        source=filepath,
+        name=name or filename,
+        attachment_type=getattr(AttachmentType, filetype.upper(), None),
+        extension=extension,
+    )
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/assert_control.py` & `httpfpt-0.6.3/httpfpt/utils/assert_control.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,435 +1,436 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import re
-
-from decimal import Decimal
-from typing import Any
-
-from jsonpath import findall
-from jsonschema import validate
-from jsonschema.exceptions import ValidationError
-
-from httpfpt.common.errors import AssertSyntaxError, JsonPathFindError
-from httpfpt.common.log import log
-from httpfpt.db.mysql_db import mysql_client
-from httpfpt.enums.assert_type import AssertType
-from httpfpt.enums.sql_type import SqlType
-
-
-class Asserter:
-    def _code_asserter(self, response: dict, assert_text: str) -> None:
-        """
-        **代码断言器, 像 pytest 断言一样使用它**
-
-        基本语法::
-            1. assert  期望值 条件 取值表达式(pm.response.get()...)
-            2. assert 期望值 条件 取值表达式(pm.response.get()...), 错误信息(可选, 如果不填写, 记得去掉前面的逗号, 建议填写)
-
-        扩展语法::
-            dirty-equals 断言库专属, 请不要在断言内容中使用带有函数引用的断言方式, 仅支持简易验证操作, 使用前,
-            请阅读它的使用文档, `github <https://github.com/samuelcolvin/dirty-equals>`_
-
-            1. assert 取值表达式(pm.response.get()...) 条件(== 或 !=) 类型
-
-        取值说明::
-            与 postman 相似, 但又完全不同, 你只能通过全程手动脚本来控制断言数据, 并且, 需要以 pm.response.get 作为比较值的开头,
-            后面获取的内容中, 需要以 .get() 为基础, 视情况添加 python 代码的一些简单方法并确保它们符合常规 assert 语法
-
-        取值范围::
-
-            {
-                'url': '',
-                'status_code': 200,
-                'elapsed': 0,
-                'headers': {},
-                'cookies': {},
-                'result': {},
-                'content': {},
-                'text': {},
-                'stat': {'execute_time': 'None'},
-                'sql_data': {},
-            }
-
-        一些简单的例子::
-            1. assert 200 == pm.response.get('status_code')
-            2. assert 'success' != pm.response.get('msg')[1]
-            3. assert 'com' in pm.response.get('content').get('url')
-            4. assert pm.response.get('header').get('httpfpt') == IsDict(version=0.0.1)
-            5. assert pm.response.get('content').get('id') == IsUUID
-
-        :param response:
-        :param assert_text:
-        :return:
-        """  # noqa: E501
-        log.info(f'执行 code 断言：{assert_text}')
-        self._exec_code_assert(response, assert_text)
-
-    def _json_asserter(self, response: dict, assert_text: dict) -> None:
-        """
-        **json 提取断言器**
-
-        基本语法::
-            1. $.key
-            2. ...
-
-        语法说明::
-            符合 jsonpath 取值语法即可, `jsonpath <https://jg-rp.github.io/python-jsonpath/syntax/>`_
-
-        取值范围::
-            与 code 断言器一致
-
-        一些简单的例子::
-            1. $.status_code
-            2. $.sql_data.username
-            3. $.headers.*
-
-        :param response:
-        :param assert_text:
-        :return:
-        """
-        if not isinstance(assert_text, dict):
-            raise AssertSyntaxError('json 断言内容格式错误, 请检查断言脚本是否为 dict 格式')
-        try:
-            assert_check = assert_text['check']
-            assert_value = assert_text['value']
-            assert_type = assert_text['type']
-            assert_jsonpath = assert_text['jsonpath']
-        except KeyError as e:
-            raise AssertSyntaxError(f'json 断言格式错误, 请检查: {e}')
-        else:
-            response_value = findall(assert_jsonpath, response)
-            if response_value:
-                log.info(f'执行 json 断言：{assert_text}')
-                self._exec_json_assert(assert_check, assert_value, assert_type, response_value[0])
-            else:
-                raise JsonPathFindError(f'jsonpath 取值失败, 表达式: {assert_jsonpath}')
-
-    def _sql_asserter(self, assert_text: dict) -> None:
-        """
-        **sql 提取断言器**
-
-        提取方法与 json 断言器相同
-
-        :param assert_text:
-        :return:
-        """
-        if not isinstance(assert_text, dict):
-            raise AssertSyntaxError('sql 断言内容格式错误, 请检查断言脚本是否为 dict 格式')
-        try:
-            assert_check = assert_text['check']
-            assert_value = assert_text['value']
-            assert_type = assert_text['type']
-            assert_sql = assert_text['sql']
-            assert_jsonpath = assert_text['jsonpath']
-        except KeyError as e:
-            raise AssertSyntaxError(f'SQL 断言格式错误, 请检查: {e}')
-        else:
-            if assert_sql.split(' ')[0].upper() != SqlType.select:
-                raise AssertSyntaxError(f'SQL 断言 {assert_check}:{assert_type} 执行失败，请检查 SQL 是否为 DQL 类型')
-            sql_data = mysql_client.exec_case_sql(assert_sql)
-            if not isinstance(sql_data, dict):
-                raise JsonPathFindError('jsonpath 取值失败, SQL 语句执行结果不是有效的 dict 类型')
-            sql_value = findall(assert_jsonpath, sql_data)
-            if sql_value:
-                log.info(f'执行 SQL 断言：{assert_text}')
-                self._exec_json_assert(assert_check, assert_value, assert_type, sql_value[0])
-            else:
-                raise JsonPathFindError(f'jsonpath 取值失败, 表达式: {assert_jsonpath}')
-
-    @staticmethod
-    def _jsonschema_asserter(response: dict, assert_text: dict) -> None:
-        """
-        **jsonschema 断言器**
-
-        提取方法与 json 断言器相同
-
-        :param response:
-        :param assert_text:
-        :return:
-        """
-        if not isinstance(assert_text, dict):
-            raise AssertSyntaxError('jsonschema 断言内容格式错误, 请检查断言脚本是否为 dict 格式')
-        try:
-            assert_check = assert_text['check']
-            assert_type = assert_text['type']
-            assert_jsonschema = assert_text['jsonschema']
-        except KeyError as e:
-            raise AssertSyntaxError(f'jsonschema 断言格式错误, 请检查: {e}')
-        else:
-            if assert_type != 'jsonschema':
-                raise AssertSyntaxError('jsonschema 断言类型错误，类型必须为 "jsonschema"')
-            log.info(f'执行 jsonschema 断言：{assert_text}')
-            try:
-                validate(response['json'], assert_jsonschema)
-            except ValidationError as e:
-                log.error(f'{assert_check or e}')
-                raise e
-
-    @staticmethod
-    def _re_asserter(response: dict, assert_text: dict) -> None:
-        """
-        **正则断言器**
-
-        :param response:
-        :param assert_text:
-        :return:
-        """
-        if not isinstance(assert_text, dict):
-            raise AssertSyntaxError('正则断言内容格式错误, 请检查断言脚本是否为 dict 格式')
-        try:
-            assert_check = assert_text['check']
-            assert_type = assert_text['type']
-            assert_pattern = assert_text['pattern']
-            assert_jsonpath = assert_text['jsonpath']
-        except KeyError as e:
-            raise AssertSyntaxError(f'正则断言格式错误, 请检查: {e}')
-        else:
-            if assert_type != 're':
-                raise AssertSyntaxError('正则断言类型错误，类型必须为 "re"')
-            response_value = findall(assert_jsonpath, response)
-            if response_value:
-                log.info(f'执行 re 断言：{assert_text}')
-                result = re.match(assert_pattern, str(response_value[0]))
-                if not result:
-                    e = assert_check or '正则断言失败，响应内容与正则表达式不相符'
-                    raise AssertionError(e)
-            else:
-                raise JsonPathFindError(f'jsonpath 取值失败, 表达式: {assert_jsonpath}')
-
-    @staticmethod
-    def _exec_code_assert(response: dict, assert_text: str) -> None:
-        """
-        执行 code 断言
-
-        :param response:
-        :param assert_text:
-        :return:
-        """
-        assert_split = assert_text.split(' ')
-        if not assert_text.startswith('assert '):
-            raise AssertSyntaxError(f'code 断言取值表达式格式错误, 不符合语法规范: {assert_text}')
-        if len(assert_split) < 4 or len(assert_split) > 6:
-            raise AssertSyntaxError(f'code 断言取值表达式格式错误, 不符合语法规范: {assert_text}')
-        else:
-
-            def exec_assertion() -> None:
-                """执行断言（闭包函数）"""
-                get_code = pm_code.split('.')[2:]
-                if len(get_code) == 1:
-                    use_code = get_code[0]
-                else:
-                    use_code = '.'.join(get_code)
-                # 如果断言有转型
-                if use_code.endswith('))'):
-                    use_code = use_code.replace('))', ')')
-                if not use_code.startswith('get('):
-                    raise AssertSyntaxError(
-                        'code 断言取值表达式格式错误, 取值表达式条件不允许, 请在首位改用 get() 方法取值'
-                    )
-                else:
-                    try:
-                        response_value = eval(f'{response}.{use_code}')
-                    except Exception as e:
-                        err_msg = str(e.args).replace("'", '"').replace('\\', '')
-                        raise AssertSyntaxError(f'code 断言取值表达式格式错误, {use_code} 取值失败, 详情: {err_msg}')
-                    else:
-                        # 执行断言
-                        py_conversion_functions_exec_re = re.compile(
-                            rf'(\b(?:{py_conversion_functions_re_str}))\((.*?)\)(?=[^)]*$)'  # noqa: ignore
-                        )
-                        format_assert_text = py_conversion_functions_exec_re.sub(
-                            lambda x: x.group(1) + f'("""{response_value}""")', assert_text
-                        )
-                        if 'pm.response.get' in format_assert_text:
-                            format_assert_text = format_assert_text.replace(pm_code, '{}', 1).format(response_value)
-                        if len(assert_split) == 4:
-                            # stdout 作为没有自定义断言错误时的信息补充
-                            # 当断言错误触发时, 如果错误信息中包含自定义错误, 此项可忽略
-                            log.warning('Warning: 此 code 断言未自定义错误提示信息')
-                        if dirty_equals_assert:
-                            exec('from dirty_equals import *')
-                        exec(format_assert_text)
-
-            py_conversion_functions_re_str = 'str|int|float|bool|list|tuple|set|dict'
-            py_conversion_functions_pm_get_re = re.compile(rf'^({py_conversion_functions_re_str})\(pm\.response\.get')
-            # 是否 dirty-equals 断言表达式
-            dirty_equals_assert = True
-            if not assert_split[1].startswith('pm.response.get'):
-                if not py_conversion_functions_pm_get_re.match(assert_split[1]):
-                    dirty_equals_assert = False
-            if dirty_equals_assert:
-                if assert_split[2] not in ['==', '!=']:
-                    raise AssertSyntaxError(
-                        f'code 断言取值表达式格式错误, 含有不支持的 dirty-equals 断言类型 {assert_split[2]}'
-                    )
-                # 处理比较值获取代码
-                pm_code = assert_split[1]
-                # 执行断言
-                exec_assertion()
-            else:
-                assert_expr_type = ['==', '!=', '>', '<', '>=', '<=', 'in', 'not']
-                if assert_split[2] not in assert_expr_type:
-                    raise AssertSyntaxError(
-                        f'code 断言表达式格式错误, 含有不支持的断言类型: {assert_split[2]}, 仅支持: {assert_expr_type}'
-                    )
-                else:
-                    if assert_split[2] == 'not':
-                        if assert_split[3] != 'in':
-                            raise AssertSyntaxError(
-                                f'code 断言表达式格式错误, 含有不支持的断言类型: {" ".join(assert_split[2:4])}'
-                            )
-                        else:
-                            if not assert_split[4].startswith('pm.response.get'):
-                                if not py_conversion_functions_pm_get_re.match(assert_split[4]):
-                                    raise AssertSyntaxError(
-                                        f'code 断言取值表达式格式错误, 含有不支持的断言取值表达式: {assert_split[4]}'
-                                    )
-                            # 如果包含自定义错误信息
-                            if len(assert_split) == 6:
-                                pm_code = assert_split[4].replace(',', '')
-                            else:
-                                pm_code = assert_split[4]
-                    else:
-                        # 非 dirty-equals 或 not in 断言表达式
-                        if not assert_split[3].startswith('pm.response.get'):
-                            if not py_conversion_functions_pm_get_re.match(assert_split[3]):
-                                raise AssertSyntaxError(
-                                    f'code 断言取值表达式格式错误, 含有不支持的断言取值表达式: {assert_split[3]}'
-                                )
-                        if len(assert_split) == 5:
-                            pm_code = assert_split[3].replace(',', '')
-                        else:
-                            pm_code = assert_split[3]
-                    # 执行断言
-                    exec_assertion()
-
-    @staticmethod
-    def _exec_json_assert(assert_check: str | None, expected_value: Any, assert_type: str, actual_value: Any) -> None:
-        """
-        执行 jsonpath 断言
-
-        :param assert_check:
-        :param expected_value:
-        :param assert_type:
-        :param actual_value:
-        :return:
-        """
-        if assert_type == AssertType.equal:
-            assert expected_value == actual_value, (
-                assert_check or f'预期结果: {Decimal(str(expected_value))} 不等于实际结果: {Decimal(str(actual_value))}'
-            )
-
-        elif assert_type == AssertType.not_equal:
-            assert expected_value != actual_value, (
-                assert_check or f'预期结果: {Decimal(str(expected_value))} 等于实际结果: {Decimal(str(actual_value))}'
-            )
-
-        elif assert_type == AssertType.greater_than:
-            assert expected_value > actual_value, (
-                assert_check or f'预期结果: {Decimal(str(expected_value))} 不大于实际结果: {Decimal(str(actual_value))}'
-            )
-
-        elif assert_type == AssertType.greater_than_or_equal:
-            assert expected_value >= actual_value, (
-                assert_check
-                or f'预期结果: {Decimal(str(expected_value))} 不大于等于实际结果: {Decimal(str(actual_value))}'
-            )
-
-        elif assert_type == AssertType.less_than:
-            assert expected_value < actual_value, (
-                assert_check or f'预期结果: {Decimal(str(expected_value))} 不小于实际结果: {Decimal(str(actual_value))}'
-            )
-
-        elif assert_type == AssertType.less_than_or_equal:
-            assert expected_value <= actual_value, (
-                assert_check
-                or f'预期结果: {Decimal(str(expected_value))} 不小于等于实际结果: {Decimal(str(actual_value))}'
-            )
-
-        elif assert_type == AssertType.string_equal:
-            assert str(expected_value) == str(actual_value), (
-                assert_check or f'预期结果(str): {str(expected_value)} 不等于实际结果(str): {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.length_equal:
-            assert len(str(expected_value)) == len(str(actual_value)), (
-                assert_check or f'预期结果: {str(expected_value)} 长度不等于实际结果: {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.not_length_equal:
-            assert len(str(expected_value)) != len(str(actual_value)), (
-                assert_check or f'预期结果: {str(expected_value)} 长度等于实际结果: {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.length_greater_than:
-            assert len(str(expected_value)) > len(str(actual_value)), (
-                assert_check or f'预期结果: {str(expected_value)} 长度不大于实际结果: {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.length_greater_than_or_equal:
-            assert len(str(expected_value)) >= len(str(actual_value)), (
-                assert_check or f'预期结果: {str(expected_value)} 长度不大于等于实际结果: {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.length_less_than:
-            assert len(str(expected_value)) < len(str(actual_value)), (
-                assert_check or f'预期结果: {str(expected_value)} 长度不小于实际结果: {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.length_less_than_or_equal:
-            assert len(str(expected_value)) <= len(str(actual_value)), (
-                assert_check or f'预期结果: {str(expected_value)} 长度不小于等于实际结果: {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.contains:
-            assert str(expected_value) in str(actual_value), (
-                assert_check or f'预期结果: {str(expected_value)} 不包含实际结果: {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.not_contains:
-            assert str(expected_value) not in str(actual_value), (
-                assert_check or f'预期结果: {str(expected_value)} 包含实际结果: {str(actual_value)}'
-            )
-
-        elif assert_type == AssertType.startswith:
-            assert str(actual_value).startswith(str(expected_value)), (
-                assert_check or f'实际结果: {str(actual_value)} 的开头不是预期结果: {str(expected_value)}'
-            )
-
-        elif assert_type == AssertType.endswith:
-            assert str(actual_value).endswith(str(expected_value)), (
-                assert_check or f'实际结果: {str(actual_value)} 的结尾不是预期结果: {str(expected_value)}'
-            )
-
-        else:
-            raise ValueError(f'断言表达式格式错误, 含有不支持的断言类型: {assert_type}')
-
-    def exec_asserter(self, response: dict, assert_text: str | dict | None) -> None:
-        """
-        根据断言内容自动选择断言器执行
-
-        :param response:
-        :param assert_text:
-        :return:
-        """
-        if isinstance(assert_text, str):
-            self._code_asserter(response, assert_text)
-        elif isinstance(assert_text, dict):
-            sql = assert_text.get('sql')
-            jsonschema = assert_text.get('jsonschema')
-            pattern = assert_text.get('pattern')
-            if sql:
-                self._sql_asserter(assert_text)
-            elif jsonschema:
-                self._jsonschema_asserter(response, assert_text)
-            elif pattern:
-                self._re_asserter(response, assert_text)
-            else:
-                self._json_asserter(response, assert_text)
-        else:
-            raise AssertSyntaxError(f'断言表达式格式错误: {assert_text}')
-
-
-asserter = Asserter()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import re
+
+from decimal import Decimal
+from typing import Any
+
+from jsonpath import findall
+from jsonschema import validate
+from jsonschema.exceptions import ValidationError
+
+from httpfpt.common.errors import AssertSyntaxError, JsonPathFindError
+from httpfpt.common.log import log
+from httpfpt.db.mysql_db import mysql_client
+from httpfpt.enums.assert_type import AssertType
+from httpfpt.enums.sql_type import SqlType
+
+
+class Asserter:
+    def _code_asserter(self, response: dict, assert_text: str) -> None:
+        """
+        **代码断言器, 像 pytest 断言一样使用它**
+
+        基本语法::
+            1. assert  期望值 条件 取值表达式(pm.response.get()...)
+            2. assert 期望值 条件 取值表达式(pm.response.get()...), 错误信息(可选, 如果不填写, 记得去掉前面的逗号, 建议填写)
+
+        扩展语法::
+            dirty-equals 断言库专属, 请不要在断言内容中使用带有函数引用的断言方式, 仅支持简易验证操作, 使用前,
+            请阅读它的使用文档, `github <https://github.com/samuelcolvin/dirty-equals>`_
+
+            1. assert 取值表达式(pm.response.get()...) 条件(== 或 !=) 类型
+
+        取值说明::
+            与 postman 相似, 但又完全不同, 你只能通过全程手动脚本来控制断言数据, 并且, 需要以 pm.response.get 作为比较值的开头,
+            后面获取的内容中, 需要以 .get() 为基础, 视情况添加 python 代码的一些简单方法并确保它们符合常规 assert 语法
+
+        取值范围::
+
+            {
+                'url': '',
+                'status_code': 200,
+                'elapsed': 0,
+                'headers': {},
+                'cookies': {},
+                'result': {},
+                'content': {},
+                'text': {},
+                'stat': {'execute_time': 'None'},
+                'sql_data': {},
+            }
+
+        一些简单的例子::
+            1. assert 200 == pm.response.get('status_code')
+            2. assert 'success' != pm.response.get('msg')[1]
+            3. assert 'com' in pm.response.get('content').get('url')
+            4. assert pm.response.get('header').get('httpfpt') == IsDict(version=0.0.1)
+            5. assert pm.response.get('content').get('id') == IsUUID
+
+        :param response:
+        :param assert_text:
+        :return:
+        """  # noqa: E501
+        log.info(f'执行 code 断言：{assert_text}')
+        self._exec_code_assert(response, assert_text)
+
+    def _json_asserter(self, response: dict, assert_text: dict) -> None:
+        """
+        **json 提取断言器**
+
+        基本语法::
+            1. $.key
+            2. ...
+
+        语法说明::
+            符合 jsonpath 取值语法即可, `jsonpath <https://jg-rp.github.io/python-jsonpath/syntax/>`_
+
+        取值范围::
+            与 code 断言器一致
+
+        一些简单的例子::
+            1. $.status_code
+            2. $.sql_data.username
+            3. $.headers.*
+
+        :param response:
+        :param assert_text:
+        :return:
+        """
+        if not isinstance(assert_text, dict):
+            raise AssertSyntaxError('json 断言内容格式错误, 请检查断言脚本是否为 dict 格式')
+        try:
+            assert_check = assert_text['check']
+            assert_value = assert_text['value']
+            assert_type = assert_text['type']
+            assert_jsonpath = assert_text['jsonpath']
+        except KeyError as e:
+            raise AssertSyntaxError(f'json 断言格式错误, 请检查: {e}')
+        else:
+            response_value = findall(assert_jsonpath, response)
+            if response_value:
+                log.info(f'执行 json 断言：{assert_text}')
+                self._exec_json_assert(assert_check, assert_value, assert_type, response_value[0])
+            else:
+                raise JsonPathFindError(f'jsonpath 取值失败, 表达式: {assert_jsonpath}')
+
+    def _sql_asserter(self, assert_text: dict) -> None:
+        """
+        **sql 提取断言器**
+
+        提取方法与 json 断言器相同
+
+        :param assert_text:
+        :return:
+        """
+        if not isinstance(assert_text, dict):
+            raise AssertSyntaxError('sql 断言内容格式错误, 请检查断言脚本是否为 dict 格式')
+        try:
+            assert_check = assert_text['check']
+            assert_value = assert_text['value']
+            assert_type = assert_text['type']
+            assert_sql = assert_text['sql']
+            assert_fetch = assert_text.get('fetch')
+            assert_jsonpath = assert_text['jsonpath']
+        except KeyError as e:
+            raise AssertSyntaxError(f'SQL 断言格式错误, 请检查: {e}')
+        else:
+            if assert_sql.split(' ')[0].upper() != SqlType.select:
+                raise AssertSyntaxError(f'SQL 断言 {assert_check}:{assert_type} 执行失败，请检查 SQL 是否为 DQL 类型')
+            sql_data = mysql_client.exec_case_sql(assert_sql, assert_fetch)
+            if not isinstance(sql_data, dict):
+                raise JsonPathFindError('jsonpath 取值失败, SQL 语句执行结果不是有效的 dict 类型')
+            sql_value = findall(assert_jsonpath, sql_data)
+            if sql_value:
+                log.info(f'执行 SQL 断言：{assert_text}')
+                self._exec_json_assert(assert_check, assert_value, assert_type, sql_value[0])
+            else:
+                raise JsonPathFindError(f'jsonpath 取值失败, 表达式: {assert_jsonpath}')
+
+    @staticmethod
+    def _jsonschema_asserter(response: dict, assert_text: dict) -> None:
+        """
+        **jsonschema 断言器**
+
+        提取方法与 json 断言器相同
+
+        :param response:
+        :param assert_text:
+        :return:
+        """
+        if not isinstance(assert_text, dict):
+            raise AssertSyntaxError('jsonschema 断言内容格式错误, 请检查断言脚本是否为 dict 格式')
+        try:
+            assert_check = assert_text['check']
+            assert_type = assert_text['type']
+            assert_jsonschema = assert_text['jsonschema']
+        except KeyError as e:
+            raise AssertSyntaxError(f'jsonschema 断言格式错误, 请检查: {e}')
+        else:
+            if assert_type != 'jsonschema':
+                raise AssertSyntaxError('jsonschema 断言类型错误，类型必须为 "jsonschema"')
+            log.info(f'执行 jsonschema 断言：{assert_text}')
+            try:
+                validate(response['json'], assert_jsonschema)
+            except ValidationError as e:
+                log.error(f'{assert_check or e}')
+                raise e
+
+    @staticmethod
+    def _re_asserter(response: dict, assert_text: dict) -> None:
+        """
+        **正则断言器**
+
+        :param response:
+        :param assert_text:
+        :return:
+        """
+        if not isinstance(assert_text, dict):
+            raise AssertSyntaxError('正则断言内容格式错误, 请检查断言脚本是否为 dict 格式')
+        try:
+            assert_check = assert_text['check']
+            assert_type = assert_text['type']
+            assert_pattern = assert_text['pattern']
+            assert_jsonpath = assert_text['jsonpath']
+        except KeyError as e:
+            raise AssertSyntaxError(f'正则断言格式错误, 请检查: {e}')
+        else:
+            if assert_type != 're':
+                raise AssertSyntaxError('正则断言类型错误，类型必须为 "re"')
+            response_value = findall(assert_jsonpath, response)
+            if response_value:
+                log.info(f'执行 re 断言：{assert_text}')
+                result = re.match(assert_pattern, str(response_value[0]))
+                if not result:
+                    e = assert_check or '正则断言失败，响应内容与正则表达式不相符'
+                    raise AssertionError(e)
+            else:
+                raise JsonPathFindError(f'jsonpath 取值失败, 表达式: {assert_jsonpath}')
+
+    @staticmethod
+    def _exec_code_assert(response: dict, assert_text: str) -> None:
+        """
+        执行 code 断言
+
+        :param response:
+        :param assert_text:
+        :return:
+        """
+        assert_split = assert_text.split(' ')
+        if not assert_text.startswith('assert '):
+            raise AssertSyntaxError(f'code 断言取值表达式格式错误, 不符合语法规范: {assert_text}')
+        if len(assert_split) < 4 or len(assert_split) > 6:
+            raise AssertSyntaxError(f'code 断言取值表达式格式错误, 不符合语法规范: {assert_text}')
+        else:
+
+            def exec_assertion() -> None:
+                """执行断言（闭包函数）"""
+                get_code = pm_code.split('.')[2:]
+                if len(get_code) == 1:
+                    use_code = get_code[0]
+                else:
+                    use_code = '.'.join(get_code)
+                # 如果断言有转型
+                if use_code.endswith('))'):
+                    use_code = use_code.replace('))', ')')
+                if not use_code.startswith('get('):
+                    raise AssertSyntaxError(
+                        'code 断言取值表达式格式错误, 取值表达式条件不允许, 请在首位改用 get() 方法取值'
+                    )
+                else:
+                    try:
+                        response_value = eval(f'{response}.{use_code}')
+                    except Exception as e:
+                        err_msg = str(e.args).replace("'", '"').replace('\\', '')
+                        raise AssertSyntaxError(f'code 断言取值表达式格式错误, {use_code} 取值失败, 详情: {err_msg}')
+                    else:
+                        # 执行断言
+                        py_conversion_functions_exec_re = re.compile(
+                            rf'(\b(?:{py_conversion_functions_re_str}))\((.*?)\)(?=[^)]*$)'  # noqa: ignore
+                        )
+                        format_assert_text = py_conversion_functions_exec_re.sub(
+                            lambda x: x.group(1) + f'("""{response_value}""")', assert_text
+                        )
+                        if 'pm.response.get' in format_assert_text:
+                            format_assert_text = format_assert_text.replace(pm_code, '{}', 1).format(response_value)
+                        if len(assert_split) == 4:
+                            # stdout 作为没有自定义断言错误时的信息补充
+                            # 当断言错误触发时, 如果错误信息中包含自定义错误, 此项可忽略
+                            log.warning('Warning: 此 code 断言未自定义错误提示信息')
+                        if dirty_equals_assert:
+                            exec('from dirty_equals import *')
+                        exec(format_assert_text)
+
+            py_conversion_functions_re_str = 'str|int|float|bool|list|tuple|set|dict'
+            py_conversion_functions_pm_get_re = re.compile(rf'^({py_conversion_functions_re_str})\(pm\.response\.get')
+            # 是否 dirty-equals 断言表达式
+            dirty_equals_assert = True
+            if not assert_split[1].startswith('pm.response.get'):
+                if not py_conversion_functions_pm_get_re.match(assert_split[1]):
+                    dirty_equals_assert = False
+            if dirty_equals_assert:
+                if assert_split[2] not in ['==', '!=']:
+                    raise AssertSyntaxError(
+                        f'code 断言取值表达式格式错误, 含有不支持的 dirty-equals 断言类型 {assert_split[2]}'
+                    )
+                # 处理比较值获取代码
+                pm_code = assert_split[1]
+                # 执行断言
+                exec_assertion()
+            else:
+                assert_expr_type = ['==', '!=', '>', '<', '>=', '<=', 'in', 'not']
+                if assert_split[2] not in assert_expr_type:
+                    raise AssertSyntaxError(
+                        f'code 断言表达式格式错误, 含有不支持的断言类型: {assert_split[2]}, 仅支持: {assert_expr_type}'
+                    )
+                else:
+                    if assert_split[2] == 'not':
+                        if assert_split[3] != 'in':
+                            raise AssertSyntaxError(
+                                f'code 断言表达式格式错误, 含有不支持的断言类型: {" ".join(assert_split[2:4])}'
+                            )
+                        else:
+                            if not assert_split[4].startswith('pm.response.get'):
+                                if not py_conversion_functions_pm_get_re.match(assert_split[4]):
+                                    raise AssertSyntaxError(
+                                        f'code 断言取值表达式格式错误, 含有不支持的断言取值表达式: {assert_split[4]}'
+                                    )
+                            # 如果包含自定义错误信息
+                            if len(assert_split) == 6:
+                                pm_code = assert_split[4].replace(',', '')
+                            else:
+                                pm_code = assert_split[4]
+                    else:
+                        # 非 dirty-equals 或 not in 断言表达式
+                        if not assert_split[3].startswith('pm.response.get'):
+                            if not py_conversion_functions_pm_get_re.match(assert_split[3]):
+                                raise AssertSyntaxError(
+                                    f'code 断言取值表达式格式错误, 含有不支持的断言取值表达式: {assert_split[3]}'
+                                )
+                        if len(assert_split) == 5:
+                            pm_code = assert_split[3].replace(',', '')
+                        else:
+                            pm_code = assert_split[3]
+                    # 执行断言
+                    exec_assertion()
+
+    @staticmethod
+    def _exec_json_assert(assert_check: str | None, expected_value: Any, assert_type: str, actual_value: Any) -> None:
+        """
+        执行 jsonpath 断言
+
+        :param assert_check:
+        :param expected_value:
+        :param assert_type:
+        :param actual_value:
+        :return:
+        """
+        if assert_type == AssertType.equal:
+            assert expected_value == actual_value, (
+                assert_check or f'预期结果: {Decimal(str(expected_value))} 不等于实际结果: {Decimal(str(actual_value))}'
+            )
+
+        elif assert_type == AssertType.not_equal:
+            assert expected_value != actual_value, (
+                assert_check or f'预期结果: {Decimal(str(expected_value))} 等于实际结果: {Decimal(str(actual_value))}'
+            )
+
+        elif assert_type == AssertType.greater_than:
+            assert expected_value > actual_value, (
+                assert_check or f'预期结果: {Decimal(str(expected_value))} 不大于实际结果: {Decimal(str(actual_value))}'
+            )
+
+        elif assert_type == AssertType.greater_than_or_equal:
+            assert expected_value >= actual_value, (
+                assert_check
+                or f'预期结果: {Decimal(str(expected_value))} 不大于等于实际结果: {Decimal(str(actual_value))}'
+            )
+
+        elif assert_type == AssertType.less_than:
+            assert expected_value < actual_value, (
+                assert_check or f'预期结果: {Decimal(str(expected_value))} 不小于实际结果: {Decimal(str(actual_value))}'
+            )
+
+        elif assert_type == AssertType.less_than_or_equal:
+            assert expected_value <= actual_value, (
+                assert_check
+                or f'预期结果: {Decimal(str(expected_value))} 不小于等于实际结果: {Decimal(str(actual_value))}'
+            )
+
+        elif assert_type == AssertType.string_equal:
+            assert str(expected_value) == str(actual_value), (
+                assert_check or f'预期结果(str): {str(expected_value)} 不等于实际结果(str): {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.length_equal:
+            assert len(str(expected_value)) == len(str(actual_value)), (
+                assert_check or f'预期结果: {str(expected_value)} 长度不等于实际结果: {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.not_length_equal:
+            assert len(str(expected_value)) != len(str(actual_value)), (
+                assert_check or f'预期结果: {str(expected_value)} 长度等于实际结果: {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.length_greater_than:
+            assert len(str(expected_value)) > len(str(actual_value)), (
+                assert_check or f'预期结果: {str(expected_value)} 长度不大于实际结果: {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.length_greater_than_or_equal:
+            assert len(str(expected_value)) >= len(str(actual_value)), (
+                assert_check or f'预期结果: {str(expected_value)} 长度不大于等于实际结果: {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.length_less_than:
+            assert len(str(expected_value)) < len(str(actual_value)), (
+                assert_check or f'预期结果: {str(expected_value)} 长度不小于实际结果: {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.length_less_than_or_equal:
+            assert len(str(expected_value)) <= len(str(actual_value)), (
+                assert_check or f'预期结果: {str(expected_value)} 长度不小于等于实际结果: {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.contains:
+            assert str(expected_value) in str(actual_value), (
+                assert_check or f'预期结果: {str(expected_value)} 不包含实际结果: {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.not_contains:
+            assert str(expected_value) not in str(actual_value), (
+                assert_check or f'预期结果: {str(expected_value)} 包含实际结果: {str(actual_value)}'
+            )
+
+        elif assert_type == AssertType.startswith:
+            assert str(actual_value).startswith(str(expected_value)), (
+                assert_check or f'实际结果: {str(actual_value)} 的开头不是预期结果: {str(expected_value)}'
+            )
+
+        elif assert_type == AssertType.endswith:
+            assert str(actual_value).endswith(str(expected_value)), (
+                assert_check or f'实际结果: {str(actual_value)} 的结尾不是预期结果: {str(expected_value)}'
+            )
+
+        else:
+            raise ValueError(f'断言表达式格式错误, 含有不支持的断言类型: {assert_type}')
+
+    def exec_asserter(self, response: dict, assert_text: str | dict | None) -> None:
+        """
+        根据断言内容自动选择断言器执行
+
+        :param response:
+        :param assert_text:
+        :return:
+        """
+        if isinstance(assert_text, str):
+            self._code_asserter(response, assert_text)
+        elif isinstance(assert_text, dict):
+            sql = assert_text.get('sql')
+            jsonschema = assert_text.get('jsonschema')
+            pattern = assert_text.get('pattern')
+            if sql:
+                self._sql_asserter(assert_text)
+            elif jsonschema:
+                self._jsonschema_asserter(response, assert_text)
+            elif pattern:
+                self._re_asserter(response, assert_text)
+            else:
+                self._json_asserter(response, assert_text)
+        else:
+            raise AssertSyntaxError(f'断言表达式格式错误: {assert_text}')
+
+
+asserter = Asserter()
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/auth_plugins.py` & `httpfpt-0.6.3/httpfpt/utils/auth_plugins.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import json
-
-from functools import lru_cache
-
-import requests
-
-from jsonpath import findall
-
-from httpfpt.common.errors import AuthError, SendRequestError
-from httpfpt.common.yaml_handler import read_yaml
-from httpfpt.core.path_conf import httpfpt_path
-from httpfpt.db.redis_db import redis_client
-from httpfpt.enums.request.auth import AuthType
-from httpfpt.utils.enum_control import get_enum_values
-
-
-class AuthPlugins:
-    def __init__(self) -> None:
-        self.auth_data = self.get_auth_data()
-        self.is_auth = self.auth_data['is_auth']
-        self.auth_type = self.auth_data['auth_type']
-        self.auth_type_verify()
-        self.timeout = self.auth_data[f'{self.auth_type}']['timeout'] or 86400
-
-    @lru_cache
-    def get_auth_data(self) -> dict:
-        """获取授权数据"""
-        auth_data = read_yaml(httpfpt_path.auth_conf_dir, filename='auth.yaml')
-        return auth_data
-
-    def auth_type_verify(self) -> None:
-        """授权类型检查"""
-        _allow_auth_type = get_enum_values(AuthType)
-        if self.auth_type not in _allow_auth_type:
-            raise AuthError(f'认证类型错误, 允许 {_allow_auth_type} 之一, 请检查认证配置文件')
-
-    def request_auth(self) -> requests.Response:
-        try:
-            url = self.auth_data[f'{self.auth_type}']['url']
-            username = self.auth_data[f'{self.auth_type}']['username']
-            password = self.auth_data[f'{self.auth_type}']['password']
-            headers = self.auth_data[f'{self.auth_type}']['headers']
-            request_data = {
-                'url': url,
-                'data': {'username': username, 'password': password},
-                'headers': headers,
-                'proxies': {'http': None, 'https': None},
-            }
-            if 'application/json' in str(headers):
-                request_data.update({'json': request_data.pop('data')})
-            response = requests.post(**request_data)
-            response.raise_for_status()
-        except Exception as e:
-            raise SendRequestError(f'授权接口请求响应异常: {e}')
-        return response
-
-    @property
-    def bearer_token(self) -> str:
-        cache_bearer_token = redis_client.get(f'{redis_client.token_prefix}:bearer_token', logging=False)
-        if cache_bearer_token:
-            token = cache_bearer_token
-        else:
-            res = self.request_auth()
-            jp_token = findall(self.auth_data[f'{self.auth_type}']['token_key'], res.json())
-            token = jp_token[0]
-            if not token:
-                raise AuthError('Token 获取失败，请检查登录接口响应或 token 提取表达式')
-            redis_client.set(f'{redis_client.token_prefix}:bearer_token', token, ex=self.timeout)
-        return token
-
-    @property
-    def bearer_token_custom(self) -> str:
-        cache_bearer_token_custom = redis_client.get(f'{redis_client.token_prefix}:bearer_token_custom', logging=False)
-        if cache_bearer_token_custom:
-            token = cache_bearer_token_custom
-        else:
-            token = self.auth_data[f'{self.auth_type}']['token']
-            redis_client.set(f'{redis_client.token_prefix}:bearer_token_custom', token, ex=self.timeout)
-        return token
-
-    @property
-    def header_cookie(self) -> dict:
-        cache_cookie = redis_client.get(f'{redis_client.cookie_prefix}:header_cookie', logging=False)
-        if cache_cookie:
-            cookies = json.loads(cache_cookie)
-        else:
-            res = self.request_auth()
-            res_cookie = res.cookies
-            cookies = {k: v for k, v in res_cookie.items()}
-            if not cookies:
-                raise AuthError('Cookie 获取失败，请检查登录接口响应')
-            redis_client.set(
-                f'{redis_client.cookie_prefix}:header_cookie', json.dumps(cookies, ensure_ascii=False), ex=self.timeout
-            )
-        return cookies
-
-
-auth = AuthPlugins()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+import json
+
+from functools import lru_cache
+
+import requests
+
+from jsonpath import findall
+
+from httpfpt.common.errors import AuthError, SendRequestError
+from httpfpt.common.yaml_handler import read_yaml
+from httpfpt.core.path_conf import httpfpt_path
+from httpfpt.db.redis_db import redis_client
+from httpfpt.enums.request.auth import AuthType
+from httpfpt.utils.enum_control import get_enum_values
+
+
+class AuthPlugins:
+    def __init__(self) -> None:
+        self.auth_data = self.get_auth_data()
+        self.is_auth = self.auth_data['is_auth']
+        self.auth_type = self.auth_data['auth_type']
+        self.auth_type_verify()
+        self.timeout = self.auth_data[f'{self.auth_type}']['timeout'] or 86400
+
+    @lru_cache
+    def get_auth_data(self) -> dict:
+        """获取授权数据"""
+        auth_data = read_yaml(httpfpt_path.auth_conf_dir, filename='auth.yaml')
+        return auth_data
+
+    def auth_type_verify(self) -> None:
+        """授权类型检查"""
+        _allow_auth_type = get_enum_values(AuthType)
+        if self.auth_type not in _allow_auth_type:
+            raise AuthError(f'认证类型错误, 允许 {_allow_auth_type} 之一, 请检查认证配置文件')
+
+    def request_auth(self) -> requests.Response:
+        try:
+            url = self.auth_data[f'{self.auth_type}']['url']
+            username = self.auth_data[f'{self.auth_type}']['username']
+            password = self.auth_data[f'{self.auth_type}']['password']
+            headers = self.auth_data[f'{self.auth_type}']['headers']
+            request_data = {
+                'url': url,
+                'data': {'username': username, 'password': password},
+                'headers': headers,
+                'proxies': {'http': None, 'https': None},
+            }
+            if 'application/json' in str(headers):
+                request_data.update({'json': request_data.pop('data')})
+            response = requests.post(**request_data)
+            response.raise_for_status()
+        except Exception as e:
+            raise SendRequestError(f'授权接口请求响应异常: {e}')
+        return response
+
+    @property
+    def bearer_token(self) -> str:
+        cache_bearer_token = redis_client.get(f'{redis_client.token_prefix}:bearer_token', logging=False)
+        if cache_bearer_token:
+            token = cache_bearer_token
+        else:
+            res = self.request_auth()
+            jp_token = findall(self.auth_data[f'{self.auth_type}']['token_key'], res.json())
+            token = jp_token[0]
+            if not token:
+                raise AuthError('Token 获取失败，请检查登录接口响应或 token 提取表达式')
+            redis_client.set(f'{redis_client.token_prefix}:bearer_token', token, ex=self.timeout)
+        return token
+
+    @property
+    def bearer_token_custom(self) -> str:
+        cache_bearer_token_custom = redis_client.get(f'{redis_client.token_prefix}:bearer_token_custom', logging=False)
+        if cache_bearer_token_custom:
+            token = cache_bearer_token_custom
+        else:
+            token = self.auth_data[f'{self.auth_type}']['token']
+            redis_client.set(f'{redis_client.token_prefix}:bearer_token_custom', token, ex=self.timeout)
+        return token
+
+    @property
+    def header_cookie(self) -> dict:
+        cache_cookie = redis_client.get(f'{redis_client.cookie_prefix}:header_cookie', logging=False)
+        if cache_cookie:
+            cookies = json.loads(cache_cookie)
+        else:
+            res = self.request_auth()
+            res_cookie = res.cookies
+            cookies = {k: v for k, v in res_cookie.items()}
+            if not cookies:
+                raise AuthError('Cookie 获取失败，请检查登录接口响应')
+            redis_client.set(
+                f'{redis_client.cookie_prefix}:header_cookie', json.dumps(cookies, ensure_ascii=False), ex=self.timeout
+            )
+        return cookies
+
+
+auth = AuthPlugins()
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/case_auto_generator.py` & `httpfpt-0.6.3/httpfpt/utils/case_auto_generator.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import os.path
-
-from pathlib import Path
-
-from httpfpt.core.get_conf import httpfpt_config
-from httpfpt.core.path_conf import httpfpt_path
-from httpfpt.utils.file_control import get_file_property, search_all_case_data_files, search_all_testcase_files
-from httpfpt.utils.rich_console import console
-
-
-def auto_generate_testcases(rewrite: bool = False) -> None:
-    """
-    自动创建测试用例
-
-    :param rewrite:
-    :return:
-    """
-    # 获取所用用例数据文件
-    case_data_files = search_all_case_data_files()
-    if len(case_data_files) == 0:
-        raise FileNotFoundError('自动生成用例失败，未在指定项目下找到测试用例数据文件，请检查项目目录是否正确')
-
-    # 获取所有测试用例文件
-    testcase_files = search_all_testcase_files()
-
-    # 获取所有用例文件名
-    case_filenames = []
-    case_file_root_names = []
-    for _ in case_data_files:
-        case_filenames.append(_)
-        case_file_root_names.append(get_file_property(_)[1])
-
-    # 获取所有测试用例数据文件名
-    testcase_filenames = []
-    for _ in testcase_files:
-        testcase_filenames.append(get_file_property(_)[0])
-
-    # 获取需要创建的测试用例文件名
-    create_file_root_names = []
-    for root_name in case_file_root_names:
-        if not rewrite:
-            if (
-                (root_name if root_name.startswith('test_') else 'test_' + root_name) + '.py'
-            ) not in testcase_filenames:
-                create_file_root_names.append(root_name)
-        else:
-            create_file_root_names.append(root_name)
-    if len(create_file_root_names) == 0:
-        console.print('😝 用例已经很完善了, 添加新测试用例数据后再来生成吧~')
-        return
-
-    console.print('⏳ 疯狂自动生成中...')
-
-    for create_file_root_name in create_file_root_names:
-        for case_filename in case_filenames:
-            file_property = get_file_property(case_filename)
-            if create_file_root_name == file_property[1]:
-                testcase_class_name = ''.join(name.title() for name in create_file_root_name.split('_'))
-                testcase_func_name = create_file_root_name
-                if not create_file_root_name.startswith('test_'):
-                    testcase_class_name = 'Test' + testcase_class_name
-                    testcase_func_name = 'test_' + testcase_func_name
-                case_code = f'''#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import allure
-import pytest
-
-from httpfpt.common.send_request import send_request
-from httpfpt.utils.request.case_data_parse import get_testcase_data
-
-allure_data, ddt_data, ids = get_testcase_data(filename='{file_property[0]}')
-
-
-@allure.epic(allure_data['epic'])
-@allure.feature(allure_data['feature'])
-class {testcase_class_name}:
-    """{testcase_class_name.replace('Test', '')}"""
-
-    @allure.story(allure_data['story'])
-    @pytest.mark.parametrize('data', ddt_data, ids=ids)
-    def {testcase_func_name}(self, data):
-        """{create_file_root_name}"""
-        send_request.send_request(data)
-'''
-                # 创建测试用例文件
-                tag = case_filename.split(httpfpt_config.PROJECT_NAME)[1].split(os.path.sep)[1:-1]
-                new_testcase_filename = testcase_func_name + '.py'
-                if tag:
-                    case_path = os.path.join(
-                        httpfpt_path.testcase_dir, httpfpt_config.PROJECT_NAME, *tag, new_testcase_filename
-                    )
-                else:
-                    case_path = os.path.join(
-                        httpfpt_path.testcase_dir, httpfpt_config.PROJECT_NAME, new_testcase_filename
-                    )
-                new_testcase_dir = Path(case_path).parent  # type: ignore
-                if not new_testcase_dir.exists():
-                    new_testcase_dir.mkdir(parents=True, exist_ok=True)
-                with open(case_path, 'w', encoding='utf-8') as f:
-                    f.write(case_code)
-                console.print(f'📄 Created: {new_testcase_filename}')
-
-    console.print('✅ 测试用例自动生成完成')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+import os.path
+
+from pathlib import Path
+
+from httpfpt.core.get_conf import httpfpt_config
+from httpfpt.core.path_conf import httpfpt_path
+from httpfpt.utils.file_control import get_file_property, search_all_case_data_files, search_all_testcase_files
+from httpfpt.utils.rich_console import console
+
+
+def auto_generate_testcases(rewrite: bool = False) -> None:
+    """
+    自动创建测试用例
+
+    :param rewrite:
+    :return:
+    """
+    # 获取所用用例数据文件
+    case_data_files = search_all_case_data_files()
+    if len(case_data_files) == 0:
+        raise FileNotFoundError('自动生成用例失败，未在指定项目下找到测试用例数据文件，请检查项目目录是否正确')
+
+    # 获取所有测试用例文件
+    testcase_files = search_all_testcase_files()
+
+    # 获取所有用例文件名
+    case_filenames = []
+    case_file_root_names = []
+    for _ in case_data_files:
+        case_filenames.append(_)
+        case_file_root_names.append(get_file_property(_)[1])
+
+    # 获取所有测试用例数据文件名
+    testcase_filenames = []
+    for _ in testcase_files:
+        testcase_filenames.append(get_file_property(_)[0])
+
+    # 获取需要创建的测试用例文件名
+    create_file_root_names = []
+    for root_name in case_file_root_names:
+        if not rewrite:
+            if (
+                (root_name if root_name.startswith('test_') else 'test_' + root_name) + '.py'
+            ) not in testcase_filenames:
+                create_file_root_names.append(root_name)
+        else:
+            create_file_root_names.append(root_name)
+    if len(create_file_root_names) == 0:
+        console.print('😝 用例已经很完善了, 添加新测试用例数据后再来生成吧~')
+        return
+
+    console.print('⏳ 疯狂自动生成中...')
+
+    for create_file_root_name in create_file_root_names:
+        for case_filename in case_filenames:
+            file_property = get_file_property(case_filename)
+            if create_file_root_name == file_property[1]:
+                testcase_class_name = ''.join(name.title() for name in create_file_root_name.split('_'))
+                testcase_func_name = create_file_root_name
+                if not create_file_root_name.startswith('test_'):
+                    testcase_class_name = 'Test' + testcase_class_name
+                    testcase_func_name = 'test_' + testcase_func_name
+                case_code = f'''#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+import allure
+import pytest
+
+from httpfpt.common.send_request import send_request
+from httpfpt.utils.request.case_data_parse import get_testcase_data
+
+allure_data, ddt_data, ids = get_testcase_data(filename='{file_property[0]}')
+
+
+@allure.epic(allure_data['epic'])
+@allure.feature(allure_data['feature'])
+class {testcase_class_name}:
+    """{testcase_class_name.replace('Test', '')}"""
+
+    @allure.story(allure_data['story'])
+    @pytest.mark.parametrize('data', ddt_data, ids=ids)
+    def {testcase_func_name}(self, data):
+        """{create_file_root_name}"""
+        send_request.send_request(data)
+'''
+                # 创建测试用例文件
+                tag = case_filename.split(httpfpt_config.PROJECT_NAME)[1].split(os.path.sep)[1:-1]
+                new_testcase_filename = testcase_func_name + '.py'
+                if tag:
+                    case_path = os.path.join(
+                        httpfpt_path.testcase_dir, httpfpt_config.PROJECT_NAME, *tag, new_testcase_filename
+                    )
+                else:
+                    case_path = os.path.join(
+                        httpfpt_path.testcase_dir, httpfpt_config.PROJECT_NAME, new_testcase_filename
+                    )
+                new_testcase_dir = Path(case_path).parent  # type: ignore
+                if not new_testcase_dir.exists():
+                    new_testcase_dir.mkdir(parents=True, exist_ok=True)
+                with open(case_path, 'w', encoding='utf-8') as f:
+                    f.write(case_code)
+                console.print(f'📄 Created: {new_testcase_filename}')
+
+    console.print('✅ 测试用例自动生成完成')
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/cli/about_testcase.py` & `httpfpt-0.6.3/httpfpt/utils/cli/about_testcase.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import os.path
-
-import cappa
-
-from pydantic import ValidationError
-from rich.prompt import Confirm
-
-from httpfpt.common.json_handler import read_json_file
-from httpfpt.common.yaml_handler import read_yaml
-from httpfpt.core.get_conf import httpfpt_config
-from httpfpt.core.path_conf import httpfpt_path
-from httpfpt.enums.case_data_type import CaseDataType
-from httpfpt.schemas.case_data import CaseData
-from httpfpt.utils.case_auto_generator import auto_generate_testcases
-from httpfpt.utils.file_control import get_file_property, search_all_case_data_files
-from httpfpt.utils.rich_console import console
-
-
-def testcase_data_verify(verify: str) -> None:
-    """测试数据验证"""
-    msg: str = ''
-    try:
-        count: int = 0
-        if verify.lower() == 'all':
-            console.print('\n🔥 开始验证所有测试数据结构...')
-            file_list = search_all_case_data_files()
-            for file in file_list:
-                file_type = get_file_property(file)[2]
-                if file_type == CaseDataType.JSON:
-                    file_data = read_json_file(file)
-                else:
-                    file_data = read_yaml(file)
-                CaseData.model_validate(file_data)
-        else:
-            console.print(f'🔥 开始验证 {verify} 测试数据结构...')
-            file_type = get_file_property(verify)[2]
-            if os.path.isfile(verify):
-                data_path = os.path.join(httpfpt_path.case_data_dir, httpfpt_config.PROJECT_NAME)
-                if file_type == CaseDataType.JSON:
-                    file_data = read_json_file(str(data_path), verify)
-                else:
-                    file_data = read_yaml(str(data_path), verify)
-            else:
-                if file_type == CaseDataType.JSON:
-                    file_data = read_json_file(verify)
-                else:
-                    file_data = read_yaml(verify)
-            CaseData.model_validate(file_data)
-    except ValidationError as e:
-        count = e.error_count()
-        msg += str(e)
-    except Exception as e:
-        console.print(f'\n❌ 验证测试数据 {verify} 结构失败: {e}')
-        raise e
-    if count > 0:
-        raise cappa.Exit(f'\n❌ 验证测试数据 {verify} 结构失败: {msg}', code=1)
-    else:
-        console.print('✅ 验证测试数据结构成功')
-
-
-def generate_testcases() -> None:
-    """生成测试用例"""
-    console.print(
-        '\n'
-        'Warning: 此操作生成的测试用例是依赖测试数据文件而决定的,\n'
-        '         如果你手动创建的测试用例与测试数据文件名称相吻合,\n'
-        '         那么此操作将不能完全保证你的手动创建测试用例继续保留,\n'
-        '         如果你依然执行此操作, 请谨慎选择重新生成所有测试用例。\n',
-        style='bold #ffd700',
-    )
-    result = Confirm.ask('⚠️ 是否重新生成所有测试用例?', default=False)
-    try:
-        if result:
-            console.print('🔥 开始重新生成所有测试用例...')
-            auto_generate_testcases(rewrite=True)
-        else:
-            console.print('🔥 开始生成新测试用例...')
-            auto_generate_testcases()
-    except Exception as e:
-        console.print(f'\n❌ 自动生成测试用例失败: {e}')
-        raise e
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+import os.path
+
+import cappa
+
+from pydantic import ValidationError
+from rich.prompt import Confirm
+
+from httpfpt.common.json_handler import read_json_file
+from httpfpt.common.yaml_handler import read_yaml
+from httpfpt.core.get_conf import httpfpt_config
+from httpfpt.core.path_conf import httpfpt_path
+from httpfpt.enums.case_data_type import CaseDataType
+from httpfpt.schemas.case_data import CaseData
+from httpfpt.utils.case_auto_generator import auto_generate_testcases
+from httpfpt.utils.file_control import get_file_property, search_all_case_data_files
+from httpfpt.utils.rich_console import console
+
+
+def testcase_data_verify(verify: str) -> None:
+    """测试数据验证"""
+    msg: str = ''
+    try:
+        count: int = 0
+        if verify.lower() == 'all':
+            console.print('\n🔥 开始验证所有测试数据结构...')
+            file_list = search_all_case_data_files()
+            for file in file_list:
+                file_type = get_file_property(file)[2]
+                if file_type == CaseDataType.JSON:
+                    file_data = read_json_file(file)
+                else:
+                    file_data = read_yaml(file)
+                CaseData.model_validate(file_data)
+        else:
+            console.print(f'🔥 开始验证 {verify} 测试数据结构...')
+            file_type = get_file_property(verify)[2]
+            if os.path.isfile(verify):
+                data_path = os.path.join(httpfpt_path.case_data_dir, httpfpt_config.PROJECT_NAME)
+                if file_type == CaseDataType.JSON:
+                    file_data = read_json_file(str(data_path), verify)
+                else:
+                    file_data = read_yaml(str(data_path), verify)
+            else:
+                if file_type == CaseDataType.JSON:
+                    file_data = read_json_file(verify)
+                else:
+                    file_data = read_yaml(verify)
+            CaseData.model_validate(file_data)
+    except ValidationError as e:
+        count = e.error_count()
+        msg += str(e)
+    except Exception as e:
+        console.print(f'\n❌ 验证测试数据 {verify} 结构失败: {e}')
+        raise e
+    if count > 0:
+        raise cappa.Exit(f'\n❌ 验证测试数据 {verify} 结构失败: {msg}', code=1)
+    else:
+        console.print('✅ 验证测试数据结构成功')
+
+
+def generate_testcases() -> None:
+    """生成测试用例"""
+    console.print(
+        '\n'
+        'Warning: 此操作生成的测试用例是依赖测试数据文件而决定的,\n'
+        '         如果你手动创建的测试用例与测试数据文件名称相吻合,\n'
+        '         那么此操作将不能完全保证你的手动创建测试用例继续保留,\n'
+        '         如果你依然执行此操作, 请谨慎选择重新生成所有测试用例。\n',
+        style='bold #ffd700',
+    )
+    result = Confirm.ask('⚠️ 是否重新生成所有测试用例?', default=False)
+    try:
+        if result:
+            console.print('🔥 开始重新生成所有测试用例...')
+            auto_generate_testcases(rewrite=True)
+        else:
+            console.print('🔥 开始生成新测试用例...')
+            auto_generate_testcases()
+    except Exception as e:
+        console.print(f'\n❌ 自动生成测试用例失败: {e}')
+        raise e
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/cli/import_case_data.py` & `httpfpt-0.6.3/httpfpt/utils/cli/import_case_data.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-from rich.prompt import Confirm
-
-from httpfpt.utils.data_manage.apifox import ApiFoxParser
-from httpfpt.utils.data_manage.git_repo import GitRepoPaser
-from httpfpt.utils.data_manage.openapi import SwaggerParser
-from httpfpt.utils.rich_console import console
-
-
-def import_openapi_case_data(openapi: tuple[str, str]) -> None:
-    """导入 openapi 测试用例数据"""
-    console.print(f'\n📩 正在导入测试用例数据到项目: [#0087ff]{openapi[1]}[/#0087ff]')
-    result = Confirm.ask('❓ 确认执行此操作吗?', default=False)
-    if result:
-        console.print('🔥 开始导入 openapi 数据...')
-        try:
-            SwaggerParser().import_openapi_to_yaml(openapi[0], openapi[1])
-        except Exception as e:
-            console.print('\n❌ 导入 openapi 数据失败')
-            raise e
-
-
-def import_apifox_case_data(apifox: tuple[str, str]) -> None:
-    """导入 apifox 测试用例数据"""
-    console.print(
-        '\n'
-        'Beta: 此命令目前处于测试阶段, 请谨慎使用。\n'
-        'Warning: 如果现有文件名与导入文件名相同, 此命令目前会覆盖写入用例数据, 请谨慎操作。\n',
-        style='bold #ffd700',
-    )
-    result = Confirm.ask('⚠️ 确认执行此操作吗?', default=False)
-    if result:
-        console.print('🔥 开始导入 apifox 数据...')
-        try:
-            ApiFoxParser().import_apifox_to_yaml(apifox[0], apifox[1])
-        except Exception as e:
-            console.print('\n❌ 导入 apifox 数据失败:')
-            raise e
-
-
-def import_har_case_data(har: tuple[str, str]) -> None:
-    """导入 har 测试用例数据"""
-    console.print('\n🚧 此功能暂未开发')
-
-
-def import_jmeter_case_data(jmeter: tuple[str, str]) -> None:
-    """导入 jmeter 测试用例数据"""
-    console.print('\n🚧 此功能暂未开发')
-
-
-def import_postman_case_data(postman: tuple[str, str]) -> None:
-    """导入 postman 测试用例数据"""
-    console.print('\n🚧 此功能暂未开发')
-
-
-def import_git_case_data(src: str) -> None:
-    """导入 git 仓库测试数据"""
-    console.print(f'\n🚀 正在导入 git 仓库测试数据到本地: {src}')
-    console.print('🔥 开始导入 git 仓库测试数据...\n')
-    try:
-        GitRepoPaser.import_git_to_local(src)
-    except Exception as e:
-        console.print(f'\n❌ 导入 git 仓库测试数据失败: {e}')
-        raise e
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from rich.prompt import Confirm
+
+from httpfpt.utils.data_manage.apifox import ApiFoxParser
+from httpfpt.utils.data_manage.git_repo import GitRepoPaser
+from httpfpt.utils.data_manage.openapi import SwaggerParser
+from httpfpt.utils.rich_console import console
+
+
+def import_openapi_case_data(openapi: tuple[str, str]) -> None:
+    """导入 openapi 测试用例数据"""
+    console.print(f'\n📩 正在导入测试用例数据到项目: [#0087ff]{openapi[1]}[/#0087ff]')
+    result = Confirm.ask('❓ 确认执行此操作吗?', default=False)
+    if result:
+        console.print('🔥 开始导入 openapi 数据...')
+        try:
+            SwaggerParser().import_openapi_to_yaml(openapi[0], openapi[1])
+        except Exception as e:
+            console.print('\n❌ 导入 openapi 数据失败')
+            raise e
+
+
+def import_apifox_case_data(apifox: tuple[str, str]) -> None:
+    """导入 apifox 测试用例数据"""
+    console.print(
+        '\n'
+        'Beta: 此命令目前处于测试阶段, 请谨慎使用。\n'
+        'Warning: 如果现有文件名与导入文件名相同, 此命令目前会覆盖写入用例数据, 请谨慎操作。\n',
+        style='bold #ffd700',
+    )
+    result = Confirm.ask('⚠️ 确认执行此操作吗?', default=False)
+    if result:
+        console.print('🔥 开始导入 apifox 数据...')
+        try:
+            ApiFoxParser().import_apifox_to_yaml(apifox[0], apifox[1])
+        except Exception as e:
+            console.print('\n❌ 导入 apifox 数据失败:')
+            raise e
+
+
+def import_har_case_data(har: tuple[str, str]) -> None:
+    """导入 har 测试用例数据"""
+    console.print('\n🚧 此功能暂未开发')
+
+
+def import_jmeter_case_data(jmeter: tuple[str, str]) -> None:
+    """导入 jmeter 测试用例数据"""
+    console.print('\n🚧 此功能暂未开发')
+
+
+def import_postman_case_data(postman: tuple[str, str]) -> None:
+    """导入 postman 测试用例数据"""
+    console.print('\n🚧 此功能暂未开发')
+
+
+def import_git_case_data(src: str) -> None:
+    """导入 git 仓库测试数据"""
+    console.print(f'\n🚀 正在导入 git 仓库测试数据到本地: {src}')
+    console.print('🔥 开始导入 git 仓库测试数据...\n')
+    try:
+        GitRepoPaser.import_git_to_local(src)
+    except Exception as e:
+        console.print(f'\n❌ 导入 git 仓库测试数据失败: {e}')
+        raise e
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/cli/new_project.py` & `httpfpt-0.6.3/httpfpt/utils/cli/new_project.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import os
-import platform
-import shutil
-
-from importlib.resources import path as import_path
-from time import sleep
-
-import cappa
-
-from rich.prompt import Prompt
-from rich.syntax import Syntax
-
-from httpfpt.utils.rich_console import console
-
-
-def create_new_project() -> None:
-    name = Prompt.ask('❓ Set your project a name', default='httpfpt_project')
-    path = Prompt.ask('❓ Set your project path (relative or absolute path, which automatically parses.)', default='.')
-    if path != '.':
-        if not os.path.isdir(path):
-            raise cappa.Exit(f'\n❌ The "{path}" is not a directory', code=1)
-    with console.status('[bold green]The project is being created...[/]'):
-        console.print(end='\n')
-        sleep(2)
-
-        project_path = os.path.abspath(os.sep.join([path, name]))
-        if os.path.exists(project_path):
-            raise cappa.Exit(f'\n❌ The "{project_path}" directory is not empty', code=1)
-        os.makedirs(project_path)
-        console.print('📁 Created the project folder')
-        sleep(2)
-
-        core_path = os.path.join(project_path, 'core')
-        with import_path('httpfpt.core', '') as core_data:
-            patterns = ['__init__.py', 'get_conf.py', 'path_conf.py']
-            shutil.copytree(core_data, core_path, ignore=shutil.ignore_patterns(*patterns))
-            console.print('📄 Created core files')
-            sleep(2)
-
-        data_path = os.path.join(project_path, 'data')
-        with import_path('httpfpt.data', '') as case_data:
-            shutil.copytree(case_data, data_path)
-            console.print('📄 Created case data samples')
-            sleep(2)
-
-        init_file = os.path.join(project_path, '__init__.py')
-        with import_path('httpfpt', '__init__.py') as pytest_init:
-            shutil.copyfile(pytest_init, init_file)
-
-        conftest_file = os.path.join(project_path, 'conftest.py')
-        with import_path('httpfpt', 'conftest.py') as conftest:
-            shutil.copyfile(conftest, conftest_file)
-            console.print('📄 Created pytest conftest')
-            sleep(1)
-
-        pytest_file = os.path.join(project_path, 'pytest.ini')
-        with import_path('httpfpt', 'pytest.ini') as pytest_ini:
-            shutil.copyfile(pytest_ini, pytest_file)
-            console.print('📄 Created pytest ini')
-            sleep(1)
-
-        run_tpl = """#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from httpfpt.run import run as httpfpt_run
-
-httpfpt_run(testcase_generate=True)
-
-"""
-        with open(os.path.join(project_path, 'run.py'), 'w', encoding='utf-8') as f:
-            f.write(run_tpl)
-            console.print('📄 Created run pytest file')
-
-    console.print(
-        f'\n🎉 The project <{name}> has been created.'
-        f'\n🌳 The project is located in the directory: [cyan]{project_path}[/]'
-        f'\n⚠️ Before accessing HTTPFPT, be sure to set the environment variable '
-        '[yellow]HTTPFPT_PROJECT_PATH[/] to the current project directory',
-        end='\n\n',
-    )
-    if platform.system().lower() == 'windows':
-        env_var_cmd = f"""
-# Windows
-> setx HTTPFPT_PROJECT_PATH "{project_path}"
-        """
-    else:
-        env_var_cmd = f"""
-# Unix
-> vim ~/.bashrc
-> export PATH=$PATH:{project_path}
-        """
-    console.print(Syntax(env_var_cmd, 'shell', line_numbers=True))
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import os
+import platform
+import shutil
+
+from importlib.resources import path as import_path
+from time import sleep
+
+import cappa
+
+from rich.prompt import Prompt
+from rich.syntax import Syntax
+
+from httpfpt.utils.rich_console import console
+
+
+def create_new_project() -> None:
+    name = Prompt.ask('❓ Set your project a name', default='httpfpt_project')
+    path = Prompt.ask('❓ Set your project path (relative or absolute path, which automatically parses.)', default='.')
+    if path != '.':
+        if not os.path.isdir(path):
+            raise cappa.Exit(f'\n❌ The "{path}" is not a directory', code=1)
+    with console.status('[bold green]The project is being created...[/]'):
+        console.print(end='\n')
+        sleep(2)
+
+        project_path = os.path.abspath(os.sep.join([path, name]))
+        if os.path.exists(project_path):
+            raise cappa.Exit(f'\n❌ The "{project_path}" directory is not empty', code=1)
+        os.makedirs(project_path)
+        console.print('📁 Created the project folder')
+        sleep(2)
+
+        core_path = os.path.join(project_path, 'core')
+        with import_path('httpfpt.core', '') as core_data:
+            patterns = ['__init__.py', 'get_conf.py', 'path_conf.py']
+            shutil.copytree(core_data, core_path, ignore=shutil.ignore_patterns(*patterns))
+            console.print('📄 Created core files')
+            sleep(2)
+
+        data_path = os.path.join(project_path, 'data')
+        with import_path('httpfpt.data', '') as case_data:
+            shutil.copytree(case_data, data_path)
+            console.print('📄 Created case data samples')
+            sleep(2)
+
+        init_file = os.path.join(project_path, '__init__.py')
+        with import_path('httpfpt', '__init__.py') as pytest_init:
+            shutil.copyfile(pytest_init, init_file)
+
+        conftest_file = os.path.join(project_path, 'conftest.py')
+        with import_path('httpfpt', 'conftest.py') as conftest:
+            shutil.copyfile(conftest, conftest_file)
+            console.print('📄 Created pytest conftest')
+            sleep(1)
+
+        pytest_file = os.path.join(project_path, 'pytest.ini')
+        with import_path('httpfpt', 'pytest.ini') as pytest_ini:
+            shutil.copyfile(pytest_ini, pytest_file)
+            console.print('📄 Created pytest ini')
+            sleep(1)
+
+        run_tpl = """#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from httpfpt.run import run as httpfpt_run
+
+httpfpt_run(testcase_generate=True)
+
+"""
+        with open(os.path.join(project_path, 'run.py'), 'w', encoding='utf-8') as f:
+            f.write(run_tpl)
+            console.print('📄 Created run pytest file')
+
+    console.print(
+        f'\n🎉 The project <{name}> has been created.'
+        f'\n🌳 The project is located in the directory: [cyan]{project_path}[/]'
+        f'\n⚠️ Before accessing HTTPFPT, be sure to set the environment variable '
+        '[yellow]HTTPFPT_PROJECT_PATH[/] to the current project directory',
+        end='\n\n',
+    )
+    if platform.system().lower() == 'windows':
+        env_var_cmd = f"""
+# Windows
+> setx HTTPFPT_PROJECT_PATH "{project_path}"
+        """
+    else:
+        env_var_cmd = f"""
+# Unix
+> vim ~/.bashrc
+> export PATH=$PATH:{project_path}
+        """
+    console.print(Syntax(env_var_cmd, 'shell', line_numbers=True))
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/data_manage/apifox.py` & `httpfpt-0.6.3/httpfpt/utils/data_manage/apifox.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import copy
-import os
-
-from httpfpt.common.json_handler import read_json_file
-from httpfpt.common.yaml_handler import write_yaml
-from httpfpt.core.get_conf import httpfpt_config
-from httpfpt.core.path_conf import httpfpt_path
-from httpfpt.utils.data_manage.base_format import format_value
-from httpfpt.utils.file_control import get_file_property
-from httpfpt.utils.rich_console import console
-
-
-class ApiFoxParser:
-    def import_apifox_to_yaml(self, source: str, project: str | None = None) -> None:
-        """
-        导入 apifox 数据到 yaml
-
-        :param source:
-        :param project:
-        :return:
-        """
-        data = read_json_file(source)
-        apifox = data.get('apifoxProject')
-        if not apifox:
-            raise ValueError('获取 apifox 数据失败，请使用合法的 apifox 文件')
-        if apifox != '1.0.0':
-            raise Exception('不受支持的 apifox 版本')
-        try:
-            case_config = {}
-            case_config.update(
-                {
-                    'allure': {
-                        'epic': data['info']['name'],
-                        'feature': data['tags'][0]['name'] if data.get('tags') is not None else '未知',
-                        'story': data['info']['description'],
-                    },
-                    'request': {'env': 'dev.env'},
-                    'module': data['info']['name'],
-                }
-            )
-            tag_case = {}
-            root_case = {}
-            for i in data['apiCollection'][0]['items']:
-                if i.get('items') is None:
-                    case = self.get_apifox_step(i)
-                    root_case = copy.deepcopy(root_case)
-                    if root_case.get('root') is None:
-                        root_case.update({'root': [case]})
-                    else:
-                        root_case['root'].append(case)
-                # 多级子目录数据
-                else:
-                    pass  # todo 二叉树数据解析
-            if (len(tag_case) or len(root_case)) > 0:
-                console.print('⏳ 奋力导入中...')
-            # 写入项目 tag 目录
-            if len(tag_case) > 0:
-                for k, v in tag_case.items():
-                    case_config['allure']['feature'] = case_config['module'] = k
-                    case_file_data = {'config': case_config, 'test_steps': v}
-                    write_yaml(
-                        httpfpt_path.case_data_dir,
-                        os.sep.join(
-                            [project or httpfpt_config.PROJECT_NAME, k, get_file_property(source)[1] + '.yaml']
-                        ),
-                        case_file_data,
-                        mode='w',
-                    )
-            # 写入项目根目录
-            if len(root_case) > 0:
-                for v in root_case.values():
-                    case_file_data = {'config': case_config, 'test_steps': v}
-                    write_yaml(
-                        httpfpt_path.case_data_dir,
-                        os.sep.join([project or httpfpt_config.PROJECT_NAME, get_file_property(source)[1] + '.yaml']),
-                        case_file_data,
-                        mode='w',
-                    )
-            console.print('✅ 导入 apifox 数据成功')
-        except Exception as e:
-            raise e
-
-    @staticmethod
-    def get_apifox_params(value: dict) -> dict | None:
-        """
-        获取查询参数
-
-        :param value:
-        :return:
-        """
-        data = {}
-        params = value.get('query')
-        if params is not None:
-            for i in params:
-                if i['type'] != 'file':
-                    data[i['name']] = format_value(i.get('type', 'object'))
-        return data if len(data) > 0 else None
-
-    @staticmethod
-    def get_apifox_headers(value: dict) -> dict | None:
-        """
-        获取查询参数
-
-        :param value:
-        :return:
-        """
-        data = {}
-        header_type = value['type']
-        if header_type != 'none':
-            data = {'Content-Type': f'{header_type}'}
-        return data if len(data) > 0 else None
-
-    @staticmethod
-    def get_apifox_request_data(value: dict) -> dict | None:
-        """
-        获取请求 data
-
-        :param value:
-        :return:
-        """
-        body = {}
-        data = value.get('jsonSchema')
-        if data is not None:
-            for k, v in data['properties'].items():
-                body[k] = format_value(v.get('type', 'object'))
-        return body if len(body) > 0 else None
-
-    @staticmethod
-    def get_apifox_request_files(value: dict) -> dict | None:
-        """
-        获取请求 files
-
-        :param value:
-        :return:
-        """
-        files = {}
-        data = value.get('parameters')
-        if data is not None and len(data) > 0:
-            for i in data:
-                if i.get('type') == 'file':
-                    files[i['name']] = format_value('object')
-        return files if len(files) > 0 else None
-
-    def get_apifox_step(self, value: dict) -> dict:
-        """
-        获取 apifox 用例
-
-        :param value:
-        :return:
-        """
-        params = self.get_apifox_params(value['api']['parameters'])
-        headers = self.get_apifox_headers(value['api']['requestBody'])
-        data_type = None
-        if headers is not None:
-            data_type = 'json' if 'application/json' in headers else 'data'
-        data = self.get_apifox_request_data(value['api']['requestBody'])
-        files = self.get_apifox_request_files(value['api']['requestBody'])
-        case_id = value.get('api').get('operationId')
-        case = {
-            'name': value.get('name'),
-            'case_id': case_id if case_id is not None or case_id != '' else value.get('api').get('id'),
-            'description': value.get('api').get('description'),
-            'is_run': True if value.get('status') in ['released', 'tested'] else False,
-            'request': {
-                'method': value.get('api').get('method'),
-                'url': value.get('api').get('path'),
-                'params': params,
-                'headers': headers,
-                'data_type': data_type,
-                'data': data,
-                'files': files,
-            },
-        }
-        return case
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import copy
+import os
+
+from httpfpt.common.json_handler import read_json_file
+from httpfpt.common.yaml_handler import write_yaml
+from httpfpt.core.get_conf import httpfpt_config
+from httpfpt.core.path_conf import httpfpt_path
+from httpfpt.utils.data_manage.base_format import format_value
+from httpfpt.utils.file_control import get_file_property
+from httpfpt.utils.rich_console import console
+
+
+class ApiFoxParser:
+    def import_apifox_to_yaml(self, source: str, project: str | None = None) -> None:
+        """
+        导入 apifox 数据到 yaml
+
+        :param source:
+        :param project:
+        :return:
+        """
+        data = read_json_file(source)
+        apifox = data.get('apifoxProject')
+        if not apifox:
+            raise ValueError('获取 apifox 数据失败，请使用合法的 apifox 文件')
+        if apifox != '1.0.0':
+            raise Exception('不受支持的 apifox 版本')
+        try:
+            case_config = {}
+            case_config.update(
+                {
+                    'allure': {
+                        'epic': data['info']['name'],
+                        'feature': data['tags'][0]['name'] if data.get('tags') is not None else '未知',
+                        'story': data['info']['description'],
+                    },
+                    'request': {'env': 'dev.env'},
+                    'module': data['info']['name'],
+                }
+            )
+            tag_case = {}
+            root_case = {}
+            for i in data['apiCollection'][0]['items']:
+                if i.get('items') is None:
+                    case = self.get_apifox_step(i)
+                    root_case = copy.deepcopy(root_case)
+                    if root_case.get('root') is None:
+                        root_case.update({'root': [case]})
+                    else:
+                        root_case['root'].append(case)
+                # 多级子目录数据
+                else:
+                    pass  # todo 二叉树数据解析
+            if (len(tag_case) or len(root_case)) > 0:
+                console.print('⏳ 奋力导入中...')
+            # 写入项目 tag 目录
+            if len(tag_case) > 0:
+                for k, v in tag_case.items():
+                    case_config['allure']['feature'] = case_config['module'] = k
+                    case_file_data = {'config': case_config, 'test_steps': v}
+                    write_yaml(
+                        httpfpt_path.case_data_dir,
+                        os.sep.join(
+                            [project or httpfpt_config.PROJECT_NAME, k, get_file_property(source)[1] + '.yaml']
+                        ),
+                        case_file_data,
+                        mode='w',
+                    )
+            # 写入项目根目录
+            if len(root_case) > 0:
+                for v in root_case.values():
+                    case_file_data = {'config': case_config, 'test_steps': v}
+                    write_yaml(
+                        httpfpt_path.case_data_dir,
+                        os.sep.join([project or httpfpt_config.PROJECT_NAME, get_file_property(source)[1] + '.yaml']),
+                        case_file_data,
+                        mode='w',
+                    )
+            console.print('✅ 导入 apifox 数据成功')
+        except Exception as e:
+            raise e
+
+    @staticmethod
+    def get_apifox_params(value: dict) -> dict | None:
+        """
+        获取查询参数
+
+        :param value:
+        :return:
+        """
+        data = {}
+        params = value.get('query')
+        if params is not None:
+            for i in params:
+                if i['type'] != 'file':
+                    data[i['name']] = format_value(i.get('type', 'object'))
+        return data if len(data) > 0 else None
+
+    @staticmethod
+    def get_apifox_headers(value: dict) -> dict | None:
+        """
+        获取查询参数
+
+        :param value:
+        :return:
+        """
+        data = {}
+        header_type = value['type']
+        if header_type != 'none':
+            data = {'Content-Type': f'{header_type}'}
+        return data if len(data) > 0 else None
+
+    @staticmethod
+    def get_apifox_request_data(value: dict) -> dict | None:
+        """
+        获取请求 data
+
+        :param value:
+        :return:
+        """
+        body = {}
+        data = value.get('jsonSchema')
+        if data is not None:
+            for k, v in data['properties'].items():
+                body[k] = format_value(v.get('type', 'object'))
+        return body if len(body) > 0 else None
+
+    @staticmethod
+    def get_apifox_request_files(value: dict) -> dict | None:
+        """
+        获取请求 files
+
+        :param value:
+        :return:
+        """
+        files = {}
+        data = value.get('parameters')
+        if data is not None and len(data) > 0:
+            for i in data:
+                if i.get('type') == 'file':
+                    files[i['name']] = format_value('object')
+        return files if len(files) > 0 else None
+
+    def get_apifox_step(self, value: dict) -> dict:
+        """
+        获取 apifox 用例
+
+        :param value:
+        :return:
+        """
+        params = self.get_apifox_params(value['api']['parameters'])
+        headers = self.get_apifox_headers(value['api']['requestBody'])
+        data_type = None
+        if headers is not None:
+            data_type = 'json' if 'application/json' in headers else 'data'
+        data = self.get_apifox_request_data(value['api']['requestBody'])
+        files = self.get_apifox_request_files(value['api']['requestBody'])
+        case_id = value.get('api').get('operationId')
+        case = {
+            'name': value.get('name'),
+            'case_id': case_id if case_id is not None or case_id != '' else value.get('api').get('id'),
+            'description': value.get('api').get('description'),
+            'is_run': True if value.get('status') in ['released', 'tested'] else False,
+            'request': {
+                'method': value.get('api').get('method'),
+                'url': value.get('api').get('path'),
+                'params': params,
+                'headers': headers,
+                'data_type': data_type,
+                'data': data,
+                'files': files,
+            },
+        }
+        return case
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/data_manage/base_format.py` & `httpfpt-0.6.3/httpfpt/utils/data_manage/base_format.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-
-def format_value(value_type: str) -> str | int | float | bool | dict | list:
-    """
-    根据数据类型格式化数据
-
-    :param value_type:
-    :return:
-    """
-    if value_type == 'string':
-        v = ''
-    elif value_type == 'integer':  # noqa: SIM114
-        v = 0
-    elif value_type == 'number':
-        v = 0
-    elif value_type == 'boolean':
-        v = False
-    elif value_type == 'object':
-        v = {}
-    elif value_type == 'array':
-        v = [{}]
-    elif value_type == 'arrayString':
-        v = []
-    else:
-        raise Exception(f'存在不支持的类型：{value_type}')
-    return v
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+
+def format_value(value_type: str) -> str | int | float | bool | dict | list:
+    """
+    根据数据类型格式化数据
+
+    :param value_type:
+    :return:
+    """
+    if value_type == 'string':
+        v = ''
+    elif value_type == 'integer':  # noqa: SIM114
+        v = 0
+    elif value_type == 'number':
+        v = 0
+    elif value_type == 'boolean':
+        v = False
+    elif value_type == 'object':
+        v = {}
+    elif value_type == 'array':
+        v = [{}]
+    elif value_type == 'arrayString':
+        v = []
+    else:
+        raise Exception(f'存在不支持的类型：{value_type}')
+    return v
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/data_manage/git_repo.py` & `httpfpt-0.6.3/httpfpt/utils/data_manage/git_repo.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-import os
-import shutil
-
-from pydantic import ValidationError
-
-from httpfpt.common.json_handler import read_json_file
-from httpfpt.common.yaml_handler import read_yaml
-from httpfpt.enums.case_data_type import CaseDataType
-from httpfpt.schemas.case_data import CaseData
-from httpfpt.utils.file_control import get_file_property, search_all_case_data_files
-from httpfpt.utils.pydantic_parser import parse_error
-from httpfpt.utils.rich_console import console
-
-
-class GitRepoPaser:
-    @staticmethod
-    def import_git_to_local(src: str) -> None:
-        """
-        导入 git 仓库测试数据
-
-        :param src:
-        :return:
-        """
-
-        if 'https' not in src:
-            raise ValueError('❌ Git 仓库克隆地址错误, 请使用 https 地址')
-
-        try:
-            online_dir_path = os.path.join(os.path.abspath('./data/test_data'), 'online_test_data')
-            console.print(online_dir_path)
-            if os.path.exists(online_dir_path):
-                shutil.rmtree(online_dir_path)
-            os.makedirs(online_dir_path)
-            result = os.system(f'cd {online_dir_path} && git clone {src}')
-            shutil.rmtree(os.path.join(online_dir_path, '.git'))
-        except Exception as e:
-            raise RuntimeError(f'❌ Git 仓库测试数据拉取失败：{e}')
-        if result == 0:
-            console.print('\n✅ Git 仓库数据文件拉取成功')
-        else:
-            raise RuntimeError('❌ Git 仓库测试数据拉取失败，请检查 Git 地址是否正确')
-
-        console.print('\n🔥 开始自动验证测试数据结构...')
-        all_case_data_file = search_all_case_data_files(online_dir_path)
-        if len(all_case_data_file) == 0:
-            raise FileNotFoundError('❌ 未在拉取的 Git 仓库中找到测试用例数据文件，请检查 Git 地址是否正确')
-        all_case_data = []
-        for file in all_case_data_file:
-            file_type = get_file_property(file)[2]
-            if file_type == CaseDataType.JSON:
-                file_data = read_json_file(file)
-            else:
-                file_data = read_yaml(file)
-            all_case_data.append(file_data)
-        count: int = 0
-        for case_data in all_case_data:
-            try:
-                CaseData.model_validate(case_data)
-            except ValidationError as e:
-                count += parse_error(e)
-        if count > 0:
-            raise ValueError(f'❌ Git 仓库用例数据校验失败，共有 {count} 处错误, 错误详情请查看日志')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+import os
+import shutil
+
+from pydantic import ValidationError
+
+from httpfpt.common.json_handler import read_json_file
+from httpfpt.common.yaml_handler import read_yaml
+from httpfpt.enums.case_data_type import CaseDataType
+from httpfpt.schemas.case_data import CaseData
+from httpfpt.utils.file_control import get_file_property, search_all_case_data_files
+from httpfpt.utils.pydantic_parser import parse_error
+from httpfpt.utils.rich_console import console
+
+
+class GitRepoPaser:
+    @staticmethod
+    def import_git_to_local(src: str) -> None:
+        """
+        导入 git 仓库测试数据
+
+        :param src:
+        :return:
+        """
+
+        if 'https' not in src:
+            raise ValueError('❌ Git 仓库克隆地址错误, 请使用 https 地址')
+
+        try:
+            online_dir_path = os.path.join(os.path.abspath('./data/test_data'), 'online_test_data')
+            console.print(online_dir_path)
+            if os.path.exists(online_dir_path):
+                shutil.rmtree(online_dir_path)
+            os.makedirs(online_dir_path)
+            result = os.system(f'cd {online_dir_path} && git clone {src}')
+            shutil.rmtree(os.path.join(online_dir_path, '.git'))
+        except Exception as e:
+            raise RuntimeError(f'❌ Git 仓库测试数据拉取失败：{e}')
+        if result == 0:
+            console.print('\n✅ Git 仓库数据文件拉取成功')
+        else:
+            raise RuntimeError('❌ Git 仓库测试数据拉取失败，请检查 Git 地址是否正确')
+
+        console.print('\n🔥 开始自动验证测试数据结构...')
+        all_case_data_file = search_all_case_data_files(online_dir_path)
+        if len(all_case_data_file) == 0:
+            raise FileNotFoundError('❌ 未在拉取的 Git 仓库中找到测试用例数据文件，请检查 Git 地址是否正确')
+        all_case_data = []
+        for file in all_case_data_file:
+            file_type = get_file_property(file)[2]
+            if file_type == CaseDataType.JSON:
+                file_data = read_json_file(file)
+            else:
+                file_data = read_yaml(file)
+            all_case_data.append(file_data)
+        count: int = 0
+        for case_data in all_case_data:
+            try:
+                CaseData.model_validate(case_data)
+            except ValidationError as e:
+                count += parse_error(e)
+        if count > 0:
+            raise ValueError(f'❌ Git 仓库用例数据校验失败，共有 {count} 处错误, 错误详情请查看日志')
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/data_manage/openapi.py` & `httpfpt-0.6.3/httpfpt/utils/data_manage/openapi.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,410 +1,410 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import copy
-import os
-import warnings
-
-import requests
-
-from rich.prompt import Confirm
-
-from httpfpt.common.json_handler import read_json_file
-from httpfpt.common.yaml_handler import write_yaml
-from httpfpt.core.get_conf import httpfpt_config
-from httpfpt.core.path_conf import httpfpt_path
-from httpfpt.utils.data_manage.base_format import format_value
-from httpfpt.utils.file_control import get_file_property
-from httpfpt.utils.rich_console import console
-from httpfpt.utils.time_control import get_current_timestamp
-
-
-class SwaggerParser:
-    def __init__(self, version: int | None = None, data: dict | None = None):
-        """
-        初始化参数
-
-        :param version:
-        :param data:
-        """
-        self.version = version
-        self.data = data
-
-    def import_openapi_to_yaml(self, openapi_source: str, project: str | None = None) -> None:
-        """
-        导入 openapi 数据到 yaml
-
-        :param openapi_source:
-        :param project:
-        :return:
-        """
-        global warn_operationId
-        self.get_swagger_data(openapi_source)
-        try:
-            # 测试用例数据配置项
-            case_config = {}
-            case_config.update(
-                {
-                    'allure': {
-                        'epic': self.data['info']['title'],
-                        'feature': self.data['tags'][0]['name'] if self.data.get('tags') is not None else '未知',
-                        'story': self.data['info']['description'],
-                    },
-                    'request': {'env': 'dev.env'},
-                    'module': self.data['info']['title'],
-                }
-            )
-
-            # 测试用例数据
-            case = {}
-            # 子目录
-            tag = ''
-            # 子目录测试用例数据
-            tag_case = {}
-            # 根目录测试用例数据
-            root_case = {}
-
-            is_tag = Confirm.ask('❓ 是否按 openapi 标签划分数据存放目录?', default=True)
-            for url, values in self.data['paths'].items():
-                for method, values_map in values.items():
-                    params = self.get_swagger_params(values_map)
-                    headers = self.get_swagger_headers(values_map)
-                    if self.version == 2:
-                        data = self.get_swagger_request_data(values_map) if method.lower() != 'get' else None
-                        files = self.get_swagger_request_files(values_map) if method.lower() != 'get' else None
-                    else:
-                        try:
-                            schema = (
-                                values_map['requestBody']['content'][headers['Content-Type']]['schema']['$ref'].split(
-                                    '/'
-                                )[-1]
-                                if values_map.get('requestBody') is not None
-                                else None
-                            )
-                        except KeyError:
-                            schema = values_map['requestBody']['content'][headers['Content-Type']]['schema']
-                            warn_operationId = values_map['operationId']
-                        data = self.get_swagger_request_data(schema) if schema is not None else None
-                        files = self.get_swagger_request_files(schema) if schema is not None else None
-                    data_type = None
-                    if headers is not None:
-                        data_type = 'json' if 'application/json' in headers else 'data'
-                    case = copy.deepcopy(case)
-                    case.update(
-                        {
-                            'name': values_map.get('summary'),
-                            'case_id': values_map.get('operationId'),
-                            'description': values_map.get('description'),
-                            'is_run': values_map.get('deprecated', True),
-                            'request': {
-                                'method': method,
-                                'url': url,
-                                'params': params,
-                                'headers': headers,
-                                'data_type': data_type,
-                                'data': data,
-                                'files': files,
-                            },
-                        }
-                    )
-                    tags = values_map.get('tags')
-                    # 按 tag 划分目录
-                    if is_tag:
-                        if tags is not None:
-                            dp_tag = copy.deepcopy(tag)
-                            tag = tags[0]
-                            tag_case.update({tag: [case]}) if dp_tag != tag else tag_case[tag].append(case)
-                        else:
-                            root_case = copy.deepcopy(root_case)
-                            root_case.update({'root': [case]}) if root_case.get('root') is None else root_case[
-                                'root'
-                            ].append(case)
-                    # 不按 tag 划分目录
-                    else:
-                        if tags:
-                            dp_tag = copy.deepcopy(tag)
-                            tag = tags[0]
-                            root_case.update({tag: [case]}) if dp_tag != tag else root_case[tag].append(case)
-                        else:
-                            root_case = copy.deepcopy(root_case)
-                            root_case.update({'root': [case]}) if root_case.get('root') is None else root_case[
-                                'root'
-                            ].append(case)
-            if len(tag_case) > 0 or len(root_case) > 0:
-                # 文件创建提醒
-                file_list = []
-                if len(tag_case) > 0:
-                    for k, v in tag_case.items():
-                        tag_filename = os.sep.join(
-                            [
-                                project or httpfpt_config.PROJECT_NAME,
-                                k,
-                                get_file_property(openapi_source)[1] + '.yaml'
-                                if not openapi_source.startswith('http')
-                                else f'openapi_{k}.yaml',
-                            ]
-                        )
-                        file_list.append(tag_filename)
-                if len(root_case) > 0:
-                    for k, v in root_case.items():
-                        if k == 'root':
-                            root_filename = os.sep.join(
-                                [
-                                    project or httpfpt_config.PROJECT_NAME,
-                                    get_file_property(openapi_source)[1] + '.yaml'
-                                    if not openapi_source.startswith('http')
-                                    else f'openapi_{get_current_timestamp()}.yaml',
-                                ]
-                            )
-                        else:
-                            root_filename = os.sep.join(
-                                [
-                                    project or httpfpt_config.PROJECT_NAME,
-                                    get_file_property(openapi_source)[1] + '.yaml'
-                                    if not openapi_source.startswith('http')
-                                    else f'openapi_{k}.yaml',
-                                ]
-                            )
-                        file_list.append(root_filename)
-                console.print('⚠️ 即将创建以下数据文件:')
-                for i in file_list:
-                    console.print(f'\n\tdata\\test_data\\{i}')
-                is_force_write = Confirm.ask(
-                    '\n👁️ 请检查是否存在同名文件, 此操作将强制覆盖写入所有数据文件, 是否继续执行? (此操作不可逆)',
-                    default=False,
-                )
-                # 强制写入
-                if is_force_write:
-                    console.print('⏳ 奋力导入中...')
-                    # 写入项目 tag 目录
-                    if len(tag_case) > 0:
-                        for k, v in tag_case.items():
-                            case_config['allure']['feature'] = case_config['module'] = k
-                            case_file_data = {'config': case_config, 'test_steps': v}
-                            write_yaml(
-                                httpfpt_path.case_data_dir,
-                                os.sep.join(
-                                    [
-                                        project or httpfpt_config.PROJECT_NAME,
-                                        k,
-                                        get_file_property(openapi_source)[1] + '.yaml'
-                                        if not openapi_source.startswith('http')
-                                        else f'openapi_{k}.yaml',
-                                    ]
-                                ),
-                                case_file_data,
-                                mode='w',
-                            )
-                    # 写入项目根目录
-                    if len(root_case) > 0:
-                        for k, v in root_case.items():
-                            if k == 'root':
-                                filename = (
-                                    get_file_property(openapi_source)[1] + '.yaml'
-                                    if not openapi_source.startswith('http')
-                                    else f'openapi_{get_current_timestamp()}.yaml'
-                                )
-                            else:
-                                filename = (
-                                    get_file_property(openapi_source)[1] + '.yaml'
-                                    if not openapi_source.startswith('http')
-                                    else f'openapi_{k}.yaml'
-                                )
-                            case_file_data = {'config': case_config, 'test_steps': v}
-                            write_yaml(
-                                httpfpt_path.case_data_dir,
-                                os.sep.join([project or httpfpt_config.PROJECT_NAME, filename]),
-                                case_file_data,
-                                mode='w',
-                            )
-                # 选择写入
-                else:
-                    console.print('⚠️ 已取消强制覆写入所有数据文件')
-                    is_next = Confirm.ask('❓ 是否进行逐一选择创建数据文件?', default=True)
-                    if is_next:
-                        # 写入项目 tag 目录
-                        if len(tag_case) > 0:
-                            for k, v in tag_case.items():
-                                case_config['allure']['feature'] = case_config['module'] = k
-                                case_file_data = {'config': case_config, 'test_steps': v}
-                                tag_filename = os.sep.join(
-                                    [
-                                        project or httpfpt_config.PROJECT_NAME,
-                                        k,
-                                        get_file_property(openapi_source)[1] + '.yaml'
-                                        if not openapi_source.startswith('http')
-                                        else f'openapi_{k}.yaml',
-                                    ]
-                                )
-                                is_write = Confirm.ask(f'❓ 是否需要创建 {tag_filename} 数据文件?', default=True)
-                                if is_write:
-                                    write_yaml(httpfpt_path.case_data_dir, tag_filename, case_file_data, mode='w')
-                        # 写入项目根目录
-                        if len(root_case) > 0:
-                            for k, v in root_case.items():
-                                if k == 'root':
-                                    root_filename = (
-                                        get_file_property(openapi_source)[1] + '.yaml'
-                                        if not openapi_source.startswith('http')
-                                        else f'openapi_{get_current_timestamp()}.yaml'
-                                    )
-                                else:
-                                    root_filename = (
-                                        get_file_property(openapi_source)[1] + '.yaml'
-                                        if not openapi_source.startswith('http')
-                                        else f'openapi_{k}.yaml'
-                                    )
-                                is_write = Confirm.ask(f'❓ 是否需要创建 {root_filename} 数据文件?', default=True)
-                                if is_write:
-                                    case_file_data = {'config': case_config, 'test_steps': v}
-                                    write_yaml(
-                                        httpfpt_path.case_data_dir,
-                                        os.sep.join([project or httpfpt_config.PROJECT_NAME, root_filename]),
-                                        case_file_data,
-                                        mode='w',
-                                    )
-            console.print('✅ 导入 openapi 数据成功')
-        except Exception as e:
-            raise e
-
-    def get_swagger_data(self, openapi_source: str) -> None:
-        """
-        请求 swagger 数据
-
-        :param openapi_source:
-        :return:
-        """
-        if openapi_source.startswith('http'):
-            request = requests.session()
-            request.trust_env = False
-            data = request.get(openapi_source).json()
-            openapi = data.get('openapi')
-            swagger = data.get('swagger')
-            if not (openapi or swagger):
-                raise ValueError('请输入正确的 openapi 地址')
-        else:
-            data = read_json_file(openapi_source)
-            openapi = data.get('openapi')
-            swagger = data.get('swagger')
-            if not (openapi or swagger):
-                raise ValueError('获取 openapi 数据失败，请使用合法的 openapi 文件')
-        if openapi is not None and int(openapi.split('.')[0]) == 3:
-            self.version = 3
-        elif swagger == '2.0':
-            self.version = 2
-        else:
-            raise Exception('不受支持的 openapi 版本')
-        self.data = data
-
-    def get_swagger_params(self, value: dict) -> dict | None:
-        """
-        获取查询参数
-
-        :param value:
-        :return:
-        """
-        data = {}
-        if self.version == 2:
-            params = value.get('parameters')
-            if params is not None:
-                for i in params:
-                    if i['in'] == 'path':
-                        data = {i['name']: None}
-            return data if len(data) > 0 else None
-        else:
-            params = value.get('parameters')
-            if params is not None:
-                for i in params:
-                    data = {i['name']: None}
-            return data if len(data) > 0 else None
-
-    def get_swagger_headers(self, value: dict) -> dict | None:
-        """
-        获取查询参数
-
-        :param value:
-        :return:
-        """
-        data = {}
-        if self.version == 2:
-            headers = value.get('consumes')
-            if headers is not None:
-                data = {'Content-Type': headers[0]}
-            return data if len(data) > 0 else None
-        else:
-            headers = value.get('requestBody')
-            if headers is not None:
-                content = headers['content']
-                data = {'Content-Type': f'{[k for k in content.keys()][0]}'}
-            return data if len(data) > 0 else None
-
-    def get_swagger_schema_data(self, name: str) -> dict:
-        """
-        获取 schema 数据
-
-        :param name:
-        :return:
-        """
-        if self.version == 2:
-            data = self.data.get('definitions').get(name)
-        else:
-            data = self.data.get('components').get('schemas').get(name)
-        return data
-
-    def get_swagger_request_data(self, value: dict | str) -> dict | None:
-        """
-        获取请求 data
-
-        :param value:
-        :return:
-        """
-        data = {}
-        if self.version == 2:
-            if len(value['parameters']) > 0:
-                for i in value['parameters']:
-                    if i.get('type') is None:
-                        data[i['name']] = format_value('object')  # type: ignore
-                    else:
-                        if i.get('type') != 'file':
-                            data[i['name']] = format_value(i.get('type', 'object'))  # type: ignore
-            return data if len(data) > 0 else None
-        else:
-            if not isinstance(value, dict):
-                schema_data = self.get_swagger_schema_data(value)
-                for k, v in schema_data['properties'].items():
-                    if v.get('format') is None:
-                        data[k] = format_value(v.get('type', 'object'))
-                    else:
-                        if v.get('format') != 'binary':
-                            data[k] = format_value(v.get('type', 'object'))
-            else:
-                # 请求体使用了非 schema 格式入参
-                warnings.warn(f'接口(ID) {warn_operationId} 使用了非 schema 入参')
-                if value.get('type') is None:
-                    data[value['title']] = format_value('object')
-                else:
-                    if value.get('type') != 'file':
-                        data[value['title']] = format_value(value.get('type', 'object'))
-            return data if len(data) > 0 else None
-
-    def get_swagger_request_files(self, value: str | dict) -> dict | None:
-        """
-        获取请求 files
-
-        :param value:
-        :return:
-        """
-        files = {}
-        if self.version == 2:
-            for v in value['parameters']:
-                if v.get('type') == 'file':
-                    files[v.get('name')] = format_value('object')
-            return files if len(files) > 0 else None
-        else:
-            if not isinstance(value, dict):
-                schema_data = self.get_swagger_schema_data(value)
-                for k, v in schema_data['properties'].items():
-                    if v.get('format') == 'binary':
-                        files[k] = format_value(v.get('type', 'object'))
-                return files if len(files) > 0 else None
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import copy
+import os
+import warnings
+
+import requests
+
+from rich.prompt import Confirm
+
+from httpfpt.common.json_handler import read_json_file
+from httpfpt.common.yaml_handler import write_yaml
+from httpfpt.core.get_conf import httpfpt_config
+from httpfpt.core.path_conf import httpfpt_path
+from httpfpt.utils.data_manage.base_format import format_value
+from httpfpt.utils.file_control import get_file_property
+from httpfpt.utils.rich_console import console
+from httpfpt.utils.time_control import get_current_timestamp
+
+
+class SwaggerParser:
+    def __init__(self, version: int | None = None, data: dict | None = None):
+        """
+        初始化参数
+
+        :param version:
+        :param data:
+        """
+        self.version = version
+        self.data = data
+
+    def import_openapi_to_yaml(self, openapi_source: str, project: str | None = None) -> None:
+        """
+        导入 openapi 数据到 yaml
+
+        :param openapi_source:
+        :param project:
+        :return:
+        """
+        global warn_operationId
+        self.get_swagger_data(openapi_source)
+        try:
+            # 测试用例数据配置项
+            case_config = {}
+            case_config.update(
+                {
+                    'allure': {
+                        'epic': self.data['info']['title'],
+                        'feature': self.data['tags'][0]['name'] if self.data.get('tags') is not None else '未知',
+                        'story': self.data['info']['description'],
+                    },
+                    'request': {'env': 'dev.env'},
+                    'module': self.data['info']['title'],
+                }
+            )
+
+            # 测试用例数据
+            case = {}
+            # 子目录
+            tag = ''
+            # 子目录测试用例数据
+            tag_case = {}
+            # 根目录测试用例数据
+            root_case = {}
+
+            is_tag = Confirm.ask('❓ 是否按 openapi 标签划分数据存放目录?', default=True)
+            for url, values in self.data['paths'].items():
+                for method, values_map in values.items():
+                    params = self.get_swagger_params(values_map)
+                    headers = self.get_swagger_headers(values_map)
+                    if self.version == 2:
+                        data = self.get_swagger_request_data(values_map) if method.lower() != 'get' else None
+                        files = self.get_swagger_request_files(values_map) if method.lower() != 'get' else None
+                    else:
+                        try:
+                            schema = (
+                                values_map['requestBody']['content'][headers['Content-Type']]['schema']['$ref'].split(
+                                    '/'
+                                )[-1]
+                                if values_map.get('requestBody') is not None
+                                else None
+                            )
+                        except KeyError:
+                            schema = values_map['requestBody']['content'][headers['Content-Type']]['schema']
+                            warn_operationId = values_map['operationId']
+                        data = self.get_swagger_request_data(schema) if schema is not None else None
+                        files = self.get_swagger_request_files(schema) if schema is not None else None
+                    data_type = None
+                    if headers is not None:
+                        data_type = 'json' if 'application/json' in headers else 'data'
+                    case = copy.deepcopy(case)
+                    case.update(
+                        {
+                            'name': values_map.get('summary'),
+                            'case_id': values_map.get('operationId'),
+                            'description': values_map.get('description'),
+                            'is_run': values_map.get('deprecated', True),
+                            'request': {
+                                'method': method,
+                                'url': url,
+                                'params': params,
+                                'headers': headers,
+                                'data_type': data_type,
+                                'data': data,
+                                'files': files,
+                            },
+                        }
+                    )
+                    tags = values_map.get('tags')
+                    # 按 tag 划分目录
+                    if is_tag:
+                        if tags is not None:
+                            dp_tag = copy.deepcopy(tag)
+                            tag = tags[0]
+                            tag_case.update({tag: [case]}) if dp_tag != tag else tag_case[tag].append(case)
+                        else:
+                            root_case = copy.deepcopy(root_case)
+                            root_case.update({'root': [case]}) if root_case.get('root') is None else root_case[
+                                'root'
+                            ].append(case)
+                    # 不按 tag 划分目录
+                    else:
+                        if tags:
+                            dp_tag = copy.deepcopy(tag)
+                            tag = tags[0]
+                            root_case.update({tag: [case]}) if dp_tag != tag else root_case[tag].append(case)
+                        else:
+                            root_case = copy.deepcopy(root_case)
+                            root_case.update({'root': [case]}) if root_case.get('root') is None else root_case[
+                                'root'
+                            ].append(case)
+            if len(tag_case) > 0 or len(root_case) > 0:
+                # 文件创建提醒
+                file_list = []
+                if len(tag_case) > 0:
+                    for k, v in tag_case.items():
+                        tag_filename = os.sep.join(
+                            [
+                                project or httpfpt_config.PROJECT_NAME,
+                                k,
+                                get_file_property(openapi_source)[1] + '.yaml'
+                                if not openapi_source.startswith('http')
+                                else f'openapi_{k}.yaml',
+                            ]
+                        )
+                        file_list.append(tag_filename)
+                if len(root_case) > 0:
+                    for k, v in root_case.items():
+                        if k == 'root':
+                            root_filename = os.sep.join(
+                                [
+                                    project or httpfpt_config.PROJECT_NAME,
+                                    get_file_property(openapi_source)[1] + '.yaml'
+                                    if not openapi_source.startswith('http')
+                                    else f'openapi_{get_current_timestamp()}.yaml',
+                                ]
+                            )
+                        else:
+                            root_filename = os.sep.join(
+                                [
+                                    project or httpfpt_config.PROJECT_NAME,
+                                    get_file_property(openapi_source)[1] + '.yaml'
+                                    if not openapi_source.startswith('http')
+                                    else f'openapi_{k}.yaml',
+                                ]
+                            )
+                        file_list.append(root_filename)
+                console.print('⚠️ 即将创建以下数据文件:')
+                for i in file_list:
+                    console.print(f'\n\tdata\\test_data\\{i}')
+                is_force_write = Confirm.ask(
+                    '\n👁️ 请检查是否存在同名文件, 此操作将强制覆盖写入所有数据文件, 是否继续执行? (此操作不可逆)',
+                    default=False,
+                )
+                # 强制写入
+                if is_force_write:
+                    console.print('⏳ 奋力导入中...')
+                    # 写入项目 tag 目录
+                    if len(tag_case) > 0:
+                        for k, v in tag_case.items():
+                            case_config['allure']['feature'] = case_config['module'] = k
+                            case_file_data = {'config': case_config, 'test_steps': v}
+                            write_yaml(
+                                httpfpt_path.case_data_dir,
+                                os.sep.join(
+                                    [
+                                        project or httpfpt_config.PROJECT_NAME,
+                                        k,
+                                        get_file_property(openapi_source)[1] + '.yaml'
+                                        if not openapi_source.startswith('http')
+                                        else f'openapi_{k}.yaml',
+                                    ]
+                                ),
+                                case_file_data,
+                                mode='w',
+                            )
+                    # 写入项目根目录
+                    if len(root_case) > 0:
+                        for k, v in root_case.items():
+                            if k == 'root':
+                                filename = (
+                                    get_file_property(openapi_source)[1] + '.yaml'
+                                    if not openapi_source.startswith('http')
+                                    else f'openapi_{get_current_timestamp()}.yaml'
+                                )
+                            else:
+                                filename = (
+                                    get_file_property(openapi_source)[1] + '.yaml'
+                                    if not openapi_source.startswith('http')
+                                    else f'openapi_{k}.yaml'
+                                )
+                            case_file_data = {'config': case_config, 'test_steps': v}
+                            write_yaml(
+                                httpfpt_path.case_data_dir,
+                                os.sep.join([project or httpfpt_config.PROJECT_NAME, filename]),
+                                case_file_data,
+                                mode='w',
+                            )
+                # 选择写入
+                else:
+                    console.print('⚠️ 已取消强制覆写入所有数据文件')
+                    is_next = Confirm.ask('❓ 是否进行逐一选择创建数据文件?', default=True)
+                    if is_next:
+                        # 写入项目 tag 目录
+                        if len(tag_case) > 0:
+                            for k, v in tag_case.items():
+                                case_config['allure']['feature'] = case_config['module'] = k
+                                case_file_data = {'config': case_config, 'test_steps': v}
+                                tag_filename = os.sep.join(
+                                    [
+                                        project or httpfpt_config.PROJECT_NAME,
+                                        k,
+                                        get_file_property(openapi_source)[1] + '.yaml'
+                                        if not openapi_source.startswith('http')
+                                        else f'openapi_{k}.yaml',
+                                    ]
+                                )
+                                is_write = Confirm.ask(f'❓ 是否需要创建 {tag_filename} 数据文件?', default=True)
+                                if is_write:
+                                    write_yaml(httpfpt_path.case_data_dir, tag_filename, case_file_data, mode='w')
+                        # 写入项目根目录
+                        if len(root_case) > 0:
+                            for k, v in root_case.items():
+                                if k == 'root':
+                                    root_filename = (
+                                        get_file_property(openapi_source)[1] + '.yaml'
+                                        if not openapi_source.startswith('http')
+                                        else f'openapi_{get_current_timestamp()}.yaml'
+                                    )
+                                else:
+                                    root_filename = (
+                                        get_file_property(openapi_source)[1] + '.yaml'
+                                        if not openapi_source.startswith('http')
+                                        else f'openapi_{k}.yaml'
+                                    )
+                                is_write = Confirm.ask(f'❓ 是否需要创建 {root_filename} 数据文件?', default=True)
+                                if is_write:
+                                    case_file_data = {'config': case_config, 'test_steps': v}
+                                    write_yaml(
+                                        httpfpt_path.case_data_dir,
+                                        os.sep.join([project or httpfpt_config.PROJECT_NAME, root_filename]),
+                                        case_file_data,
+                                        mode='w',
+                                    )
+            console.print('✅ 导入 openapi 数据成功')
+        except Exception as e:
+            raise e
+
+    def get_swagger_data(self, openapi_source: str) -> None:
+        """
+        请求 swagger 数据
+
+        :param openapi_source:
+        :return:
+        """
+        if openapi_source.startswith('http'):
+            request = requests.session()
+            request.trust_env = False
+            data = request.get(openapi_source).json()
+            openapi = data.get('openapi')
+            swagger = data.get('swagger')
+            if not (openapi or swagger):
+                raise ValueError('请输入正确的 openapi 地址')
+        else:
+            data = read_json_file(openapi_source)
+            openapi = data.get('openapi')
+            swagger = data.get('swagger')
+            if not (openapi or swagger):
+                raise ValueError('获取 openapi 数据失败，请使用合法的 openapi 文件')
+        if openapi is not None and int(openapi.split('.')[0]) == 3:
+            self.version = 3
+        elif swagger == '2.0':
+            self.version = 2
+        else:
+            raise Exception('不受支持的 openapi 版本')
+        self.data = data
+
+    def get_swagger_params(self, value: dict) -> dict | None:
+        """
+        获取查询参数
+
+        :param value:
+        :return:
+        """
+        data = {}
+        if self.version == 2:
+            params = value.get('parameters')
+            if params is not None:
+                for i in params:
+                    if i['in'] == 'path':
+                        data = {i['name']: None}
+            return data if len(data) > 0 else None
+        else:
+            params = value.get('parameters')
+            if params is not None:
+                for i in params:
+                    data = {i['name']: None}
+            return data if len(data) > 0 else None
+
+    def get_swagger_headers(self, value: dict) -> dict | None:
+        """
+        获取查询参数
+
+        :param value:
+        :return:
+        """
+        data = {}
+        if self.version == 2:
+            headers = value.get('consumes')
+            if headers is not None:
+                data = {'Content-Type': headers[0]}
+            return data if len(data) > 0 else None
+        else:
+            headers = value.get('requestBody')
+            if headers is not None:
+                content = headers['content']
+                data = {'Content-Type': f'{[k for k in content.keys()][0]}'}
+            return data if len(data) > 0 else None
+
+    def get_swagger_schema_data(self, name: str) -> dict:
+        """
+        获取 schema 数据
+
+        :param name:
+        :return:
+        """
+        if self.version == 2:
+            data = self.data.get('definitions').get(name)
+        else:
+            data = self.data.get('components').get('schemas').get(name)
+        return data
+
+    def get_swagger_request_data(self, value: dict | str) -> dict | None:
+        """
+        获取请求 data
+
+        :param value:
+        :return:
+        """
+        data = {}
+        if self.version == 2:
+            if len(value['parameters']) > 0:
+                for i in value['parameters']:
+                    if i.get('type') is None:
+                        data[i['name']] = format_value('object')  # type: ignore
+                    else:
+                        if i.get('type') != 'file':
+                            data[i['name']] = format_value(i.get('type', 'object'))  # type: ignore
+            return data if len(data) > 0 else None
+        else:
+            if not isinstance(value, dict):
+                schema_data = self.get_swagger_schema_data(value)
+                for k, v in schema_data['properties'].items():
+                    if v.get('format') is None:
+                        data[k] = format_value(v.get('type', 'object'))
+                    else:
+                        if v.get('format') != 'binary':
+                            data[k] = format_value(v.get('type', 'object'))
+            else:
+                # 请求体使用了非 schema 格式入参
+                warnings.warn(f'接口(ID) {warn_operationId} 使用了非 schema 入参')
+                if value.get('type') is None:
+                    data[value['title']] = format_value('object')
+                else:
+                    if value.get('type') != 'file':
+                        data[value['title']] = format_value(value.get('type', 'object'))
+            return data if len(data) > 0 else None
+
+    def get_swagger_request_files(self, value: str | dict) -> dict | None:
+        """
+        获取请求 files
+
+        :param value:
+        :return:
+        """
+        files = {}
+        if self.version == 2:
+            for v in value['parameters']:
+                if v.get('type') == 'file':
+                    files[v.get('name')] = format_value('object')
+            return files if len(files) > 0 else None
+        else:
+            if not isinstance(value, dict):
+                schema_data = self.get_swagger_schema_data(value)
+                for k, v in schema_data['properties'].items():
+                    if v.get('format') == 'binary':
+                        files[k] = format_value(v.get('type', 'object'))
+                return files if len(files) > 0 else None
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/file_control.py` & `httpfpt-0.6.3/httpfpt/utils/file_control.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import glob
-import os.path
-
-from pathlib import Path
-
-from httpfpt.core.get_conf import httpfpt_config
-from httpfpt.core.path_conf import httpfpt_path
-
-
-def get_file_property(filepath: str) -> tuple[str, str, str]:
-    """
-    获取文件属性
-
-    :param filepath:
-    :return:
-    """
-    file = Path(filepath)
-    filename = file.name
-    file_root_name = file.stem
-    filetype = file.suffix[1:]
-    return filename, file_root_name, filetype
-
-
-def search_all_case_data_files(filepath: str | None = None) -> list:
-    """
-    搜索指定项目目录下(包括子目录)所有测试用例数据文件
-
-    :return:
-    """
-    case_data_filepath = (
-        os.path.join(httpfpt_path.case_data_dir, f'{httpfpt_config.PROJECT_NAME}') if filepath is None else filepath
-    )
-    files = (
-        glob.glob(os.path.join(case_data_filepath, '**', '*.yaml'), recursive=True)
-        + glob.glob(os.path.join(case_data_filepath, '**', '*.yml'), recursive=True)
-        + glob.glob(os.path.join(case_data_filepath, '**', '*.json'), recursive=True)
-    )
-    return files
-
-
-def search_all_testcase_files() -> list:
-    """
-    搜索指定项目目录下(包括子目录)所有测试用例文件
-
-    :return:
-    """
-    files = glob.glob(
-        os.path.join(httpfpt_path.testcase_dir, f'{httpfpt_config.PROJECT_NAME}', '**', 'test_*.py'), recursive=True
-    )
-    return files
-
-
-def get_file_hash(filepath: str) -> str:
-    """
-    获取文件 hash (hash256) 值
-
-    :param filepath:
-    :return:
-    """
-    import hashlib
-
-    with open(filepath, 'rb') as f:
-        contents = f.read()
-        file_hash = hashlib.sha256(contents).hexdigest()
-    return file_hash
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import glob
+import os.path
+
+from pathlib import Path
+
+from httpfpt.core.get_conf import httpfpt_config
+from httpfpt.core.path_conf import httpfpt_path
+
+
+def get_file_property(filepath: str) -> tuple[str, str, str]:
+    """
+    获取文件属性
+
+    :param filepath:
+    :return:
+    """
+    file = Path(filepath)
+    filename = file.name
+    file_root_name = file.stem
+    filetype = file.suffix[1:]
+    return filename, file_root_name, filetype
+
+
+def search_all_case_data_files(filepath: str | None = None) -> list:
+    """
+    搜索指定项目目录下(包括子目录)所有测试用例数据文件
+
+    :return:
+    """
+    case_data_filepath = (
+        os.path.join(httpfpt_path.case_data_dir, f'{httpfpt_config.PROJECT_NAME}') if filepath is None else filepath
+    )
+    files = (
+        glob.glob(os.path.join(case_data_filepath, '**', '*.yaml'), recursive=True)
+        + glob.glob(os.path.join(case_data_filepath, '**', '*.yml'), recursive=True)
+        + glob.glob(os.path.join(case_data_filepath, '**', '*.json'), recursive=True)
+    )
+    return files
+
+
+def search_all_testcase_files() -> list:
+    """
+    搜索指定项目目录下(包括子目录)所有测试用例文件
+
+    :return:
+    """
+    files = glob.glob(
+        os.path.join(httpfpt_path.testcase_dir, f'{httpfpt_config.PROJECT_NAME}', '**', 'test_*.py'), recursive=True
+    )
+    return files
+
+
+def get_file_hash(filepath: str) -> str:
+    """
+    获取文件 hash (hash256) 值
+
+    :param filepath:
+    :return:
+    """
+    import hashlib
+
+    with open(filepath, 'rb') as f:
+        contents = f.read()
+        file_hash = hashlib.sha256(contents).hexdigest()
+    return file_hash
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/relate_testcase_executor.py` & `httpfpt-0.6.3/httpfpt/utils/relate_testcase_executor.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import ast
-import json
-
-from jsonpath import findall
-
-from httpfpt.common.errors import CorrelateTestCaseError, JsonPathFindError
-from httpfpt.common.log import log
-from httpfpt.common.variable_cache import variable_cache
-from httpfpt.db.redis_db import redis_client
-from httpfpt.enums.setup_type import SetupType
-from httpfpt.utils.allure_control import allure_step
-from httpfpt.utils.request.vars_extractor import var_extractor
-
-
-def exec_setup_testcase(parsed_data: dict, setup_testcase: str | dict) -> dict | None:
-    """
-    执行前置关联测试用例
-
-    :param parsed_data:
-    :param setup_testcase:
-    :return:
-    """
-    # 判断是否关联用例自身
-    parsed_case_id = parsed_data['case_id']
-    error_text = '执行关联测试用例失败，禁止关联自身'
-    if isinstance(setup_testcase, dict):
-        if setup_testcase['case_id'] == parsed_case_id:
-            raise CorrelateTestCaseError(error_text)
-    elif isinstance(setup_testcase, str):
-        if setup_testcase == parsed_case_id:
-            raise CorrelateTestCaseError(error_text)
-
-    # 判断关联测试用例是否存在
-    all_case_id = ast.literal_eval(redis_client.get(f'{redis_client.prefix}:case_id_list'))
-    error_text = '执行关联测试用例失败，未在测试用例中找到关联测试用例，请检查关联测试用例 case_id 是否存在'
-    if isinstance(setup_testcase, dict):
-        if setup_testcase['case_id'] not in all_case_id:
-            raise CorrelateTestCaseError(error_text)
-    elif isinstance(setup_testcase, str):
-        if setup_testcase not in all_case_id:
-            raise CorrelateTestCaseError(error_text)
-
-    # 执行关联测试用例
-    relate_count = 0
-    # 用例中 testcase 参数为更新请求数据或提取变量时
-    if isinstance(setup_testcase, dict):
-        relate_count += 1
-        relate_case_id = setup_testcase['case_id']
-        relate_case_filename = redis_client.get(f'{redis_client.case_id_file_prefix}:{relate_case_id}')
-        case_data = redis_client.get(f'{redis_client.case_data_prefix}:{relate_case_filename}')
-        case_data = json.loads(case_data)
-        case_data_test_steps = case_data['test_steps']
-        if isinstance(case_data_test_steps, list):
-            for case_test_steps in case_data_test_steps:
-                if relate_case_id == case_test_steps['case_id']:
-                    relate_case_steps = case_test_steps
-                    is_circular_relate(parsed_case_id, relate_case_steps)
-                    if setup_testcase.get('request') is not None:
-                        testcase_data = {
-                            'test_steps': relate_case_steps,
-                            'update_request_data': setup_testcase['request'],
-                        }
-                        case_data.update(testcase_data)
-                        response = relate_testcase_exec_with_new_request_data(case_data)
-                        # 使用更新请求数据后的请求响应提取变量
-                        if setup_testcase.get('response') is not None:
-                            testcase_data = {
-                                'set_var_response': setup_testcase['response'],
-                            }
-                            relate_testcase_extract_with_response(testcase_data, response)
-                    else:
-                        if setup_testcase.get('response') is not None:
-                            testcase_data = {
-                                'test_steps': relate_case_steps,
-                                'set_var_response': setup_testcase['response'],
-                            }
-                            case_data.update(testcase_data)
-                            relate_testcase_extract(case_data)
-        else:
-            relate_case_steps = case_data_test_steps
-            is_circular_relate(parsed_case_id, relate_case_steps)
-            if setup_testcase.get('request') is not None:
-                testcase_data = {'update_request_data': setup_testcase['request']}
-                case_data.update(testcase_data)
-                response = relate_testcase_exec_with_new_request_data(case_data)
-                if setup_testcase.get('response') is not None:
-                    testcase_data = {'set_var_response': setup_testcase['response']}
-                    relate_testcase_extract_with_response(testcase_data, response)
-            else:
-                if setup_testcase.get('response') is not None:
-                    testcase_data = {'set_var_response': setup_testcase['response']}
-                    case_data.update(testcase_data)
-                    relate_testcase_extract(case_data)
-
-    # 用例中 testcase 参数为直接关联测试用例时
-    elif isinstance(setup_testcase, str):
-        relate_case_filename = redis_client.get(f'{redis_client.case_id_file_prefix}:{setup_testcase}')
-        case_data = redis_client.get(f'{redis_client.case_data_prefix}:{relate_case_filename}')
-        case_data = json.loads(case_data)
-        case_data_test_steps = case_data['test_steps']
-        if isinstance(case_data_test_steps, list):
-            for case_test_steps in case_data_test_steps:
-                if setup_testcase == case_test_steps['case_id']:
-                    relate_case_steps = case_test_steps
-                    is_circular_relate(parsed_case_id, relate_case_steps)
-                    new_data = {'test_steps': relate_case_steps}
-                    case_data.update(new_data)
-                    relate_testcase_exec(case_data)
-        else:
-            relate_case_steps = case_data_test_steps
-            is_circular_relate(parsed_case_id, relate_case_steps)
-            relate_testcase_exec(case_data)
-
-    if relate_count > 0:
-        # 应用关联测试用例变量到请求数据，使用模糊匹配，可能有解析速度优化效果
-        if '^' in str(parsed_data):
-            relate_parsed_data = var_extractor.relate_vars_replace(parsed_data)
-            return relate_parsed_data
-
-
-def is_circular_relate(current_case_id: str, relate_case_steps: dict) -> None:
-    """
-    判断是否循环关联
-
-    :param current_case_id:
-    :param relate_case_steps:
-    :return:
-    """
-    relate_case_setup_testcases = []
-    try:
-        relate_case_setup = relate_case_steps['setup']
-        if relate_case_setup:
-            for setup in relate_case_setup:
-                for key, value in setup.items():
-                    if key == SetupType.TESTCASE:
-                        if isinstance(value, str):
-                            relate_case_setup_testcases.append(value)
-                        if isinstance(value, dict):
-                            relate_case_setup_testcases.append(value['case_id'])
-    except KeyError:
-        pass
-    else:
-        if relate_case_setup_testcases:
-            for relate_testcase in relate_case_setup_testcases:
-                text = '关联测试用例执行失败，关联测试用例中的前置关联测试用例包含当前测试用例，导致循环引用'
-                if current_case_id == relate_testcase:
-                    raise CorrelateTestCaseError(text)
-
-
-def relate_testcase_extract(testcase_data: dict) -> None:
-    """
-    关联测试用例提取变量
-
-    :param testcase_data:
-    :return:
-    """
-    from httpfpt.common.send_request import send_request
-
-    msg = f'>>> 执行关联测试用例变量提取：{testcase_data["test_steps"]["case_id"]}'
-    log.debug(msg)
-    allure_step(msg, '此文件为空')
-    response = send_request.send_request(testcase_data, log_data=False, relate_log=True)
-    relate_testcase_extract_with_response(testcase_data, response)
-    log.info('<<< 关联测试用例变量提取执行完成')
-
-
-def relate_testcase_extract_with_response(testcase_data: dict, response: dict) -> None:
-    """
-    关联测试用例提取变量（基于请求响应）
-
-    :param testcase_data:
-    :param response:
-    :return:
-    """
-    for s in testcase_data['set_var_response']:
-        value = findall(s['jsonpath'], response)
-        if value:
-            variable_cache.set(s['key'], value[0], tag='relate_testcase')
-        else:
-            raise JsonPathFindError('jsonpath 取值失败，表达式: {}'.format(s['jsonpath']))
-
-
-def relate_testcase_exec_with_new_request_data(testcase_data: dict) -> dict:
-    """
-    关联测试用例（使用新请求数据）执行
-
-    :param testcase_data:
-    :return:
-    """
-    from httpfpt.common.send_request import send_request
-
-    msg = f'>>> 执行关联测试用例（使用新请求数据）：{testcase_data["test_steps"]["case_id"]}'
-    log.debug(msg)
-    allure_step(msg, '此文件为空')
-    for u in testcase_data['update_request_data']:
-        keys = u['jsonpath'].split('.')[1:]
-        new_request_data = {}
-        current_level = new_request_data
-        for key in keys[:-1]:
-            current_level[key] = {}
-            current_level = current_level[key]
-        current_level[keys[-1]] = u['value']
-        testcase_data['test_steps']['request'].update(new_request_data)
-        log.info(f'更新关联测试用例请求数据：{new_request_data}')
-    response = send_request.send_request(testcase_data, log_data=False, relate_log=True)
-    log.info('<<< 关联测试用例（使用新请求数据）执行完成')
-    return response
-
-
-def relate_testcase_exec(testcase_data: dict) -> None:
-    """
-    关联测试用例执行
-
-    :param testcase_data:
-    :return:
-    """
-    from httpfpt.common.send_request import send_request
-
-    msg = f'>>> 执行关联测试用例：{testcase_data["test_steps"]["case_id"]}'
-    log.debug(msg)
-    allure_step(msg, '此文件为空')
-    send_request.send_request(testcase_data, log_data=False, relate_log=True)
-    log.info('<<< 关联测试用例执行完成')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import ast
+import json
+
+from jsonpath import findall
+
+from httpfpt.common.errors import CorrelateTestCaseError, JsonPathFindError
+from httpfpt.common.log import log
+from httpfpt.common.variable_cache import variable_cache
+from httpfpt.db.redis_db import redis_client
+from httpfpt.enums.setup_type import SetupType
+from httpfpt.utils.allure_control import allure_step
+from httpfpt.utils.request.vars_extractor import var_extractor
+
+
+def exec_setup_testcase(parsed_data: dict, setup_testcase: str | dict) -> dict | None:
+    """
+    执行前置关联测试用例
+
+    :param parsed_data:
+    :param setup_testcase:
+    :return:
+    """
+    # 判断是否关联用例自身
+    parsed_case_id = parsed_data['case_id']
+    error_text = '执行关联测试用例失败，禁止关联自身'
+    if isinstance(setup_testcase, dict):
+        if setup_testcase['case_id'] == parsed_case_id:
+            raise CorrelateTestCaseError(error_text)
+    elif isinstance(setup_testcase, str):
+        if setup_testcase == parsed_case_id:
+            raise CorrelateTestCaseError(error_text)
+
+    # 判断关联测试用例是否存在
+    all_case_id = ast.literal_eval(redis_client.get(f'{redis_client.prefix}:case_id_list'))
+    error_text = '执行关联测试用例失败，未在测试用例中找到关联测试用例，请检查关联测试用例 case_id 是否存在'
+    if isinstance(setup_testcase, dict):
+        if setup_testcase['case_id'] not in all_case_id:
+            raise CorrelateTestCaseError(error_text)
+    elif isinstance(setup_testcase, str):
+        if setup_testcase not in all_case_id:
+            raise CorrelateTestCaseError(error_text)
+
+    # 执行关联测试用例
+    relate_count = 0
+    # 用例中 testcase 参数为更新请求数据或提取变量时
+    if isinstance(setup_testcase, dict):
+        relate_count += 1
+        relate_case_id = setup_testcase['case_id']
+        relate_case_filename = redis_client.get(f'{redis_client.case_id_file_prefix}:{relate_case_id}')
+        case_data = redis_client.get(f'{redis_client.case_data_prefix}:{relate_case_filename}')
+        case_data = json.loads(case_data)
+        case_data_test_steps = case_data['test_steps']
+        if isinstance(case_data_test_steps, list):
+            for case_test_steps in case_data_test_steps:
+                if relate_case_id == case_test_steps['case_id']:
+                    relate_case_steps = case_test_steps
+                    is_circular_relate(parsed_case_id, relate_case_steps)
+                    if setup_testcase.get('request') is not None:
+                        testcase_data = {
+                            'test_steps': relate_case_steps,
+                            'update_request_data': setup_testcase['request'],
+                        }
+                        case_data.update(testcase_data)
+                        response = relate_testcase_exec_with_new_request_data(case_data)
+                        # 使用更新请求数据后的请求响应提取变量
+                        if setup_testcase.get('response') is not None:
+                            testcase_data = {
+                                'set_var_response': setup_testcase['response'],
+                            }
+                            relate_testcase_extract_with_response(testcase_data, response)
+                    else:
+                        if setup_testcase.get('response') is not None:
+                            testcase_data = {
+                                'test_steps': relate_case_steps,
+                                'set_var_response': setup_testcase['response'],
+                            }
+                            case_data.update(testcase_data)
+                            relate_testcase_extract(case_data)
+        else:
+            relate_case_steps = case_data_test_steps
+            is_circular_relate(parsed_case_id, relate_case_steps)
+            if setup_testcase.get('request') is not None:
+                testcase_data = {'update_request_data': setup_testcase['request']}
+                case_data.update(testcase_data)
+                response = relate_testcase_exec_with_new_request_data(case_data)
+                if setup_testcase.get('response') is not None:
+                    testcase_data = {'set_var_response': setup_testcase['response']}
+                    relate_testcase_extract_with_response(testcase_data, response)
+            else:
+                if setup_testcase.get('response') is not None:
+                    testcase_data = {'set_var_response': setup_testcase['response']}
+                    case_data.update(testcase_data)
+                    relate_testcase_extract(case_data)
+
+    # 用例中 testcase 参数为直接关联测试用例时
+    elif isinstance(setup_testcase, str):
+        relate_case_filename = redis_client.get(f'{redis_client.case_id_file_prefix}:{setup_testcase}')
+        case_data = redis_client.get(f'{redis_client.case_data_prefix}:{relate_case_filename}')
+        case_data = json.loads(case_data)
+        case_data_test_steps = case_data['test_steps']
+        if isinstance(case_data_test_steps, list):
+            for case_test_steps in case_data_test_steps:
+                if setup_testcase == case_test_steps['case_id']:
+                    relate_case_steps = case_test_steps
+                    is_circular_relate(parsed_case_id, relate_case_steps)
+                    new_data = {'test_steps': relate_case_steps}
+                    case_data.update(new_data)
+                    relate_testcase_exec(case_data)
+        else:
+            relate_case_steps = case_data_test_steps
+            is_circular_relate(parsed_case_id, relate_case_steps)
+            relate_testcase_exec(case_data)
+
+    if relate_count > 0:
+        # 应用关联测试用例变量到请求数据，使用模糊匹配，可能有解析速度优化效果
+        if '^' in str(parsed_data):
+            relate_parsed_data = var_extractor.relate_vars_replace(parsed_data)
+            return relate_parsed_data
+
+
+def is_circular_relate(current_case_id: str, relate_case_steps: dict) -> None:
+    """
+    判断是否循环关联
+
+    :param current_case_id:
+    :param relate_case_steps:
+    :return:
+    """
+    relate_case_setup_testcases = []
+    try:
+        relate_case_setup = relate_case_steps['setup']
+        if relate_case_setup:
+            for setup in relate_case_setup:
+                for key, value in setup.items():
+                    if key == SetupType.TESTCASE:
+                        if isinstance(value, str):
+                            relate_case_setup_testcases.append(value)
+                        if isinstance(value, dict):
+                            relate_case_setup_testcases.append(value['case_id'])
+    except KeyError:
+        pass
+    else:
+        if relate_case_setup_testcases:
+            for relate_testcase in relate_case_setup_testcases:
+                text = '关联测试用例执行失败，关联测试用例中的前置关联测试用例包含当前测试用例，导致循环引用'
+                if current_case_id == relate_testcase:
+                    raise CorrelateTestCaseError(text)
+
+
+def relate_testcase_extract(testcase_data: dict) -> None:
+    """
+    关联测试用例提取变量
+
+    :param testcase_data:
+    :return:
+    """
+    from httpfpt.common.send_request import send_request
+
+    msg = f'>>> 执行关联测试用例变量提取：{testcase_data["test_steps"]["case_id"]}'
+    log.debug(msg)
+    allure_step(msg, '此文件为空')
+    response = send_request.send_request(testcase_data, log_data=False, relate_log=True)
+    relate_testcase_extract_with_response(testcase_data, response)
+    log.info('<<< 关联测试用例变量提取执行完成')
+
+
+def relate_testcase_extract_with_response(testcase_data: dict, response: dict) -> None:
+    """
+    关联测试用例提取变量（基于请求响应）
+
+    :param testcase_data:
+    :param response:
+    :return:
+    """
+    for s in testcase_data['set_var_response']:
+        value = findall(s['jsonpath'], response)
+        if value:
+            variable_cache.set(s['key'], value[0], tag='relate_testcase')
+        else:
+            raise JsonPathFindError('jsonpath 取值失败，表达式: {}'.format(s['jsonpath']))
+
+
+def relate_testcase_exec_with_new_request_data(testcase_data: dict) -> dict:
+    """
+    关联测试用例（使用新请求数据）执行
+
+    :param testcase_data:
+    :return:
+    """
+    from httpfpt.common.send_request import send_request
+
+    msg = f'>>> 执行关联测试用例（使用新请求数据）：{testcase_data["test_steps"]["case_id"]}'
+    log.debug(msg)
+    allure_step(msg, '此文件为空')
+    for u in testcase_data['update_request_data']:
+        keys = u['jsonpath'].split('.')[1:]
+        new_request_data = {}
+        current_level = new_request_data
+        for key in keys[:-1]:
+            current_level[key] = {}
+            current_level = current_level[key]
+        current_level[keys[-1]] = u['value']
+        testcase_data['test_steps']['request'].update(new_request_data)
+        log.info(f'更新关联测试用例请求数据：{new_request_data}')
+    response = send_request.send_request(testcase_data, log_data=False, relate_log=True)
+    log.info('<<< 关联测试用例（使用新请求数据）执行完成')
+    return response
+
+
+def relate_testcase_exec(testcase_data: dict) -> None:
+    """
+    关联测试用例执行
+
+    :param testcase_data:
+    :return:
+    """
+    from httpfpt.common.send_request import send_request
+
+    msg = f'>>> 执行关联测试用例：{testcase_data["test_steps"]["case_id"]}'
+    log.debug(msg)
+    allure_step(msg, '此文件为空')
+    send_request.send_request(testcase_data, log_data=False, relate_log=True)
+    log.info('<<< 关联测试用例执行完成')
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/request/hook_executor.py` & `httpfpt-0.6.3/httpfpt/utils/request/hook_executor.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import json
-import re
-
-from typing import Any
-
-from httpfpt.common.log import log
-from httpfpt.enums.setup_type import SetupType
-from httpfpt.enums.teardown_type import TeardownType
-
-
-class HookExecutor:
-    def __init__(self) -> None:
-        # hook 开头: a-zA-Z_
-        # hook 表达: ${func()} 或 ${func(1, 2)}
-        self.func_re = re.compile(r'\${([a-zA-Z_]\w*\([$\w.\-/\s=,]*\))}')
-
-    def hook_func_value_replace(self, target: dict) -> Any:
-        """
-        执行除前后置 hook 以外的所有 hook 函数并替换为它的返回值
-
-        :param target:
-        :return:
-        """
-        # 数据排除
-        setup = target['test_steps'].get('setup')
-        teardown = target['test_steps'].get('teardown')
-        setup_hooks_with_index = []
-        teardown_hooks_with_index = []
-        if setup:
-            setup_hooks_with_index.extend(
-                [(i, item) for i, item in enumerate(setup) if item.get(SetupType.HOOK) is not None]
-            )
-            if setup_hooks_with_index:
-                target['test_steps']['setup'] = [
-                    item for item in target['test_steps']['setup'] if item.get(SetupType.HOOK) is None
-                ]
-        if teardown:
-            teardown_hooks_with_index.extend(
-                [(i, item) for i, item in enumerate(teardown) if item.get(TeardownType.HOOK) is not None]
-            )
-            if teardown_hooks_with_index:
-                target['test_steps']['teardown'] = [
-                    item for item in target['test_steps']['teardown'] if item.get(TeardownType.HOOK) is None
-                ]
-
-        str_target = json.dumps(target, ensure_ascii=False)
-
-        match = self.func_re.search(str_target)
-        if not match:
-            return target
-
-        # hook 返回值替换
-        exec('from httpfpt.data.hooks import *')
-        for match in self.func_re.finditer(str_target):
-            hook_key = match.group(1)
-            try:
-                # locals() 获取到执行函数内所有变量并以字典形式返回
-                loc = locals()
-                exec(f'result = {hook_key}')
-                value = str(loc['result'])
-                str_target = self.func_re.sub(value, str_target, 1)
-                log.info(f'请求数据函数 {hook_key} 返回值替换完成')
-            except Exception as e:
-                log.error(f'请求数据函数 {hook_key} 返回值替换失败: {e}')
-                raise e
-
-        dict_target = json.loads(str_target)
-
-        # 数据还原
-        if setup:
-            if setup_hooks_with_index:
-                for i, item in setup_hooks_with_index:
-                    target['test_steps']['setup'].insert(i, item)
-        if teardown:
-            if teardown_hooks_with_index:
-                for i, item in teardown_hooks_with_index:
-                    target['test_steps']['teardown'].insert(i, item)
-
-        return dict_target
-
-    def exec_hook_func(self, hook_var: str) -> None:
-        """
-        执行 hook 函数不返回任何值
-
-        :param hook_var:
-        :return:
-        """
-        key = self.func_re.search(hook_var)
-        func = key.group(1)
-        exec('from httpfpt.data.hooks import *')
-        log.info(f'执行 hook：{func}')
-        exec(func)
-
-    @staticmethod
-    def exec_any_code(code: str) -> bool:
-        """
-        执行任何函数
-
-        :param code:
-        :return:
-        """
-        exec('import os')
-        exec('import sys')
-        result = eval(code)
-        log.info(f'执行代码：{code}')
-        return result
-
-
-hook_executor = HookExecutor()
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import json
+import re
+
+from typing import Any
+
+from httpfpt.common.log import log
+from httpfpt.enums.setup_type import SetupType
+from httpfpt.enums.teardown_type import TeardownType
+
+
+class HookExecutor:
+    def __init__(self) -> None:
+        # hook 开头: a-zA-Z_
+        # hook 表达: ${func()} 或 ${func(1, 2)}
+        self.func_re = re.compile(r'\${([a-zA-Z_]\w*\([$\w.\-/\s=,]*\))}')
+
+    def hook_func_value_replace(self, target: dict) -> Any:
+        """
+        执行除前后置 hook 以外的所有 hook 函数并替换为它的返回值
+
+        :param target:
+        :return:
+        """
+        # 数据排除
+        setup = target['test_steps'].get('setup')
+        teardown = target['test_steps'].get('teardown')
+        setup_hooks_with_index = []
+        teardown_hooks_with_index = []
+        if setup:
+            setup_hooks_with_index.extend(
+                [(i, item) for i, item in enumerate(setup) if item.get(SetupType.HOOK) is not None]
+            )
+            if setup_hooks_with_index:
+                target['test_steps']['setup'] = [
+                    item for item in target['test_steps']['setup'] if item.get(SetupType.HOOK) is None
+                ]
+        if teardown:
+            teardown_hooks_with_index.extend(
+                [(i, item) for i, item in enumerate(teardown) if item.get(TeardownType.HOOK) is not None]
+            )
+            if teardown_hooks_with_index:
+                target['test_steps']['teardown'] = [
+                    item for item in target['test_steps']['teardown'] if item.get(TeardownType.HOOK) is None
+                ]
+
+        str_target = json.dumps(target, ensure_ascii=False)
+
+        match = self.func_re.search(str_target)
+        if not match:
+            return target
+
+        # hook 返回值替换
+        exec('from httpfpt.data.hooks import *')
+        for match in self.func_re.finditer(str_target):
+            hook_key = match.group(1)
+            try:
+                # locals() 获取到执行函数内所有变量并以字典形式返回
+                loc = locals()
+                exec(f'result = {hook_key}')
+                value = str(loc['result'])
+                str_target = self.func_re.sub(value, str_target, 1)
+                log.info(f'请求数据函数 {hook_key} 返回值替换完成')
+            except Exception as e:
+                log.error(f'请求数据函数 {hook_key} 返回值替换失败: {e}')
+                raise e
+
+        dict_target = json.loads(str_target)
+
+        # 数据还原
+        if setup:
+            if setup_hooks_with_index:
+                for i, item in setup_hooks_with_index:
+                    target['test_steps']['setup'].insert(i, item)
+        if teardown:
+            if teardown_hooks_with_index:
+                for i, item in teardown_hooks_with_index:
+                    target['test_steps']['teardown'].insert(i, item)
+
+        return dict_target
+
+    def exec_hook_func(self, hook_var: str) -> None:
+        """
+        执行 hook 函数不返回任何值
+
+        :param hook_var:
+        :return:
+        """
+        key = self.func_re.search(hook_var)
+        func = key.group(1)
+        exec('from httpfpt.data.hooks import *')
+        log.info(f'执行 hook：{func}')
+        exec(func)
+
+    @staticmethod
+    def exec_any_code(code: str) -> bool:
+        """
+        执行任何函数
+
+        :param code:
+        :return:
+        """
+        exec('import os')
+        exec('import sys')
+        result = eval(code)
+        log.info(f'执行代码：{code}')
+        return result
+
+
+hook_executor = HookExecutor()
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/request/ids_extract.py` & `httpfpt-0.6.3/httpfpt/utils/request/ids_extract.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-from httpfpt.common.errors import RequestDataParseError
-
-
-def get_ids(request_data: dict | list) -> list:
-    """
-    从请求数据获取数据驱动下的 ids 数据
-
-    :param request_data: 请求数据
-    :return:
-    """
-    ids = []
-    try:
-        if isinstance(request_data, dict):
-            module = request_data['config']['module']
-            case_id = request_data['test_steps']['case_id']
-            ids.append(f'module: {module}, case_id: {case_id}')
-        else:
-            for data in request_data:
-                module = data['config']['module']
-                case_id = data['test_steps']['case_id']
-                ids.append(f'module: {module}, case_id: {case_id}')
-    except KeyError as e:
-        raise RequestDataParseError('测试用例 ids 获取失败, 请检查测试用例数据是否符合规范: {}'.format(e))
-    return ids
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+from httpfpt.common.errors import RequestDataParseError
+
+
+def get_ids(request_data: dict | list) -> list:
+    """
+    从请求数据获取数据驱动下的 ids 数据
+
+    :param request_data: 请求数据
+    :return:
+    """
+    ids = []
+    try:
+        if isinstance(request_data, dict):
+            module = request_data['config']['module']
+            case_id = request_data['test_steps']['case_id']
+            ids.append(f'module: {module}, case_id: {case_id}')
+        else:
+            for data in request_data:
+                module = data['config']['module']
+                case_id = data['test_steps']['case_id']
+                ids.append(f'module: {module}, case_id: {case_id}')
+    except KeyError as e:
+        raise RequestDataParseError('测试用例 ids 获取失败, 请检查测试用例数据是否符合规范: {}'.format(e))
+    return ids
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/request/vars_recorder.py` & `httpfpt-0.6.3/httpfpt/utils/request/vars_recorder.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from jsonpath import findall
-
-from httpfpt.common.env_handler import write_env_vars
-from httpfpt.common.errors import JsonPathFindError, VariableError
-from httpfpt.common.variable_cache import variable_cache
-from httpfpt.common.yaml_handler import write_yaml_vars
-from httpfpt.core.path_conf import httpfpt_path
-from httpfpt.enums.var_type import VarType
-
-
-def record_variables(jsonpath: str, target: dict, key: str, set_type: str, env: str) -> None:
-    """
-    记录变量
-
-    :param jsonpath:
-    :param set_type:
-    :param target:
-    :param key:
-    :param env:
-    :return:
-    """
-    value = findall(jsonpath, target)
-    if not value:
-        raise JsonPathFindError(f'jsonpath 取值失败, 表达式: {jsonpath}')
-    value_str = str(value[0])
-    if set_type == VarType.CACHE:
-        variable_cache.set(key, value_str)
-    elif set_type == VarType.ENV:
-        write_env_vars(httpfpt_path.run_env_dir, env, key, value_str)
-    elif set_type == VarType.GLOBAL:
-        write_yaml_vars({key: value_str})
-    else:
-        raise VariableError(f'变量设置失败, 用例参数 "type: {set_type}" 值错误, 请使用 cache / env / global')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from jsonpath import findall
+
+from httpfpt.common.env_handler import write_env_vars
+from httpfpt.common.errors import JsonPathFindError, VariableError
+from httpfpt.common.variable_cache import variable_cache
+from httpfpt.common.yaml_handler import write_yaml_vars
+from httpfpt.core.path_conf import httpfpt_path
+from httpfpt.enums.var_type import VarType
+
+
+def record_variables(jsonpath: str, target: dict, key: str, set_type: str, env: str) -> None:
+    """
+    记录变量
+
+    :param jsonpath:
+    :param set_type:
+    :param target:
+    :param key:
+    :param env:
+    :return:
+    """
+    value = findall(jsonpath, target)
+    if not value:
+        raise JsonPathFindError(f'jsonpath 取值失败, 表达式: {jsonpath}')
+    value_str = str(value[0])
+    if set_type == VarType.CACHE:
+        variable_cache.set(key, value_str)
+    elif set_type == VarType.ENV:
+        write_env_vars(httpfpt_path.run_env_dir, env, key, value_str)
+    elif set_type == VarType.GLOBAL:
+        write_yaml_vars({key: value_str})
+    else:
+        raise VariableError(f'变量设置失败, 用例参数 "type: {set_type}" 值错误, 请使用 cache / env / global')
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/send_report/dingding.py` & `httpfpt-0.6.3/httpfpt/utils/send_report/dingding.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from httpfpt.common.log import log
-from httpfpt.core.get_conf import httpfpt_config
-
-
-class DingDing:
-    def __init__(self, content: dict):
-        self.content = content
-
-    def send(self) -> None:
-        try:
-            import requests
-
-            headers = {'Content-Type': 'application/json; charset=utf-8', 'Connection': 'close'}
-            data = {
-                'msgtype': 'markdown',
-                'markdown': {
-                    'title': httpfpt_config.TEST_REPORT_TITLE,
-                    'text': f"> ## {httpfpt_config.PROJECT_NAME} 自动化测试报告\n\n"
-                    f"> 👤 测试人员: {httpfpt_config.TESTER_NAME}\n\n"
-                    f"> 🤖 测试结果: {self.content['result']}\n\n"
-                    f"> ✅ 通过用例: {self.content['passed']}\n\n"
-                    f"> 🔧 失败用例: {self.content['failed']}\n\n"
-                    f"> ❌ 错误用例: {self.content['error']}\n\n"
-                    f"> ⚠️ 跳过用例: {self.content['skipped']}\n\n"
-                    f"> ⌛ 开始时间: {self.content['started_time']}\n\n"
-                    f"> ⏱️ 执行耗时: {self.content['elapsed']}\n\n"
-                    f"> ➡️ [查看详情](https://foryourself)",
-                },
-            }
-            response = requests.session().post(
-                url=httpfpt_config.DINGDING_WEBHOOK,
-                json=data,
-                headers=headers,
-                proxies=httpfpt_config.DINGDING_PROXY,  # type: ignore
-            )
-            response.raise_for_status()
-        except Exception as e:
-            log.error(f'钉钉消息发送异常: {e}')
-        else:
-            log.success('钉钉消息发送成功')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from httpfpt.common.log import log
+from httpfpt.core.get_conf import httpfpt_config
+
+
+class DingDing:
+    def __init__(self, content: dict):
+        self.content = content
+
+    def send(self) -> None:
+        try:
+            import requests
+
+            headers = {'Content-Type': 'application/json; charset=utf-8', 'Connection': 'close'}
+            data = {
+                'msgtype': 'markdown',
+                'markdown': {
+                    'title': httpfpt_config.TEST_REPORT_TITLE,
+                    'text': f"> ## {httpfpt_config.PROJECT_NAME} 自动化测试报告\n\n"
+                    f"> 👤 测试人员: {httpfpt_config.TESTER_NAME}\n\n"
+                    f"> 🤖 测试结果: {self.content['result']}\n\n"
+                    f"> ✅ 通过用例: {self.content['passed']}\n\n"
+                    f"> 🔧 失败用例: {self.content['failed']}\n\n"
+                    f"> ❌ 错误用例: {self.content['error']}\n\n"
+                    f"> ⚠️ 跳过用例: {self.content['skipped']}\n\n"
+                    f"> ⌛ 开始时间: {self.content['started_time']}\n\n"
+                    f"> ⏱️ 执行耗时: {self.content['elapsed']}\n\n"
+                    f"> ➡️ [查看详情](https://foryourself)",
+                },
+            }
+            response = requests.session().post(
+                url=httpfpt_config.DINGDING_WEBHOOK,
+                json=data,
+                headers=headers,
+                proxies=httpfpt_config.DINGDING_PROXY,  # type: ignore
+            )
+            response.raise_for_status()
+        except Exception as e:
+            log.error(f'钉钉消息发送异常: {e}')
+        else:
+            log.success('钉钉消息发送成功')
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/send_report/email.py` & `httpfpt-0.6.3/httpfpt/utils/send_report/email.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from __future__ import annotations
-
-import smtplib
-import time
-
-from email.mime.application import MIMEApplication
-from email.mime.multipart import MIMEMultipart
-from email.mime.text import MIMEText
-from importlib.resources import open_text
-
-from jinja2 import Template
-
-from httpfpt.common.log import log
-from httpfpt.core.get_conf import httpfpt_config
-from httpfpt.enums.email_type import EmailType
-from httpfpt.utils.file_control import get_file_property
-
-
-class SendEmail:
-    def __init__(self, content: dict, filename: str | None = None):
-        self.content = content
-        self.filename = filename
-
-    def take_report(self) -> MIMEMultipart:
-        """
-        获取报告
-        """
-        msg = MIMEMultipart()
-        msg['Subject'] = httpfpt_config.TEST_REPORT_TITLE
-        msg['From'] = httpfpt_config.EMAIL_USER
-        msg['date'] = time.strftime('%a, %d %b %Y %H:%M:%S %z')
-        self.content.update({'test_title': httpfpt_config.TEST_REPORT_TITLE})
-        self.content.update({'tester_name': httpfpt_config.TESTER_NAME})
-
-        # 邮件正文
-        with open_text('httpfpt.templates', 'email_notification.html') as f:
-            html = Template(f.read())
-
-        mail_body = MIMEText(html.render(**self.content), _subtype='html', _charset='utf-8')
-        msg.attach(mail_body)
-
-        # 读取要发送的附件
-        if self.filename:
-            with open(self.filename, 'rb') as f:
-                annex_body = f.read()
-                # 邮件附件
-                att1 = MIMEApplication(annex_body)
-                att1['Content-Type'] = 'application/octet-stream'
-                att1['Content-Disposition'] = f'attachment; filename={get_file_property(self.filename)[0]}'
-                msg.attach(att1)
-
-        return msg
-
-    def take_error(self) -> MIMEMultipart:
-        """
-        获取错误信息
-        """
-        msg = MIMEMultipart()
-        msg['Subject'] = 'HttpFpt 运行异常通知'
-        msg['From'] = httpfpt_config.EMAIL_USER
-        msg['date'] = time.strftime('%a, %d %b %Y %H:%M:%S %z')
-
-        # 邮件正文
-        with open_text('httpfpt.templates', 'email_notification.html') as f:
-            html = Template(f.read())
-
-        mail_body = MIMEText(html.render(**self.content), _subtype='html', _charset='utf-8')
-        msg.attach(mail_body)
-
-        return msg
-
-    def _send(self, msg_type: int) -> None:
-        """
-        发送邮件
-        """
-        msg = ''
-        if msg_type == EmailType.REPORT:
-            msg = self.take_report().as_string()
-        elif msg_type == EmailType.ERROR:
-            msg = self.take_error().as_string()
-        if httpfpt_config.EMAIL_SSL:
-            smtp = smtplib.SMTP_SSL(host=httpfpt_config.EMAIL_SERVER, port=httpfpt_config.EMAIL_PORT)
-        else:
-            smtp = smtplib.SMTP(host=httpfpt_config.EMAIL_SERVER, port=httpfpt_config.EMAIL_PORT)
-        smtp.login(httpfpt_config.EMAIL_USER, httpfpt_config.EMAIL_PASSWORD)
-        smtp.sendmail(httpfpt_config.EMAIL_USER, httpfpt_config.EMAIL_SEND_TO, msg)
-        smtp.quit()
-
-    def send_report(self) -> None:
-        try:
-            self._send(0)
-        except Exception as e:
-            log.error(f'测试报告邮件发送失败: {e}')
-        else:
-            log.info('测试报告邮件发送成功')
-
-    def send_error(self) -> None:
-        try:
-            self._send(1)
-        except Exception as e:
-            log.error(f'运行异常通知邮件发送失败: {e}')
-        else:
-            log.info('运行异常通知邮件发送成功')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import smtplib
+import time
+
+from email.mime.application import MIMEApplication
+from email.mime.multipart import MIMEMultipart
+from email.mime.text import MIMEText
+from importlib.resources import open_text
+
+from jinja2 import Template
+
+from httpfpt.common.log import log
+from httpfpt.core.get_conf import httpfpt_config
+from httpfpt.enums.email_type import EmailType
+from httpfpt.utils.file_control import get_file_property
+
+
+class SendEmail:
+    def __init__(self, content: dict, filename: str | None = None):
+        self.content = content
+        self.filename = filename
+
+    def take_report(self) -> MIMEMultipart:
+        """
+        获取报告
+        """
+        msg = MIMEMultipart()
+        msg['Subject'] = httpfpt_config.TEST_REPORT_TITLE
+        msg['From'] = httpfpt_config.EMAIL_USER
+        msg['date'] = time.strftime('%a, %d %b %Y %H:%M:%S %z')
+        self.content.update({'test_title': httpfpt_config.TEST_REPORT_TITLE})
+        self.content.update({'tester_name': httpfpt_config.TESTER_NAME})
+
+        # 邮件正文
+        with open_text('httpfpt.templates', 'email_notification.html') as f:
+            html = Template(f.read())
+
+        mail_body = MIMEText(html.render(**self.content), _subtype='html', _charset='utf-8')
+        msg.attach(mail_body)
+
+        # 读取要发送的附件
+        if self.filename:
+            with open(self.filename, 'rb') as f:
+                annex_body = f.read()
+                # 邮件附件
+                att1 = MIMEApplication(annex_body)
+                att1['Content-Type'] = 'application/octet-stream'
+                att1['Content-Disposition'] = f'attachment; filename={get_file_property(self.filename)[0]}'
+                msg.attach(att1)
+
+        return msg
+
+    def take_error(self) -> MIMEMultipart:
+        """
+        获取错误信息
+        """
+        msg = MIMEMultipart()
+        msg['Subject'] = 'HttpFpt 运行异常通知'
+        msg['From'] = httpfpt_config.EMAIL_USER
+        msg['date'] = time.strftime('%a, %d %b %Y %H:%M:%S %z')
+
+        # 邮件正文
+        with open_text('httpfpt.templates', 'email_notification.html') as f:
+            html = Template(f.read())
+
+        mail_body = MIMEText(html.render(**self.content), _subtype='html', _charset='utf-8')
+        msg.attach(mail_body)
+
+        return msg
+
+    def _send(self, msg_type: int) -> None:
+        """
+        发送邮件
+        """
+        msg = ''
+        if msg_type == EmailType.REPORT:
+            msg = self.take_report().as_string()
+        elif msg_type == EmailType.ERROR:
+            msg = self.take_error().as_string()
+        if httpfpt_config.EMAIL_SSL:
+            smtp = smtplib.SMTP_SSL(host=httpfpt_config.EMAIL_SERVER, port=httpfpt_config.EMAIL_PORT)
+        else:
+            smtp = smtplib.SMTP(host=httpfpt_config.EMAIL_SERVER, port=httpfpt_config.EMAIL_PORT)
+        smtp.login(httpfpt_config.EMAIL_USER, httpfpt_config.EMAIL_PASSWORD)
+        smtp.sendmail(httpfpt_config.EMAIL_USER, httpfpt_config.EMAIL_SEND_TO, msg)
+        smtp.quit()
+
+    def send_report(self) -> None:
+        try:
+            self._send(0)
+        except Exception as e:
+            log.error(f'测试报告邮件发送失败: {e}')
+        else:
+            log.info('测试报告邮件发送成功')
+
+    def send_error(self) -> None:
+        try:
+            self._send(1)
+        except Exception as e:
+            log.error(f'运行异常通知邮件发送失败: {e}')
+        else:
+            log.info('运行异常通知邮件发送成功')
```

### Comparing `httpfpt-0.6.2/httpfpt/utils/send_report/feishu.py` & `httpfpt-0.6.3/httpfpt/utils/send_report/feishu.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-from httpfpt.common.log import log
-from httpfpt.core.get_conf import httpfpt_config
-
-
-class FeiShu:
-    def __init__(self, content: dict):
-        self.content = content
-
-    def send(self) -> None:
-        # 发送飞书消息
-        try:
-            import requests
-
-            headers = {'Content-Type': 'application/json; charset=utf-8', 'Connection': 'close'}
-            data = {
-                'msg_type': 'post',
-                'content': {
-                    'post': {
-                        'zh_cn': {
-                            'title': httpfpt_config.TEST_REPORT_TITLE,
-                            'content': [
-                                [{'tag': 'text', 'text': f'👤 测试人员: {httpfpt_config.TESTER_NAME}'}],
-                                [{'tag': 'text', 'text': f"🤖 测试结果: {self.content['result']}"}],
-                                [{'tag': 'text', 'text': f"✅ 通过用例: {self.content['passed']}"}],
-                                [{'tag': 'text', 'text': f"🔧 失败用例: {self.content['failed']}"}],
-                                [{'tag': 'text', 'text': f"❌ 错误用例: {self.content['error']}"}],
-                                [{'tag': 'text', 'text': f"⚠️ 跳过用例: {self.content['skipped']}"}],
-                                [{'tag': 'text', 'text': f"⌛ 开始时间: {self.content['started_time']}"}],
-                                [{'tag': 'text', 'text': f"⏱️ 执行耗时: {self.content['elapsed']}"}],
-                                [{'tag': 'a', 'text': '➡️ 查看详情', 'href': 'https://foryourself'}],
-                            ],
-                        }
-                    }
-                },
-            }
-            response = requests.session().post(
-                url=httpfpt_config.FEISHU_WEBHOOK,
-                json=data,
-                headers=headers,
-                proxies=httpfpt_config.FEISHU_PROXY,  # type: ignore
-            )
-            response.raise_for_status()
-        except Exception as e:
-            log.error(f'飞书消息发送异常: {e}')
-        else:
-            log.success('飞书消息发送成功')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+from httpfpt.common.log import log
+from httpfpt.core.get_conf import httpfpt_config
+
+
+class FeiShu:
+    def __init__(self, content: dict):
+        self.content = content
+
+    def send(self) -> None:
+        # 发送飞书消息
+        try:
+            import requests
+
+            headers = {'Content-Type': 'application/json; charset=utf-8', 'Connection': 'close'}
+            data = {
+                'msg_type': 'post',
+                'content': {
+                    'post': {
+                        'zh_cn': {
+                            'title': httpfpt_config.TEST_REPORT_TITLE,
+                            'content': [
+                                [{'tag': 'text', 'text': f'👤 测试人员: {httpfpt_config.TESTER_NAME}'}],
+                                [{'tag': 'text', 'text': f"🤖 测试结果: {self.content['result']}"}],
+                                [{'tag': 'text', 'text': f"✅ 通过用例: {self.content['passed']}"}],
+                                [{'tag': 'text', 'text': f"🔧 失败用例: {self.content['failed']}"}],
+                                [{'tag': 'text', 'text': f"❌ 错误用例: {self.content['error']}"}],
+                                [{'tag': 'text', 'text': f"⚠️ 跳过用例: {self.content['skipped']}"}],
+                                [{'tag': 'text', 'text': f"⌛ 开始时间: {self.content['started_time']}"}],
+                                [{'tag': 'text', 'text': f"⏱️ 执行耗时: {self.content['elapsed']}"}],
+                                [{'tag': 'a', 'text': '➡️ 查看详情', 'href': 'https://foryourself'}],
+                            ],
+                        }
+                    }
+                },
+            }
+            response = requests.session().post(
+                url=httpfpt_config.FEISHU_WEBHOOK,
+                json=data,
+                headers=headers,
+                proxies=httpfpt_config.FEISHU_PROXY,  # type: ignore
+            )
+            response.raise_for_status()
+        except Exception as e:
+            log.error(f'飞书消息发送异常: {e}')
+        else:
+            log.success('飞书消息发送成功')
```

### Comparing `httpfpt-0.6.2/pyproject.toml` & `httpfpt-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "v0.6.2"
+version = "v0.6.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://wu-clan.github.io/httpfpt_docs/"
 repository = "https://github.com/wu-clan/httpfpt"
```

### Comparing `httpfpt-0.6.2/PKG-INFO` & `httpfpt-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpfpt
-Version: 0.6.2
+Version: 0.6.3
 Summary: 基于 HTTP 请求的快速数据驱动 pytest 接口自动化测试框架
 Home-page: https://wu-clan.github.io/httpfpt_docs/
 Author-Email: Wu Clan <jianhengwu0407@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

