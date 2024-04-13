# Comparing `tmp/haupt-2.1.6.tar.gz` & `tmp/haupt-2.1.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haupt-2.1.6.tar", last modified: Sat Apr 13 15:11:07 2024, max compression
+gzip compressed data, was "haupt-2.1.6rc0.tar", last modified: Tue Apr  9 14:09:20 2024, max compression
```

## Comparing `haupt-2.1.6.tar` & `haupt-2.1.6rc0.tar`

### file list

```diff
@@ -1,635 +1,634 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.371891 haupt-2.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 15:10:57.000000 haupt-2.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-13 15:11:07.371891 haupt-2.1.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.271891 haupt-2.1.6/haupt/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.271891 haupt-2.1.6/haupt/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.271891 haupt-2.1.6/haupt/apis/agents/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/agents/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/agents/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.271891 haupt-2.1.6/haupt/apis/bookmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/bookmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/bookmarks/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.271891 haupt-2.1.6/haupt/apis/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/endpoints/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/endpoints/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.271891 haupt-2.1.6/haupt/apis/methods/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/methods/entity_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/methods/project_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/methods/run_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/methods/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.271891 haupt-2.1.6/haupt/apis/project_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/project_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/project_resources/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.275891 haupt-2.1.6/haupt/apis/project_resources/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/project_resources/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/project_resources/views/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/project_resources/views/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.275891 haupt-2.1.6/haupt/apis/projects/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/projects/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/projects/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.275891 haupt-2.1.6/haupt/apis/run_lineage/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/run_lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/run_lineage/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/run_lineage/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.275891 haupt-2.1.6/haupt/apis/runs/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/runs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/runs/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/runs/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.275891 haupt-2.1.6/haupt/apis/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/artifacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.279891 haupt-2.1.6/haupt/apis/serializers/base/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/bookmarks_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/is_managed.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/names.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/owner_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/resources_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/user_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/base/uuid_slug_related_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/project_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/project_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/serializers/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.279891 haupt-2.1.6/haupt/apis/versions/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/versions/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/apis/versions/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.279891 haupt-2.1.6/haupt/background/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.279891 haupt-2.1.6/haupt/background/celeryp/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/celeryp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/celeryp/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/celeryp/executions.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/celeryp/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/celeryp/polyaxon_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/celeryp/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/celeryp/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/celeryp/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.279891 haupt-2.1.6/haupt/background/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/scheduler/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/background/scheduler/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.283891 haupt-2.1.6/haupt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/queues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.283891 haupt-2.1.6/haupt/cli/runners/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/cron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/runners/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/cli/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.283891 haupt-2.1.6/haupt/common/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.287891 haupt-2.1.6/haupt/common/apis/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/gzip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.287891 haupt-2.1.6/haupt/common/apis/index/
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/index/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/index/health.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/index/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.259891 haupt-2.1.6/haupt/common/apis/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.287891 haupt-2.1.6/haupt/common/apis/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/templates/admin/base_site.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.287891 haupt-2.1.6/haupt/common/apis/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/templates/base/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/templates/base/modal_index.html
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/templates/base/wizard_error.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.287891 haupt-2.1.6/haupt/common/apis/templates/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/templates/common/root.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.287891 haupt-2.1.6/haupt/common/apis/urls/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/urls/agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/urls/project_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/urls/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/urls/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/urls/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/apis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.287891 haupt-2.1.6/haupt/common/auditor/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/auditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/auditor/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/auditor/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.287891 haupt-2.1.6/haupt/common/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/authentication/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/authentication/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/authentication/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.291891 haupt-2.1.6/haupt/common/checks/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/checks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/checks/health_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/checks/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.291891 haupt-2.1.6/haupt/common/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/commands/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.291891 haupt-2.1.6/haupt/common/commands/management/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/commands/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.291891 haupt-2.1.6/haupt/common/commands/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/commands/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/commands/management/commands/create_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/commands/management/commands/createuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/commands/management/commands/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.291891 haupt-2.1.6/haupt/common/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.291891 haupt-2.1.6/haupt/common/conf/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/handlers/env_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/handlers/settings_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/option_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/option_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/conf/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/content_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.291891 haupt-2.1.6/haupt/common/db/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/db/inserter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/db/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/db/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.295891 haupt-2.1.6/haupt/common/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/endpoints/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/endpoints/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/endpoints/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/endpoints/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/endpoints/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.295891 haupt-2.1.6/haupt/common/events/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.295891 haupt-2.1.6/haupt/common/events/auditor_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/auditor_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/auditor_subscriptions/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/auditor_subscriptions/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/auditor_subscriptions/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/auditor_subscriptions/component_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/auditor_subscriptions/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/auditor_subscriptions/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/auditor_subscriptions/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/event_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/event_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/event_subjects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.295891 haupt-2.1.6/haupt/common/events/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/component_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/model_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/events/registry/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/memory_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.299891 haupt-2.1.6/haupt/common/options/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.299891 haupt-2.1.6/haupt/common/options/conf_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/conf_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/conf_subscriptions/cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/conf_subscriptions/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/conf_subscriptions/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/conf_subscriptions/installation.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/conf_subscriptions/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/conf_subscriptions/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/conf_subscriptions/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/option.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/option_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/option_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/option_owners.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/option_subjects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.299891 haupt-2.1.6/haupt/common/options/registry/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/registry/cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/registry/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/registry/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/registry/installation.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/registry/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/registry/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/options/registry/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.299891 haupt-2.1.6/haupt/common/query/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/query/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/redis_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/service_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.303891 haupt-2.1.6/haupt/common/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/cors.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.303891 haupt-2.1.6/haupt/common/settings/services/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/services/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/services/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/services/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/settings/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.303891 haupt-2.1.6/haupt/common/test_cases/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/test_cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/test_cases/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.303891 haupt-2.1.6/haupt/common/test_clients/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/test_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/test_clients/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/user_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.303891 haupt-2.1.6/haupt/common/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/validation/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/validation/slugs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/common/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.303891 haupt-2.1.6/haupt/db/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.307891 haupt-2.1.6/haupt/db/abstracts/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/color.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/contributors.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/describable.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/live_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/nameable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/project_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/run_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/run_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/run_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/uid.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/users.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/abstracts/visibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.311891 haupt-2.1.6/haupt/db/administration/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/administration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/administration/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/administration/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/administration/register.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/administration/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/administration/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/defs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.311891 haupt-2.1.6/haupt/db/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/factories/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/factories/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/factories/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/factories/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.311891 haupt-2.1.6/haupt/db/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19103 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/agents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/deleted.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/dummy_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/live_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/managers/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.315891 haupt-2.1.6/haupt/db/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/mixins/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/mixins/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/mixins/sub_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/mixins/unique_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.315891 haupt-2.1.6/haupt/db/models/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/project_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/project_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/run_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/models/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.315891 haupt-2.1.6/haupt/db/pgsql/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.315891 haupt-2.1.6/haupt/db/pgsql/db/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.319891 haupt-2.1.6/haupt/db/pgsql/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    20518 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0002_auto_20200807_1247.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0003_run_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0004_auto_20200905_1523.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0005_auto_20201005_0913.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0006_auto_20201020_1705.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0007_auto_20201121_1332.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0008_run_wait_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0009_project_unique_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0010_auto_20210429_1539.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0011_alter_artifact_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0012_alter_artifact_updated_at_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0013_major_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/0014_remove_run_is_managed_project_archived_at_and_duration_wait_time_to_float_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/pgsql/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.319891 haupt-2.1.6/haupt/db/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/queries/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/queries/runs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.319891 haupt-2.1.6/haupt/db/query_managers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/callback_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/project_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/query_managers/run_edge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.319891 haupt-2.1.6/haupt/db/signals/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/signals/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/signals/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/signals/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/signals/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.319891 haupt-2.1.6/haupt/db/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/sqlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.319891 haupt-2.1.6/haupt/db/sqlite/db/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/sqlite/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/sqlite/db/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.319891 haupt-2.1.6/haupt/db/sqlite/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    35956 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/sqlite/db/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/sqlite/db/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/db/sqlite/db/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.323891 haupt-2.1.6/haupt/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/managers/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/managers/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/managers/sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.323891 haupt-2.1.6/haupt/orchestration/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.323891 haupt-2.1.6/haupt/orchestration/crons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/crons/deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/crons/heartbeats.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/crons/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.323891 haupt-2.1.6/haupt/orchestration/executor/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/executor/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/executor/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/executor/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.323891 haupt-2.1.6/haupt/orchestration/executor/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/executor/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/executor/subscriptions/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.323891 haupt-2.1.6/haupt/orchestration/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19441 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/operations/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.323891 haupt-2.1.6/haupt/orchestration/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53997 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/scheduler/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    74337 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/orchestration/scheduler/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.323891 haupt-2.1.6/haupt/polyconf/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.327891 haupt-2.1.6/haupt/polyconf/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/asgi/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/asgi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/asgi/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/asgi/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/config_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.327891 haupt-2.1.6/haupt/polyconf/config_settings/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/config_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/config_settings/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/polyconf/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.327891 haupt-2.1.6/haupt/proxies/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.327891 haupt-2.1.6/haupt/proxies/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/generators/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/generators/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/generators/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/generators/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.331891 haupt-2.1.6/haupt/proxies/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.331891 haupt-2.1.6/haupt/proxies/schemas/api/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/api/uwsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/buffering.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/charset.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/error_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/favicon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/forward.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.331891 haupt-2.1.6/haupt/proxies/schemas/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/gateway/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/gateway/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/gateway/healthz.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/gateway/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/gzip.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/listen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/robots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/scaffold.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/ssl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.331891 haupt-2.1.6/haupt/proxies/schemas/streams/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/streams/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/streams/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/streams/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/proxies/schemas/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.331891 haupt-2.1.6/haupt/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16549 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/schemas/platform_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/schemas/proxies_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/schemas/sandbox_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.267891 haupt-2.1.6/haupt/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.267891 haupt-2.1.6/haupt/static/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.331891 haupt-2.1.6/haupt/static/dist/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/css/global.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/css/global_modal.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.343891 haupt-2.1.6/haupt/static/dist/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/js/0.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)  3772290 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/js/1.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)    68534 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/js/2.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   410638 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/js/3.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   192251 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/js/4.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)    23193 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/js/5.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)   411926 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/js/6.bundle.js
--rw-r--r--   0 runner    (1001) docker     (127)  2240021 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/dist/js/7.bundle.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.347891 haupt-2.1.6/haupt/static/errors/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/errors/50x.html
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/errors/permission.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.347891 haupt-2.1.6/haupt/static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    25380 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/403.svg
--rw-r--r--   0 runner    (1001) docker     (127)    13004 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/404.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15858 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/50x.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-danger.ico
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-danger.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-primary.ico
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-primary.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-running.ico
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-running.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-stopped.ico
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-stopped.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-success.ico
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-success.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-warning.ico
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon-warning.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/logo_small.png
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/images/logo_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.267891 haupt-2.1.6/haupt/static/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.347891 haupt-2.1.6/haupt/static/vendors/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.351891 haupt-2.1.6/haupt/static/vendors/fonts/dosis/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/dosis/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27069 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.eot
--rw-r--r--   0 runner    (1001) docker     (127)    71085 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.svg
--rw-r--r--   0 runner    (1001) docker     (127)    66980 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    32948 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff
--rw-r--r--   0 runner    (1001) docker     (127)    26508 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.351891 haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)    61056 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.355891 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (127)    77083 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.eot
--rw-r--r--   0 runner    (1001) docker     (127)    60850 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.svg
--rw-r--r--   0 runner    (1001) docker     (127)   184424 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    80588 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff
--rw-r--r--   0 runner    (1001) docker     (127)    62208 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77159 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.eot
--rw-r--r--   0 runner    (1001) docker     (127)    58839 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.svg
--rw-r--r--   0 runner    (1001) docker     (127)   183688 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    80556 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff
--rw-r--r--   0 runner    (1001) docker     (127)    62104 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77546 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)    60072 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)   184592 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    81008 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    62688 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.367891 haupt-2.1.6/haupt/static/vendors/js/
--rw-r--r--   0 runner    (1001) docker     (127)   959287 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/bokeh.3.2.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    24977 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/create-plotly-component.2.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   100277 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/highlight.10.1.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/moment-timezone.0.5.32.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    58913 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/moment.2.30.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)  3608773 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/plotly.2.28.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   131882 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/react-dom.production.18.0.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/react.production.18.0.2.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    65227 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/vega-embed@6.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   248899 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/vega-lite@5.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   511113 2024-04-13 15:10:58.000000 haupt-2.1.6/haupt/static/vendors/js/vega@5.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.367891 haupt-2.1.6/haupt/streams/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.367891 haupt-2.1.6/haupt/streams/connections/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/connections/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.367891 haupt-2.1.6/haupt/streams/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/controllers/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/controllers/k8s_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/controllers/k8s_crd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/controllers/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/controllers/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/controllers/uploads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.371891 haupt-2.1.6/haupt/streams/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/auth_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/endpoints/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.371891 haupt-2.1.6/haupt/streams/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/tasks/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-13 15:10:57.000000 haupt-2.1.6/haupt/streams/tasks/op_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:11:07.271891 haupt-2.1.6/haupt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-13 15:11:07.000000 haupt-2.1.6/haupt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20402 2024-04-13 15:11:07.000000 haupt-2.1.6/haupt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:11:07.000000 haupt-2.1.6/haupt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-13 15:11:07.000000 haupt-2.1.6/haupt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-13 15:11:07.000000 haupt-2.1.6/haupt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 15:11:07.000000 haupt-2.1.6/haupt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-13 15:11:07.371891 haupt-2.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-13 15:10:57.000000 haupt-2.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.185652 haupt-2.1.6rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-09 14:09:20.185652 haupt-2.1.6rc0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.069652 haupt-2.1.6rc0/haupt/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.069652 haupt-2.1.6rc0/haupt/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.069652 haupt-2.1.6rc0/haupt/apis/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/agents/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/agents/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.069652 haupt-2.1.6rc0/haupt/apis/bookmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/bookmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/bookmarks/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.069652 haupt-2.1.6rc0/haupt/apis/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/endpoints/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/endpoints/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.073652 haupt-2.1.6rc0/haupt/apis/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/methods/entity_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10611 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/methods/project_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/methods/run_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/methods/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.073652 haupt-2.1.6rc0/haupt/apis/project_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/project_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/project_resources/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.073652 haupt-2.1.6rc0/haupt/apis/project_resources/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/project_resources/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/project_resources/views/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13986 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/project_resources/views/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.073652 haupt-2.1.6rc0/haupt/apis/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/projects/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/projects/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.073652 haupt-2.1.6rc0/haupt/apis/run_lineage/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/run_lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/run_lineage/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/run_lineage/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.073652 haupt-2.1.6rc0/haupt/apis/runs/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/runs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/runs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/runs/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.077652 haupt-2.1.6rc0/haupt/apis/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/artifacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.077652 haupt-2.1.6rc0/haupt/apis/serializers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/bookmarks_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/is_managed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/owner_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/resources_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/user_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/base/uuid_slug_related_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/project_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14690 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/serializers/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.077652 haupt-2.1.6rc0/haupt/apis/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/versions/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/apis/versions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.077652 haupt-2.1.6rc0/haupt/background/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.081652 haupt-2.1.6rc0/haupt/background/celeryp/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/celeryp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/celeryp/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/celeryp/executions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/celeryp/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/celeryp/polyaxon_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/celeryp/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/celeryp/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/celeryp/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.081652 haupt-2.1.6rc0/haupt/background/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/scheduler/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/background/scheduler/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.081652 haupt-2.1.6rc0/haupt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/queues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.081652 haupt-2.1.6rc0/haupt/cli/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/cron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/runners/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/cli/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.085652 haupt-2.1.6rc0/haupt/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.085652 haupt-2.1.6rc0/haupt/common/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/gzip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.085652 haupt-2.1.6rc0/haupt/common/apis/index/
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/index/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/index/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/index/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.057652 haupt-2.1.6rc0/haupt/common/apis/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.085652 haupt-2.1.6rc0/haupt/common/apis/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.085652 haupt-2.1.6rc0/haupt/common/apis/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/templates/base/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/templates/base/modal_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/templates/base/wizard_error.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.089652 haupt-2.1.6rc0/haupt/common/apis/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/templates/common/root.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.089652 haupt-2.1.6rc0/haupt/common/apis/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/urls/agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/urls/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/urls/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/urls/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/urls/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/apis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.089652 haupt-2.1.6rc0/haupt/common/auditor/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/auditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/auditor/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/auditor/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.089652 haupt-2.1.6rc0/haupt/common/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/authentication/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/authentication/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/authentication/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.089652 haupt-2.1.6rc0/haupt/common/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/checks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/checks/health_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/checks/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.089652 haupt-2.1.6rc0/haupt/common/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/commands/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.089652 haupt-2.1.6rc0/haupt/common/commands/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/commands/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.093652 haupt-2.1.6rc0/haupt/common/commands/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/commands/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/commands/management/commands/create_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/commands/management/commands/createuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/commands/management/commands/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.097652 haupt-2.1.6rc0/haupt/common/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.097652 haupt-2.1.6rc0/haupt/common/conf/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/handlers/env_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/handlers/settings_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/option_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/option_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/conf/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/content_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.097652 haupt-2.1.6rc0/haupt/common/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/db/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/db/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/db/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.101652 haupt-2.1.6rc0/haupt/common/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9051 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/endpoints/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/endpoints/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/endpoints/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/endpoints/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/endpoints/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.101652 haupt-2.1.6rc0/haupt/common/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.101652 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/component_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/event_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/event_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/event_subjects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.105652 haupt-2.1.6rc0/haupt/common/events/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/component_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/events/registry/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/memory_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.105652 haupt-2.1.6rc0/haupt/common/options/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.109652 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/option_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/option_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/option_owners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/option_subjects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.109652 haupt-2.1.6rc0/haupt/common/options/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/registry/cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/registry/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/registry/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/registry/installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/registry/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/registry/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/options/registry/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.109652 haupt-2.1.6rc0/haupt/common/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/query/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/redis_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/service_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.113652 haupt-2.1.6rc0/haupt/common/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.113652 haupt-2.1.6rc0/haupt/common/settings/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/services/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/services/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/services/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/settings/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.113652 haupt-2.1.6rc0/haupt/common/test_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/test_cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/test_cases/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.113652 haupt-2.1.6rc0/haupt/common/test_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/test_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/test_clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/user_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.113652 haupt-2.1.6rc0/haupt/common/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/validation/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/validation/slugs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/common/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.113652 haupt-2.1.6rc0/haupt/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.117652 haupt-2.1.6rc0/haupt/db/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/contributors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/describable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/live_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/nameable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/run_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/run_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/run_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/uid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/abstracts/visibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.117652 haupt-2.1.6rc0/haupt/db/administration/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/administration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/administration/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/administration/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/administration/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/administration/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/administration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/defs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.121652 haupt-2.1.6rc0/haupt/db/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/factories/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/factories/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/factories/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/factories/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.121652 haupt-2.1.6rc0/haupt/db/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19103 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/deleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/dummy_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/live_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/managers/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.121652 haupt-2.1.6rc0/haupt/db/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/mixins/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/mixins/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/mixins/sub_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/mixins/unique_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.125652 haupt-2.1.6rc0/haupt/db/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/project_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/project_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/run_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/models/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.125652 haupt-2.1.6rc0/haupt/db/pgsql/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.125652 haupt-2.1.6rc0/haupt/db/pgsql/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.125652 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    20518 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0002_auto_20200807_1247.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0003_run_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0004_auto_20200905_1523.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0005_auto_20201005_0913.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0006_auto_20201020_1705.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0007_auto_20201121_1332.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0008_run_wait_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0009_project_unique_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0010_auto_20210429_1539.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0011_alter_artifact_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0012_alter_artifact_updated_at_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0013_major_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0014_remove_run_is_managed_project_archived_at_and_duration_wait_time_to_float_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/pgsql/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.129652 haupt-2.1.6rc0/haupt/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/queries/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/queries/runs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.129652 haupt-2.1.6rc0/haupt/db/query_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/callback_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/project_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10268 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/query_managers/run_edge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.129652 haupt-2.1.6rc0/haupt/db/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/signals/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/signals/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/signals/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/signals/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.129652 haupt-2.1.6rc0/haupt/db/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/sqlite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.129652 haupt-2.1.6rc0/haupt/db/sqlite/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/sqlite/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/sqlite/db/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.129652 haupt-2.1.6rc0/haupt/db/sqlite/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    35956 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/sqlite/db/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/sqlite/db/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/db/sqlite/db/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.129652 haupt-2.1.6rc0/haupt/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/managers/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/managers/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/managers/sandbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.129652 haupt-2.1.6rc0/haupt/orchestration/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.133652 haupt-2.1.6rc0/haupt/orchestration/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/crons/deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/crons/heartbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/crons/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.133652 haupt-2.1.6rc0/haupt/orchestration/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/executor/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/executor/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/executor/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.133652 haupt-2.1.6rc0/haupt/orchestration/executor/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/executor/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/executor/subscriptions/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.133652 haupt-2.1.6rc0/haupt/orchestration/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19441 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/operations/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.133652 haupt-2.1.6rc0/haupt/orchestration/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53997 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/scheduler/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74337 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/orchestration/scheduler/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.133652 haupt-2.1.6rc0/haupt/polyconf/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.133652 haupt-2.1.6rc0/haupt/polyconf/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/asgi/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/asgi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/asgi/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/asgi/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/config_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.137652 haupt-2.1.6rc0/haupt/polyconf/config_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/config_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/config_settings/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/polyconf/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.137652 haupt-2.1.6rc0/haupt/proxies/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.137652 haupt-2.1.6rc0/haupt/proxies/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/generators/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/generators/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/generators/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/generators/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.141652 haupt-2.1.6rc0/haupt/proxies/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.141652 haupt-2.1.6rc0/haupt/proxies/schemas/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/api/uwsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/buffering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/charset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/error_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/favicon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.141652 haupt-2.1.6rc0/haupt/proxies/schemas/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/gateway/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/gateway/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/gateway/healthz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/gateway/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/gzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/listen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/robots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10255 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.141652 haupt-2.1.6rc0/haupt/proxies/schemas/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/streams/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/streams/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/streams/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/proxies/schemas/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.145652 haupt-2.1.6rc0/haupt/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16549 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/schemas/platform_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/schemas/proxies_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/schemas/sandbox_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.065652 haupt-2.1.6rc0/haupt/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.065652 haupt-2.1.6rc0/haupt/static/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.145652 haupt-2.1.6rc0/haupt/static/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/css/global.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/css/global_modal.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.153652 haupt-2.1.6rc0/haupt/static/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/js/0.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3772290 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/js/1.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68534 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/js/2.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   410638 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/js/3.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   192251 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/js/4.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23193 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/js/5.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)   411926 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/js/6.bundle.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2240021 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/dist/js/7.bundle.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.161652 haupt-2.1.6rc0/haupt/static/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/errors/50x.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/errors/permission.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.161652 haupt-2.1.6rc0/haupt/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    25380 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/403.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    13004 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/404.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15858 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/50x.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-danger.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-danger.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-primary.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-primary.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-running.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-running.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-stopped.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-stopped.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-success.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-success.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-warning.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon-warning.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/static/images/logo_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.065652 haupt-2.1.6rc0/haupt/static/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.161652 haupt-2.1.6rc0/haupt/static/vendors/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.165652 haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27069 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    71085 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    66980 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    32948 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    26508 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.165652 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    61056 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.169652 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    77083 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    60850 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   184424 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    80588 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    62208 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77159 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    58839 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   183688 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    80556 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    62104 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77546 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    60072 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   184592 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    81008 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    62688 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.181652 haupt-2.1.6rc0/haupt/static/vendors/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   959287 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/bokeh.3.2.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24977 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/create-plotly-component.2.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   100277 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/highlight.10.1.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/moment-timezone.0.5.32.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58913 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/moment.2.30.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3608773 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/plotly.2.28.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   131882 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/react-dom.production.18.0.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/react.production.18.0.2.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65227 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/vega-embed@6.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   248899 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/vega-lite@5.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   511113 2024-04-09 14:09:13.000000 haupt-2.1.6rc0/haupt/static/vendors/js/vega@5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.181652 haupt-2.1.6rc0/haupt/streams/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.181652 haupt-2.1.6rc0/haupt/streams/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/connections/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.181652 haupt-2.1.6rc0/haupt/streams/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/controllers/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/controllers/k8s_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/controllers/k8s_crd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/controllers/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/controllers/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/controllers/uploads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.185652 haupt-2.1.6rc0/haupt/streams/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/endpoints/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.185652 haupt-2.1.6rc0/haupt/streams/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/tasks/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/haupt/streams/tasks/op_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:09:20.069652 haupt-2.1.6rc0/haupt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-09 14:09:19.000000 haupt-2.1.6rc0/haupt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20373 2024-04-09 14:09:19.000000 haupt-2.1.6rc0/haupt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:09:19.000000 haupt-2.1.6rc0/haupt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 14:09:19.000000 haupt-2.1.6rc0/haupt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-09 14:09:19.000000 haupt-2.1.6rc0/haupt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 14:09:19.000000 haupt-2.1.6rc0/haupt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-09 14:09:20.185652 haupt-2.1.6rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-09 14:09:12.000000 haupt-2.1.6rc0/setup.py
```

### Comparing `haupt-2.1.6/PKG-INFO` & `haupt-2.1.6rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haupt
-Version: 2.1.6
+Version: 2.1.6rc0
 Summary: Lineage metadata API, artifacts streams, sandbox, ML-API, and spaces for Polyaxon.
 Home-page: https://github.com/polyaxon/haupt
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: AGPLv3
```

### Comparing `haupt-2.1.6/haupt/apis/agents/views.py` & `haupt-2.1.6rc0/haupt/apis/agents/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/apps.py` & `haupt-2.1.6rc0/haupt/apis/apps.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/bookmarks/views.py` & `haupt-2.1.6rc0/haupt/apis/bookmarks/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/endpoints/project.py` & `haupt-2.1.6rc0/haupt/apis/endpoints/project.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/endpoints/run.py` & `haupt-2.1.6rc0/haupt/apis/endpoints/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/methods/entity_stages.py` & `haupt-2.1.6rc0/haupt/apis/methods/entity_stages.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/methods/project_resources.py` & `haupt-2.1.6rc0/haupt/apis/methods/project_resources.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/methods/run_lineage.py` & `haupt-2.1.6rc0/haupt/apis/methods/run_lineage.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/methods/runs.py` & `haupt-2.1.6rc0/haupt/apis/methods/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/patterns.py` & `haupt-2.1.6rc0/haupt/apis/patterns.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/project_resources/urls.py` & `haupt-2.1.6rc0/haupt/apis/project_resources/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/project_resources/views/runs.py` & `haupt-2.1.6rc0/haupt/apis/project_resources/views/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/project_resources/views/versions.py` & `haupt-2.1.6rc0/haupt/apis/project_resources/views/versions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/projects/urls.py` & `haupt-2.1.6rc0/haupt/apis/projects/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/projects/views.py` & `haupt-2.1.6rc0/haupt/apis/projects/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/run_lineage/urls.py` & `haupt-2.1.6rc0/haupt/apis/run_lineage/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/run_lineage/views.py` & `haupt-2.1.6rc0/haupt/apis/run_lineage/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/runs/urls.py` & `haupt-2.1.6rc0/haupt/apis/runs/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/runs/views.py` & `haupt-2.1.6rc0/haupt/apis/runs/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/artifacts.py` & `haupt-2.1.6rc0/haupt/apis/serializers/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/base/bookmarks_mixin.py` & `haupt-2.1.6rc0/haupt/apis/serializers/base/bookmarks_mixin.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/base/is_managed.py` & `haupt-2.1.6rc0/haupt/apis/serializers/base/is_managed.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/base/names.py` & `haupt-2.1.6rc0/haupt/apis/serializers/base/names.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/base/settings.py` & `haupt-2.1.6rc0/haupt/apis/serializers/base/settings.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/base/tags.py` & `haupt-2.1.6rc0/haupt/apis/serializers/base/tags.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/project_stats.py` & `haupt-2.1.6rc0/haupt/apis/serializers/project_stats.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/project_versions.py` & `haupt-2.1.6rc0/haupt/apis/serializers/project_versions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/projects.py` & `haupt-2.1.6rc0/haupt/apis/serializers/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/serializers/runs.py` & `haupt-2.1.6rc0/haupt/apis/serializers/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/apis/versions/views.py` & `haupt-2.1.6rc0/haupt/apis/versions/views.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/background/celeryp/executions.py` & `haupt-2.1.6rc0/haupt/background/celeryp/executions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/background/celeryp/polyaxon_task.py` & `haupt-2.1.6rc0/haupt/background/celeryp/polyaxon_task.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/background/celeryp/queues.py` & `haupt-2.1.6rc0/haupt/background/celeryp/queues.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/background/celeryp/routes.py` & `haupt-2.1.6rc0/haupt/background/celeryp/routes.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/background/celeryp/tasks.py` & `haupt-2.1.6rc0/haupt/background/celeryp/tasks.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/background/scheduler/apps.py` & `haupt-2.1.6rc0/haupt/background/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/manage.py` & `haupt-2.1.6rc0/haupt/cli/manage.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/proxies.py` & `haupt-2.1.6rc0/haupt/cli/proxies.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/runners/base.py` & `haupt-2.1.6rc0/haupt/cli/runners/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/runners/config.py` & `haupt-2.1.6rc0/haupt/cli/runners/config.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/runners/cron.py` & `haupt-2.1.6rc0/haupt/cli/runners/cron.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/runners/manage.py` & `haupt-2.1.6rc0/haupt/cli/runners/manage.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/runners/sandbox.py` & `haupt-2.1.6rc0/haupt/cli/runners/sandbox.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/runners/server.py` & `haupt-2.1.6rc0/haupt/cli/runners/server.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/runners/streams.py` & `haupt-2.1.6rc0/haupt/cli/runners/streams.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/runners/viewer.py` & `haupt-2.1.6rc0/haupt/cli/runners/viewer.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/sandbox.py` & `haupt-2.1.6rc0/haupt/cli/sandbox.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/server.py` & `haupt-2.1.6rc0/haupt/cli/server.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/streams.py` & `haupt-2.1.6rc0/haupt/cli/streams.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/cli/viewer.py` & `haupt-2.1.6rc0/haupt/cli/viewer.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/filters.py` & `haupt-2.1.6rc0/haupt/common/apis/filters.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/gzip.py` & `haupt-2.1.6rc0/haupt/common/apis/gzip.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/index/__init__.py` & `haupt-2.1.6rc0/haupt/common/apis/index/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/index/health.py` & `haupt-2.1.6rc0/haupt/common/apis/index/health.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/paginator.py` & `haupt-2.1.6rc0/haupt/common/apis/paginator.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/regex.py` & `haupt-2.1.6rc0/haupt/common/apis/regex.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/templates/admin/base_site.html` & `haupt-2.1.6rc0/haupt/common/apis/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/templates/base/index.html` & `haupt-2.1.6rc0/haupt/common/apis/templates/base/index.html`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/templates/base/modal_index.html` & `haupt-2.1.6rc0/haupt/common/apis/templates/base/modal_index.html`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/templates/common/root.html` & `haupt-2.1.6rc0/haupt/common/apis/templates/common/root.html`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/urls/project_versions.py` & `haupt-2.1.6rc0/haupt/common/apis/urls/project_versions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/urls/projects.py` & `haupt-2.1.6rc0/haupt/common/apis/urls/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/apis/urls/runs.py` & `haupt-2.1.6rc0/haupt/common/apis/urls/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/auditor/__init__.py` & `haupt-2.1.6rc0/haupt/common/auditor/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/auditor/service.py` & `haupt-2.1.6rc0/haupt/common/auditor/service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/authentication/base.py` & `haupt-2.1.6rc0/haupt/common/authentication/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/authentication/bot.py` & `haupt-2.1.6rc0/haupt/common/authentication/bot.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/authentication/internal.py` & `haupt-2.1.6rc0/haupt/common/authentication/internal.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/checks/results.py` & `haupt-2.1.6rc0/haupt/common/checks/results.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/commands/management/commands/createuser.py` & `haupt-2.1.6rc0/haupt/common/commands/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/commands/management/commands/tables.py` & `haupt-2.1.6rc0/haupt/common/commands/management/commands/tables.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/conf/__init__.py` & `haupt-2.1.6rc0/haupt/common/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/conf/handlers/env_handler.py` & `haupt-2.1.6rc0/haupt/common/conf/handlers/env_handler.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/conf/handlers/settings_handler.py` & `haupt-2.1.6rc0/haupt/common/conf/handlers/settings_handler.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/conf/option_service.py` & `haupt-2.1.6rc0/haupt/common/conf/option_service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/db/inserter.py` & `haupt-2.1.6rc0/haupt/common/db/inserter.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/db/runs.py` & `haupt-2.1.6rc0/haupt/common/db/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/db/updater.py` & `haupt-2.1.6rc0/haupt/common/db/updater.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/endpoints/base.py` & `haupt-2.1.6rc0/haupt/common/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/endpoints/files.py` & `haupt-2.1.6rc0/haupt/common/endpoints/files.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/endpoints/mixins.py` & `haupt-2.1.6rc0/haupt/common/endpoints/mixins.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/endpoints/validation.py` & `haupt-2.1.6rc0/haupt/common/endpoints/validation.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/auditor_subscriptions/artifact_version.py` & `haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/artifact_version.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/auditor_subscriptions/component_version.py` & `haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/component_version.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/auditor_subscriptions/model_version.py` & `haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/model_version.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/auditor_subscriptions/run.py` & `haupt-2.1.6rc0/haupt/common/events/auditor_subscriptions/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/event.py` & `haupt-2.1.6rc0/haupt/common/events/event.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/event_actions.py` & `haupt-2.1.6rc0/haupt/common/events/event_actions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/event_context.py` & `haupt-2.1.6rc0/haupt/common/events/event_context.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/event_manager.py` & `haupt-2.1.6rc0/haupt/common/events/event_manager.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/event_service.py` & `haupt-2.1.6rc0/haupt/common/events/event_service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/event_subjects.py` & `haupt-2.1.6rc0/haupt/common/events/event_subjects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/registry/archive.py` & `haupt-2.1.6rc0/haupt/common/events/registry/archive.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/registry/artifact_version.py` & `haupt-2.1.6rc0/haupt/common/events/registry/artifact_version.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/registry/attributes.py` & `haupt-2.1.6rc0/haupt/common/events/registry/attributes.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/registry/bookmark.py` & `haupt-2.1.6rc0/haupt/common/events/registry/bookmark.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/registry/component_version.py` & `haupt-2.1.6rc0/haupt/common/events/registry/component_version.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/registry/model_version.py` & `haupt-2.1.6rc0/haupt/common/events/registry/model_version.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/registry/project.py` & `haupt-2.1.6rc0/haupt/common/events/registry/project.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/events/registry/run.py` & `haupt-2.1.6rc0/haupt/common/events/registry/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/headers.py` & `haupt-2.1.6rc0/haupt/common/headers.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/json_utils.py` & `haupt-2.1.6rc0/haupt/common/json_utils.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/memory_manager.py` & `haupt-2.1.6rc0/haupt/common/memory_manager.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/conf_subscriptions/core.py` & `haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/core.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/conf_subscriptions/installation.py` & `haupt-2.1.6rc0/haupt/common/options/conf_subscriptions/installation.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/feature.py` & `haupt-2.1.6rc0/haupt/common/options/feature.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/option.py` & `haupt-2.1.6rc0/haupt/common/options/option.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/option_manager.py` & `haupt-2.1.6rc0/haupt/common/options/option_manager.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/option_owners.py` & `haupt-2.1.6rc0/haupt/common/options/option_owners.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/registry/cleaning.py` & `haupt-2.1.6rc0/haupt/common/options/registry/cleaning.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/registry/containers.py` & `haupt-2.1.6rc0/haupt/common/options/registry/containers.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/registry/core.py` & `haupt-2.1.6rc0/haupt/common/options/registry/core.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/registry/installation.py` & `haupt-2.1.6rc0/haupt/common/options/registry/installation.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/registry/k8s.py` & `haupt-2.1.6rc0/haupt/common/options/registry/k8s.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/registry/scheduler.py` & `haupt-2.1.6rc0/haupt/common/options/registry/scheduler.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/options/registry/stats.py` & `haupt-2.1.6rc0/haupt/common/options/registry/stats.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/permissions.py` & `haupt-2.1.6rc0/haupt/common/permissions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/query/service.py` & `haupt-2.1.6rc0/haupt/common/query/service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/service_interface.py` & `haupt-2.1.6rc0/haupt/common/service_interface.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/apps.py` & `haupt-2.1.6rc0/haupt/common/settings/apps.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/assets.py` & `haupt-2.1.6rc0/haupt/common/settings/assets.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/celery.py` & `haupt-2.1.6rc0/haupt/common/settings/celery.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/context_processors.py` & `haupt-2.1.6rc0/haupt/common/settings/context_processors.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/core.py` & `haupt-2.1.6rc0/haupt/common/settings/core.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/cors.py` & `haupt-2.1.6rc0/haupt/common/settings/cors.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/defaults.py` & `haupt-2.1.6rc0/haupt/common/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/logging.py` & `haupt-2.1.6rc0/haupt/common/settings/logging.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/middlewares.py` & `haupt-2.1.6rc0/haupt/common/settings/middlewares.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/services/api.py` & `haupt-2.1.6rc0/haupt/common/settings/services/api.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/services/background.py` & `haupt-2.1.6rc0/haupt/common/settings/services/background.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/services/streams.py` & `haupt-2.1.6rc0/haupt/common/settings/services/streams.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/settings/ui.py` & `haupt-2.1.6rc0/haupt/common/settings/ui.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/test_cases/base.py` & `haupt-2.1.6rc0/haupt/common/test_cases/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/test_clients/base.py` & `haupt-2.1.6rc0/haupt/common/test_clients/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/validation/blacklist.py` & `haupt-2.1.6rc0/haupt/common/validation/blacklist.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/validation/slugs.py` & `haupt-2.1.6rc0/haupt/common/validation/slugs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/common/workers.py` & `haupt-2.1.6rc0/haupt/common/workers.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/artifacts.py` & `haupt-2.1.6rc0/haupt/db/abstracts/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/bookmarks.py` & `haupt-2.1.6rc0/haupt/db/abstracts/bookmarks.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/catalogs.py` & `haupt-2.1.6rc0/haupt/db/abstracts/catalogs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/events.py` & `haupt-2.1.6rc0/haupt/db/abstracts/project_versions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,46 @@
-from django.core.validators import validate_slug
 from django.db import models
 
+from haupt.common.validation.slugs import validate_slug_with_dots
+from haupt.db.abstracts.catalogs import BaseCatalog
 from haupt.db.abstracts.contributors import ContributorsModel
-from haupt.db.abstracts.diff import DiffModel
-from haupt.db.abstracts.duration import DurationModel
-from haupt.db.abstracts.nameable import NameableModel
-from haupt.db.abstracts.status import StatusModel
-from haupt.db.abstracts.tag import TagModel
-from haupt.db.abstracts.uid import UuidModel
-from haupt.db.defs import Models
+from haupt.db.abstracts.readme import ReadmeModel
+from haupt.db.abstracts.stage import StageModel
+from haupt.db.abstracts.state import OptionalStateModel
+from polyaxon.schemas import V1ProjectVersionKind
 
 
-class BaseEvent(
-    UuidModel,
-    DiffModel,
-    DurationModel,
-    NameableModel,
-    StatusModel,
-    TagModel,
-    ContributorsModel,
+class BaseProjectVersion(
+    BaseCatalog, StageModel, ReadmeModel, OptionalStateModel, ContributorsModel
 ):
-    name = models.CharField(
-        max_length=128,
-        blank=True,
-        null=True,
-        default=None,
-        validators=[validate_slug],
-    )
-    version = models.ForeignKey(
-        "db.ProjectVersion", on_delete=models.CASCADE, related_name="events"
-    )
-    session = models.CharField(
-        max_length=128,
-        blank=True,
-        null=True,
-        default=None,
+    live_state = None
+
+    kind = models.CharField(
+        max_length=12,
         db_index=True,
-        validators=[validate_slug],
+        choices=V1ProjectVersionKind.to_choices(),
     )
-    user = models.CharField(
-        max_length=128,
+    name = models.CharField(max_length=128, validators=[validate_slug_with_dots])
+    project = models.ForeignKey(
+        "db.Project", on_delete=models.CASCADE, related_name="versions"
+    )
+    content = models.TextField(
+        help_text="The yaml/json content/metadata.",
         blank=True,
         null=True,
-        default=None,
-        db_index=True,
-        validators=[validate_slug],
     )
-    project = models.ForeignKey(
-        Models.get_db_model_name("Project"),
-        on_delete=models.CASCADE,
-        related_name="runs",
+    lineage = models.ManyToManyField(
+        "db.ArtifactLineage", blank=True, related_name="versions"
     )
-    meta_info = models.JSONField(null=True, blank=True, default=dict)
-    inputs = models.JSONField(null=True, blank=True)
-    outputs = models.JSONField(null=True, blank=True)
-    parent = models.ForeignKey(
-        "self",
+    run = models.ForeignKey(
+        "db.Run",
         on_delete=models.CASCADE,
-        related_name="children",
-        null=True,
+        related_name="versions",
         blank=True,
+        null=True,
     )
 
-    class Meta:
+    class Meta(BaseCatalog.Meta):
         abstract = True
         app_label = "db"
-        db_table = "db_event"
-        indexes = [models.Index(fields=["name"])]
+        db_table = "db_projectversion"
+        unique_together = (("project", "name", "kind"),)
```

### Comparing `haupt-2.1.6/haupt/db/abstracts/live_state.py` & `haupt-2.1.6rc0/haupt/db/abstracts/live_state.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/nameable.py` & `haupt-2.1.6rc0/haupt/db/abstracts/nameable.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/run_edges.py` & `haupt-2.1.6rc0/haupt/db/abstracts/run_edges.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/run_pipelines.py` & `haupt-2.1.6rc0/haupt/db/abstracts/run_pipelines.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/runs.py` & `haupt-2.1.6rc0/haupt/db/abstracts/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/stage.py` & `haupt-2.1.6rc0/haupt/db/abstracts/stage.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/stats.py` & `haupt-2.1.6rc0/haupt/db/abstracts/stats.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/status.py` & `haupt-2.1.6rc0/haupt/db/abstracts/status.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/abstracts/tag.py` & `haupt-2.1.6rc0/haupt/db/abstracts/tag.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/administration/projects.py` & `haupt-2.1.6rc0/haupt/db/administration/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/administration/runs.py` & `haupt-2.1.6rc0/haupt/db/administration/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/administration/utils.py` & `haupt-2.1.6rc0/haupt/db/administration/utils.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/defs.py` & `haupt-2.1.6rc0/haupt/db/defs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/factories/users.py` & `haupt-2.1.6rc0/haupt/db/factories/users.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/agents.py` & `haupt-2.1.6rc0/haupt/db/managers/agents.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/artifacts.py` & `haupt-2.1.6rc0/haupt/db/managers/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/bookmarks.py` & `haupt-2.1.6rc0/haupt/db/managers/bookmarks.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/cache.py` & `haupt-2.1.6rc0/haupt/db/managers/cache.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/deleted.py` & `haupt-2.1.6rc0/haupt/db/managers/deleted.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/flows.py` & `haupt-2.1.6rc0/haupt/db/managers/flows.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/live_state.py` & `haupt-2.1.6rc0/haupt/db/managers/live_state.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/projects.py` & `haupt-2.1.6rc0/haupt/db/managers/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/queues.py` & `haupt-2.1.6rc0/haupt/db/managers/queues.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/runs.py` & `haupt-2.1.6rc0/haupt/db/managers/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/stages.py` & `haupt-2.1.6rc0/haupt/db/managers/stages.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/stats.py` & `haupt-2.1.6rc0/haupt/db/managers/stats.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/statuses.py` & `haupt-2.1.6rc0/haupt/db/managers/statuses.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/managers/versions.py` & `haupt-2.1.6rc0/haupt/db/managers/versions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/models/projects.py` & `haupt-2.1.6rc0/haupt/db/models/projects.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0001_initial.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0003_run_pipeline.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0003_run_pipeline.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0004_auto_20200905_1523.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0004_auto_20200905_1523.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0005_auto_20201005_0913.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0005_auto_20201005_0913.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0006_auto_20201020_1705.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0006_auto_20201020_1705.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0007_auto_20201121_1332.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0007_auto_20201121_1332.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0008_run_wait_time.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0008_run_wait_time.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0009_project_unique_name.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0009_project_unique_name.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0010_auto_20210429_1539.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0010_auto_20210429_1539.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0012_alter_artifact_updated_at_and_more.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0012_alter_artifact_updated_at_and_more.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0013_major_upgrade.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0013_major_upgrade.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/pgsql/db/migrations/0014_remove_run_is_managed_project_archived_at_and_duration_wait_time_to_float_and_more.py` & `haupt-2.1.6rc0/haupt/db/pgsql/db/migrations/0014_remove_run_is_managed_project_archived_at_and_duration_wait_time_to_float_and_more.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/queries/artifacts.py` & `haupt-2.1.6rc0/haupt/db/queries/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/queries/runs.py` & `haupt-2.1.6rc0/haupt/db/queries/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/query_managers/artifact.py` & `haupt-2.1.6rc0/haupt/db/query_managers/artifact.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/query_managers/bookmarks.py` & `haupt-2.1.6rc0/haupt/db/query_managers/bookmarks.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/query_managers/callback_conditions.py` & `haupt-2.1.6rc0/haupt/db/query_managers/callback_conditions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/query_managers/project.py` & `haupt-2.1.6rc0/haupt/db/query_managers/project.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/query_managers/project_version.py` & `haupt-2.1.6rc0/haupt/db/query_managers/project_version.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/query_managers/run.py` & `haupt-2.1.6rc0/haupt/db/query_managers/run.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/query_managers/run_edge.py` & `haupt-2.1.6rc0/haupt/db/query_managers/run_edge.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/signals/bookmarks.py` & `haupt-2.1.6rc0/haupt/db/signals/bookmarks.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/signals/runs.py` & `haupt-2.1.6rc0/haupt/db/signals/runs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/signals/versions.py` & `haupt-2.1.6rc0/haupt/db/signals/versions.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/db/sqlite/db/migrations/0001_initial.py` & `haupt-2.1.6rc0/haupt/db/sqlite/db/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/main.py` & `haupt-2.1.6rc0/haupt/main.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/managers/platform.py` & `haupt-2.1.6rc0/haupt/managers/platform.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/managers/proxies.py` & `haupt-2.1.6rc0/haupt/managers/proxies.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/managers/sandbox.py` & `haupt-2.1.6rc0/haupt/managers/sandbox.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/crons/deletion.py` & `haupt-2.1.6rc0/haupt/orchestration/crons/deletion.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/crons/heartbeats.py` & `haupt-2.1.6rc0/haupt/orchestration/crons/heartbeats.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/crons/stats.py` & `haupt-2.1.6rc0/haupt/orchestration/crons/stats.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/executor/__init__.py` & `haupt-2.1.6rc0/haupt/orchestration/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/executor/handlers.py` & `haupt-2.1.6rc0/haupt/orchestration/executor/handlers.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/executor/service.py` & `haupt-2.1.6rc0/haupt/orchestration/executor/service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/operations/service.py` & `haupt-2.1.6rc0/haupt/orchestration/operations/service.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/scheduler/manager.py` & `haupt-2.1.6rc0/haupt/orchestration/scheduler/manager.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/orchestration/scheduler/resolver.py` & `haupt-2.1.6rc0/haupt/orchestration/scheduler/resolver.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/polyconf/asgi/sandbox.py` & `haupt-2.1.6rc0/haupt/polyconf/asgi/sandbox.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/polyconf/asgi/server.py` & `haupt-2.1.6rc0/haupt/polyconf/asgi/server.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/polyconf/asgi/streams.py` & `haupt-2.1.6rc0/haupt/polyconf/asgi/streams.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/polyconf/asgi/viewer.py` & `haupt-2.1.6rc0/haupt/polyconf/asgi/viewer.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/polyconf/config_settings/__init__.py` & `haupt-2.1.6rc0/haupt/polyconf/config_settings/__init__.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/generators/gateway.py` & `haupt-2.1.6rc0/haupt/proxies/generators/gateway.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/api/base.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/api/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/api/uwsgi.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/api/uwsgi.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/auth.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/auth.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/dns.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/dns.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/forward.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/forward.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/gateway/api.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/gateway/api.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/gateway/base.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/gateway/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/locations.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/locations.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/scaffold.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/scaffold.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/server.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/server.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/services.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/services.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/ssl.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/ssl.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/streams/api.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/streams/api.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/streams/base.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/streams/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/streams/k8s.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/streams/k8s.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/proxies/schemas/urls.py` & `haupt-2.1.6rc0/haupt/proxies/schemas/urls.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/schemas/platform_config.py` & `haupt-2.1.6rc0/haupt/schemas/platform_config.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/schemas/proxies_config.py` & `haupt-2.1.6rc0/haupt/schemas/proxies_config.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/schemas/sandbox_config.py` & `haupt-2.1.6rc0/haupt/schemas/sandbox_config.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/settings.py` & `haupt-2.1.6rc0/haupt/settings.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/css/global.min.css` & `haupt-2.1.6rc0/haupt/static/dist/css/global.min.css`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/css/global_modal.min.css` & `haupt-2.1.6rc0/haupt/static/dist/css/global_modal.min.css`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/js/0.bundle.js` & `haupt-2.1.6rc0/haupt/static/dist/js/0.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/js/1.bundle.js` & `haupt-2.1.6rc0/haupt/static/dist/js/1.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/js/2.bundle.js` & `haupt-2.1.6rc0/haupt/static/dist/js/2.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/js/3.bundle.js` & `haupt-2.1.6rc0/haupt/static/dist/js/3.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/js/4.bundle.js` & `haupt-2.1.6rc0/haupt/static/dist/js/4.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/js/5.bundle.js` & `haupt-2.1.6rc0/haupt/static/dist/js/5.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/js/6.bundle.js` & `haupt-2.1.6rc0/haupt/static/dist/js/6.bundle.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/dist/js/7.bundle.js` & `haupt-2.1.6rc0/haupt/static/dist/js/7.bundle.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -26467,15 +26467,15 @@
                 componentDidUpdate() {
                     this.props.isCE && this.props.installationKey && !this.timer && this.setTimer()
                 }
                 componentWillUnmount() {
                     this.clearTimer()
                 }
                 setTimer = () => {
-                    this.timer || (this.timer = setInterval((() => this.props.onFetch(this.props.installationKey, "2-1-6")), 18e5))
+                    this.timer || (this.timer = setInterval((() => this.props.onFetch(this.props.installationKey, "2-1-5")), 18e5))
                 };
                 clearTimer = () => {
                     this.timer && (clearInterval(this.timer), this.timer = null)
                 };
                 onMenuButtonClick = () => {
                     this.setState({
                         isOpen: !this.state.isOpen
@@ -26535,15 +26535,15 @@
                         target: "_blank"
                     }, {
                         name: "Issues",
                         icon: "bug",
                         href: "https://github.com/polyaxon/polyaxon/issues?q=is%3Aopen+is%3Aissue+label%3Abug",
                         target: "_blank"
                     }, {
-                        name: `Polyaxon ${this.props.isCE?"CE ":""}v2.1.6 `,
+                        name: `Polyaxon ${this.props.isCE?"CE ":""}v2.1.5 `,
                         icon: "dot",
                         href: "https://polyaxon.com/docs/releases/2-1/",
                         target: "_blank"
                     }]
                 }];
                 render() {
                     const {
```

### Comparing `haupt-2.1.6/haupt/static/errors/404.html` & `haupt-2.1.6rc0/haupt/static/errors/404.html`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/errors/50x.html` & `haupt-2.1.6rc0/haupt/static/errors/50x.html`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/errors/permission.html` & `haupt-2.1.6rc0/haupt/static/errors/permission.html`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/403.svg` & `haupt-2.1.6rc0/haupt/static/images/403.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/404.svg` & `haupt-2.1.6rc0/haupt/static/images/404.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/50x.svg` & `haupt-2.1.6rc0/haupt/static/images/50x.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-danger.ico` & `haupt-2.1.6rc0/haupt/static/images/favicon-danger.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-danger.svg` & `haupt-2.1.6rc0/haupt/static/images/favicon-danger.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-primary.ico` & `haupt-2.1.6rc0/haupt/static/images/favicon-primary.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-primary.svg` & `haupt-2.1.6rc0/haupt/static/images/favicon-primary.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-running.ico` & `haupt-2.1.6rc0/haupt/static/images/favicon-running.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-running.svg` & `haupt-2.1.6rc0/haupt/static/images/favicon-running.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-stopped.ico` & `haupt-2.1.6rc0/haupt/static/images/favicon-stopped.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-stopped.svg` & `haupt-2.1.6rc0/haupt/static/images/favicon-stopped.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-success.ico` & `haupt-2.1.6rc0/haupt/static/images/favicon-success.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-success.svg` & `haupt-2.1.6rc0/haupt/static/images/favicon-success.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-warning.ico` & `haupt-2.1.6rc0/haupt/static/images/favicon-warning.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon-warning.svg` & `haupt-2.1.6rc0/haupt/static/images/favicon-warning.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon.ico` & `haupt-2.1.6rc0/haupt/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/favicon.svg` & `haupt-2.1.6rc0/haupt/static/images/favicon.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/logo_small.png` & `haupt-2.1.6rc0/haupt/static/images/logo_small.png`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/images/logo_white.svg` & `haupt-2.1.6rc0/haupt/static/images/logo_white.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/dosis/OFL.txt` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/OFL.txt`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.eot` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.svg` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.ttf` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff2` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/dosis/dosis-v8-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/fonts.css` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/fonts.css`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.eot` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.svg` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.ttf` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff2` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-code-pro/source-code-pro-v10-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/OFL.txt` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/OFL.txt`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.eot` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.svg` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.ttf` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff2` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-300.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.eot` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.svg` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.ttf` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff2` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-600.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.eot` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.eot`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.svg` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.svg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.ttf` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff2` & `haupt-2.1.6rc0/haupt/static/vendors/fonts/source-sans-pro/source-sans-pro-v12-latin-ext_cyrillic-ext_cyrillic_greek_greek-ext_latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/bokeh.3.2.0.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/bokeh.3.2.0.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/create-plotly-component.2.6.0.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/create-plotly-component.2.6.0.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/highlight.10.1.2.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/highlight.10.1.2.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/moment-timezone.0.5.32.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/moment-timezone.0.5.32.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/moment.2.30.1.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/moment.2.30.1.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/plotly.2.28.0.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/plotly.2.28.0.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/react-dom.production.18.0.2.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/react-dom.production.18.0.2.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/react.production.18.0.2.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/react.production.18.0.2.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/vega-embed@6.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/vega-embed@6.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/vega-lite@5.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/vega-lite@5.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/static/vendors/js/vega@5.min.js` & `haupt-2.1.6rc0/haupt/static/vendors/js/vega@5.min.js`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/connections/fs.py` & `haupt-2.1.6rc0/haupt/streams/connections/fs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/controllers/events.py` & `haupt-2.1.6rc0/haupt/streams/controllers/events.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/controllers/k8s_check.py` & `haupt-2.1.6rc0/haupt/streams/controllers/k8s_check.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/controllers/logs.py` & `haupt-2.1.6rc0/haupt/streams/controllers/logs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/controllers/notebooks.py` & `haupt-2.1.6rc0/haupt/streams/controllers/notebooks.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/controllers/uploads.py` & `haupt-2.1.6rc0/haupt/streams/controllers/uploads.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/agents.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/agents.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/artifacts.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/artifacts.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/auth_request.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/auth_request.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/base.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/base.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/events.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/events.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/k8s.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/k8s.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/logs.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/logs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/notifications.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/notifications.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/utils.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/utils.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/endpoints/viewer.py` & `haupt-2.1.6rc0/haupt/streams/endpoints/viewer.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/patterns.py` & `haupt-2.1.6rc0/haupt/streams/patterns.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/tasks/logs.py` & `haupt-2.1.6rc0/haupt/streams/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/tasks/notification.py` & `haupt-2.1.6rc0/haupt/streams/tasks/notification.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt/streams/tasks/op_spec.py` & `haupt-2.1.6rc0/haupt/streams/tasks/op_spec.py`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/haupt.egg-info/PKG-INFO` & `haupt-2.1.6rc0/haupt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haupt
-Version: 2.1.6
+Version: 2.1.6rc0
 Summary: Lineage metadata API, artifacts streams, sandbox, ML-API, and spaces for Polyaxon.
 Home-page: https://github.com/polyaxon/haupt
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: AGPLv3
```

### Comparing `haupt-2.1.6/haupt.egg-info/SOURCES.txt` & `haupt-2.1.6rc0/haupt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,14 @@
 haupt/db/abstracts/bookmarks.py
 haupt/db/abstracts/catalogs.py
 haupt/db/abstracts/color.py
 haupt/db/abstracts/contributors.py
 haupt/db/abstracts/describable.py
 haupt/db/abstracts/diff.py
 haupt/db/abstracts/duration.py
-haupt/db/abstracts/events.py
 haupt/db/abstracts/live_state.py
 haupt/db/abstracts/nameable.py
 haupt/db/abstracts/project_versions.py
 haupt/db/abstracts/projects.py
 haupt/db/abstracts/readme.py
 haupt/db/abstracts/run_edges.py
 haupt/db/abstracts/run_pipelines.py
```

### Comparing `haupt-2.1.6/haupt.egg-info/requires.txt` & `haupt-2.1.6rc0/haupt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/setup.cfg` & `haupt-2.1.6rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `haupt-2.1.6/setup.py` & `haupt-2.1.6rc0/setup.py`

 * *Files identical despite different names*

