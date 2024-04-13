# Comparing `tmp/dcicutils-8.8.3.1b3.tar.gz` & `tmp/dcicutils-8.8.3.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.3.1b3.tar", max compression
+gzip compressed data, was "dcicutils-8.8.3.1b4.tar", max compression
```

## Comparing `dcicutils-8.8.3.1b3.tar` & `dcicutils-8.8.3.1b4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1102 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/README.rst
--rw-r--r--   0        0        0        0 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     3108 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7414 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/data_utils.py
--rw-r--r--   0        0        0     4666 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    72972 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     2663 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/log_utils.py
--rw-r--r--   0        0        0   102210 2024-04-13 12:10:27.264815 dcicutils-8.8.3.1b3/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30480 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    14543 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    58450 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2027 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4714 2024-04-13 12:10:27.268815 dcicutils-8.8.3.1b3/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.3.1b3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/README.rst
+-rw-r--r--   0        0        0        0 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3108 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7414 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/data_utils.py
+-rw-r--r--   0        0        0     4666 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-13 12:12:31.007566 dcicutils-8.8.3.1b4/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   102210 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30480 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    14463 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-13 12:12:31.011566 dcicutils-8.8.3.1b4/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    58450 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4714 2024-04-13 12:12:31.015565 dcicutils-8.8.3.1b4/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.3.1b4/PKG-INFO
```

### Comparing `dcicutils-8.8.3.1b3/LICENSE.txt` & `dcicutils-8.8.3.1b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/README.rst` & `dcicutils-8.8.3.1b4/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/base.py` & `dcicutils-8.8.3.1b4/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/bundle_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/captured_output.py` & `dcicutils-8.8.3.1b4/dcicutils/captured_output.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/codebuild_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/command_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/common.py` & `dcicutils-8.8.3.1b4/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/contribution_scripts.py` & `dcicutils-8.8.3.1b4/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/contribution_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/creds_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/data_readers.py` & `dcicutils-8.8.3.1b4/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/data_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/datetime_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/deployment_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/diff_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/docker_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/ecr_scripts.py` & `dcicutils-8.8.3.1b4/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/ecr_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/ecs_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/env_base.py` & `dcicutils-8.8.3.1b4/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/env_manager.py` & `dcicutils-8.8.3.1b4/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/env_scripts.py` & `dcicutils-8.8.3.1b4/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/env_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.3.1b4/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/es_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/exceptions.py` & `dcicutils-8.8.3.1b4/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/ff_mocks.py` & `dcicutils-8.8.3.1b4/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/ff_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/file_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.3.1b4/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/glacier_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/jh_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.3.1b4/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/kibana/readme.md` & `dcicutils-8.8.3.1b4/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/lang_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.3.1b4/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.3.1b4/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.3.1b4/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/license_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/log_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/misc_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/opensearch_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/portal_object_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/portal_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/progress_bar.py` & `dcicutils-8.8.3.1b4/dcicutils/progress_bar.py`

 * *Files 6% similar despite different names*

```diff
@@ -255,33 +255,30 @@
     def _define_tidy_output_hack(self) -> None:
         # Some minor tqdm output tidying-up which for annoying anomalies; tqdm forces
         # a colon (:) before the percentage, e.g. ":  25%|"; and while we're at it do
         # a little ASCII progress animation, requiring a special ([progress]) sentinal
         # string in the display string where the progress bar should actually go,
         # which we do in _format_description. Other minor things too; see below.
         sys_stdout_write = sys.stdout.write
-        total_most_recent = None
-        progress_most_recent = None
-        description_most_recent = None
+        last_total = None ; last_progress = None ; last_text = None  # noqa
         def tidy_stdout_write(text: str) -> None:  # noqa
             nonlocal self, sys_stdout_write, sentinel_internal, spina, spini, spinn
-            nonlocal total_most_recent, progress_most_recent, description_most_recent
+            nonlocal last_total, last_progress, last_text
             def replace_first(value: str, match: str, replacement: str) -> str:  # noqa
                 return value[:i] + replacement + value[i + len(match):] if (i := value.find(match)) >= 0 else value
             def remove_extra_trailing_spaces(text: str) -> str:  # noqa
                 while text.endswith("  "):
                     text = text[:-1]
                 return text
-            if not text or not self._bar:
+            if not text:
                 return
-            if (self._bar.total == total_most_recent) and (self._bar.n == progress_most_recent):
-                return
-            total_most_recent = self._bar.total
-            progress_most_recent = self._bar.n
-            description_most_recent = self._description
+            if self._bar:
+                if ((self._bar.total == last_total) and (self._bar.n == last_progress) and (last_text == text)):
+                    return
+                last_total = self._bar.total ; last_progress = self._bar.n ; last_text = text  # noqa
             if (self._disabled or self._done) and sentinel_internal in text:
                 # Another hack to really disable output on interrupt; in this case we set
                 # tqdm.disable to True, but output can still dribble out, so if the output
                 # looks like it is from tqdm and we are disabled/done then do no output.
                 return
             if sentinel_internal in text:
                 spinc = spina[spini % spinn] if not ("100%|" in text) else "| ✓" ; spini += 1  # noqa
```

### Comparing `dcicutils-8.8.3.1b3/dcicutils/project_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/qa_checkers.py` & `dcicutils-8.8.3.1b4/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/qa_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/redis_tools.py` & `dcicutils-8.8.3.1b4/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/redis_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/s3_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/schema_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.3.1b4/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.3.1b4/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.3.1b4/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/secrets_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/sheet_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/snapshot_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/structured_data.py` & `dcicutils-8.8.3.1b4/dcicutils/structured_data.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/submitr/progress_constants.py` & `dcicutils-8.8.3.1b4/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.8.3.1b4/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/task_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/trace_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/validation_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/variant_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/dcicutils/zip_utils.py` & `dcicutils-8.8.3.1b4/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b3/pyproject.toml` & `dcicutils-8.8.3.1b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.3.1b3"  # TODO: To become 8.8.4
+version = "8.8.3.1b4"  # TODO: To become 8.8.4
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.3.1b3/PKG-INFO` & `dcicutils-8.8.3.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.3.1b3
+Version: 8.8.3.1b4
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

