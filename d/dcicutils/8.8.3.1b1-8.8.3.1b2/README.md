# Comparing `tmp/dcicutils-8.8.3.1b1.tar.gz` & `tmp/dcicutils-8.8.3.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-8.8.3.1b1.tar", max compression
+gzip compressed data, was "dcicutils-8.8.3.1b2.tar", max compression
```

## Comparing `dcicutils-8.8.3.1b1.tar` & `dcicutils-8.8.3.1b2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1102 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/LICENSE.txt
--rw-r--r--   0        0        0     1166 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/README.rst
--rw-r--r--   0        0        0        0 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    34669 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/bundle_utils.py
--rw-r--r--   0        0        0     2522 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/captured_output.py
--rw-r--r--   0        0        0    13786 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3955 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/common.py
--rw-r--r--   0        0        0     2015 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/contribution_scripts.py
--rw-r--r--   0        0        0    25653 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/contribution_utils.py
--rw-r--r--   0        0        0    11113 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     7414 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/data_readers.py
--rw-r--r--   0        0        0     3098 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/data_utils.py
--rw-r--r--   0        0        0     4666 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/datetime_utils.py
--rw-r--r--   0        0        0    69908 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46970 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2024-04-12 17:29:10.097720 dcicutils-8.8.3.1b1/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    72972 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/ff_utils.py
--rw-r--r--   0        0        0     2663 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/file_utils.py
--rw-r--r--   0        0        0    10026 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    34149 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    28151 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/lang_utils.py
--rw-r--r--   0        0        0      278 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/license_policies/c4-infrastructure.jsonc
--rw-r--r--   0        0        0      296 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/license_policies/c4-python-infrastructure.jsonc
--rw-r--r--   0        0        0     5790 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/license_policies/park-lab-common-server.jsonc
--rw-r--r--   0        0        0    18864 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/license_policies/park-lab-common.jsonc
--rw-r--r--   0        0        0     3260 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
--rw-r--r--   0        0        0      283 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/license_policies/park-lab-pipeline.jsonc
--rw-r--r--   0        0        0    46978 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/license_utils.py
--rw-r--r--   0        0        0    10883 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/log_utils.py
--rw-r--r--   0        0        0   102210 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    15422 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/portal_object_utils.py
--rw-r--r--   0        0        0    30480 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/portal_utils.py
--rw-r--r--   0        0        0    13554 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/progress_bar.py
--rw-r--r--   0        0        0    31250 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20534 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   160208 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     7055 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28868 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    10095 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/schema_utils.py
--rw-r--r--   0        0        0    13889 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0     4184 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/scripts/run_license_checker.py
--rw-r--r--   0        0        0    26262 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/scripts/view_portal_object.py
--rw-r--r--   0        0        0    19745 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    33629 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/sheet_utils.py
--rw-r--r--   0        0        0    22961 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0    58218 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/structured_data.py
--rw-r--r--   0        0        0     2895 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/submitr/progress_constants.py
--rw-r--r--   0        0        0     3467 2024-04-12 17:29:10.101720 dcicutils-8.8.3.1b1/dcicutils/submitr/ref_lookup_strategy.py
--rw-r--r--   0        0        0     8082 2024-04-12 17:29:10.105720 dcicutils-8.8.3.1b1/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1403 2024-04-12 17:29:10.105720 dcicutils-8.8.3.1b1/dcicutils/tmpfile_utils.py
--rw-r--r--   0        0        0     1769 2024-04-12 17:29:10.105720 dcicutils-8.8.3.1b1/dcicutils/trace_utils.py
--rw-r--r--   0        0        0    14797 2024-04-12 17:29:10.105720 dcicutils-8.8.3.1b1/dcicutils/validation_utils.py
--rw-r--r--   0        0        0     4343 2024-04-12 17:29:10.105720 dcicutils-8.8.3.1b1/dcicutils/variant_utils.py
--rw-r--r--   0        0        0     2027 2024-04-12 17:29:10.105720 dcicutils-8.8.3.1b1/dcicutils/zip_utils.py
--rw-r--r--   0        0        0     4714 2024-04-12 17:29:10.105720 dcicutils-8.8.3.1b1/pyproject.toml
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.3.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/README.rst
+-rw-r--r--   0        0        0        0 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    34669 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/bundle_utils.py
+-rw-r--r--   0        0        0     3108 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/captured_output.py
+-rw-r--r--   0        0        0    13786 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3955 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/common.py
+-rw-r--r--   0        0        0     2015 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/contribution_scripts.py
+-rw-r--r--   0        0        0    25653 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/contribution_utils.py
+-rw-r--r--   0        0        0    11113 2024-04-12 21:14:33.440362 dcicutils-8.8.3.1b2/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     7414 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/data_readers.py
+-rw-r--r--   0        0        0     3098 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/data_utils.py
+-rw-r--r--   0        0        0     4666 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/datetime_utils.py
+-rw-r--r--   0        0        0    69908 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46970 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    72972 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0     2663 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/file_utils.py
+-rw-r--r--   0        0        0    10026 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    34149 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    28151 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0      278 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/license_policies/c4-infrastructure.jsonc
+-rw-r--r--   0        0        0      296 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/license_policies/c4-python-infrastructure.jsonc
+-rw-r--r--   0        0        0     5790 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/license_policies/park-lab-common-server.jsonc
+-rw-r--r--   0        0        0    18864 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/license_policies/park-lab-common.jsonc
+-rw-r--r--   0        0        0     3260 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc
+-rw-r--r--   0        0        0      283 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/license_policies/park-lab-pipeline.jsonc
+-rw-r--r--   0        0        0    46978 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/license_utils.py
+-rw-r--r--   0        0        0    10883 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/log_utils.py
+-rw-r--r--   0        0        0   102210 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    15422 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/portal_object_utils.py
+-rw-r--r--   0        0        0    30480 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/portal_utils.py
+-rw-r--r--   0        0        0    14091 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/progress_bar.py
+-rw-r--r--   0        0        0    31250 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20534 2024-04-12 21:14:33.444362 dcicutils-8.8.3.1b2/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   160208 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     7055 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28868 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    10095 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/schema_utils.py
+-rw-r--r--   0        0        0    13889 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0     4184 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/scripts/run_license_checker.py
+-rw-r--r--   0        0        0    26262 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/scripts/view_portal_object.py
+-rw-r--r--   0        0        0    19745 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    33629 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/sheet_utils.py
+-rw-r--r--   0        0        0    22961 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0    58450 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/structured_data.py
+-rw-r--r--   0        0        0     2895 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/submitr/progress_constants.py
+-rw-r--r--   0        0        0     3467 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/submitr/ref_lookup_strategy.py
+-rw-r--r--   0        0        0     8082 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1403 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/tmpfile_utils.py
+-rw-r--r--   0        0        0     1769 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0    14797 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/validation_utils.py
+-rw-r--r--   0        0        0     4343 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/variant_utils.py
+-rw-r--r--   0        0        0     2027 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/dcicutils/zip_utils.py
+-rw-r--r--   0        0        0     4714 2024-04-12 21:14:33.448362 dcicutils-8.8.3.1b2/pyproject.toml
+-rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 dcicutils-8.8.3.1b2/PKG-INFO
```

### Comparing `dcicutils-8.8.3.1b1/LICENSE.txt` & `dcicutils-8.8.3.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/README.rst` & `dcicutils-8.8.3.1b2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/base.py` & `dcicutils-8.8.3.1b2/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/beanstalk_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/bundle_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/bundle_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/captured_output.py` & `dcicutils-8.8.3.1b2/dcicutils/captured_output.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 from typing import Optional
 
 _real_stdout = sys.stdout
 _real_stderr = sys.stderr
 
 
 @contextmanager
-def captured_output(capture: bool = True):
+def captured_output(capture: bool = True, encoding: Optional[str] = None):
     """
     Context manager to capture any/all output to stdout or stderr, and not actually output it to stdout
     or stderr. Yields and object with a get_captured_output() method to get the output captured thus far,
     and another uncaptured_print() method to actually print the given output to stdout, even though output
     to stdout is being captured. Can be useful, for example, in creating command-line scripts which invoke
     code which outputs a lot of info, warning, error, etc to stdout or stderr, and we want to suprress that
     output; but with the yielded uncaptured_print() method output specific to the script can actually be
     output (to stdout); and/or can also optionally output any/all captured output, e.g. for debugging or
     troubleshooting purposes. Disable this capture, without having to restructure your code WRT the usage
     of the with-clause with this context manager, pass False as an argument to this context manager.
     """
 
     original_stdout = _real_stdout
     original_stderr = _real_stderr
-    captured_output = io.StringIO()
+    captured_output = io.StringIO() if not encoding else _EncodedStringIO(encoding)
 
     def set_original_output() -> None:
         sys.stdout = original_stdout
         sys.stderr = original_stderr
 
     def set_captured_output() -> None:
         if capture:
@@ -64,7 +64,23 @@
     sys.stdout = _real_stdout
     sys.stderr = _real_stderr
     try:
         yield
     finally:
         sys.stdout = original_stdout
         sys.stderr = original_stderr
+
+
+class _EncodedStringIO:
+    def __init__(self, encoding: str = "utf-8"):
+        self.encoding = encoding
+        self.buffer = io.BytesIO()
+    def write(self, s):  # noqa
+        self.buffer.write(s.encode(self.encoding))
+    def flush(self):  # noqa
+        self.buffer.flush()
+    def getvalue(self):  # noqa
+        return self.buffer.getvalue().decode(self.encoding)
+    def __str__(self):  # noqa
+        return self.getvalue()
+    def __repr__(self):  # noqa
+        return repr(self.getvalue())
```

### Comparing `dcicutils-8.8.3.1b1/dcicutils/cloudformation_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/codebuild_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/command_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/common.py` & `dcicutils-8.8.3.1b2/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/contribution_scripts.py` & `dcicutils-8.8.3.1b2/dcicutils/contribution_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/contribution_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/contribution_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/creds_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/data_readers.py` & `dcicutils-8.8.3.1b2/dcicutils/data_readers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/data_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/datetime_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/deployment_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/diff_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/docker_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/ecr_scripts.py` & `dcicutils-8.8.3.1b2/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/ecr_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/ecs_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/env_base.py` & `dcicutils-8.8.3.1b2/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/env_manager.py` & `dcicutils-8.8.3.1b2/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/env_scripts.py` & `dcicutils-8.8.3.1b2/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/env_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/env_utils_legacy.py` & `dcicutils-8.8.3.1b2/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/es_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/exceptions.py` & `dcicutils-8.8.3.1b2/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/ff_mocks.py` & `dcicutils-8.8.3.1b2/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/ff_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/file_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/function_cache_decorator.py` & `dcicutils-8.8.3.1b2/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/glacier_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/jh_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/kibana/dashboards.json` & `dcicutils-8.8.3.1b2/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/kibana/readme.md` & `dcicutils-8.8.3.1b2/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/lang_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/license_policies/park-lab-common-server.jsonc` & `dcicutils-8.8.3.1b2/dcicutils/license_policies/park-lab-common-server.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/license_policies/park-lab-common.jsonc` & `dcicutils-8.8.3.1b2/dcicutils/license_policies/park-lab-common.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc` & `dcicutils-8.8.3.1b2/dcicutils/license_policies/park-lab-gpl-pipeline.jsonc`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/license_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/license_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/log_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/misc_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/obfuscation_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/opensearch_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/portal_object_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/portal_object_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/portal_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/portal_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/progress_bar.py` & `dcicutils-8.8.3.1b2/dcicutils/progress_bar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import namedtuple
 from signal import signal, SIGINT
 import sys
 import threading
 import time
 from tqdm import tqdm
 from types import FrameType as frame
-from typing import Callable, Optional, Union
+from typing import Callable, List, Optional, Union
 from contextlib import contextmanager
 from dcicutils.command_utils import yes_or_no
 
 
 class TQDM(tqdm):
 
     """
@@ -50,20 +50,19 @@
                  catch_interrupt: bool = True,
                  interrupt: Optional[Callable] = None,
                  interrupt_continue: Optional[Callable] = None,
                  interrupt_stop: Optional[Callable] = None,
                  interrupt_exit: bool = False,
                  interrupt_exit_message: Optional[Union[Callable, str]] = None,
                  interrupt_message: Optional[str] = None,
-                 printf: Optional[Callable] = None,
-                 tidy_output_hack: bool = True) -> None:
+                 tidy_output_hack: bool = True,
+                 capture_output_for_testing: bool = False) -> None:
         self._bar = None
         self._disabled = False
         self._done = False
-        self._printf = printf if callable(printf) else print
         self._tidy_output_hack = (tidy_output_hack is True)
         self._started = time.time()
         self._stop_requested = False
         # Interrupt handling. We do not do the actual (signal) interrupt setup
         # in self._initialize as that could be called from a (sub) thread; and in
         # Python we can only set a signal (SIGINT in our case) on the main thread.
         self._catch_interrupt = (catch_interrupt is True)
@@ -86,15 +85,15 @@
         self._interrupt_handler = None
         if self._catch_interrupt:
             self._interrupt_handler = self._define_interrupt_handler()
         if self._tidy_output_hack is True:
             self._tidy_output_hack = self._define_tidy_output_hack()
         self._total = total if isinstance(total, int) and total >= 0 else 0
         self._description = self._format_description(description)
-        # self._initialize()
+        self._captured_output_for_testing = [] if capture_output_for_testing else None
 
     def _initialize(self) -> bool:
         # Do not actually create the tqdm object unless/until we have a positive total.
         if (self._bar is None) and (self._total > 0):
             bar_format = "{l_bar}{bar}| {n_fmt}/{total_fmt} | {rate_fmt} | {elapsed}{postfix} | ETA: {remaining} "
             self._bar = TQDM(total=self._total, desc=self._description,
                              dynamic_ncols=True, bar_format=bar_format, unit="", file=sys.stdout)
@@ -193,27 +192,31 @@
     def started(self) -> None:
         return self._started
 
     @property
     def duration(self) -> None:
         return time.time() - self._started
 
+    @property
+    def captured_output_for_testing(self) -> Optional[List[str]]:
+        return self._captured_output_for_testing
+
     def _format_description(self, value: str) -> str:
         if not isinstance(value, str):
             value = ""
         if self._tidy_output_hack and not value.endswith(self._tidy_output_hack.sentinel):
             value += self._tidy_output_hack.sentinel
         return value
 
     def _define_interrupt_handler(self) -> None:
         def handle_interrupt(signum: int, frame: frame) -> None:  # noqa
             nonlocal self
             def handle_secondary_interrupt(signum: int, frame: frame) -> None:  # noqa
                 nonlocal self
-                self._printf("\nEnter 'yes' or 'no' or CTRL-\\ to completely abort ...")
+                print("\nEnter 'yes' or 'no' or CTRL-\\ to completely abort ...")
             self.disable()
             self._interrupt(self) if self._interrupt else None
             set_interrupt_handler(handle_secondary_interrupt)
             if yes_or_no(f"\nALERT! You have interrupted this {self._interrupt_message or 'process'}."
                          f" Do you want to stop{' (exit)' if self._interrupt_exit else ''}?"):
                 # Here there was an interrupt (CTRL-C) and the user confirmed (yes)
                 # that they want to stop the process; if the interrupt_stop handler
@@ -222,15 +225,15 @@
                 if self._interrupt_stop:
                     interrupt_stop = self._interrupt_stop(self)
                     if (interrupt_stop is True) or ((interrupt_stop is None) and (self._interrupt_exit is True)):
                         self.done()
                         restore_interrupt_handler()
                         if self._interrupt_exit_message:
                             if isinstance(interrupt_exit_message := self._interrupt_exit_message(self), str):
-                                self._printf(interrupt_exit_message)
+                                print(interrupt_exit_message)
                         exit(1)
                     elif interrupt_stop is False or ((interrupt_stop is None) and (self._interrupt_exit is False)):
                         set_interrupt_handler(handle_interrupt)
                         interrupt_continue = self._interrupt_continue(self) if self._interrupt_continue else None
                         if not (interrupt_continue is False):
                             self.enable()
                         return
@@ -257,28 +260,37 @@
         # string in the display string where the progress bar should actually go,
         # which we do in _format_description. Other minor things too; see below.
         sys_stdout_write = sys.stdout.write
         def tidy_stdout_write(text: str) -> None:  # noqa
             nonlocal self, sys_stdout_write, sentinel_internal, spina, spini, spinn
             def replace_first(value: str, match: str, replacement: str) -> str:  # noqa
                 return value[:i] + replacement + value[i + len(match):] if (i := value.find(match)) >= 0 else value
+            def remove_extra_trailing_spaces(text: str) -> str:  # noqa
+                while text.endswith("  "):
+                    text = text[:-1]
+                return text
+            if not text:
+                return
             if (self._disabled or self._done) and sentinel_internal in text:
                 # Another hack to really disable output on interrupt; in this case we set
                 # tqdm.disable to True, but output can still dribble out, so if the output
                 # looks like it is from tqdm and we are disabled/done then do no output.
                 return
             if sentinel_internal in text:
                 spinc = spina[spini % spinn] if not ("100%|" in text) else "| ✓" ; spini += 1  # noqa
                 text = replace_first(text, sentinel_internal, f" {spinc}")
                 text = replace_first(text, "%|", "% ◀|")
+                text = remove_extra_trailing_spaces(text)
                 # Another oddity: for the rate sometimes tqdm intermittently prints
                 # something like "1.54s/" rather than "1.54/s"; something to do with
                 # the unit we gave, which is empty; idunno; just replace it here.
                 text = replace_first(text, "s/ ", "/s ")
             sys_stdout_write(text)
+            if self._captured_output_for_testing is not None:
+                self._captured_output_for_testing.append(text)
             sys.stdout.flush()
         def restore_stdout_write() -> None:  # noqa
             nonlocal sys_stdout_write
             if sys_stdout_write is not None:
                 sys.stdout.write = sys_stdout_write
         sys.stdout.write = tidy_stdout_write
         spina = ["|", "/", "—", "◦", "\\"] ; spini = 0 ; spinn = len(spina)  # noqa
```

### Comparing `dcicutils-8.8.3.1b1/dcicutils/project_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/qa_checkers.py` & `dcicutils-8.8.3.1b2/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/qa_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/redis_tools.py` & `dcicutils-8.8.3.1b2/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/redis_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/s3_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/schema_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-8.8.3.1b2/dcicutils/scripts/publish_to_pypi.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/scripts/run_license_checker.py` & `dcicutils-8.8.3.1b2/dcicutils/scripts/run_license_checker.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/scripts/view_portal_object.py` & `dcicutils-8.8.3.1b2/dcicutils/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/secrets_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/sheet_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/sheet_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/snapshot_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/ssl_certificate_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/structured_data.py` & `dcicutils-8.8.3.1b2/dcicutils/structured_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -650,15 +650,17 @@
         return map_datetime
 
     def _map_function_ref(self, typeinfo: dict) -> Callable:
         def map_ref(value: str, link_to: str, portal: Optional[Portal], src: Optional[str]) -> Any:
             nonlocal self, typeinfo
             if self._norefs:
                 if value:
-                    self._resolved_refs.add((f"/{link_to}/{value}", None))
+                    # Dump the src because this cannot add dictionary to a set; note that
+                    # this is ONLY used for smaht-submitr/submit-metadata-bundle --info --refs.
+                    self._resolved_refs.add((f"/{link_to}/{value}", json.dumps(src) if isinstance(src, dict) else None))
                 return value
             if not value:
                 if (column := typeinfo.get("column")) and column in self.data.get("required", []):
                     self._unresolved_refs.append({"src": src, "error": f"/{link_to}/<null>"})
             elif portal:
                 if not (resolved := portal.ref_exists(link_to, value, True)):
                     self._unresolved_refs.append({"src": src, "error": f"/{link_to}/{value}"})
```

### Comparing `dcicutils-8.8.3.1b1/dcicutils/submitr/progress_constants.py` & `dcicutils-8.8.3.1b2/dcicutils/submitr/progress_constants.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/submitr/ref_lookup_strategy.py` & `dcicutils-8.8.3.1b2/dcicutils/submitr/ref_lookup_strategy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/task_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/tmpfile_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/tmpfile_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/trace_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/validation_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/variant_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/variant_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/dcicutils/zip_utils.py` & `dcicutils-8.8.3.1b2/dcicutils/zip_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-8.8.3.1b1/pyproject.toml` & `dcicutils-8.8.3.1b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "8.8.3.1b1"  # TODO: To become 8.8.4
+version = "8.8.3.1b2"  # TODO: To become 8.8.4
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-8.8.3.1b1/PKG-INFO` & `dcicutils-8.8.3.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 8.8.3.1b1
+Version: 8.8.3.1b2
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
```

