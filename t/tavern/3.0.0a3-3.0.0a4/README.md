# Comparing `tmp/tavern-3.0.0a3.tar.gz` & `tmp/tavern-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tavern-3.0.0a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tavern-3.0.0a4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tavern-3.0.0a3.tar` & `tavern-3.0.0a4.tar`

### file list

```diff
@@ -1,226 +1,226 @@
--rw-r--r--   0        0        0     1271 2023-12-23 17:57:23.499714 tavern-3.0.0a3/.dockerignore
--rw-r--r--   0        0        0       99 2024-01-20 13:06:48.128624 tavern-3.0.0a3/.gitattributes
--rw-r--r--   0        0        0       23 2023-11-04 16:24:35.280382 tavern-3.0.0a3/.github/FUNDING.yml
--rw-r--r--   0        0        0     3242 2024-01-20 18:24:56.398873 tavern-3.0.0a3/.github/workflows/main.yml
--rw-r--r--   0        0        0     1310 2024-01-20 13:06:48.131958 tavern-3.0.0a3/.gitignore
--rw-r--r--   0        0        0      725 2024-01-20 18:24:56.398873 tavern-3.0.0a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       43 2023-10-22 10:53:53.056714 tavern-3.0.0a3/.prettierignore
--rw-r--r--   0        0        0      431 2023-11-04 16:24:35.280382 tavern-3.0.0a3/.readthedocs.yaml
--rw-r--r--   0        0        0    16897 2024-01-20 18:24:47.162177 tavern-3.0.0a3/CHANGELOG.md
--rw-r--r--   0        0        0     1837 2024-01-20 13:06:48.131958 tavern-3.0.0a3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1055 2023-10-22 10:53:53.056714 tavern-3.0.0a3/LICENSE
--rw-r--r--   0        0        0      152 2024-01-20 13:06:48.131958 tavern-3.0.0a3/MANIFEST.in
--rw-r--r--   0        0        0     8342 2023-10-22 10:53:53.056714 tavern-3.0.0a3/README.md
--rw-r--r--   0        0        0     7508 2024-01-20 18:24:38.418816 tavern-3.0.0a3/constraints.txt
--rw-r--r--   0        0        0        9 2023-10-22 10:53:53.056714 tavern-3.0.0a3/docs/.gitignore
--rw-r--r--   0        0        0      607 2023-10-22 10:53:53.056714 tavern-3.0.0a3/docs/Makefile
--rw-r--r--   0        0        0        6 2023-10-22 10:53:53.056714 tavern-3.0.0a3/docs/source/.gitignore
--rw-r--r--   0        0        0      851 2023-10-22 10:53:53.056714 tavern-3.0.0a3/docs/source/_static/favicon.png
--rw-r--r--   0        0        0     1448 2023-10-22 10:53:53.056714 tavern-3.0.0a3/docs/source/_static/icon.png
--rw-r--r--   0        0        0    70972 2024-01-20 18:24:56.398873 tavern-3.0.0a3/docs/source/basics.md
--rw-r--r--   0        0        0     5807 2024-01-20 18:24:56.402207 tavern-3.0.0a3/docs/source/conf.py
--rw-r--r--   0        0        0     4186 2023-11-04 16:24:35.280382 tavern-3.0.0a3/docs/source/cookbook.md
--rw-r--r--   0        0        0     7667 2023-10-22 10:53:53.060047 tavern-3.0.0a3/docs/source/debugging.md
--rw-r--r--   0        0        0     7883 2023-10-22 10:53:53.060047 tavern-3.0.0a3/docs/source/examples.md
--rw-r--r--   0        0        0     5188 2024-01-20 13:06:48.131958 tavern-3.0.0a3/docs/source/grpc.md
--rw-r--r--   0        0        0    12311 2023-11-04 16:24:35.280382 tavern-3.0.0a3/docs/source/http.md
--rw-r--r--   0        0        0     1528 2024-01-20 18:24:56.398873 tavern-3.0.0a3/docs/source/index.md
--rw-r--r--   0        0        0     9433 2023-10-22 10:53:53.060047 tavern-3.0.0a3/docs/source/mqtt.md
--rw-r--r--   0        0        0    11359 2023-10-22 10:53:53.060047 tavern-3.0.0a3/docs/source/plugins.md
--rw-r--r--   0        0        0     2895 2023-10-22 10:53:53.060047 tavern-3.0.0a3/docs/source/server.md
--rw-r--r--   0        0        0      220 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/advanced/Dockerfile
--rw-r--r--   0        0        0      401 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/advanced/advanced.md
--rw-r--r--   0        0        0      149 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/advanced/common.yaml
--rw-r--r--   0        0        0      126 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/advanced/docker-compose.yaml
--rw-r--r--   0        0        0     3551 2024-01-18 13:28:20.874570 tavern-3.0.0a3/example/advanced/server.py
--rw-r--r--   0        0        0     4046 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/advanced/test_server.tavern.yaml
--rw-r--r--   0        0        0      673 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/advanced/testing_utils.py
--rw-r--r--   0        0        0      210 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/components/Dockerfile
--rw-r--r--   0        0        0      168 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/components/common.yaml
--rw-r--r--   0        0        0      717 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/components/components.md
--rw-r--r--   0        0        0      594 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/components/components/auth_stage.yaml
--rw-r--r--   0        0        0      126 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/components/docker-compose.yaml
--rw-r--r--   0        0        0     1642 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/components/server.py
--rw-r--r--   0        0        0      633 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/components/test_hello.tavern.yaml
--rw-r--r--   0        0        0      612 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/components/test_ping.tavern.yaml
--rw-r--r--   0        0        0      195 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/cookies/Dockerfile
--rw-r--r--   0        0        0      117 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/cookies/common.yaml
--rw-r--r--   0        0        0      147 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/cookies/cookies.md
--rw-r--r--   0        0        0      126 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/cookies/docker-compose.yaml
--rw-r--r--   0        0        0     2973 2024-01-18 13:28:20.874570 tavern-3.0.0a3/example/cookies/server.py
--rw-r--r--   0        0        0     3245 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/cookies/test_server.tavern.yaml
--rw-r--r--   0        0        0      202 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/generate_from_openapi/Pipfile
--rw-r--r--   0        0        0    13687 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/generate_from_openapi/Pipfile.lock
--rw-r--r--   0        0        0     2106 2024-01-20 14:41:47.330398 tavern-3.0.0a3/example/generate_from_openapi/pub_tavern.py
--rw-r--r--   0        0        0      144 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/generate_from_openapi/readme.md
--rw-r--r--   0        0        0      566 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/generate_from_openapi/test_example_output.tavern.yaml
--rw-r--r--   0        0        0      601 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/Dockerfile
--rw-r--r--   0        0        0      159 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/common.yaml
--rw-r--r--   0        0        0      455 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/conftest.py
--rw-r--r--   0        0        0      206 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/docker-compose.yaml
--rw-r--r--   0        0        0      295 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/helloworld_v1_precompiled.proto
--rw-r--r--   0        0        0     1443 2024-01-20 13:42:01.354969 tavern-3.0.0a3/example/grpc/helloworld_v1_precompiled_pb2.py
--rw-r--r--   0        0        0      595 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/helloworld_v1_precompiled_pb2.pyi
--rw-r--r--   0        0        0     2586 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/helloworld_v1_precompiled_pb2_grpc.py
--rw-r--r--   0        0        0      261 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/helloworld_v2_compiled.proto
--rw-r--r--   0        0        0      286 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/helloworld_v3_reflected.proto
--rwxr-xr-x   0        0        0      178 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/regenerate.sh
--rw-r--r--   0        0        0     2905 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/server/server.py
--rw-r--r--   0        0        0     6456 2024-01-20 13:06:48.131958 tavern-3.0.0a3/example/grpc/test_grpc.tavern.yaml
--rw-r--r--   0        0        0      202 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/hooks/Dockerfile
--rw-r--r--   0        0        0      990 2023-11-04 16:24:35.283715 tavern-3.0.0a3/example/hooks/conftest.py
--rw-r--r--   0        0        0      126 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/hooks/docker-compose.yaml
--rw-r--r--   0        0        0      464 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/hooks/server.py
--rw-r--r--   0        0        0      620 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/hooks/test_server.tavern.yaml
--rw-r--r--   0        0        0      844 2023-11-04 16:24:35.283715 tavern-3.0.0a3/example/mqtt/README.md
--rw-r--r--   0        0        0      158 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/mqtt/common.yaml
--rw-r--r--   0        0        0     2583 2023-11-04 16:24:35.283715 tavern-3.0.0a3/example/mqtt/conftest.py
--rw-r--r--   0        0        0      990 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/mqtt/docker-compose.yaml
--rw-r--r--   0        0        0      135 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/mqtt/fluent.conf
--rw-r--r--   0        0        0      158 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/mqtt/listener.Dockerfile
--rw-r--r--   0        0        0     4851 2023-11-04 16:24:35.283715 tavern-3.0.0a3/example/mqtt/listener.py
--rw-r--r--   0        0        0      169 2023-11-04 16:24:35.283715 tavern-3.0.0a3/example/mqtt/mosquitto.conf
--rw-r--r--   0        0        0      120 2023-11-04 16:24:35.283715 tavern-3.0.0a3/example/mqtt/mosquitto_passwd
--rw-r--r--   0        0        0      393 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/mqtt/server.Dockerfile
--rw-r--r--   0        0        0     4690 2024-01-18 13:28:20.874570 tavern-3.0.0a3/example/mqtt/server.py
--rw-r--r--   0        0        0    15562 2023-11-04 16:24:35.283715 tavern-3.0.0a3/example/mqtt/test_mqtt.tavern.yaml
--rw-r--r--   0        0        0     3381 2023-11-04 16:24:35.283715 tavern-3.0.0a3/example/mqtt/test_mqtt_failures.tavern.yaml
--rw-r--r--   0        0        0      197 2024-01-06 15:34:53.978905 tavern-3.0.0a3/example/mqtt/testing_utils.py
--rw-r--r--   0        0        0     1167 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/simple/running_tests.md
--rw-r--r--   0        0        0      464 2023-12-23 17:57:23.503047 tavern-3.0.0a3/example/simple/server.py
--rw-r--r--   0        0        0     1996 2023-10-22 10:53:53.060047 tavern-3.0.0a3/example/simple/test_server.tavern.yaml
--rw-r--r--   0        0        0     4789 2024-01-20 18:24:56.402207 tavern-3.0.0a3/pyproject.toml
--rw-r--r--   0        0        0    88688 2024-01-20 18:24:38.422149 tavern-3.0.0a3/requirements.txt
--rwxr-xr-x   0        0        0      222 2023-10-22 10:53:53.060047 tavern-3.0.0a3/scripts/coverage.sh
--rwxr-xr-x   0        0        0      407 2023-10-22 10:53:53.060047 tavern-3.0.0a3/scripts/release.sh
--rwxr-xr-x   0        0        0      324 2024-01-20 18:24:56.398873 tavern-3.0.0a3/scripts/smoke.bash
--rwxr-xr-x   0        0        0      616 2023-10-22 10:53:53.060047 tavern-3.0.0a3/scripts/update-changelog.bash
--rw-r--r--   0        0        0      101 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/__init__.py
--rw-r--r--   0        0        0        0 2023-10-29 14:00:16.070308 tavern-3.0.0a3/tavern/_core/__init__.py
--rw-r--r--   0        0        0    20659 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/dict_util.py
--rw-r--r--   0        0        0     4603 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/exceptions.py
--rw-r--r--   0        0        0     4719 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/extfunctions.py
--rw-r--r--   0        0        0       96 2023-10-22 10:53:53.060047 tavern-3.0.0a3/tavern/_core/formatted_str.py
--rw-r--r--   0        0        0      943 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/general.py
--rw-r--r--   0        0        0     2586 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/jmesutils.py
--rw-r--r--   0        0        0    12646 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/loader.py
--rw-r--r--   0        0        0     9897 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/plugins.py
--rw-r--r--   0        0        0      275 2023-10-22 10:53:53.060047 tavern-3.0.0a3/tavern/_core/pytest/__init__.py
--rw-r--r--   0        0        0     2229 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/pytest/config.py
--rw-r--r--   0        0        0     7439 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/pytest/error.py
--rw-r--r--   0        0        0    13354 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/pytest/file.py
--rw-r--r--   0        0        0     2508 2024-01-20 13:06:48.131958 tavern-3.0.0a3/tavern/_core/pytest/hooks.py
--rw-r--r--   0        0        0    10582 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/pytest/item.py
--rw-r--r--   0        0        0     2117 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/pytest/newhooks.py
--rw-r--r--   0        0        0     6696 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/pytest/util.py
--rw-r--r--   0        0        0     1857 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/report.py
--rw-r--r--   0        0        0    12125 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/run.py
--rw-r--r--   0        0        0        0 2023-10-22 10:53:53.060047 tavern-3.0.0a3/tavern/_core/schema/__init__.py
--rw-r--r--   0        0        0    15782 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/schema/extensions.py
--rw-r--r--   0        0        0     4379 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/schema/files.py
--rw-r--r--   0        0        0     7149 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/schema/jsonschema.py
--rw-r--r--   0        0        0    10613 2024-01-20 13:06:48.131958 tavern-3.0.0a3/tavern/_core/schema/tests.jsonschema.yaml
--rw-r--r--   0        0        0     7927 2024-01-20 13:06:48.131958 tavern-3.0.0a3/tavern/_core/schema/tests.schema.yaml
--rw-r--r--   0        0        0     1098 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/stage_lines.py
--rw-r--r--   0        0        0     5139 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/strict_util.py
--rw-r--r--   0        0        0      380 2024-01-20 18:20:07.221269 tavern-3.0.0a3/tavern/_core/strtobool.py
--rw-r--r--   0        0        0     3970 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/testhelpers.py
--rw-r--r--   0        0        0     2647 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_core/tincture.py
--rw-r--r--   0        0        0        0 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tavern/_plugins/__init__.py
--rw-r--r--   0        0        0      590 2024-01-20 13:06:48.131958 tavern-3.0.0a3/tavern/_plugins/grpc/__init__.py
--rw-r--r--   0        0        0    10529 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/grpc/client.py
--rw-r--r--   0        0        0     1329 2024-01-20 13:06:48.135291 tavern-3.0.0a3/tavern/_plugins/grpc/jsonschema.yaml
--rw-r--r--   0        0        0     5283 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/grpc/protos.py
--rw-r--r--   0        0        0     2394 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/grpc/request.py
--rw-r--r--   0        0        0     5838 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/grpc/response.py
--rw-r--r--   0        0        0      921 2024-01-20 13:06:48.135291 tavern-3.0.0a3/tavern/_plugins/grpc/schema.yaml
--rw-r--r--   0        0        0      865 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/grpc/tavernhook.py
--rw-r--r--   0        0        0        0 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tavern/_plugins/mqtt/__init__.py
--rw-r--r--   0        0        0    17679 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/mqtt/client.py
--rw-r--r--   0        0        0     4013 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tavern/_plugins/mqtt/jsonschema.yaml
--rw-r--r--   0        0        0     2515 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/mqtt/request.py
--rw-r--r--   0        0        0    11481 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/mqtt/response.py
--rw-r--r--   0        0        0     3233 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tavern/_plugins/mqtt/schema.yaml
--rw-r--r--   0        0        0     1376 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/mqtt/tavernhook.py
--rw-r--r--   0        0        0        0 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tavern/_plugins/rest/__init__.py
--rw-r--r--   0        0        0     6549 2024-01-20 18:24:56.398873 tavern-3.0.0a3/tavern/_plugins/rest/files.py
--rw-r--r--   0        0        0    16169 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/_plugins/rest/request.py
--rw-r--r--   0        0        0     8236 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/_plugins/rest/response.py
--rw-r--r--   0        0        0      876 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/_plugins/rest/tavernhook.py
--rw-r--r--   0        0        0     3182 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/core.py
--rw-r--r--   0        0        0     2745 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/entry.py
--rw-r--r--   0        0        0     7534 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/helpers.py
--rw-r--r--   0        0        0      693 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/request.py
--rw-r--r--   0        0        0     9798 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tavern/response.py
--rw-r--r--   0        0        0     1051 2024-01-20 18:24:38.422149 tavern-3.0.0a3/tests/conftest.py
--rw-r--r--   0        0        0       37 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/881_1.json
--rw-r--r--   0        0        0       41 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/881_2.yaml
--rw-r--r--   0        0        0      202 2023-12-23 17:57:23.506380 tavern-3.0.0a3/tests/integration/Dockerfile
--rw-r--r--   0        0        0       33 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/OK.json.gz
--rw-r--r--   0        0        0        3 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/OK.txt
--rw-r--r--   0        0        0      504 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/README.md
--rw-r--r--   0        0        0      608 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/common.yaml
--rw-r--r--   0        0        0      734 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/conftest.py
--rw-r--r--   0        0        0      126 2023-12-23 17:57:23.506380 tavern-3.0.0a3/tests/integration/docker-compose.yaml
--rw-r--r--   0        0        0      362 2024-01-20 18:20:07.221269 tavern-3.0.0a3/tests/integration/ext_functions.py
--rw-r--r--   0        0        0      203 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/extra.yaml
--rw-r--r--   0        0        0      254 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/global_cfg.yaml
--rw-r--r--   0        0        0       91 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/parametrize_includes.yaml
--rw-r--r--   0        0        0    13044 2024-01-20 18:20:07.221269 tavern-3.0.0a3/tests/integration/server.py
--rw-r--r--   0        0        0      297 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_allure.tavern.yaml
--rw-r--r--   0        0        0      659 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_auth_key.tavern.yaml
--rw-r--r--   0        0        0      624 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_certs.tavern.yaml
--rw-r--r--   0        0        0      823 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/test_control_flow.tavern.yaml
--rw-r--r--   0        0        0     1569 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_cookie_remember.tavern.yaml
--rw-r--r--   0        0        0     6106 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_cookies.tavern.yaml
--rw-r--r--   0        0        0     2448 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_data_key.tavern.yaml
--rw-r--r--   0        0        0       29 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_dummy.py
--rw-r--r--   0        0        0      331 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_env_var_format.tavern.yaml
--rw-r--r--   0        0        0      277 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_error.tavern.yaml
--rw-r--r--   0        0        0     3614 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/test_external_functions.tavern.yaml
--rw-r--r--   0        0        0     5435 2023-12-23 17:57:23.506380 tavern-3.0.0a3/tests/integration/test_files.tavern.yaml
--rw-r--r--   0        0        0     2704 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/test_fixtures.tavern.yaml
--rw-r--r--   0        0        0      799 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_follow_redirects.tavern.yaml
--rw-r--r--   0        0        0     1028 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_header_comparisons.tavern.yaml
--rw-r--r--   0        0        0     1269 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_helpers.tavern.yaml
--rw-r--r--   0        0        0     1072 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/test_include.tavern.yaml
--rw-r--r--   0        0        0     4837 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_jmes.tavern.yaml
--rw-r--r--   0        0        0    15252 2024-01-06 15:34:53.978905 tavern-3.0.0a3/tests/integration/test_parametrize.tavern.yaml
--rw-r--r--   0        0        0     2167 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_regex.tavern.yaml
--rw-r--r--   0        0        0     2031 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_response_types.tavern.yaml
--rw-r--r--   0        0        0     2372 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_retry.tavern.yaml
--rw-r--r--   0        0        0      575 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_save_dict_value.tavern.yaml
--rw-r--r--   0        0        0      970 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_selective_tests.tavern.yaml
--rw-r--r--   0        0        0     2432 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_skipped_tests.tavern.yaml
--rw-r--r--   0        0        0     1506 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_status_codes.tavern.yaml
--rw-r--r--   0        0        0      235 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_stream.tavern.yaml
--rw-r--r--   0        0        0    10926 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_strict_key_checks.tavern.yaml
--rw-r--r--   0        0        0     1951 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_timeout.tavern.yaml
--rw-r--r--   0        0        0     1126 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/test_tincture.tavern.yaml
--rw-r--r--   0        0        0    12933 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/integration/test_typetokens.tavern.yaml
--rw-r--r--   0        0        0     1415 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/test_validate_pykwalify.tavern.yaml
--rw-r--r--   0        0        0        0 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/integration/testfile.txt
--rw-r--r--   0        0        0      650 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/logging.yaml
--rw-r--r--   0        0        0      931 2024-01-20 13:06:48.135291 tavern-3.0.0a3/tests/unit/conftest.py
--rw-r--r--   0        0        0     9580 2024-01-20 18:20:07.221269 tavern-3.0.0a3/tests/unit/response/test_mqtt_response.py
--rw-r--r--   0        0        0    12240 2024-01-20 18:20:07.224603 tavern-3.0.0a3/tests/unit/response/test_rest.py
--rw-r--r--   0        0        0        0 2024-01-20 13:06:48.135291 tavern-3.0.0a3/tests/unit/tavern_grpc/__init__.py
--rw-r--r--   0        0        0     6192 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tests/unit/tavern_grpc/test_grpc.py
--rw-r--r--   0        0        0      336 2024-01-20 13:06:48.135291 tavern-3.0.0a3/tests/unit/tavern_grpc/test_services.proto
--rw-r--r--   0        0        0     1614 2024-01-20 14:48:43.784905 tavern-3.0.0a3/tests/unit/tavern_grpc/test_services_pb2.py
--rw-r--r--   0        0        0      671 2024-01-20 13:06:48.135291 tavern-3.0.0a3/tests/unit/tavern_grpc/test_services_pb2.pyi
--rw-r--r--   0        0        0     4137 2024-01-20 14:48:44.048239 tavern-3.0.0a3/tests/unit/tavern_grpc/test_services_pb2_grpc.py
--rw-r--r--   0        0        0     1565 2024-01-20 13:06:48.135291 tavern-3.0.0a3/tests/unit/test_call_run.py
--rw-r--r--   0        0        0    20143 2023-11-04 16:24:35.283715 tavern-3.0.0a3/tests/unit/test_core.py
--rw-r--r--   0        0        0      798 2024-01-20 13:06:48.135291 tavern-3.0.0a3/tests/unit/test_extensions.py
--rw-r--r--   0        0        0    14238 2024-01-20 18:20:07.224603 tavern-3.0.0a3/tests/unit/test_helpers.py
--rw-r--r--   0        0        0     7137 2024-01-20 18:24:56.402207 tavern-3.0.0a3/tests/unit/test_mqtt.py
--rw-r--r--   0        0        0     5791 2023-11-04 16:24:35.287048 tavern-3.0.0a3/tests/unit/test_pytest_hooks.py
--rw-r--r--   0        0        0    16788 2023-11-04 16:24:35.287048 tavern-3.0.0a3/tests/unit/test_request.py
--rw-r--r--   0        0        0     6131 2023-12-23 17:57:23.506380 tavern-3.0.0a3/tests/unit/test_schema.py
--rw-r--r--   0        0        0     1030 2023-10-22 10:53:53.063381 tavern-3.0.0a3/tests/unit/test_strict_util.py
--rw-r--r--   0        0        0     3289 2024-01-18 18:38:53.613931 tavern-3.0.0a3/tests/unit/test_tinctures.py
--rw-r--r--   0        0        0    14898 2023-11-04 16:24:35.287048 tavern-3.0.0a3/tests/unit/test_utilities.py
--rw-r--r--   0        0        0     2559 2024-01-20 18:24:38.422149 tavern-3.0.0a3/tox-integration.ini
--rw-r--r--   0        0        0      653 2024-01-20 18:24:38.422149 tavern-3.0.0a3/tox.ini
--rw-r--r--   0        0        0    11288 1970-01-01 00:00:00.000000 tavern-3.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1271 2023-12-23 17:57:23.499714 tavern-3.0.0a4/.dockerignore
+-rw-r--r--   0        0        0       99 2024-01-20 13:06:48.128624 tavern-3.0.0a4/.gitattributes
+-rw-r--r--   0        0        0       23 2023-11-04 16:24:35.280382 tavern-3.0.0a4/.github/FUNDING.yml
+-rw-r--r--   0        0        0     3229 2024-01-27 15:02:40.567056 tavern-3.0.0a4/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1310 2024-01-20 13:06:48.131958 tavern-3.0.0a4/.gitignore
+-rw-r--r--   0        0        0      725 2024-01-27 15:02:40.567056 tavern-3.0.0a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       43 2023-10-22 10:53:53.056714 tavern-3.0.0a4/.prettierignore
+-rw-r--r--   0        0        0      431 2023-11-04 16:24:35.280382 tavern-3.0.0a4/.readthedocs.yaml
+-rw-r--r--   0        0        0    17048 2024-01-27 15:30:15.839613 tavern-3.0.0a4/CHANGELOG.md
+-rw-r--r--   0        0        0     1837 2024-01-20 13:06:48.131958 tavern-3.0.0a4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1055 2023-10-22 10:53:53.056714 tavern-3.0.0a4/LICENSE
+-rw-r--r--   0        0        0      152 2024-01-20 13:06:48.131958 tavern-3.0.0a4/MANIFEST.in
+-rw-r--r--   0        0        0     8342 2023-10-22 10:53:53.056714 tavern-3.0.0a4/README.md
+-rw-r--r--   0        0        0     7508 2024-01-27 15:02:03.823595 tavern-3.0.0a4/constraints.txt
+-rw-r--r--   0        0        0        9 2023-10-22 10:53:53.056714 tavern-3.0.0a4/docs/.gitignore
+-rw-r--r--   0        0        0      607 2023-10-22 10:53:53.056714 tavern-3.0.0a4/docs/Makefile
+-rw-r--r--   0        0        0        6 2023-10-22 10:53:53.056714 tavern-3.0.0a4/docs/source/.gitignore
+-rw-r--r--   0        0        0      851 2023-10-22 10:53:53.056714 tavern-3.0.0a4/docs/source/_static/favicon.png
+-rw-r--r--   0        0        0     1448 2023-10-22 10:53:53.056714 tavern-3.0.0a4/docs/source/_static/icon.png
+-rw-r--r--   0        0        0    70972 2024-01-27 15:02:03.823595 tavern-3.0.0a4/docs/source/basics.md
+-rw-r--r--   0        0        0     5807 2024-01-27 15:30:14.849609 tavern-3.0.0a4/docs/source/conf.py
+-rw-r--r--   0        0        0     4186 2023-11-04 16:24:35.280382 tavern-3.0.0a4/docs/source/cookbook.md
+-rw-r--r--   0        0        0     7667 2023-10-22 10:53:53.060047 tavern-3.0.0a4/docs/source/debugging.md
+-rw-r--r--   0        0        0     7883 2023-10-22 10:53:53.060047 tavern-3.0.0a4/docs/source/examples.md
+-rw-r--r--   0        0        0     5188 2024-01-20 13:06:48.131958 tavern-3.0.0a4/docs/source/grpc.md
+-rw-r--r--   0        0        0    12311 2023-11-04 16:24:35.280382 tavern-3.0.0a4/docs/source/http.md
+-rw-r--r--   0        0        0     1528 2024-01-27 15:02:03.823595 tavern-3.0.0a4/docs/source/index.md
+-rw-r--r--   0        0        0     9433 2023-10-22 10:53:53.060047 tavern-3.0.0a4/docs/source/mqtt.md
+-rw-r--r--   0        0        0    11359 2023-10-22 10:53:53.060047 tavern-3.0.0a4/docs/source/plugins.md
+-rw-r--r--   0        0        0     2895 2023-10-22 10:53:53.060047 tavern-3.0.0a4/docs/source/server.md
+-rw-r--r--   0        0        0      220 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/advanced/Dockerfile
+-rw-r--r--   0        0        0      401 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/advanced/advanced.md
+-rw-r--r--   0        0        0      149 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/advanced/common.yaml
+-rw-r--r--   0        0        0      126 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/advanced/docker-compose.yaml
+-rw-r--r--   0        0        0     3551 2024-01-18 13:28:20.874570 tavern-3.0.0a4/example/advanced/server.py
+-rw-r--r--   0        0        0     4046 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/advanced/test_server.tavern.yaml
+-rw-r--r--   0        0        0      673 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/advanced/testing_utils.py
+-rw-r--r--   0        0        0      210 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/components/Dockerfile
+-rw-r--r--   0        0        0      168 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/components/common.yaml
+-rw-r--r--   0        0        0      717 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/components/components.md
+-rw-r--r--   0        0        0      594 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/components/components/auth_stage.yaml
+-rw-r--r--   0        0        0      126 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/components/docker-compose.yaml
+-rw-r--r--   0        0        0     1642 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/components/server.py
+-rw-r--r--   0        0        0      633 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/components/test_hello.tavern.yaml
+-rw-r--r--   0        0        0      612 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/components/test_ping.tavern.yaml
+-rw-r--r--   0        0        0      195 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/cookies/Dockerfile
+-rw-r--r--   0        0        0      117 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/cookies/common.yaml
+-rw-r--r--   0        0        0      147 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/cookies/cookies.md
+-rw-r--r--   0        0        0      126 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/cookies/docker-compose.yaml
+-rw-r--r--   0        0        0     2973 2024-01-18 13:28:20.874570 tavern-3.0.0a4/example/cookies/server.py
+-rw-r--r--   0        0        0     3245 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/cookies/test_server.tavern.yaml
+-rw-r--r--   0        0        0      202 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/generate_from_openapi/Pipfile
+-rw-r--r--   0        0        0    13687 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/generate_from_openapi/Pipfile.lock
+-rw-r--r--   0        0        0     2106 2024-01-20 14:41:47.330398 tavern-3.0.0a4/example/generate_from_openapi/pub_tavern.py
+-rw-r--r--   0        0        0      144 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/generate_from_openapi/readme.md
+-rw-r--r--   0        0        0      566 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/generate_from_openapi/test_example_output.tavern.yaml
+-rw-r--r--   0        0        0      601 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/Dockerfile
+-rw-r--r--   0        0        0      159 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/common.yaml
+-rw-r--r--   0        0        0      455 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/conftest.py
+-rw-r--r--   0        0        0      206 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/docker-compose.yaml
+-rw-r--r--   0        0        0      295 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/helloworld_v1_precompiled.proto
+-rw-r--r--   0        0        0     1443 2024-01-20 13:42:01.354969 tavern-3.0.0a4/example/grpc/helloworld_v1_precompiled_pb2.py
+-rw-r--r--   0        0        0      595 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/helloworld_v1_precompiled_pb2.pyi
+-rw-r--r--   0        0        0     2586 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/helloworld_v1_precompiled_pb2_grpc.py
+-rw-r--r--   0        0        0      261 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/helloworld_v2_compiled.proto
+-rw-r--r--   0        0        0      286 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/helloworld_v3_reflected.proto
+-rwxr-xr-x   0        0        0      178 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/regenerate.sh
+-rw-r--r--   0        0        0     2905 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/server/server.py
+-rw-r--r--   0        0        0     6456 2024-01-20 13:06:48.131958 tavern-3.0.0a4/example/grpc/test_grpc.tavern.yaml
+-rw-r--r--   0        0        0      202 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/hooks/Dockerfile
+-rw-r--r--   0        0        0      990 2023-11-04 16:24:35.283715 tavern-3.0.0a4/example/hooks/conftest.py
+-rw-r--r--   0        0        0      126 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/hooks/docker-compose.yaml
+-rw-r--r--   0        0        0      464 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/hooks/server.py
+-rw-r--r--   0        0        0      620 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/hooks/test_server.tavern.yaml
+-rw-r--r--   0        0        0      844 2023-11-04 16:24:35.283715 tavern-3.0.0a4/example/mqtt/README.md
+-rw-r--r--   0        0        0      158 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/mqtt/common.yaml
+-rw-r--r--   0        0        0     2583 2023-11-04 16:24:35.283715 tavern-3.0.0a4/example/mqtt/conftest.py
+-rw-r--r--   0        0        0      990 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/mqtt/docker-compose.yaml
+-rw-r--r--   0        0        0      135 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/mqtt/fluent.conf
+-rw-r--r--   0        0        0      158 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/mqtt/listener.Dockerfile
+-rw-r--r--   0        0        0     4851 2023-11-04 16:24:35.283715 tavern-3.0.0a4/example/mqtt/listener.py
+-rw-r--r--   0        0        0      169 2023-11-04 16:24:35.283715 tavern-3.0.0a4/example/mqtt/mosquitto.conf
+-rw-r--r--   0        0        0      120 2023-11-04 16:24:35.283715 tavern-3.0.0a4/example/mqtt/mosquitto_passwd
+-rw-r--r--   0        0        0      393 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/mqtt/server.Dockerfile
+-rw-r--r--   0        0        0     4690 2024-01-18 13:28:20.874570 tavern-3.0.0a4/example/mqtt/server.py
+-rw-r--r--   0        0        0    15562 2023-11-04 16:24:35.283715 tavern-3.0.0a4/example/mqtt/test_mqtt.tavern.yaml
+-rw-r--r--   0        0        0     3381 2023-11-04 16:24:35.283715 tavern-3.0.0a4/example/mqtt/test_mqtt_failures.tavern.yaml
+-rw-r--r--   0        0        0      197 2024-01-06 15:34:53.978905 tavern-3.0.0a4/example/mqtt/testing_utils.py
+-rw-r--r--   0        0        0     1167 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/simple/running_tests.md
+-rw-r--r--   0        0        0      464 2023-12-23 17:57:23.503047 tavern-3.0.0a4/example/simple/server.py
+-rw-r--r--   0        0        0     1996 2023-10-22 10:53:53.060047 tavern-3.0.0a4/example/simple/test_server.tavern.yaml
+-rw-r--r--   0        0        0     4789 2024-01-27 15:30:14.849609 tavern-3.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0    88688 2024-01-27 15:02:03.826928 tavern-3.0.0a4/requirements.txt
+-rwxr-xr-x   0        0        0      222 2023-10-22 10:53:53.060047 tavern-3.0.0a4/scripts/coverage.sh
+-rwxr-xr-x   0        0        0      407 2023-10-22 10:53:53.060047 tavern-3.0.0a4/scripts/release.sh
+-rwxr-xr-x   0        0        0      327 2024-01-27 15:12:07.675707 tavern-3.0.0a4/scripts/smoke.bash
+-rwxr-xr-x   0        0        0      616 2023-10-22 10:53:53.060047 tavern-3.0.0a4/scripts/update-changelog.bash
+-rw-r--r--   0        0        0      101 2024-01-27 15:30:14.849609 tavern-3.0.0a4/tavern/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-29 14:00:16.070308 tavern-3.0.0a4/tavern/_core/__init__.py
+-rw-r--r--   0        0        0    20919 2024-01-27 15:23:23.118129 tavern-3.0.0a4/tavern/_core/dict_util.py
+-rw-r--r--   0        0        0     4603 2024-01-27 15:02:03.826928 tavern-3.0.0a4/tavern/_core/exceptions.py
+-rw-r--r--   0        0        0     4860 2024-01-27 15:19:36.450648 tavern-3.0.0a4/tavern/_core/extfunctions.py
+-rw-r--r--   0        0        0       96 2023-10-22 10:53:53.060047 tavern-3.0.0a4/tavern/_core/formatted_str.py
+-rw-r--r--   0        0        0      949 2024-01-27 15:19:36.443981 tavern-3.0.0a4/tavern/_core/general.py
+-rw-r--r--   0        0        0     2611 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/_core/jmesutils.py
+-rw-r--r--   0        0        0    12642 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/_core/loader.py
+-rw-r--r--   0        0        0     9891 2024-01-27 15:02:40.567056 tavern-3.0.0a4/tavern/_core/plugins.py
+-rw-r--r--   0        0        0      275 2023-10-22 10:53:53.060047 tavern-3.0.0a4/tavern/_core/pytest/__init__.py
+-rw-r--r--   0        0        0     2229 2024-01-27 15:02:03.826928 tavern-3.0.0a4/tavern/_core/pytest/config.py
+-rw-r--r--   0        0        0     7497 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/_core/pytest/error.py
+-rw-r--r--   0        0        0    13629 2024-01-27 15:22:10.661202 tavern-3.0.0a4/tavern/_core/pytest/file.py
+-rw-r--r--   0        0        0     2632 2024-01-27 15:02:40.567056 tavern-3.0.0a4/tavern/_core/pytest/hooks.py
+-rw-r--r--   0        0        0    10623 2024-01-27 15:19:36.450648 tavern-3.0.0a4/tavern/_core/pytest/item.py
+-rw-r--r--   0        0        0     2250 2024-01-27 15:19:36.443981 tavern-3.0.0a4/tavern/_core/pytest/newhooks.py
+-rw-r--r--   0        0        0     6793 2024-01-27 15:19:36.443981 tavern-3.0.0a4/tavern/_core/pytest/util.py
+-rw-r--r--   0        0        0     1911 2024-01-27 15:19:36.443981 tavern-3.0.0a4/tavern/_core/report.py
+-rw-r--r--   0        0        0    12125 2024-01-27 15:02:40.567056 tavern-3.0.0a4/tavern/_core/run.py
+-rw-r--r--   0        0        0        0 2023-10-22 10:53:53.060047 tavern-3.0.0a4/tavern/_core/schema/__init__.py
+-rw-r--r--   0        0        0    16038 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/_core/schema/extensions.py
+-rw-r--r--   0        0        0     4373 2024-01-27 15:02:40.567056 tavern-3.0.0a4/tavern/_core/schema/files.py
+-rw-r--r--   0        0        0     7149 2024-01-27 15:02:03.830261 tavern-3.0.0a4/tavern/_core/schema/jsonschema.py
+-rw-r--r--   0        0        0    10613 2024-01-20 13:06:48.131958 tavern-3.0.0a4/tavern/_core/schema/tests.jsonschema.yaml
+-rw-r--r--   0        0        0     7927 2024-01-20 13:06:48.131958 tavern-3.0.0a4/tavern/_core/schema/tests.schema.yaml
+-rw-r--r--   0        0        0     1659 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/_core/stage_lines.py
+-rw-r--r--   0        0        0     5139 2024-01-27 15:02:03.830261 tavern-3.0.0a4/tavern/_core/strict_util.py
+-rw-r--r--   0        0        0      380 2024-01-20 18:20:07.221269 tavern-3.0.0a4/tavern/_core/strtobool.py
+-rw-r--r--   0        0        0     3997 2024-01-27 15:19:36.443981 tavern-3.0.0a4/tavern/_core/testhelpers.py
+-rw-r--r--   0        0        0     2778 2024-01-27 15:19:36.443981 tavern-3.0.0a4/tavern/_core/tincture.py
+-rw-r--r--   0        0        0        0 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tavern/_plugins/__init__.py
+-rw-r--r--   0        0        0      590 2024-01-20 13:06:48.131958 tavern-3.0.0a4/tavern/_plugins/grpc/__init__.py
+-rw-r--r--   0        0        0    10557 2024-01-27 15:03:13.937172 tavern-3.0.0a4/tavern/_plugins/grpc/client.py
+-rw-r--r--   0        0        0     1329 2024-01-20 13:06:48.135291 tavern-3.0.0a4/tavern/_plugins/grpc/jsonschema.yaml
+-rw-r--r--   0        0        0     5283 2024-01-27 15:02:03.830261 tavern-3.0.0a4/tavern/_plugins/grpc/protos.py
+-rw-r--r--   0        0        0     2381 2024-01-27 15:21:31.611062 tavern-3.0.0a4/tavern/_plugins/grpc/request.py
+-rw-r--r--   0        0        0     5854 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/_plugins/grpc/response.py
+-rw-r--r--   0        0        0      921 2024-01-20 13:06:48.135291 tavern-3.0.0a4/tavern/_plugins/grpc/schema.yaml
+-rw-r--r--   0        0        0      883 2024-01-27 15:02:40.567056 tavern-3.0.0a4/tavern/_plugins/grpc/tavernhook.py
+-rw-r--r--   0        0        0        0 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tavern/_plugins/mqtt/__init__.py
+-rw-r--r--   0        0        0    18125 2024-01-27 15:19:36.450648 tavern-3.0.0a4/tavern/_plugins/mqtt/client.py
+-rw-r--r--   0        0        0     4013 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tavern/_plugins/mqtt/jsonschema.yaml
+-rw-r--r--   0        0        0     2515 2024-01-27 15:02:03.833595 tavern-3.0.0a4/tavern/_plugins/mqtt/request.py
+-rw-r--r--   0        0        0    11582 2024-01-27 15:19:36.450648 tavern-3.0.0a4/tavern/_plugins/mqtt/response.py
+-rw-r--r--   0        0        0     3233 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tavern/_plugins/mqtt/schema.yaml
+-rw-r--r--   0        0        0     1460 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/_plugins/mqtt/tavernhook.py
+-rw-r--r--   0        0        0        0 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tavern/_plugins/rest/__init__.py
+-rw-r--r--   0        0        0     6549 2024-01-27 15:02:03.833595 tavern-3.0.0a4/tavern/_plugins/rest/files.py
+-rw-r--r--   0        0        0    16165 2024-01-27 15:19:36.450648 tavern-3.0.0a4/tavern/_plugins/rest/request.py
+-rw-r--r--   0        0        0     8307 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/_plugins/rest/response.py
+-rw-r--r--   0        0        0      958 2024-01-27 15:19:36.443981 tavern-3.0.0a4/tavern/_plugins/rest/tavernhook.py
+-rw-r--r--   0        0        0     3097 2024-01-27 15:04:12.554042 tavern-3.0.0a4/tavern/core.py
+-rw-r--r--   0        0        0     2745 2024-01-27 15:02:03.833595 tavern-3.0.0a4/tavern/entry.py
+-rw-r--r--   0        0        0     7599 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/helpers.py
+-rw-r--r--   0        0        0      693 2024-01-27 14:41:40.632683 tavern-3.0.0a4/tavern/request.py
+-rw-r--r--   0        0        0     9933 2024-01-27 15:19:36.447315 tavern-3.0.0a4/tavern/response.py
+-rw-r--r--   0        0        0     1051 2024-01-27 15:02:03.833595 tavern-3.0.0a4/tests/conftest.py
+-rw-r--r--   0        0        0       37 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/881_1.json
+-rw-r--r--   0        0        0       41 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/881_2.yaml
+-rw-r--r--   0        0        0      202 2023-12-23 17:57:23.506380 tavern-3.0.0a4/tests/integration/Dockerfile
+-rw-r--r--   0        0        0       33 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/OK.json.gz
+-rw-r--r--   0        0        0        3 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/OK.txt
+-rw-r--r--   0        0        0      504 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/README.md
+-rw-r--r--   0        0        0      608 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/common.yaml
+-rw-r--r--   0        0        0      734 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/conftest.py
+-rw-r--r--   0        0        0      126 2023-12-23 17:57:23.506380 tavern-3.0.0a4/tests/integration/docker-compose.yaml
+-rw-r--r--   0        0        0      362 2024-01-20 18:20:07.221269 tavern-3.0.0a4/tests/integration/ext_functions.py
+-rw-r--r--   0        0        0      203 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/extra.yaml
+-rw-r--r--   0        0        0      254 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/global_cfg.yaml
+-rw-r--r--   0        0        0       91 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/parametrize_includes.yaml
+-rw-r--r--   0        0        0    13044 2024-01-20 18:20:07.221269 tavern-3.0.0a4/tests/integration/server.py
+-rw-r--r--   0        0        0      297 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_allure.tavern.yaml
+-rw-r--r--   0        0        0      659 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_auth_key.tavern.yaml
+-rw-r--r--   0        0        0      624 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_certs.tavern.yaml
+-rw-r--r--   0        0        0      823 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/test_control_flow.tavern.yaml
+-rw-r--r--   0        0        0     1569 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_cookie_remember.tavern.yaml
+-rw-r--r--   0        0        0     6106 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_cookies.tavern.yaml
+-rw-r--r--   0        0        0     2448 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_data_key.tavern.yaml
+-rw-r--r--   0        0        0       29 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_dummy.py
+-rw-r--r--   0        0        0      331 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_env_var_format.tavern.yaml
+-rw-r--r--   0        0        0      277 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_error.tavern.yaml
+-rw-r--r--   0        0        0     3614 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/test_external_functions.tavern.yaml
+-rw-r--r--   0        0        0     5435 2023-12-23 17:57:23.506380 tavern-3.0.0a4/tests/integration/test_files.tavern.yaml
+-rw-r--r--   0        0        0     2704 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/test_fixtures.tavern.yaml
+-rw-r--r--   0        0        0      799 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_follow_redirects.tavern.yaml
+-rw-r--r--   0        0        0     1028 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_header_comparisons.tavern.yaml
+-rw-r--r--   0        0        0     1269 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_helpers.tavern.yaml
+-rw-r--r--   0        0        0     1072 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/test_include.tavern.yaml
+-rw-r--r--   0        0        0     4837 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_jmes.tavern.yaml
+-rw-r--r--   0        0        0    15252 2024-01-06 15:34:53.978905 tavern-3.0.0a4/tests/integration/test_parametrize.tavern.yaml
+-rw-r--r--   0        0        0     2167 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_regex.tavern.yaml
+-rw-r--r--   0        0        0     2031 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_response_types.tavern.yaml
+-rw-r--r--   0        0        0     2372 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_retry.tavern.yaml
+-rw-r--r--   0        0        0      575 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_save_dict_value.tavern.yaml
+-rw-r--r--   0        0        0      970 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_selective_tests.tavern.yaml
+-rw-r--r--   0        0        0     2432 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_skipped_tests.tavern.yaml
+-rw-r--r--   0        0        0     1506 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_status_codes.tavern.yaml
+-rw-r--r--   0        0        0      235 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_stream.tavern.yaml
+-rw-r--r--   0        0        0    10926 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_strict_key_checks.tavern.yaml
+-rw-r--r--   0        0        0     1951 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_timeout.tavern.yaml
+-rw-r--r--   0        0        0     1126 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/test_tincture.tavern.yaml
+-rw-r--r--   0        0        0    12933 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/integration/test_typetokens.tavern.yaml
+-rw-r--r--   0        0        0     1415 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/test_validate_pykwalify.tavern.yaml
+-rw-r--r--   0        0        0        0 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/integration/testfile.txt
+-rw-r--r--   0        0        0      650 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/logging.yaml
+-rw-r--r--   0        0        0      931 2024-01-20 13:06:48.135291 tavern-3.0.0a4/tests/unit/conftest.py
+-rw-r--r--   0        0        0     9580 2024-01-20 18:20:07.221269 tavern-3.0.0a4/tests/unit/response/test_mqtt_response.py
+-rw-r--r--   0        0        0    12240 2024-01-20 18:20:07.224603 tavern-3.0.0a4/tests/unit/response/test_rest.py
+-rw-r--r--   0        0        0        0 2024-01-20 13:06:48.135291 tavern-3.0.0a4/tests/unit/tavern_grpc/__init__.py
+-rw-r--r--   0        0        0     6192 2024-01-27 15:02:03.833595 tavern-3.0.0a4/tests/unit/tavern_grpc/test_grpc.py
+-rw-r--r--   0        0        0      336 2024-01-20 13:06:48.135291 tavern-3.0.0a4/tests/unit/tavern_grpc/test_services.proto
+-rw-r--r--   0        0        0     1614 2024-01-20 14:48:43.784905 tavern-3.0.0a4/tests/unit/tavern_grpc/test_services_pb2.py
+-rw-r--r--   0        0        0      671 2024-01-20 13:06:48.135291 tavern-3.0.0a4/tests/unit/tavern_grpc/test_services_pb2.pyi
+-rw-r--r--   0        0        0     4137 2024-01-20 14:48:44.048239 tavern-3.0.0a4/tests/unit/tavern_grpc/test_services_pb2_grpc.py
+-rw-r--r--   0        0        0     1565 2024-01-20 13:06:48.135291 tavern-3.0.0a4/tests/unit/test_call_run.py
+-rw-r--r--   0        0        0    20143 2023-11-04 16:24:35.283715 tavern-3.0.0a4/tests/unit/test_core.py
+-rw-r--r--   0        0        0      798 2024-01-20 13:06:48.135291 tavern-3.0.0a4/tests/unit/test_extensions.py
+-rw-r--r--   0        0        0    14238 2024-01-20 18:20:07.224603 tavern-3.0.0a4/tests/unit/test_helpers.py
+-rw-r--r--   0        0        0     8444 2024-01-27 15:13:08.132586 tavern-3.0.0a4/tests/unit/test_mqtt.py
+-rw-r--r--   0        0        0     5791 2023-11-04 16:24:35.287048 tavern-3.0.0a4/tests/unit/test_pytest_hooks.py
+-rw-r--r--   0        0        0    16788 2023-11-04 16:24:35.287048 tavern-3.0.0a4/tests/unit/test_request.py
+-rw-r--r--   0        0        0     6131 2023-12-23 17:57:23.506380 tavern-3.0.0a4/tests/unit/test_schema.py
+-rw-r--r--   0        0        0     1030 2023-10-22 10:53:53.063381 tavern-3.0.0a4/tests/unit/test_strict_util.py
+-rw-r--r--   0        0        0     3289 2024-01-18 18:38:53.613931 tavern-3.0.0a4/tests/unit/test_tinctures.py
+-rw-r--r--   0        0        0    14898 2023-11-04 16:24:35.287048 tavern-3.0.0a4/tests/unit/test_utilities.py
+-rw-r--r--   0        0        0     2206 2024-01-27 15:02:40.567056 tavern-3.0.0a4/tox-integration.ini
+-rw-r--r--   0        0        0      653 2024-01-27 15:02:03.833595 tavern-3.0.0a4/tox.ini
+-rw-r--r--   0        0        0    11288 1970-01-01 00:00:00.000000 tavern-3.0.0a4/PKG-INFO
```

### Comparing `tavern-3.0.0a3/.dockerignore` & `tavern-3.0.0a4/.dockerignore`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/.github/workflows/main.yml` & `tavern-3.0.0a4/.github/workflows/main.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,17 @@
       - feat/3.0-release
 
 jobs:
   simple-checks:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - uses: pre-commit/action@v3.0.0
 
   unit-tests:
     runs-on: ubuntu-latest
@@ -39,32 +39,32 @@
             TOXCFG: tox.ini
 
     env:
       TOXENV: ${{ matrix.TOXENV }}
       TOXCFG: ${{ matrix.TOXCFG }}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         env:
           cache-name: cache-${{ matrix.TOXENV }}
         with:
           path: .tox
           key: ${{ runner.os }}-tox-${{ env.cache-name }}-${{ hashFiles('pyproject.toml', 'constraints.txt') }}
 
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml', 'constraints.txt') }}
           restore-keys: |
             ${{ runner.os }}-pip-
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - name: install deps
         run: |
           pip install tox -c constraints.txt
 
@@ -97,35 +97,35 @@
         image: docker
 
     env:
       TOXENV: ${{ matrix.TOXENV }}
       TOXCFG: ${{ matrix.TOXCFG }}
 
     steps:
-      - uses: jpribyl/action-docker-layer-caching@v0.1.1
+      - uses: docker/setup-buildx-action@v3
         continue-on-error: true
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         env:
           cache-name: cache-${{ matrix.TOXENV }}
         with:
           path: .tox
           key: ${{ runner.os }}-tox-${{ env.cache-name }}-${{ hashFiles('pyproject.toml', 'constraints.txt') }}
 
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml', 'constraints.txt') }}
           restore-keys: |
             ${{ runner.os }}-pip-
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.11"
 
       - name: Install Protoc
         if: ${{ contains(matrix.TOXENV, 'grpc') }}
         uses: arduino/setup-protoc@v2
         with:
```

### Comparing `tavern-3.0.0a3/.gitignore` & `tavern-3.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/.pre-commit-config.yaml` & `tavern-3.0.0a4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       - id: actionlint
         args: ["-shellcheck="]
   - repo: https://github.com/hadialqattan/pycln
     rev: v2.4.0
     hooks:
       - id: pycln
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.1.11"
+    rev: "v0.1.14"
     hooks:
       - id: ruff-format
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0
     hooks:
```

### Comparing `tavern-3.0.0a3/CHANGELOG.md` & `tavern-3.0.0a4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -424,7 +424,11 @@
 #  2.6.0           fix verify_response_with with multiple MQTT responses (2023-11-18)
 
 #  2.7.0           update minimum version of jsonschema (2023-12-26)
 
 ##  2.7.1           Fix jsonschema warnings (2023-12-26)
 
 #  2.8.0           Initial gRPC support (2024-01-20)
+
+#  2.9.0           Fix mqtt implementation checking for message publication correctly (2024-01-23)
+
+##  2.9.1           internal cleanup (2024-01-27)
```

### Comparing `tavern-3.0.0a3/CONTRIBUTING.md` & `tavern-3.0.0a4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/LICENSE` & `tavern-3.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/README.md` & `tavern-3.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/constraints.txt` & `tavern-3.0.0a4/constraints.txt`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/Makefile` & `tavern-3.0.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/_static/favicon.png` & `tavern-3.0.0a4/docs/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/_static/icon.png` & `tavern-3.0.0a4/docs/source/_static/icon.png`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/basics.md` & `tavern-3.0.0a4/docs/source/basics.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/conf.py` & `tavern-3.0.0a4/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = "1.0"
 # The full version, including alpha/beta/rc tags.
-release = "3.0.0a3"
+release = "3.0.0a4"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
```

### Comparing `tavern-3.0.0a3/docs/source/cookbook.md` & `tavern-3.0.0a4/docs/source/cookbook.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/debugging.md` & `tavern-3.0.0a4/docs/source/debugging.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/examples.md` & `tavern-3.0.0a4/docs/source/examples.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/grpc.md` & `tavern-3.0.0a4/docs/source/grpc.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/http.md` & `tavern-3.0.0a4/docs/source/http.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/index.md` & `tavern-3.0.0a4/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/mqtt.md` & `tavern-3.0.0a4/docs/source/mqtt.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/plugins.md` & `tavern-3.0.0a4/docs/source/plugins.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/docs/source/server.md` & `tavern-3.0.0a4/docs/source/server.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/advanced/server.py` & `tavern-3.0.0a4/example/advanced/server.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/advanced/test_server.tavern.yaml` & `tavern-3.0.0a4/example/advanced/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/advanced/testing_utils.py` & `tavern-3.0.0a4/example/advanced/testing_utils.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/components/components.md` & `tavern-3.0.0a4/example/components/components.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/components/components/auth_stage.yaml` & `tavern-3.0.0a4/example/components/components/auth_stage.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/components/server.py` & `tavern-3.0.0a4/example/components/server.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/components/test_hello.tavern.yaml` & `tavern-3.0.0a4/example/components/test_hello.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/components/test_ping.tavern.yaml` & `tavern-3.0.0a4/example/components/test_ping.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/cookies/server.py` & `tavern-3.0.0a4/example/cookies/server.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/cookies/test_server.tavern.yaml` & `tavern-3.0.0a4/example/cookies/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/generate_from_openapi/Pipfile.lock` & `tavern-3.0.0a4/example/generate_from_openapi/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/generate_from_openapi/pub_tavern.py` & `tavern-3.0.0a4/example/generate_from_openapi/pub_tavern.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/generate_from_openapi/test_example_output.tavern.yaml` & `tavern-3.0.0a4/example/generate_from_openapi/test_example_output.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/grpc/Dockerfile` & `tavern-3.0.0a4/example/grpc/Dockerfile`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/grpc/helloworld_v1_precompiled_pb2.py` & `tavern-3.0.0a4/example/grpc/helloworld_v1_precompiled_pb2.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/grpc/helloworld_v1_precompiled_pb2.pyi` & `tavern-3.0.0a4/example/grpc/helloworld_v1_precompiled_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/grpc/helloworld_v1_precompiled_pb2_grpc.py` & `tavern-3.0.0a4/example/grpc/helloworld_v1_precompiled_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/grpc/server/server.py` & `tavern-3.0.0a4/example/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/grpc/test_grpc.tavern.yaml` & `tavern-3.0.0a4/example/grpc/test_grpc.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/hooks/conftest.py` & `tavern-3.0.0a4/example/hooks/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/hooks/test_server.tavern.yaml` & `tavern-3.0.0a4/example/hooks/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/mqtt/README.md` & `tavern-3.0.0a4/example/mqtt/README.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/mqtt/conftest.py` & `tavern-3.0.0a4/example/mqtt/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/mqtt/docker-compose.yaml` & `tavern-3.0.0a4/example/mqtt/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/mqtt/listener.py` & `tavern-3.0.0a4/example/mqtt/listener.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/mqtt/server.py` & `tavern-3.0.0a4/example/mqtt/server.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/mqtt/test_mqtt.tavern.yaml` & `tavern-3.0.0a4/example/mqtt/test_mqtt.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/mqtt/test_mqtt_failures.tavern.yaml` & `tavern-3.0.0a4/example/mqtt/test_mqtt_failures.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/simple/running_tests.md` & `tavern-3.0.0a4/example/simple/running_tests.md`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/example/simple/test_server.tavern.yaml` & `tavern-3.0.0a4/example/simple/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/pyproject.toml` & `tavern-3.0.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ]
 requires-python = ">=3.11"
 
 keywords = ["testing", "pytest"]
 
 name = "tavern"
 description = "Simple testing of RESTful APIs"
-version = "3.0.0a3"
+version = "3.0.0a4"
 
 dependencies = [
     "PyYAML>=6.0.1,<7",
     "jmespath>=1,<2",
     "jsonschema>=4,<5",
     "pyjwt>=2.5.0,<3",
     "pykwalify>=1.8.0,<2",
@@ -183,15 +183,15 @@
 known-first-party = ["tavern"]
 
 [tool.ruff.format]
 exclude = ["*_pb2.py", "*_pb2_grpc.py", "*_pb2.pyi"]
 docstring-code-format = true
 
 [tool.tbump.version]
-current = "3.0.0a3"
+current = "3.0.0a4"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `tavern-3.0.0a3/requirements.txt` & `tavern-3.0.0a4/requirements.txt`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/scripts/update-changelog.bash` & `tavern-3.0.0a4/scripts/update-changelog.bash`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_core/dict_util.py` & `tavern-3.0.0a4/tavern/_core/dict_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import contextlib
 import functools
 import logging
 import os
 import re
 import string
+import typing
 from collections.abc import Collection, Iterable, Mapping, Sequence
-from typing import Any, TypeVar
+from typing import (
+    Any,
+)
 
 import box
 import jmespath
 from box.box import Box
 
 from tavern._core import exceptions
 from tavern._core.loader import (
@@ -52,15 +55,15 @@
                     field_name,
                     type(would_replace),
                 )
 
     return to_format.format(**box_vars)
 
 
-def _attempt_find_include(to_format: str, box_vars: box.Box):
+def _attempt_find_include(to_format: str, box_vars: box.Box) -> str | None:
     formatter = string.Formatter()
     would_format = list(formatter.parse(to_format))
 
     yaml_tag = ForceIncludeToken.yaml_tag
 
     if len(would_format) != 1:
         raise exceptions.InvalidFormattedJsonError(
@@ -86,79 +89,88 @@
     if format_spec:
         logger.warning(
             "Conversion specifier '%s' will be ignored for %s", format_spec, to_format
         )
 
     would_replace = formatter.get_field(field_name, [], box_vars)[0]
 
-    return formatter.convert_field(would_replace, conversion)  # type: ignore
+    if conversion is None:
+        return would_replace
+
+    return formatter.convert_field(would_replace, conversion)
+
+
+T = typing.TypeVar("T", str, dict, list, tuple)
 
 
 def format_keys(
-    val: TypeConvertToken | str | dict | list | tuple | Mapping | set,
+    val: T,
     variables: Mapping | Box,
     *,
     no_double_format: bool = True,
     dangerously_ignore_string_format_errors: bool = False,
-):
+) -> T:
     """recursively format a dictionary with the given values
 
     Args:
-        val: Input to format
+        val: Input thing to format
         variables: Dictionary of keys to format it with
         no_double_format: Whether to use the 'inner formatted string' class to avoid double formatting
             This is required if passing something via pytest-xdist, such as markers:
             https://github.com/taverntesting/tavern/issues/431
         dangerously_ignore_string_format_errors: whether to ignore any string formatting errors. This will result
             in broken output, only use for debugging purposes.
 
+    Raises:
+        MissingFormatError: if a format variable was not found in variables
+
     Returns:
         recursively formatted values
     """
-    formatted = val
-
     format_keys_ = functools.partial(
         format_keys,
         dangerously_ignore_string_format_errors=dangerously_ignore_string_format_errors,
     )
 
     if not isinstance(variables, Box):
         box_vars = Box(variables)
     else:
         box_vars = variables
 
     if isinstance(val, dict):
-        formatted = {}
-        # formatted = {key: format_keys(val[key], box_vars) for key in val}
-        for key in val:
-            formatted[key] = format_keys_(val[key], box_vars)
-    elif isinstance(val, (list, tuple, set)):
-        formatted = [format_keys_(item, box_vars) for item in val]  # type: ignore
-    elif isinstance(formatted, FormattedString):
-        logger.debug("Already formatted %s, not double-formatting", formatted)
+        return {key: format_keys_(val[key], box_vars) for key in val}
+    elif isinstance(val, tuple):
+        return tuple(format_keys_(item, box_vars) for item in val)
+    elif isinstance(val, list):
+        return [format_keys_(item, box_vars) for item in val]
+    elif isinstance(val, FormattedString):
+        logger.debug("Already formatted %s, not double-formatting", val)
     elif isinstance(val, str):
+        formatted = val
         try:
             formatted = _check_and_format_values(val, box_vars)
         except exceptions.MissingFormatError:
             if not dangerously_ignore_string_format_errors:
                 raise
 
         if no_double_format:
             formatted = FormattedString(formatted)  # type: ignore
+
+        return formatted
     elif isinstance(val, TypeConvertToken):
         logger.debug("Got type convert token '%s'", val)
         if isinstance(val, ForceIncludeToken):
-            formatted = _attempt_find_include(val.value, box_vars)
+            return _attempt_find_include(val.value, box_vars)
         else:
             value = format_keys_(val.value, box_vars)
-            formatted = val.constructor(value)
+            return val.constructor(value)
     else:
-        logger.debug("Not formatting something of type '%s'", type(formatted))
+        logger.debug("Not formatting something of type '%s'", type(val))
 
-    return formatted
+    return val
 
 
 def recurse_access_key(data: dict | list[str] | Mapping, query: str):
     """
     Search for something in the given data using the given query.
 
     Example:
@@ -168,16 +180,19 @@
         >>> recurse_access_key({"a": {"b": ["c", "d"]}}, "a.b[0]")
         'c'
 
     Args:
         data: Data to search in
         query: Query to run
 
+    Raises:
+        JMESError: if there was an error parsing the query
+
     Returns:
-        object: Whatever was found by the search
+        Whatever was found by the search
     """
 
     try:
         from_jmespath = jmespath.search(query, data)
     except jmespath.exceptions.ParseError as e:
         logger.error("Error parsing JMES query")
 
@@ -192,15 +207,15 @@
             )
 
         raise exceptions.JMESError("Invalid JMES query") from e
 
     return from_jmespath
 
 
-def _deprecated_recurse_access_key(current_val: dict, keys: list[str]):
+def _deprecated_recurse_access_key(current_val: Mapping | list, keys: list[str]):
     """Given a list of keys and a dictionary, recursively access the dicionary
     using the keys until we find the key its looking for
 
     If a key is an integer, it will convert it and use it as a list index
 
     Example:
 
@@ -214,28 +229,31 @@
         keys: list of str/int of subkeys
 
     Raises:
         IndexError: list index not found in data
         KeyError: dict key not found in data
 
     Returns:
-        str or dict: value of subkey in dict
+        value of subkey in dict
     """
     logger.debug("Recursively searching for '%s' in '%s'", keys, current_val)
 
     if not keys:
         return current_val
     else:
         current_key: str | int = keys.pop(0)
 
         with contextlib.suppress(ValueError):
             current_key = int(current_key)
 
         try:
-            return _deprecated_recurse_access_key(current_val[current_key], keys)
+            return _deprecated_recurse_access_key(
+                current_val[current_key],  # type:ignore
+                keys,
+            )
         except (IndexError, KeyError, TypeError) as e:
             logger.error(
                 "%s accessing data - looking for '%s' in '%s'",
                 type(e).__name__,
                 current_key,
                 current_val,
             )
@@ -324,32 +342,32 @@
         >>> next(gen)
         (['2'], '2', 'c')
 
     Args:
         block: input matches
 
     Yields:
-        key split on dots, key, expected value
+        iterable of (key split on dots, key, expected value)
     """
     if isinstance(block, dict):
         for joined_key, expected_val in block.items():
             split_key = joined_key.split(".")
             yield split_key, joined_key, expected_val
     else:
         for idx, val in enumerate(block):
             sidx = str(idx)
             yield [sidx], sidx, val
 
 
-T = TypeVar("T", Mapping, set, Sequence, Collection)
+Checked = typing.TypeVar("Checked", dict, Collection, str)
 
 
 def check_keys_match_recursive(
-    expected_val: T,
-    actual_val: T,
+    expected_val: Checked,
+    actual_val: Checked,
     keys: list[str | int],
     strict: StrictSettingKinds = True,
 ) -> None:
     """Utility to recursively check response values
 
     expected and actual both have to be of the same type or it will raise an
     error.
@@ -446,16 +464,16 @@
                             full_err()
                         )
                     )
 
                 raise exceptions.KeyMismatchError(msg) from e
 
         if isinstance(expected_val, dict):
-            akeys = set(actual_val.keys())  # type:ignore
             ekeys = set(expected_val.keys())
+            akeys = set(actual_val.keys())  # type:ignore
 
             if akeys != ekeys:
                 extra_actual_keys = akeys - ekeys
                 extra_expected_keys = ekeys - akeys
 
                 msg = ""
                 if extra_actual_keys:
```

### Comparing `tavern-3.0.0a3/tavern/_core/exceptions.py` & `tavern-3.0.0a4/tavern/_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_core/extfunctions.py` & `tavern-3.0.0a4/tavern/_core/extfunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import importlib
 import logging
-from collections.abc import Mapping
+from collections.abc import Callable, Iterable, Mapping
 from typing import Any
 
 from tavern._core import exceptions
 
 from .dict_util import deep_dict_merge
 
 
@@ -13,47 +13,50 @@
     """
     Whether the given object is an ext function block
 
     Args:
         block: Any object
 
     Returns:
-        bool: If it is an ext function style dict
+        If it is an ext function style dict
     """
     return isinstance(block, dict) and block.get("$ext", None) is not None
 
 
 def get_pykwalify_logger(module: str | None) -> logging.Logger:
     """Get logger for this module
 
     Have to do it like this because the way that pykwalify load extension
     modules means that getting the logger the normal way just result sin it
     trying to get the root logger which won't log correctly
 
     Args:
-        module (string): name of module to get logger for
+        module: name of module to get logger for
 
+    Returns:
+        logger for given module
     """
     return logging.getLogger(module)
 
 
 def _getlogger() -> logging.Logger:
+    """Get logger for this module"""
     return get_pykwalify_logger("tavern._core.extfunctions")
 
 
-def import_ext_function(entrypoint: str):
+def import_ext_function(entrypoint: str) -> Callable:
     """Given a function name in the form of a setuptools entry point, try to
     dynamically load and return it
 
     Args:
         entrypoint: setuptools-style entrypoint in the form
             module.submodule:function
 
     Returns:
-        function: function loaded from entrypoint
+        function loaded from entrypoint
 
     Raises:
         InvalidExtFunctionError: If the module or function did not exist
     """
     logger = _getlogger()
 
     try:
@@ -76,26 +79,26 @@
         msg = f"No function named {funcname} in {module}"
         logger.exception(msg)
         raise exceptions.InvalidExtFunctionError(msg) from e
 
     return function
 
 
-def get_wrapped_response_function(ext: Mapping):
+def get_wrapped_response_function(ext: Mapping) -> Callable:
     """Wraps a ext function with arguments given in the test file
 
     This is similar to functools.wrap, but this makes sure that 'response' is
     always the first argument passed to the function
 
     Args:
         ext: $ext function dict with function, extra_args, and
             extra_kwargs to pass
 
     Returns:
-        function: Wrapped function
+        Wrapped function
     """
 
     func, args, kwargs = _get_ext_values(ext)
 
     @functools.wraps(func)
     def inner(response):
         result = func(response, *args, **kwargs)
@@ -103,15 +106,15 @@
         return result
 
     inner.func = func  # type: ignore
 
     return inner
 
 
-def get_wrapped_create_function(ext: Mapping):
+def get_wrapped_create_function(ext: Mapping) -> Callable:
     """Same as get_wrapped_response_function, but don't require a response"""
 
     func, args, kwargs = _get_ext_values(ext)
 
     @functools.wraps(func)
     def inner():
         result = func(*args, **kwargs)
@@ -119,15 +122,15 @@
         return result
 
     inner.func = func  # type: ignore
 
     return inner
 
 
-def _get_ext_values(ext: Mapping):
+def _get_ext_values(ext: Mapping) -> tuple[Callable, Iterable, Mapping]:
     if not isinstance(ext, Mapping):
         raise exceptions.InvalidExtFunctionError(
             f"ext block should be a dict, but it was a {type(ext)}"
         )
 
     args = ext.get("extra_args") or ()
     kwargs = ext.get("extra_kwargs") or {}
```

### Comparing `tavern-3.0.0a3/tavern/_core/general.py` & `tavern-3.0.0a4/tavern/_core/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from tavern._core.loader import load_single_document_yaml
 
 from .dict_util import deep_dict_merge
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def load_global_config(global_cfg_paths: list[os.PathLike]) -> dict:
+def load_global_config(global_cfg_paths: list[str | os.PathLike]) -> dict:
     """Given a list of file paths to global config files, load each of them and
     return the joined dictionary.
 
     This does a deep dict merge.
 
     Args:
         global_cfg_paths: List of filenames to load from
```

### Comparing `tavern-3.0.0a3/tavern/_core/jmesutils.py` & `tavern-3.0.0a4/tavern/_core/jmesutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import operator
 import re
 from collections.abc import Sized
-from typing import Any
+from typing import (
+    Any,
+)
 
 from tavern._core import exceptions
 
 
 def test_type(val, mytype) -> bool:
     """Check value fits one of the types, if so return true, else false"""
     typelist = TYPES.get(str(mytype).lower())
@@ -58,15 +60,15 @@
     """Exception-safe length check, returns -1 if no length on type or error"""
     try:
         return len(var)
     except TypeError:
         return -1
 
 
-def validate_comparison(each_comparison):
+def validate_comparison(each_comparison: dict[Any, Any]):
     if extra := set(each_comparison.keys()) - {"jmespath", "operator", "expected"}:
         raise exceptions.BadSchemaError(
             "Invalid keys given to JMES validation function (got extra keys: {})".format(
                 extra
             )
         )
```

### Comparing `tavern-3.0.0a3/tavern/_core/loader.py` & `tavern-3.0.0a4/tavern/_core/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,21 +33,21 @@
     """A composer that doesn't forget anchors across documents"""
 
     def get_event(self) -> None:
         ...
 
     def compose_document(self) -> Node | None:
         # Drop the DOCUMENT-START event.
-        self.get_event()
+        self.get_event()  # type:ignore
 
         # Compose the root node.
         node = self.compose_node(None, None)  # type:ignore
 
         # Drop the DOCUMENT-END event.
-        self.get_event()
+        self.get_event()  # type:ignore
 
         # If we don't drop the anchors here, then we can keep anchors across
         # documents.
         # self.anchors = {}
 
         return node
 
@@ -106,16 +106,14 @@
     SourceMappingConstructor,
     SafeConstructor,
 ):
     """YAML Loader with `!include` constructor and which can remember anchors
     between documents"""
 
     def __init__(self, stream):
-        """Initialise Loader."""
-
         try:
             self._root = os.path.split(stream.name)[0]
         except AttributeError:
             self._root = os.path.curdir
 
         Reader.__init__(self, stream)
         Scanner.__init__(self)
```

### Comparing `tavern-3.0.0a3/tavern/_core/plugins.py` & `tavern-3.0.0a4/tavern/_core/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     Todo:
         Not all of these are required for all request/response types probably
 
     Args:
         ext: class or module plugin object
 
     Returns:
-        bool: Whether the plugin has everything we need to use it
+        Whether the plugin has everything we need to use it
     """
     required = [
         # MQTTClient, requests.Session
         "session_type",
         # RestRequest, MQTTRequest
         "request_type",
         # request, mqtt_publish, grpc_request
```

### Comparing `tavern-3.0.0a3/tavern/_core/pytest/config.py` & `tavern-3.0.0a4/tavern/_core/pytest/config.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_core/pytest/error.py` & `tavern-3.0.0a4/tavern/_core/pytest/error.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,49 @@
+import dataclasses
 import json
 import logging
 import re
-from collections.abc import Mapping
+import typing
 from io import StringIO
+from typing import Any
 
 import yaml
 from _pytest._code.code import FormattedExcinfo, TerminalRepr
 from _pytest._io import TerminalWriter
 
 from tavern._core import exceptions
 from tavern._core.dict_util import format_keys
+
+if typing.TYPE_CHECKING:
+    from tavern._core.pytest.item import YamlItem
+
 from tavern._core.report import prepare_yaml
 from tavern._core.stage_lines import (
     end_mark,
     get_stage_lines,
     read_relevant_lines,
     start_mark,
 )
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@dataclasses.dataclass
 class ReprdError(TerminalRepr):
-    def __init__(self, exce, item) -> None:
-        self.exce = exce
-        self.item = item
+    exce: Any
+    item: "YamlItem"
 
-    def _get_available_format_keys(self):
+    def _get_available_format_keys(self) -> dict:
         """Try to get the format variables for the stage
 
         If we can't get the variable for this specific stage, just return the
         global config which will at least have some format variables
 
         Returns:
-            dict: variables for formatting test
+            variables for formatting test
         """
         try:
             keys = self.exce._excinfo[1].test_block_config.variables
         except AttributeError:
             logger.warning("Unable to read stage variables - error output may be wrong")
             keys = self.item.global_cfg.variables
 
@@ -133,15 +139,15 @@
 
         for line in code_lines:
             if any(i in line for i in missing_format_vars):
                 tw.line(line, red=True)
             else:
                 tw.line(line, white=True)
 
-    def _print_formatted_stage(self, tw: TerminalWriter, stage: Mapping) -> None:
+    def _print_formatted_stage(self, tw: TerminalWriter, stage: dict) -> None:
         """Print the 'formatted' stage that Tavern will actually use to send the
         request/process the response
 
         Args:
             tw: Pytest TW instance
             stage: The 'final' stage used by Tavern
         """
@@ -151,18 +157,18 @@
 
         # Format stage variables recursively
         formatted_stage = format_keys(
             stage, keys, dangerously_ignore_string_format_errors=True
         )
 
         # Replace formatted strings with strings for dumping
-        formatted_stage = prepare_yaml(formatted_stage)
+        prepared_stage = prepare_yaml(formatted_stage)
 
         # Dump formatted stage to YAML format
-        formatted_lines = yaml.dump(formatted_stage, default_flow_style=False).split(
+        formatted_lines = yaml.dump(prepared_stage, default_flow_style=False).split(
             "\n"
         )
 
         for line in formatted_lines:
             if not line:
                 continue
             tw.line(f"  {line}", white=True)
```

### Comparing `tavern-3.0.0a3/tavern/_core/pytest/file.py` & `tavern-3.0.0a4/tavern/_core/pytest/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 import copy
 import functools
 import itertools
 import logging
-from collections.abc import Iterator, Mapping
-from typing import Any
+import typing
+from collections.abc import Callable, Iterable, Iterator, Mapping
+from typing import (
+    Any,
+)
 
 import pytest
 import yaml
 from box import Box
-from pytest import MarkDecorator
+from pytest import Mark
 
 from tavern._core import exceptions
 from tavern._core.dict_util import deep_dict_merge, format_keys, get_tavern_box
 from tavern._core.extfunctions import get_wrapped_create_function, is_ext_function
 from tavern._core.loader import IncludeLoader
 from tavern._core.schema.files import verify_tests
 
 from .item import YamlItem
 from .util import load_global_cfg
 
 logger: logging.Logger = logging.getLogger(__name__)
 
-_format_without_inner = functools.partial(format_keys, no_double_format=False)
+T = typing.TypeVar("T")
+
+_format_without_inner: Callable[[T, Mapping], T] = functools.partial(
+    format_keys, no_double_format=False
+)
 
 
 def _format_test_marks(
-    original_marks: list[Any], fmt_vars: Mapping, test_name: str
-) -> tuple[list[MarkDecorator], Any]:
+    original_marks: Iterable[str | dict], fmt_vars: Mapping, test_name: str
+) -> tuple[list[Mark], list[Mapping]]:
     """Given the 'raw' marks from the test and any available format variables,
     generate new  marks for this test
 
     Args:
         original_marks: Raw string from test - should correspond to either a
             pytest builtin mark or a custom user mark
         fmt_vars: dictionary containing available format variables
         test_name: Name of test (for error logging)
 
     Returns:
-        tuple: first element is normal pytest mark objects, second element is all
+        first element is normal pytest mark objects, second element is all
             marks which were formatted (no matter their content)
 
     Todo:
         Fix doctests below - failing due to missing pytest markers
 
     Example:
 
@@ -52,16 +59,16 @@
         # >>> _format_test_marks(['{formatme}'], {'formatme': 'tavernmarker'}, 'abc')
         # (['tavernmarker'], [])
         # >>> _format_test_marks([{'skipif': '{skiptest}'}], {'skiptest': true}, 'abc')
         # (['tavernmarker'], [])
 
     """
 
-    pytest_marks = []
-    formatted_marks = []
+    pytest_marks: list[Mark] = []
+    formatted_marks: list[Mapping] = []
 
     for m in original_marks:
         if isinstance(m, str):
             # a normal mark
             m = _format_without_inner(m, fmt_vars)
             pytest_marks.append(getattr(pytest.mark, m))
         elif isinstance(m, dict):
@@ -86,80 +93,87 @@
                     formatted_marks.append({markname: extra_arg})
         else:
             raise exceptions.BadSchemaError(f"Unexpected mark type '{type(m)}'")
 
     return pytest_marks, formatted_marks
 
 
-def _generate_parametrized_test_items(keys: list, vals_combination):
+def _maybe_load_ext(pair):
+    """Try to load ext values"""
+    key, value = pair
+
+    if is_ext_function(value):
+        # If it is an ext function, load the new (or supplemental) value[s]
+        ext = value.pop("$ext")
+        f = get_wrapped_create_function(ext)
+        new_value = f()
+
+        if len(value) == 0:
+            # Use only this new value
+            return key, new_value
+        elif isinstance(new_value, dict):
+            # Merge with some existing data. At this point 'value' is known to be a dict.
+            return key, deep_dict_merge(value, f())
+        else:
+            # For example, if it's defined like
+            #
+            # - testkey: testval
+            #   $ext:
+            #     function: mod:func
+            #
+            # and 'mod:func' returns a string, it's impossible to 'merge' with the existing data.
+            logger.error("Values still in 'val': %s", value)
+            raise exceptions.BadSchemaError(
+                "There were extra key/value pairs in the 'val' for this parametrize mark, but the ext function {} returned '{}' (of type {}) that was not a dictionary. It is impossible to merge these values.".format(
+                    ext, new_value, type(new_value)
+                )
+            )
+
+    return key, value
+
+
+def _generate_parametrized_test_items(
+    keys: Iterable[str | list | tuple], vals_combination: Iterable[tuple[str, str]]
+) -> tuple[Mapping[str, Any], str]:
     """Generate test name from given key(s)/value(s) combination
 
     Args:
         keys: list of keys to format name with
-        vals_combination (tuple(str)): this combination of values for the key
+        vals_combination this combination of values for the key
+
+    Returns:
+        tuple of the variables for the stage and the generated stage name
     """
-    flattened_values = []
-    variables = {}
+    flattened_values: list[Iterable[str]] = []
+    variables: dict[str, Any] = {}
 
     # combination of keys and the values they correspond to
     for pair in zip(keys, vals_combination):
         key, value = pair
         # NOTE: If test is invalid, test names generated here will be
         # very weird looking
         if isinstance(key, str):
             variables[key] = value
-            flattened_values += [value]
+            flattened_values.append(value)
         else:
             if not isinstance(value, (list, tuple)):
                 value = [value]
 
             if len(value) != len(key):
                 raise exceptions.BadSchemaError(
                     "Invalid match between numbers of keys and number of values in parametrize mark ({} keys, {} values)".format(
-                        (key), (value)
+                        key, value
                     )
                 )
 
             for subkey, subvalue in zip(key, value):
                 variables[subkey] = subvalue
-                flattened_values += [subvalue]
-
-    def maybe_load_ext(v):
-        key, value = v
-
-        if is_ext_function(value):
-            # If it is an ext function, load the new (or supplemental) value[s]
-            ext = value.pop("$ext")
-            f = get_wrapped_create_function(ext)
-            new_value = f()
-
-            if len(value) == 0:
-                # Use only this new value
-                return key, new_value
-            elif isinstance(new_value, dict):
-                # Merge with some existing data. At this point 'value' is known to be a dict.
-                return key, deep_dict_merge(value, f())
-            else:
-                # For example, if it's defined like
-                #
-                # - testkey: testval
-                #   $ext:
-                #     function: mod:func
-                #
-                # and 'mod:func' returns a string, it's impossible to 'merge' with the existing data.
-                logger.error("Values still in 'val': %s", value)
-                raise exceptions.BadSchemaError(
-                    "There were extra key/value pairs in the 'val' for this parametrize mark, but the ext function {} returned '{}' (of type {}) that was not a dictionary. It is impossible to merge these values.".format(
-                        ext, new_value, type(new_value)
-                    )
-                )
-
-        return key, value
+                flattened_values.append(subvalue)
 
-    variables = dict(map(maybe_load_ext, variables.items()))
+    variables = dict(map(_maybe_load_ext, variables.items()))
 
     logger.debug("Variables for this combination: %s", variables)
     logger.debug("Values for this combination: %s", flattened_values)
 
     # Use for formatting parametrized values - eg {}-{}, {}-{}-{}, etc.
     inner_fmt = "-".join(["{}"] * len(flattened_values))
     inner_formatted = inner_fmt.format(*flattened_values)
@@ -167,15 +181,15 @@
     return variables, inner_formatted
 
 
 def _get_parametrized_items(
     parent: pytest.File,
     test_spec: dict,
     parametrize_marks: list[dict],
-    pytest_marks: list[MarkDecorator],
+    pytest_marks: list[Mark],
 ) -> Iterator[YamlItem]:
     """Return new items with new format values available based on the mark
 
     This will change the name from something like 'test a thing' to 'test a
     thing[param1]', 'test a thing[param2]', etc. This probably messes with
     -k
 
@@ -205,15 +219,15 @@
     try:
         combined = itertools.product(*vals)
     except TypeError as e:
         raise exceptions.BadSchemaError(
             "Invalid match between numbers of keys and number of values in parametrize mark"
         ) from e
 
-    keys = [i["parametrize"]["key"] for i in parametrize_marks]
+    keys: list[str] = [i["parametrize"]["key"] for i in parametrize_marks]
 
     for vals_combination in combined:
         logger.debug("Generating test for %s/%s", keys, vals_combination)
 
         if len(vals_combination) != len(keys):
             raise exceptions.BadSchemaError(
                 "Invalid match between numbers of keys and number of values in parametrize mark"
@@ -346,15 +360,15 @@
 
         Yields:
             Pytest 'test objects'
         """
 
         try:
             # Convert to a list so we can catch parser exceptions
-            all_tests = list(
+            all_tests: Iterable[dict] = list(
                 yaml.load_all(
                     self.path.open(encoding="utf-8"),
                     Loader=IncludeLoader,  # type:ignore
                 )
             )
         except yaml.parser.ParserError as e:
             raise exceptions.BadSchemaError from e
```

### Comparing `tavern-3.0.0a3/tavern/_core/pytest/hooks.py` & `tavern-3.0.0a4/tavern/_core/pytest/hooks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import logging
 import logging.config
 import os
 import pathlib
 import re
+import typing
 from textwrap import dedent
+from typing import Optional
+
+if typing.TYPE_CHECKING:
+    from .file import YamlFile
+
 
 import pytest
 import yaml
 
 from tavern._core import exceptions
 
 from .util import add_ini_options, add_parser_options, get_option_generic
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
     add_parser_options(parser.addoption, with_defaults=False)
     add_ini_options(parser)
 
 
-def pytest_collect_file(parent, path: os.PathLike):
+def pytest_collect_file(parent, path: os.PathLike) -> Optional["YamlFile"]:
     """On collecting files, get any files that end in .tavern.yaml or .tavern.yml as tavern
     test files
     """
 
     if int(pytest.__version__.split(".", maxsplit=1)[0]) < 7:
         raise exceptions.TavernException("Only pytest >=7 is supported")
```

### Comparing `tavern-3.0.0a3/tavern/_core/pytest/item.py` & `tavern-3.0.0a4/tavern/_core/pytest/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 import logging
 import pathlib
 from collections.abc import Iterable, MutableMapping
 
 import pytest
 import yaml
-from _pytest._code.code import TerminalRepr
+from _pytest._code.code import ExceptionInfo, TerminalRepr
 from _pytest.nodes import Node
 from pytest import Mark, MarkDecorator
 
 from tavern._core import exceptions
 from tavern._core.loader import error_on_empty_scalar
 from tavern._core.plugins import load_plugins
 from tavern._core.pytest import call_hook
@@ -30,31 +30,32 @@
 
     At the time of writing this doesn't print the error very nicely, but it
     should be enough to track down what went wrong
 
     Attributes:
         path: filename that this test came from
         spec: The whole dictionary of the test
+        global_cfg: configuration for test
     """
 
     # See https://github.com/taverntesting/tavern/issues/825
     _patched_yaml = False
 
+    global_cfg: TestConfig
+
     def __init__(
         self, *, name: str, parent, spec: MutableMapping, path: pathlib.Path, **kwargs
     ) -> None:
         if "grpc" in spec:
             logger.warning("Tavern grpc support is in an experimental stage")
 
         super().__init__(name, parent, **kwargs)
         self.path = path
         self.spec = spec
 
-        self.global_cfg: TestConfig | None = None
-
         if not YamlItem._patched_yaml:
             yaml.parser.Parser.process_empty_scalar = (  # type:ignore
                 error_on_empty_scalar
             )
 
             YamlItem._patched_yaml = True
 
@@ -257,16 +258,16 @@
                 self.global_cfg,
                 "pytest_tavern_beta_after_every_test_run",
                 test_dict=self.spec,
                 variables=self.global_cfg.variables,
             )
 
     def repr_failure(
-        self, excinfo: pytest.ExceptionInfo[BaseException], style: str | None = None
-    ) -> TerminalRepr | str:
+        self, excinfo: ExceptionInfo[BaseException], style: str | None = None
+    ) -> TerminalRepr | str | ReprdError:
         """called when self.runtest() raises an exception.
 
         By default, will raise a custom formatted traceback if it's a tavern error. if not, will use the default
         python traceback
         """
 
         if (
```

### Comparing `tavern-3.0.0a3/tavern/_core/pytest/newhooks.py` & `tavern-3.0.0a4/tavern/_core/pytest/newhooks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 import logging
+from collections.abc import MutableMapping
+from typing import Any
+
+from tavern._core.pytest.config import TestConfig
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def pytest_tavern_beta_before_every_test_run(test_dict, variables) -> None:
+def pytest_tavern_beta_before_every_test_run(test_dict: dict, variables: dict) -> None:
     """Called:
 
     - directly after fixtures are loaded for a test
     - directly before verifying the schema of the file
     - Before formatting is done on values
     - After global configuration has been loaded
     - After plugins have been loaded
 
     Modify the test in-place if you want to do something to it.
 
     Args:
-        test_dict (dict): Test to run
-        variables (dict): Available variables
+        test_dict: Test to run
+        variables: Available variables
     """
 
 
-def pytest_tavern_beta_after_every_test_run(test_dict, variables) -> None:
+def pytest_tavern_beta_after_every_test_run(test_dict: dict, variables: dict) -> None:
     """Called:
 
     - After test run
 
     Args:
-        test_dict (dict): Test to run
-        variables (dict): Available variables
+        test_dict: Test to run
+        variables: Available variables
     """
 
 
-def pytest_tavern_beta_after_every_response(expected, response) -> None:
+def pytest_tavern_beta_after_every_response(expected: Any, response: Any) -> None:
     """Called after every _response_ - including MQTT/HTTP/etc
 
     Note:
         - The response object type and the expected dict depends on what plugin you're using, and which kind of response it is!
         - MQTT responses will call this hook multiple times if multiple messages are received
 
     Args:
-        response (object): Response object.
-        expected (dict): Response block in stage
+        expected: Response block in stage
+        response: Response object.
     """
 
 
-def pytest_tavern_beta_before_every_request(request_args) -> None:
+def pytest_tavern_beta_before_every_request(request_args: MutableMapping) -> None:
     """Called just before every request - including MQTT/HTTP/etc
 
     Note:
         - The request object type depends on what plugin you're using, and which kind of request it is!
 
     Args:
-        request_args (dict): Arguments passed to the request function. By default, this is Session.request for
+        request_args: Arguments passed to the request function. By default, this is Session.request for
             HTTP and Client.publish for MQTT
     """
 
 
-def call_hook(test_block_config, hookname, **kwargs) -> None:
+def call_hook(test_block_config: TestConfig, hookname: str, **kwargs) -> None:
     """Utility to call the hooks"""
     try:
         hook = getattr(test_block_config.tavern_internal.pytest_hook_caller, hookname)
     except AttributeError:
         logger.critical("Error getting tavern hook!")
         raise
```

### Comparing `tavern-3.0.0a3/tavern/_core/pytest/util.py` & `tavern-3.0.0a4/tavern/_core/pytest/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from functools import lru_cache
-from typing import Any
+from pathlib import Path
+from typing import Any, Optional, TypeVar, Union
 
 import pytest
 
 from tavern._core.dict_util import format_keys, get_tavern_box
 from tavern._core.general import load_global_config
 from tavern._core.pytest.config import TavernInternalConfig, TestConfig
 from tavern._core.strict_util import StrictLevel
@@ -147,19 +148,19 @@
     ini_global_cfg_paths = pytest_config.getini("tavern-global-cfg") or []
     # THEN load command line, to allow overwriting of values
     cmdline_global_cfg_paths = pytest_config.getoption("tavern_global_cfg") or []
 
     all_paths = ini_global_cfg_paths + cmdline_global_cfg_paths
     global_cfg_dict = load_global_config(all_paths)
 
+    variables: dict = {}
     try:
         loaded_variables = global_cfg_dict["variables"]
     except KeyError:
         logger.debug("Nothing to format in global config files")
-        variables = {}
     else:
         tavern_box = get_tavern_box()
         variables = format_keys(loaded_variables, tavern_box)
 
     global_cfg = TestConfig(
         variables=variables,
         strict=_load_global_strictness(pytest_config),
@@ -172,38 +173,41 @@
     )
 
     return global_cfg
 
 
 def _load_global_backends(pytest_config: pytest.Config) -> dict[str, Any]:
     """Load which backend should be used"""
-    backend_settings = {}
-
-    for b in TestConfig.backends():
-        backend_settings[b] = get_option_generic(
-            pytest_config, f"tavern-{b}-backend", None
-        )
-
-    return backend_settings
+    return {
+        b: get_option_generic(pytest_config, f"tavern-{b}-backend", None)
+        for b in TestConfig.backends()
+    }
 
 
 def _load_global_strictness(pytest_config: pytest.Config) -> StrictLevel:
     """Load the global 'strictness' setting"""
 
-    options = get_option_generic(pytest_config, "tavern-strict", [])
+    options: list = get_option_generic(pytest_config, "tavern-strict", [])
 
     return StrictLevel.from_options(options)
 
 
-def _load_global_follow_redirects(pytest_config: pytest.Config):
+def _load_global_follow_redirects(pytest_config: pytest.Config) -> bool:
     """Load the global 'follow redirects' setting"""
     return get_option_generic(pytest_config, "tavern-always-follow-redirects", False)
 
 
-def get_option_generic(pytest_config: pytest.Config, flag: str, default):
+T = TypeVar("T", bound=Optional[Union[str, list, list[Path], list[str], bool]])
+
+
+def get_option_generic(
+    pytest_config: pytest.Config,
+    flag: str,
+    default: T,
+) -> T:
     """Get a configuration option or return the default
 
     Priority order is cmdline, then ini, then default"""
     cli_flag = flag.replace("-", "_")
     ini_flag = flag
 
     # Lowest priority
```

### Comparing `tavern-3.0.0a3/tavern/_core/report.py` & `tavern-3.0.0a4/tavern/_core/report.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,46 +23,46 @@
 
 from tavern._core.formatted_str import FormattedString
 from tavern._core.stage_lines import get_stage_lines, read_relevant_lines
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def prepare_yaml(val):
+def prepare_yaml(val: dict | set | list | tuple | str) -> dict | list | str:
     """Sanitises the formatted string into a format safe for dumping"""
-    formatted = val
-
     if isinstance(val, dict):
-        formatted = {}
+        prepared = {}
         # formatted = {key: format_keys(val[key], box_vars) for key in val}
         for key in val:
             if isinstance(key, FormattedString):
                 key = str(key)
-            formatted[key] = prepare_yaml(val[key])
+            prepared[key] = prepare_yaml(val[key])
+
+        return prepared
     elif isinstance(val, (list, tuple, set)):
-        formatted = [prepare_yaml(item) for item in val]
-    elif isinstance(formatted, FormattedString):
-        return str(formatted)
+        return [prepare_yaml(item) for item in val]
+    elif isinstance(val, FormattedString):
+        return str(val)
 
-    return formatted
+    return val
 
 
-def attach_stage_content(stage) -> None:
+def attach_stage_content(stage: dict) -> None:
     first_line, last_line, _ = get_stage_lines(stage)
 
     code_lines = list(read_relevant_lines(stage, first_line, last_line))
     joined = dedent("\n".join(code_lines))
     attach_text(joined, "stage_yaml", yaml_type)
 
 
-def attach_yaml(payload, name) -> None:
+def attach_yaml(payload, name: str) -> None:
     prepared = prepare_yaml(payload)
     dumped = yaml.safe_dump(prepared)
     return attach_text(dumped, name, yaml_type)
 
 
-def attach_text(payload, name, attachment_type=None) -> None:
+def attach_text(payload, name: str, attachment_type=None) -> None:
     return attach(payload, name=name, attachment_type=attachment_type)
 
 
-def wrap_step(allure_name, partial):
+def wrap_step(allure_name: str, partial):
     return step(allure_name)(partial)
```

### Comparing `tavern-3.0.0a3/tavern/_core/run.py` & `tavern-3.0.0a4/tavern/_core/run.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,18 +63,18 @@
     available_stages: list[dict],
 ) -> list[dict]:
     """
     Get any stages which were included via config files which will be available
     for use in this test
 
     Args:
-        available_stages: List of stages which already exist
         tavern_box: Available parameters for fomatting at this point
         test_block_config: Current test config dictionary
         test_spec: Specification for current test
+        available_stages: List of stages which already exist
 
     Returns:
         Fully resolved stages
     """
 
     def stage_ids(s):
         return [i["id"] for i in s]
```

### Comparing `tavern-3.0.0a3/tavern/_core/schema/extensions.py` & `tavern-3.0.0a4/tavern/_core/schema/extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 import os
 import re
-from typing import TYPE_CHECKING
+from collections.abc import Callable, Mapping
+from typing import (
+    TYPE_CHECKING,
+    Any,
+)
 
 from pykwalify.types import is_bool, is_float, is_int
 
 from tavern._core import exceptions
 from tavern._core.exceptions import BadSchemaError
 from tavern._core.extfunctions import (
     get_pykwalify_logger,
     import_ext_function,
     is_ext_function,
 )
 from tavern._core.general import valid_http_methods
-from tavern._core.loader import ApproxScalar, BoolToken, FloatToken, IntToken
+from tavern._core.loader import (
+    ApproxScalar,
+    BoolToken,
+    FloatToken,
+    IntToken,
+    TypeConvertToken,
+)
 from tavern._core.strict_util import StrictLevel
 
 if TYPE_CHECKING:
     from tavern._plugins.grpc.response import GRPCCode
 
 
 # To extend pykwalify's type validation, extend its internal functions
 # These return boolean values
-def validate_type_and_token(validate_type, token):
+def validate_type_and_token(
+    validate_type: Callable[[Any], bool], token: type[TypeConvertToken]
+):
     def validate(value):
         return validate_type(value) or isinstance(value, token)
 
     return validate
 
 
 is_int_like = validate_type_and_token(is_int, IntToken)
 is_float_like = validate_type_and_token(is_float, FloatToken)
 is_bool_like = validate_type_and_token(is_bool, BoolToken)
 
 
 # These plug into the pykwalify extension function API
-def validator_like(validate, description):
+def validator_like(validate: Callable[[Any], bool], description: str):
     def validator(value, rule_obj, path):
         if validate(value):
             return True
         else:
             err_msg = "expected '{}' type at '{}', got '{}'".format(
                 description, path, value
             )
@@ -48,15 +60,15 @@
 
 
 int_variable = validator_like(is_int_like, "int-like")
 float_variable = validator_like(is_float_like, "float-like")
 bool_variable = validator_like(is_bool_like, "bool-like")
 
 
-def _validate_one_extension(input_value) -> None:
+def _validate_one_extension(input_value: Mapping) -> None:
     expected_keys = {"function", "extra_args", "extra_kwargs"}
     extra = set(input_value) - expected_keys
 
     if extra:
         raise BadSchemaError(f"Unexpected keys passed to $ext: {extra}")
 
     if "function" not in input_value:
@@ -101,30 +113,30 @@
             _validate_one_extension(vf)
     elif isinstance(value, dict):
         _validate_one_extension(value)
 
     return True
 
 
-def validate_status_code_is_int_or_list_of_ints(value, rule_obj, path) -> bool:
+def validate_status_code_is_int_or_list_of_ints(value: Mapping, rule_obj, path) -> bool:
     err_msg = "status_code has to be an integer or a list of integers (got {})".format(
         value
     )
 
     if not isinstance(value, list) and not is_int_like(value):
         raise BadSchemaError(err_msg)
 
     if isinstance(value, list):
         if not all(is_int_like(i) for i in value):
             raise BadSchemaError(err_msg)
 
     return True
 
 
-def check_usefixtures(value, rule_obj, path) -> bool:
+def check_usefixtures(value: Mapping, rule_obj, path) -> bool:
     err_msg = "'usefixtures' has to be a list with at least one item"
 
     if not isinstance(value, (list, tuple)):
         raise BadSchemaError(err_msg)
 
     if not value:
         raise BadSchemaError(err_msg)
@@ -167,19 +179,18 @@
         for status in StatusCode:
             if status.value[0] == value:
                 return status.name
 
     return None
 
 
-def verify_oneof_id_name(value, rule_obj, path) -> bool:
+def verify_oneof_id_name(value: Mapping, rule_obj, path) -> bool:
     """Checks that if 'name' is not present, 'id' is"""
 
-    name = value.get("name")
-    if not name:
+    if not (name := value.get("name")):
         if name == "":
             raise BadSchemaError("Name cannot be empty")
 
         if not value.get("id"):
             raise BadSchemaError("If 'name' is not specified, 'id' must be specified")
 
     return True
@@ -242,15 +253,15 @@
 
     else:
         raise BadSchemaError("'key' must be a string or a list")
 
     return True
 
 
-def validate_data_key(value, rule_obj, path) -> bool:
+def validate_data_key(value, rule_obj, path: str) -> bool:
     """Validate the 'data' key in a http request
 
     From requests docs:
 
     > data - (optional) Dictionary or list of tuples [(key, value)] (will be
     > form-encoded), bytes, or file-like object to send in the body of the
     > Request.
@@ -322,15 +333,15 @@
             validate_extensions(maybe_ext_val, rule_obj, path)
         elif maybe_ext_val is not None:
             raise BadSchemaError(f"Unexpected $ext key in block at {path}")
 
     return True
 
 
-def check_strict_key(value, rule_obj, path) -> bool:
+def check_strict_key(value: list | bool, rule_obj, path) -> bool:
     """Make sure the 'strict' key is either a bool or a list"""
 
     if not isinstance(value, list) and not is_bool_like(value):
         raise BadSchemaError("'strict' has to be either a boolean or a list")
     elif isinstance(value, list):
         try:
             # Reuse validation here
@@ -339,15 +350,15 @@
             raise BadSchemaError from e
 
     # Might be a bool as well, in which case it's processed further down the line - no validation required
 
     return True
 
 
-def validate_timeout_tuple_or_float(value, rule_obj, path) -> bool:
+def validate_timeout_tuple_or_float(value: list | tuple, rule_obj, path) -> bool:
     """Make sure timeout is a float/int or a tuple of floats/ints"""
 
     err_msg = "'timeout' must be either a float/int or a 2-tuple of floats/ints - got '{}' (type {})".format(
         value, type(value)
     )
     logger = get_pykwalify_logger("tavern.schemas.extensions")
 
@@ -394,15 +405,15 @@
             raise BadSchemaError(err_msg)
         elif not all(isinstance(i, str) for i in value):
             raise BadSchemaError(err_msg)
 
     return True
 
 
-def validate_file_spec(value, rule_obj, path) -> bool:
+def validate_file_spec(value: dict, rule_obj, path) -> bool:
     """Validate file upload arguments"""
 
     logger = get_pykwalify_logger("tavern.schema.extensions")
 
     if not isinstance(value, dict):
         raise BadSchemaError(
             "File specification must be a mapping of file names to file specs, got {}".format(
```

### Comparing `tavern-3.0.0a3/tavern/_core/schema/files.py` & `tavern-3.0.0a4/tavern/_core/schema/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         """Load the schema file and cache it for future use
 
         Args:
             schema_filename (str): filename of schema
             with_plugins (bool): Whether to load plugin schema into this schema as well
 
         Returns:
-            dict: loaded schema
+            loaded schema
         """
 
         if with_plugins:
             schema = self._load_schema_with_plugins(schema_filename)
         else:
             schema = self._load_base_schema(schema_filename)
```

### Comparing `tavern-3.0.0a3/tavern/_core/schema/jsonschema.py` & `tavern-3.0.0a4/tavern/_core/schema/jsonschema.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_core/schema/tests.jsonschema.yaml` & `tavern-3.0.0a4/tavern/_core/schema/tests.jsonschema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_core/schema/tests.schema.yaml` & `tavern-3.0.0a4/tavern/_core/schema/tests.schema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_core/strict_util.py` & `tavern-3.0.0a4/tavern/_core/strict_util.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_core/testhelpers.py` & `tavern-3.0.0a4/tavern/_core/testhelpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import time
-from collections.abc import Mapping
+from collections.abc import Callable, Mapping
 from functools import wraps
 
 from tavern._core import exceptions
 from tavern._core.dict_util import format_keys
 from tavern._core.pytest.config import TestConfig
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -24,26 +24,24 @@
     except KeyError:
         pass
     else:
         logger.debug("Delaying %s request for %.2f seconds", when, length)
         time.sleep(length)
 
 
-def retry(stage: Mapping, test_block_config: TestConfig):
+def retry(stage: Mapping, test_block_config: TestConfig) -> Callable:
     """Look for retry and try to repeat the stage `retry` times.
 
     Args:
         stage: test stage
         test_block_config: Configuration for current test
     """
 
-    if "max_retries" in stage:
-        max_retries = maybe_format_max_retries(
-            stage.get("max_retries"), test_block_config
-        )
+    if r := stage.get("max_retries", None):
+        max_retries = maybe_format_max_retries(r, test_block_config)
     else:
         max_retries = 0
 
     if max_retries == 0:
 
         def catch_wrapper(fn):
             @wraps(fn)
@@ -97,19 +95,21 @@
                 return res
 
             return wrapped
 
         return retry_wrapper
 
 
-def maybe_format_max_retries(max_retries, test_block_config: TestConfig) -> int:
+def maybe_format_max_retries(
+    max_retries: str | int, test_block_config: TestConfig
+) -> int:
     """Possibly handle max_retries validation"""
 
     # Probably a format variable, or just invalid (in which case it will fail further down)
-    max_retries = format_keys(max_retries, test_block_config.variables)
+    max_retries = int(format_keys(max_retries, test_block_config.variables))  # type:ignore
 
     # Missing type token will mean that max_retries is still a string and will fail here
     # Could auto convert here as well, but keep it consistent and just fail
     if not isinstance(max_retries, int):
         raise exceptions.InvalidRetryException(
             f"Invalid type for max_retries - was {type(max_retries)}"
         )
```

### Comparing `tavern-3.0.0a3/tavern/_core/tincture.py` & `tavern-3.0.0a4/tavern/_core/tincture.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 import collections.abc
+import dataclasses
 import inspect
 import logging
+from collections.abc import Generator
 from typing import Any
 
 from tavern._core import exceptions
 from tavern._core.extfunctions import get_wrapped_response_function
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@dataclasses.dataclass
 class Tinctures:
-    def __init__(self, tinctures: list[Any]) -> None:
-        self._tinctures = tinctures
-        self._needs_response: list[Any] = []
+    tinctures: list[Any]
+    needs_response: list[Generator] = dataclasses.field(default_factory=list)
 
     def start_tinctures(self, stage: collections.abc.Mapping) -> None:
-        results = [t(stage) for t in self._tinctures]
-        self._needs_response = []
+        results = [t(stage) for t in self.tinctures]
 
         for r in results:
             if inspect.isgenerator(r):
                 # Store generator and start it
-                self._needs_response.append(r)
+                self.needs_response.append(r)
                 next(r)
 
     def end_tinctures(self, expected: collections.abc.Mapping, response) -> None:
         """
         Send the response object to any tinctures that want it
 
         Args:
-            response: The response from 'run' for the stage
+            expected: 'expected' from initial test - type varies depending on backend
+            response: The response from 'run' for the stage - type varies depending on backend
         """
-        if self._needs_response is None:
+        if self.needs_response is None:
             raise RuntimeError(
                 "should not be called before accumulating tinctures which need a response"
             )
 
-        for n in self._needs_response:
+        for n in self.needs_response:
             try:
                 n.send((expected, response))
             except StopIteration:
                 pass
             else:
                 raise RuntimeError("Tincture had more than one yield")
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/grpc/__init__.py` & `tavern-3.0.0a4/tavern/_plugins/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_plugins/grpc/client.py` & `tavern-3.0.0a4/tavern/_plugins/grpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,16 +233,17 @@
                     exc_info=True,
                 )
 
             raise exceptions.GRPCRequestException from rpc_error
 
         return self._get_grpc_service(channel, service, method)
 
-    def __enter__(self) -> None:
+    def __enter__(self) -> "GRPCClient":
         logger.debug("Connecting to GRPC")
+        return self
 
     def call(
         self,
         service: str,
         host: str | None = None,
         body: Mapping | None = None,
         timeout: int | None = None,
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/grpc/jsonschema.yaml` & `tavern-3.0.0a4/tavern/_plugins/grpc/jsonschema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_plugins/grpc/protos.py` & `tavern-3.0.0a4/tavern/_plugins/grpc/protos.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_plugins/grpc/request.py` & `tavern-3.0.0a4/tavern/_plugins/grpc/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import dataclasses
 import functools
 import json
 import logging
-from collections.abc import Mapping
 
 import grpc
 from box import Box
 
 from tavern._core import exceptions
 from tavern._core.dict_util import check_expected_keys, format_keys
 from tavern._core.pytest.config import TestConfig
 from tavern._plugins.grpc.client import GRPCClient
 from tavern.request import BaseRequest
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def get_grpc_args(rspec, test_block_config):
+def get_grpc_args(rspec: dict, test_block_config: TestConfig) -> dict:
     """Format GRPC request args"""
 
     fspec = format_keys(rspec, test_block_config.variables)
 
     # FIXME: Clarify 'json' and 'body' for grpc requests
     # FIXME 2: also it should allow proto text format. Maybe binary.
     if "json" in rspec:
@@ -43,15 +42,15 @@
 class GRPCRequest(BaseRequest):
     """Wrapper for a single GRPC request on a client
 
     Similar to RestRequest, publishes a single message.
     """
 
     def __init__(
-        self, client: GRPCClient, request_spec: Mapping, test_block_config: TestConfig
+        self, client: GRPCClient, request_spec: dict, test_block_config: TestConfig
     ) -> None:
         expected = {"host", "service", "body"}
 
         check_expected_keys(expected, request_spec)
 
         grpc_args = get_grpc_args(request_spec, test_block_config)
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/grpc/response.py` & `tavern-3.0.0a4/tavern/_plugins/grpc/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     def verify(self, response: "WrappedFuture") -> Mapping:
         grpc_response = response.response
 
         logger.debug(f"grpc status code: {grpc_response.code()}")
         logger.debug(f"grpc details: {grpc_response.details()}")
 
         # Get any keys to save
-        saved = {}
+        saved: dict[str, Any] = {}
         verify_status = [StatusCode.OK.name]
         if status := self.expected.get("status", None):
             verify_status = _to_grpc_name(status)  # type: ignore
             if not isinstance(verify_status, list):
                 verify_status = [verify_status]
 
         if grpc_response.code().name not in verify_status:
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/grpc/schema.yaml` & `tavern-3.0.0a4/tavern/_plugins/grpc/schema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_plugins/grpc/tavernhook.py` & `tavern-3.0.0a4/tavern/_plugins/grpc/tavernhook.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 session_type = GRPCClient
 
 request_type = GRPCRequest
 request_block_name = "grpc_request"
 
 
-def get_expected_from_request(response_block, test_block_config: TestConfig, session):
+def get_expected_from_request(
+    response_block, test_block_config: TestConfig, session: GRPCClient
+):
     f_expected = format_keys(response_block, test_block_config.variables)
     expected = f_expected
 
     return expected
 
 
 verifier_type = GRPCResponse
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/mqtt/client.py` & `tavern-3.0.0a4/tavern/_plugins/mqtt/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import dataclasses
 import logging
 import ssl
 import threading
 import time
 from collections.abc import Mapping, MutableMapping
 from queue import Empty, Full, Queue
+from typing import Any
 
 import paho.mqtt.client as paho
 from paho.mqtt.client import MQTTMessageInfo
 
 from tavern._core import exceptions
 from tavern._core.dict_util import check_expected_keys
 
@@ -286,15 +287,17 @@
         self._userdata = {
             "_subscription_mappings": self._subscription_mappings,
             "_subscribed": self._subscribed,
         }
         self._client.user_data_set(self._userdata)
 
     @staticmethod
-    def _on_message(client, userdata, message) -> None:
+    def _on_message(
+        client, userdata: Mapping[str, Any], message: paho.MQTTMessage
+    ) -> None:
         """Add any messages received to the queue
 
         Todo:
             If the queue is faull trigger an error in main thread somehow
         """
 
         logger.info("Received mqtt message on %s", message.topic)
@@ -344,24 +347,26 @@
     def _on_socket_open(client, userdata, socket) -> None:
         logger.debug("MQTT socket opened")
 
     @staticmethod
     def _on_socket_close(client, userdata, socket) -> None:
         logger.debug("MQTT socket closed")
 
-    def message_received(self, topic: str, timeout: int = 1):
+    def message_received(
+        self, topic: str, timeout: float | int = 1
+    ) -> paho.MQTTMessage | None:
         """Check that a message is in the message queue
 
         Args:
-            topic (str): topic to fetch message for
-            timeout (int): How long to wait before signalling that the message
+            topic: topic to fetch message for
+            timeout: How long to wait before signalling that the message
                 was not received.
 
         Returns:
-            paho.MQTTMessage: whether the message was received within the timeout
+            the message, if one was received, otherwise None
 
         Todo:
             Allow regexes for topic names? Better validation for mqtt payloads
         """
 
         try:
             with self._subscribe_lock:
@@ -377,30 +382,37 @@
 
         return msg
 
     def publish(
         self,
         topic: str,
         payload: None | bytearray | bytes | float | str = None,
-        qos=None,
-        retain=None,
+        qos: int | None = None,
+        retain: bool | None = None,
     ) -> MQTTMessageInfo:
         """publish message using paho library"""
         self._wait_for_subscriptions()
 
         logger.debug("Publishing on '%s'", topic)
 
         kwargs = {}
         if qos is not None:
             kwargs["qos"] = qos
         if retain is not None:
             kwargs["retain"] = retain
         msg = self._client.publish(topic, payload, **kwargs)
 
-        if not msg.is_published:
+        # Wait for 2*connect timeout which should be plenty to publish the message even with qos 2
+        # TODO: configurable
+        try:
+            msg.wait_for_publish(self._connect_timeout * 2)
+        except (RuntimeError, ValueError) as e:
+            raise exceptions.MQTTError("could not publish message") from e
+
+        if not msg.is_published():
             raise exceptions.MQTTError(
                 "err {:s}: {:s}".format(
                     _err_vals.get(msg.rc, "unknown"), paho.error_string(msg.rc)
                 )
             )
 
         return msg
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/mqtt/jsonschema.yaml` & `tavern-3.0.0a4/tavern/_plugins/mqtt/jsonschema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_plugins/mqtt/request.py` & `tavern-3.0.0a4/tavern/_plugins/mqtt/request.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_plugins/mqtt/response.py` & `tavern-3.0.0a4/tavern/_plugins/mqtt/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,59 +12,65 @@
 
 from tavern._core import exceptions
 from tavern._core.dict_util import check_keys_match_recursive
 from tavern._core.loader import ANYTHING
 from tavern._core.pytest.config import TestConfig
 from tavern._core.pytest.newhooks import call_hook
 from tavern._core.report import attach_yaml
-from tavern._core.strict_util import StrictSetting
+from tavern._core.strict_util import StrictOption
 from tavern.response import BaseResponse
 
 from .client import MQTTClient
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 _default_timeout = 1
 
 
 class MQTTResponse(BaseResponse):
+    response: MQTTMessage
+
     def __init__(
-        self, client: MQTTClient, name: str, expected, test_block_config: TestConfig
+        self,
+        client: MQTTClient,
+        name: str,
+        expected: TestConfig,
+        test_block_config: TestConfig,
     ) -> None:
         super().__init__(name, expected, test_block_config)
 
         self._client = client
 
-        self.received_messages = []  # type: ignore
+        self.received_messages: list = []
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.response:
-            return self.response.payload
+            return self.response.payload.decode("utf-8")
         else:
             return "<Not run yet>"
 
-    def verify(self, response) -> dict:
+    def verify(self, response: MQTTMessage) -> Mapping:
         """Ensure mqtt message has arrived
 
         Args:
             response: not used except for debug printing
         """
 
         self.response = response
 
         try:
             return self._await_response()
         finally:
             self._client.unsubscribe_all()
 
-    def _await_response(self) -> dict:
+    def _await_response(self) -> Mapping:
         """Actually wait for response
 
         Returns:
-            dict: things to save to variables for the rest of this test
+            things to save to variables for the rest of this test
         """
 
         # Get into class with metadata attached
         expected = self.expected["mqtt_responses"]
 
         by_topic = {
             m: list(v) for m, v in itertools.groupby(expected, lambda x: x["topic"])
@@ -101,15 +107,15 @@
                 self._adderr("\n".join(warnings))
 
             raise exceptions.TestFailError(
                 f"Test '{self.name:s}' failed:\n{self._str_errors():s}",
                 failures=self.errors,
             )
 
-        saved = {}
+        saved: dict = {}
 
         for msg in correct_messages:
             # Check saving things from the payload and from json
             saved.update(
                 self.maybe_get_save_values_from_save_block(
                     "payload",
                     msg.msg.payload,
@@ -144,15 +150,15 @@
         Waits for the specific message
 
         Args:
             topic: topic to listen on
             expected: expected response for this block
 
         Returns:
-            tuple(msg, list): The correct message (if any) and warnings from processing the message
+            The correct message (if any) and warnings from processing the message
         """
 
         timeout = max(m.get("timeout", _default_timeout) for m in expected)
 
         # A list of verifiers that can be used to validate messages for this topic
         verifiers = [_MessageVerifier(self.test_block_config, v) for v in expected]
 
@@ -227,29 +233,29 @@
         return correct_messages, warnings
 
 
 @dataclass
 class _ReturnedMessage:
     """An actual message returned from the API and it's matching 'expected' block."""
 
-    expected: dict
+    expected: Mapping
     msg: MQTTMessage
 
 
 class _MessageVerifier:
-    def __init__(self, test_block_config, expected) -> None:
+    def __init__(self, test_block_config: TestConfig, expected: Mapping) -> None:
         self.expires = time.time() + expected.get("timeout", _default_timeout)
 
         self.expected = expected
         self.expected_payload, self.expect_json_payload = self._get_payload_vals(
             expected
         )
 
         test_strictness = test_block_config.strict
-        self.block_strictness: StrictSetting = test_strictness.option_for("json")
+        self.block_strictness: StrictOption = test_strictness.option_for("json")
 
         # Any warnings to do with the request
         # eg, if a message was received but it didn't match, message had payload, etc.
         self.warnings: list[str] = []
 
     def is_valid(self, msg: MQTTMessage) -> bool:
         if time.time() > self.expires:
@@ -321,15 +327,15 @@
         return False
 
     @staticmethod
     def _get_payload_vals(expected: Mapping) -> tuple[str | dict | None, bool]:
         """Gets the payload from the 'expected' block
 
         Returns:
-            tuple: First element is the expected payload, second element is whether it's
+            First element is the expected payload, second element is whether it's
                 expected to be json or not
         """
         # TODO move this check to initialisation/schema checking
         if "json" in expected:
             if "payload" in expected:
                 raise exceptions.BadSchemaError(
                     "Can only specify one of 'payload' or 'json' in MQTT response"
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/mqtt/schema.yaml` & `tavern-3.0.0a4/tavern/_plugins/mqtt/schema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_plugins/mqtt/tavernhook.py` & `tavern-3.0.0a4/tavern/_plugins/mqtt/tavernhook.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from collections.abc import Iterable
 from os.path import abspath, dirname, join
 
 import yaml
 
 from tavern._core.dict_util import format_keys
 from tavern._core.pytest.config import TestConfig
 
@@ -15,16 +16,18 @@
 session_type = MQTTClient
 
 request_type = MQTTRequest
 request_block_name = "mqtt_publish"
 
 
 def get_expected_from_request(
-    response_block, test_block_config: TestConfig, session: MQTTClient
-):
+    response_block: dict | Iterable[dict],
+    test_block_config: TestConfig,
+    session: MQTTClient,
+) -> dict | None:
     expected: dict | None = None
 
     # mqtt response is not required
     if response_block:
         expected = {"mqtt_responses": []}
         if isinstance(response_block, dict):
             response_block = [response_block]
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/rest/files.py` & `tavern-3.0.0a4/tavern/_plugins/rest/files.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/_plugins/rest/request.py` & `tavern-3.0.0a4/tavern/_plugins/rest/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import contextlib
 import json
 import logging
 import warnings
-from collections.abc import Mapping, MutableMapping
+from collections.abc import Callable, Mapping
 from contextlib import ExitStack
 from itertools import filterfalse, tee
-from typing import ClassVar
+from typing import (
+    ClassVar,
+)
 from urllib.parse import quote_plus
 
 import requests
 from box.box import Box
 from requests.cookies import cookiejar_from_dict
 from requests.utils import dict_from_cookiejar
 
@@ -21,15 +23,15 @@
 from tavern._core.report import attach_yaml
 from tavern._plugins.rest.files import get_file_arguments, guess_filespec
 from tavern.request import BaseRequest
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-def get_request_args(rspec: MutableMapping, test_block_config: TestConfig) -> dict:
+def get_request_args(rspec: dict, test_block_config: TestConfig) -> dict:
     """Format the test spec given values inthe global config
 
     Todo:
         Add similar functionality to validate/save $ext functions so input
         can be generated from a function
 
     Args:
@@ -232,15 +234,15 @@
     Check for allow_redirects flag in settings/stage
 
     Args:
         rspec: request dictionary
         test_block_config: config available for test
 
     Returns:
-        bool: Whether to allow redirects for this stage or not
+        Whether to allow redirects for this stage or not
     """
     # By default, don't follow redirects
     allow_redirects = False
 
     # Then check to see if we should follow redirects based on settings
     global_follow_redirects = test_block_config.follow_redirects
     if global_follow_redirects is not None:
@@ -352,15 +354,15 @@
         self, session: requests.Session, rspec: dict, test_block_config: TestConfig
     ) -> None:
         """Prepare request
 
         Args:
             session: existing session
             rspec: test spec
-            test_block_config   : Any configuration for this the block of
+            test_block_config: Any configuration for this the block of
                 tests
 
         Raises:
             UnexpectedKeysError: If some unexpected keys were used in the test
                 spec. Only valid keyword args to requests can be passed
         """
 
@@ -391,15 +393,15 @@
         request_args = get_request_args(rspec, test_block_config)
         update_from_ext(
             request_args,
             RestRequest.optional_in_file + ["url"],
         )
 
         # Used further down, but pop it asap to avoid unwanted side effects
-        file_body = request_args.pop("file_body", None)
+        file_body: str | None = request_args.pop("file_body", None)
 
         # If there was a 'cookies' key, set it in the request
         expected_cookies = _read_expected_cookies(session, rspec, test_block_config)
         if expected_cookies is not None:
             logger.debug("Sending cookies %s in request", expected_cookies.keys())
             request_args.update(cookies=expected_cookies)
 
@@ -436,24 +438,21 @@
 
                 headers = self._request_args.get("headers", {})
                 for k, v in headers.items():
                     headers[str(k)] = str(v)
 
                 return session.request(**self._request_args)
 
-        self._prepared = prepared_request
+        self._prepared: Callable[[], requests.Response] = prepared_request
 
-    def run(self):
+    def run(self) -> requests.Response:
         """Runs the prepared request and times it
 
-        Todo:
-            time it
-
         Returns:
-            requests.Response: response object
+            response object
         """
 
         attach_yaml(
             self._request_args,
             name="rest_request",
         )
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/rest/response.py` & `tavern-3.0.0a4/tavern/_plugins/rest/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import contextlib
 import json
 import logging
 from collections.abc import Mapping
+from typing import (
+    Any,
+)
 from urllib.parse import parse_qs, urlparse
 
 import requests
 from requests.status_codes import _codes  # type:ignore
 
 from tavern._core import exceptions
 from tavern._core.dict_util import deep_dict_merge
@@ -14,23 +17,23 @@
 from tavern._core.report import attach_yaml
 from tavern.response import BaseResponse, indent_err_text
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class RestResponse(BaseResponse):
+    response: requests.Response
+
     def __init__(
         self, session, name: str, expected, test_block_config: TestConfig
     ) -> None:
         defaults = {"status_code": 200}
 
         super().__init__(name, deep_dict_merge(defaults, expected), test_block_config)
 
-        self.status_code: int | None = None
-
         def check_code(code: int) -> None:
             if int(code) not in _codes:
                 logger.warning("Unexpected status code '%s'", code)
 
         in_file = self.expected["status_code"]
         try:
             if isinstance(in_file, list):
@@ -43,15 +46,15 @@
 
     def __str__(self) -> str:
         if self.response:
             return self.response.text.strip()
         else:
             return "<Not run yet>"
 
-    def _verbose_log_response(self, response) -> None:
+    def _verbose_log_response(self, response: requests.Response) -> None:
         """Verbosely log the response object, with query params etc."""
 
         logger.info("Response: '%s'", response)
 
         def log_dict_block(block, name):
             if block:
                 to_log = name + ":"
@@ -74,15 +77,15 @@
         redirect_query_params = self._get_redirect_query_params(response)
         if redirect_query_params:
             parsed_url = urlparse(response.headers["location"])
             to_path = "{}://{}{}".format(*parsed_url)
             logger.debug("Redirect location: %s", to_path)
             log_dict_block(redirect_query_params, "Redirect URL query parameters")
 
-    def _get_redirect_query_params(self, response) -> dict[str, str]:
+    def _get_redirect_query_params(self, response: requests.Response) -> dict[str, str]:
         """If there was a redirect header, get any query parameters from it"""
 
         try:
             redirect_url = response.headers["location"]
         except KeyError as e:
             if "redirect_query_params" in self.expected.get("save", {}):
                 self._adderr(
@@ -94,25 +97,25 @@
         else:
             parsed = urlparse(redirect_url)
             qp = parsed.query
             redirect_query_params = {i: j[0] for i, j in parse_qs(qp).items()}
 
         return redirect_query_params
 
-    def _check_status_code(self, status_code, body) -> None:
+    def _check_status_code(self, status_code: int | list[int], body: Any) -> None:
         expected_code = self.expected["status_code"]
 
         if (isinstance(expected_code, int) and status_code == expected_code) or (
             isinstance(expected_code, list) and (status_code in expected_code)
         ):
             logger.debug(
                 "Status code '%s' matched expected '%s'", status_code, expected_code
             )
             return
-        elif 400 <= status_code < 500:
+        elif isinstance(status_code, int) and 400 <= status_code < 500:
             # special case if there was a bad request. This assumes that the
             # response would contain some kind of information as to why this
             # request was rejected.
             self._adderr(
                 "Status code was %s, expected %s:\n%s",
                 status_code,
                 expected_code,
@@ -143,15 +146,14 @@
             self.test_block_config,
             "pytest_tavern_beta_after_every_response",
             expected=self.expected,
             response=response,
         )
 
         self.response = response
-        self.status_code = response.status_code
 
         # Get things to use from the response
         try:
             body = response.json()
         except ValueError:
             body = None
 
@@ -173,15 +175,15 @@
             },
             name="rest_response",
         )
 
         self._maybe_run_validate_functions(response)
 
         # Get any keys to save
-        saved = {}
+        saved: dict = {}
 
         saved.update(self.maybe_get_save_values_from_save_block("json", body))
         saved.update(
             self.maybe_get_save_values_from_save_block("headers", response.headers)
         )
         saved.update(
             self.maybe_get_save_values_from_save_block(
```

### Comparing `tavern-3.0.0a3/tavern/_plugins/rest/tavernhook.py` & `tavern-3.0.0a4/tavern/_plugins/rest/tavernhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import logging
 
 import requests
 
 from tavern._core import exceptions
 from tavern._core.dict_util import format_keys
 from tavern._core.plugins import PluginHelperBase
+from tavern._core.pytest.config import TestConfig
 
 from .request import RestRequest
 from .response import RestResponse
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class TavernRestPlugin(PluginHelperBase):
     session_type = requests.Session
 
     request_type = RestRequest
     request_block_name = "request"
 
     @staticmethod
-    def get_expected_from_request(response_block, test_block_config, session):
+    def get_expected_from_request(
+        response_block: dict, test_block_config: TestConfig, session
+    ):
         if response_block is None:
             raise exceptions.MissingSettingsError(
                 "no response block specified for HTTP test stage"
             )
 
         f_expected = format_keys(response_block, test_block_config.variables)
         return f_expected
```

### Comparing `tavern-3.0.0a3/tavern/core.py` & `tavern-3.0.0a4/tavern/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 
     Returns:
         path to global config file
 
     Raises:
         InvalidSettingsError: If global config was not of the right type or a given path
             does not exist
-
-    Todo:
-        Once python 2 is dropped, allow this to take a 'path like object'
     """
 
     if isinstance(tavern_global_cfg, str):
         if not os.path.exists(tavern_global_cfg):
             raise exceptions.InvalidSettingsError(
                 f"global config file '{tavern_global_cfg}' does not exist"
             )
```

### Comparing `tavern-3.0.0a3/tavern/entry.py` & `tavern-3.0.0a4/tavern/entry.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/helpers.py` & `tavern-3.0.0a4/tavern/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
 import json
 import logging
 import re
+from collections.abc import Iterable, Mapping
 
 import jmespath
 import jwt
 import requests
 from box.box import Box
 
 from tavern._core import exceptions
@@ -63,48 +64,50 @@
         assert response.status_code == int(exception.status.split()[0])  # noqa
     except AssertionError as e:
         raise exceptions.UnexpectedExceptionError(
             "exception status code did not match"
         ) from e
 
 
-def validate_jwt(response, jwt_key, **kwargs) -> dict[str, Box]:
+def validate_jwt(
+    response: requests.Response, jwt_key: str, **kwargs
+) -> Mapping[str, Box]:
     """Make sure a jwt is valid
 
     This uses the pyjwt library to decode the jwt, so any keyword args needed
     should be passed as per that library. You will probably want to use
     verify_signature=False unless using a HMAC key because it can be a bit
     verbose to pass in a public key.
 
     This also returns the jwt so it can be used both to verify and save jwts -
     it wraps this in a Box so it can also be used for future formatting
 
     Args:
-        response (Response): requests.Response object
-        jwt_key (str): key of jwt in body of request
+        response: requests.Response object
+        jwt_key: key of jwt in body of request
         **kwargs: Any extra arguments to pass to jwt.decode
 
     Returns:
-        dict: dictionary of jwt: boxed jwt claims
+        mapping of jwt: boxed jwt claims
     """
     token = response.json()[jwt_key]
 
     decoded = jwt.decode(token, **kwargs)
 
     logger.debug("Decoded jwt to %s", decoded)
 
     return {"jwt": Box(decoded)}
 
 
-def validate_pykwalify(response, schema) -> None:
+def validate_pykwalify(response: requests.Response, schema: dict) -> None:
     """Make sure the response matches a given schema
 
     Args:
-        response (Response): reqeusts.Response object
-        schema (dict): Schema for response
+        response: reqeusts Response object
+        schema: Schema for response
     """
     try:
         to_verify = response.json()
     except TypeError as e:
         raise exceptions.BadSchemaError(
             "Tried to match a pykwalify schema against a non-json response"
         ) from e
@@ -166,15 +169,15 @@
     match = re.search(expression, content)
     if match is None:
         raise exceptions.RegexAccessError("No match for regex")
 
     return {"regex": Box(match.groupdict())}
 
 
-def validate_content(response: requests.Response, comparisons: list[str]) -> None:
+def validate_content(response: requests.Response, comparisons: Iterable[dict]) -> None:
     """Asserts expected value with actual value using JMES path expression
 
     Args:
         response: reqeusts.Response object.
         comparisons:
             A list of dict containing the following keys:
                 1. jmespath : JMES path expression to extract data from.
```

### Comparing `tavern-3.0.0a3/tavern/request.py` & `tavern-3.0.0a4/tavern/request.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tavern/response.py` & `tavern-3.0.0a4/tavern/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import dataclasses
 import logging
 import traceback
 from abc import abstractmethod
 from collections.abc import Mapping
 from textwrap import indent
-from typing import Any
+from typing import (
+    Any,
+)
 
 from tavern._core import exceptions
 from tavern._core.dict_util import check_keys_match_recursive, recurse_access_key
 from tavern._core.extfunctions import get_wrapped_response_function
 from tavern._core.pytest.config import TestConfig
 from tavern._core.strict_util import StrictOption
 
@@ -16,35 +19,31 @@
 
 def indent_err_text(err: str) -> str:
     if err == "null":
         err = "<No body>"
     return indent(err, " " * 4)
 
 
+@dataclasses.dataclass
 class BaseResponse:
-    def __init__(self, name: str, expected, test_block_config: TestConfig) -> None:
-        # Stage name
-        self.name = name
+    name: str
+    expected: Any
+    test_block_config: TestConfig
+    response: Any | None = None
 
-        # all errors in this response
-        self.errors: list[str] = []
+    validate_functions: list[Any] = dataclasses.field(init=False, default_factory=list)
+    errors: list[str] = dataclasses.field(init=False, default_factory=list)
 
-        self.validate_functions: list = []
-        self._check_for_validate_functions(expected)
-
-        self.test_block_config = test_block_config
-
-        self.expected = expected
-
-        self.response: Any | None = None
+    def __post_init__(self) -> None:
+        self._check_for_validate_functions(self.expected)
 
     def _str_errors(self) -> str:
         return "- " + "\n- ".join(self.errors)
 
-    def _adderr(self, msg, *args, e=None) -> None:
+    def _adderr(self, msg: str, *args, e=None) -> None:
         if e:
             logger.exception(msg, *args)
         else:
             logger.error(msg, *args)
         self.errors += [(msg % args)]
 
     @abstractmethod
@@ -65,18 +64,18 @@
     ) -> None:
         """Valid returned data against expected data
 
         Todo:
             Optionally use a validation library too
 
         Args:
-            strict: strictness setting for this block
             expected_block: expected data
             block: actual data
             blockname: 'name' of this block (params, mqtt, etc) for error messages
+            strict: strictness setting for this block
         """
 
         if expected_block is None:
             logger.debug("No expected %s to check against", blockname)
             return
 
         # This should be done _before_ it gets to this point - typically in get_expected_from_request from plugin
@@ -147,22 +146,22 @@
                     raise exceptions.MisplacedExtBlockException(
                         name,
                     )
 
         # Could put in an isinstance check here
         check_deprecated_validate("json")
 
-    def _maybe_run_validate_functions(self, response) -> None:
+    def _maybe_run_validate_functions(self, response: Any) -> None:
         """Run validation functions if available
 
         Note:
              'response' will be different depending on where this is called from
 
         Args:
-            response (object): Response type. This could be whatever the response type/plugin uses.
+            response: Response type. This could be whatever the response type/plugin uses.
         """
         logger.debug(
             "Calling ext function from '%s' with response '%s'", type(self), response
         )
 
         for vf in self.validate_functions:
             try:
@@ -173,15 +172,15 @@
                     vf.func,
                     indent_err_text(traceback.format_exc()),
                     e=e,
                 )
 
     def maybe_get_save_values_from_ext(
         self, response: Any, read_save_from: Mapping
-    ) -> dict:
+    ) -> Mapping:
         """If there is an $ext function in the save block, call it and save the response
 
         Args:
             response: response object. Actual contents depends on which type of
                 response is being checked
             read_save_from: the expected response (incl
                 body/json/headers/mqtt topic/etc etc) containing a spec for which things
@@ -199,15 +198,15 @@
             return {}
 
         try:
             saved = wrapped(response)
         except Exception as e:
             self._adderr(
                 "Error calling save function '%s':\n%s",
-                wrapped.func,
+                wrapped.func,  # type:ignore
                 indent_err_text(traceback.format_exc()),
                 e=e,
             )
             return {}
 
         logger.debug("saved %s from ext function", saved)
 
@@ -223,20 +222,22 @@
 
     def maybe_get_save_values_from_save_block(
         self,
         key: str,
         save_from: Mapping | None,
         *,
         outer_save_block: Mapping | None = None,
-    ) -> dict:
+    ) -> Mapping:
         """Save a value from a specific block in the response.
 
         See docs for maybe_get_save_values_from_given_block for more info
 
-        Keyword Args:
+        Args:
+            key: Name of key being used to save, for debugging
+            save_from: An element of the response from which values are being saved
             outer_save_block: Read things to save from this block instead of self.expected
         """
 
         logger.debug("save from: %s", save_from)
 
         read_save_from = outer_save_block or self.expected
         logger.debug("save spec: %s", read_save_from.get("save"))
@@ -250,26 +251,26 @@
         return self.maybe_get_save_values_from_given_block(key, save_from, to_save)
 
     def maybe_get_save_values_from_given_block(
         self,
         key: str,
         save_from: Mapping | None,
         to_save: Mapping,
-    ) -> dict:
+    ) -> Mapping:
         """Save a value from a specific block in the response.
 
         This is different from maybe_get_save_values_from_ext - depends on the kind of response
 
         Args:
             key: Name of key being used to save, for debugging
             save_from: An element of the response from which values are being saved
             to_save: block containing information about things to save
 
         Returns:
-            dict: dictionary of save_name: value, where save_name is the key we
+            mapping of save_name: value, where save_name is the key we
                 wanted to save this value as
         """
 
         saved = {}
 
         if not save_from:
             self._adderr("No %s in response (wanted to save %s)", key, to_save)
```

### Comparing `tavern-3.0.0a3/tests/conftest.py` & `tavern-3.0.0a4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/common.yaml` & `tavern-3.0.0a4/tests/integration/common.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/conftest.py` & `tavern-3.0.0a4/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/server.py` & `tavern-3.0.0a4/tests/integration/server.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_auth_key.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_auth_key.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_certs.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_certs.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_control_flow.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_control_flow.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_cookie_remember.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_cookie_remember.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_cookies.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_cookies.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_data_key.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_data_key.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_external_functions.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_external_functions.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_files.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_files.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_fixtures.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_fixtures.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_follow_redirects.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_follow_redirects.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_header_comparisons.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_header_comparisons.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_helpers.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_helpers.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_include.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_include.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_jmes.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_jmes.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_parametrize.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_parametrize.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_regex.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_regex.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_response_types.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_response_types.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_retry.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_retry.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_save_dict_value.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_save_dict_value.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_selective_tests.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_selective_tests.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_skipped_tests.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_skipped_tests.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_status_codes.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_status_codes.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_strict_key_checks.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_strict_key_checks.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_timeout.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_timeout.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_tincture.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_tincture.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_typetokens.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_typetokens.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/integration/test_validate_pykwalify.tavern.yaml` & `tavern-3.0.0a4/tests/integration/test_validate_pykwalify.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/logging.yaml` & `tavern-3.0.0a4/tests/logging.yaml`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/conftest.py` & `tavern-3.0.0a4/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/response/test_mqtt_response.py` & `tavern-3.0.0a4/tests/unit/response/test_mqtt_response.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/response/test_rest.py` & `tavern-3.0.0a4/tests/unit/response/test_rest.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/tavern_grpc/test_grpc.py` & `tavern-3.0.0a4/tests/unit/tavern_grpc/test_grpc.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/tavern_grpc/test_services_pb2.py` & `tavern-3.0.0a4/tests/unit/tavern_grpc/test_services_pb2.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/tavern_grpc/test_services_pb2.pyi` & `tavern-3.0.0a4/tests/unit/tavern_grpc/test_services_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/tavern_grpc/test_services_pb2_grpc.py` & `tavern-3.0.0a4/tests/unit/tavern_grpc/test_services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_call_run.py` & `tavern-3.0.0a4/tests/unit/test_call_run.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_core.py` & `tavern-3.0.0a4/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_extensions.py` & `tavern-3.0.0a4/tests/unit/test_extensions.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_helpers.py` & `tavern-3.0.0a4/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_mqtt.py` & `tavern-3.0.0a4/tests/unit/test_mqtt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from unittest.mock import MagicMock, Mock, patch
 
 import paho.mqtt.client as paho
 import pytest
 
 from tavern._core import exceptions
 from tavern._plugins.mqtt.client import MQTTClient, _handle_tls_args, _Subscription
@@ -16,15 +17,15 @@
     args = {"connect": {"host": "localhost"}}
 
     MQTTClient(**args)
 
 
 @pytest.fixture(name="fake_client")
 def fix_fake_client():
-    args = {"connect": {"host": "localhost"}}
+    args = {"connect": {"host": "localhost", "timeout": 0.6}}
 
     mqtt_client = MQTTClient(**args)
 
     mqtt_client._subscribed[2] = _Subscription("abc")
     mqtt_client._subscription_mappings["abc"] = 2
 
     return mqtt_client
@@ -66,36 +67,75 @@
         with patch.object(fake_client._client, "loop_start"), patch.object(
             fake_client._client, "connect_async"
         ):
             fake_client._client._state = paho.mqtt_cs_connected
             with fake_client as x:
                 assert fake_client == x
 
-    def test_assert_message_published(self, fake_client):
-        """If it couldn't immediately publish the message, error out"""
+    def test_assert_message_published_error(self, fake_client):
+        """Error waiting for it to publish"""
+
+        class FakeMessage(paho.MQTTMessageInfo):
+            def wait_for_publish(self, timeout=None):
+                raise RuntimeError
 
-        class FakeMessage:
-            is_published = False
             rc = 1
 
         with patch.object(fake_client._client, "subscribe"), patch.object(
-            fake_client._client, "publish", return_value=FakeMessage()
+            fake_client._client, "publish", return_value=FakeMessage(10)
         ):
             with pytest.raises(exceptions.MQTTError):
                 fake_client.publish("abc", "123")
 
+    def test_assert_message_published_failure(self, fake_client: MQTTClient):
+        """If it couldn't publish the message, error out"""
+
+        class FakeMessage(paho.MQTTMessageInfo):
+            def wait_for_publish(self, timeout=None):
+                return
+
+            def is_published(self):
+                return False
+
+            rc = 1
+
+        with patch.object(fake_client._client, "subscribe"), patch.object(
+            fake_client._client, "publish", return_value=FakeMessage(10)
+        ):
+            with pytest.raises(exceptions.MQTTError):
+                fake_client.publish("abc", "123")
+
+    def test_assert_message_published_delay(self, fake_client):
+        """Published but only after a small delay"""
+
+        class FakeMessage(paho.MQTTMessageInfo):
+            def wait_for_publish(self, timeout=None):
+                time.sleep(0.5)
+
+            def is_published(self):
+                return True
+
+            rc = 1
+
+        with patch.object(fake_client._client, "subscribe"), patch.object(
+            fake_client._client, "publish", return_value=FakeMessage(10)
+        ):
+            fake_client.publish("abc", "123")
+
     def test_assert_message_published_unknown_err(self, fake_client):
         """Same, but with an unknown error code"""
 
-        class FakeMessage:
-            is_published = False
+        class FakeMessage(paho.MQTTMessageInfo):
+            def is_published(self):
+                return False
+
             rc = 2342423
 
         with patch.object(fake_client._client, "subscribe"), patch.object(
-            fake_client._client, "publish", return_value=FakeMessage()
+            fake_client._client, "publish", return_value=FakeMessage(10)
         ):
             with pytest.raises(exceptions.MQTTError):
                 fake_client.publish("abc", "123")
 
 
 class TestTLS:
     def test_missing_cert_gives_error(self):
```

### Comparing `tavern-3.0.0a3/tests/unit/test_pytest_hooks.py` & `tavern-3.0.0a4/tests/unit/test_pytest_hooks.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_request.py` & `tavern-3.0.0a4/tests/unit/test_request.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_schema.py` & `tavern-3.0.0a4/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_strict_util.py` & `tavern-3.0.0a4/tests/unit/test_strict_util.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_tinctures.py` & `tavern-3.0.0a4/tests/unit/test_tinctures.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tests/unit/test_utilities.py` & `tavern-3.0.0a4/tests/unit/test_utilities.py`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/tox-integration.ini` & `tavern-3.0.0a4/tox-integration.ini`

 * *Files 8% similar despite different names*

```diff
@@ -51,13 +51,8 @@
     advanced: python -c "from tavern.core import run; exit(run('test_server.tavern.yaml', pytest_args=[ ]))"
 
     components: tavern-ci --stdout test_ping.tavern.yaml
     components: tavern-ci --stdout test_hello.tavern.yaml
     components: python -c "from tavern.core import run; exit(run('test_ping.tavern.yaml', pytest_args=[ ]))"
     components: python -c "from tavern.core import run; exit(run('test_hello.tavern.yaml', pytest_args=[ ]))"
 
-    mqtt: tavern-ci --stdout test_mqtt.tavern.yaml --cov tavern
-    mqtt: python -c "from tavern.core import run; exit(run('test_mqtt.tavern.yaml', pytest_args=['--cov-append']))"
-    mqtt: tavern-ci --stdout test_mqtt_failures.tavern.yaml
-    mqtt: python -c "from tavern.core import run; exit(run('test_mqtt_failures.tavern.yaml', pytest_args=[ ]))"
-
     docker compose stop
```

### Comparing `tavern-3.0.0a3/tox.ini` & `tavern-3.0.0a4/tox.ini`

 * *Files identical despite different names*

### Comparing `tavern-3.0.0a3/PKG-INFO` & `tavern-3.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tavern
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: Simple testing of RESTful APIs
 Keywords: testing,pytest
 Author: Michael Boulton
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

