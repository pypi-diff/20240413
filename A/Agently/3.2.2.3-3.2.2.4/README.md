# Comparing `tmp/Agently-3.2.2.3.tar.gz` & `tmp/Agently-3.2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agently-3.2.2.3.tar", last modified: Mon Apr  8 01:43:54 2024, max compression
+gzip compressed data, was "Agently-3.2.2.4.tar", last modified: Fri Apr 12 08:55:12 2024, max compression
```

## Comparing `Agently-3.2.2.3.tar` & `Agently-3.2.2.4.tar`

### file list

```diff
@@ -1,132 +1,133 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.705184 Agently-3.2.2.3/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.679647 Agently-3.2.2.3/Agently/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.680846 Agently-3.2.2.3/Agently/Agent/
--rw-r--r--   0 moxin      (501) staff       (20)    14078 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Agent/Agent.py
--rw-r--r--   0 moxin      (501) staff       (20)     2259 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Agent/AgentFactory.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Agent/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.681205 Agently-3.2.2.3/Agently/Facility/
--rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Facility/FacilityManager.py
--rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Facility/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.681702 Agently-3.2.2.3/Agently/Request/
--rw-r--r--   0 moxin      (501) staff       (20)     9783 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Request/Request.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Request/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.682118 Agently-3.2.2.3/Agently/WebSocket/
--rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/WebSocket/WebSocket.py
--rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/WebSocket/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.683640 Agently-3.2.2.3/Agently/Workflow/
--rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/Chunk.py
--rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/MainExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/Schema.py
--rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/Workflow.py
--rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.684150 Agently-3.2.2.3/Agently/Workflow/executors/
--rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/executors/StartExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/executors/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/executors/install.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.685869 Agently-3.2.2.3/Agently/Workflow/lib/
--rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/lib/BreakingHub.py
--rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/lib/ChunkExecutorABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/lib/ChunkExecutorManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/lib/Store.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/lib/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/lib/constants.py
--rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/lib/painter.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.687467 Agently-3.2.2.3/Agently/Workflow/utils/
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/utils/exec_tree.py
--rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/utils/find.py
--rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/utils/logger.py
--rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/utils/runtime_supports.py
--rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/utils/verify.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.688483 Agently-3.2.2.3/Agently/Workflow/yamlflow/
--rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/yamlflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.690031 Agently-3.2.2.3/Agently/Workflow/yamlflow/preset_chunks/
--rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/yamlflow/preset_chunks/Print.py
--rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/yamlflow/preset_chunks/Start.py
--rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
--rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/yamlflow/preset_chunks/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     5710 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/Workflow/yamlflow/yamlflow.py
--rw-r--r--   0 moxin      (501) staff       (20)      527 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/_global.py
--rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/global_plugin_manager.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.690259 Agently-3.2.2.3/Agently/plugins/
--rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.694507 Agently-3.2.2.3/Agently/plugins/agent_component/
--rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/Decorator.py
--rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/EventListener.py
--rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/OpenAIAssistant.py
--rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/ReplyReformer.py
--rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/Role.py
--rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/Search.py
--rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/Segment.py
--rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/Session.py
--rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/Status.py
--rw-r--r--   0 moxin      (501) staff       (20)     8963 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/Tool.py
--rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/UserInfo.py
--rw-r--r--   0 moxin      (501) staff       (20)     3062 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/YAMLLoader.py
--rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.694765 Agently-3.2.2.3/Agently/plugins/agent_component/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/utils/ComponentABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/agent_component/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.695461 Agently-3.2.2.3/Agently/plugins/facility/
--rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/facility/Embedding.py
--rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/facility/RoleManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/facility/StatusManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/facility/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/facility/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.695703 Agently-3.2.2.3/Agently/plugins/facility/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/facility/utils/FacilityABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/facility/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.698461 Agently-3.2.2.3/Agently/plugins/request/
--rw-r--r--   0 moxin      (501) staff       (20)     7323 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/Claude.py
--rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/ERNIE.py
--rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/Google.py
--rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/Kimi.py
--rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/MiniMax.py
--rw-r--r--   0 moxin      (501) staff       (20)    15605 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/OAIClient.py
--rw-r--r--   0 moxin      (501) staff       (20)    11446 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/OpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/ZhipuAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.698936 Agently-3.2.2.3/Agently/plugins/request/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/utils/RequestABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      118 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/request/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.699456 Agently-3.2.2.3/Agently/plugins/storage/
--rw-r--r--   0 moxin      (501) staff       (20)     3160 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/storage/FileStorage.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/storage/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/storage/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.699704 Agently-3.2.2.3/Agently/plugins/storage/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/storage/utils/StorageABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/storage/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.700196 Agently-3.2.2.3/Agently/plugins/tool/
--rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/tool/Code.py
--rw-r--r--   0 moxin      (501) staff       (20)     5915 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/tool/Web.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/tool/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/tool/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.700435 Agently-3.2.2.3/Agently/plugins/tool/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/tool/utils/ToolABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/plugins/tool/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      180 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/requirements.txt
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.704043 Agently-3.2.2.3/Agently/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/AliasManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/DataOps.py
--rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/IdGenerator.py
--rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/PluginManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/RuntimeCtx.py
--rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/StorageDelegate.py
--rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/ToolManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/check_version.py
--rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/load_json.py
--rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-08 01:38:47.000000 Agently-3.2.2.3/Agently/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-08 01:43:54.704434 Agently-3.2.2.3/Agently.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      846 2024-04-08 01:43:54.000000 Agently-3.2.2.3/Agently.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)     3745 2024-04-08 01:43:54.000000 Agently-3.2.2.3/Agently.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-08 01:43:54.000000 Agently-3.2.2.3/Agently.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)      130 2024-04-08 01:43:54.000000 Agently-3.2.2.3/Agently.egg-info/requires.txt
--rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-08 01:43:54.000000 Agently-3.2.2.3/Agently.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      846 2024-04-08 01:43:54.704985 Agently-3.2.2.3/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-08 01:43:54.705224 Agently-3.2.2.3/setup.cfg
--rw-------   0 moxin      (501) staff       (20)      974 2024-04-08 01:43:48.000000 Agently-3.2.2.3/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.938737 Agently-3.2.2.4/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.911229 Agently-3.2.2.4/Agently/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.912386 Agently-3.2.2.4/Agently/Agent/
+-rw-r--r--   0 moxin      (501) staff       (20)    14256 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Agent/Agent.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2437 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Agent/AgentFactory.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Agent/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.912752 Agently-3.2.2.4/Agently/Facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Facility/FacilityManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Facility/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.913810 Agently-3.2.2.4/Agently/Request/
+-rw-r--r--   0 moxin      (501) staff       (20)     9783 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Request/Request.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Request/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.914234 Agently-3.2.2.4/Agently/WebSocket/
+-rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/WebSocket/WebSocket.py
+-rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/WebSocket/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.915678 Agently-3.2.2.4/Agently/Workflow/
+-rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/Chunk.py
+-rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/MainExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/Schema.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/Workflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.916254 Agently-3.2.2.4/Agently/Workflow/executors/
+-rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/executors/StartExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/executors/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/executors/install.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.917381 Agently-3.2.2.4/Agently/Workflow/lib/
+-rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/BreakingHub.py
+-rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/ChunkExecutorABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/ChunkExecutorManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/Store.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/constants.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/painter.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.918537 Agently-3.2.2.4/Agently/Workflow/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/exec_tree.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/find.py
+-rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/logger.py
+-rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/runtime_supports.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/verify.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.919725 Agently-3.2.2.4/Agently/Workflow/yamlflow/
+-rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.920561 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/Print.py
+-rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/Start.py
+-rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
+-rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5728 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/yamlflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)      527 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/_global.py
+-rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/global_plugin_manager.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.920750 Agently-3.2.2.4/Agently/plugins/
+-rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.925193 Agently-3.2.2.4/Agently/plugins/agent_component/
+-rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Decorator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/EventListener.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/OpenAIAssistant.py
+-rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/ReplyReformer.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Role.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Search.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Segment.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Session.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Status.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8963 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Tool.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/UserInfo.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3308 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/YAMLLoader.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.925489 Agently-3.2.2.4/Agently/plugins/agent_component/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/utils/ComponentABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.927414 Agently-3.2.2.4/Agently/plugins/facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/Embedding.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/RoleManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/StatusManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.927768 Agently-3.2.2.4/Agently/plugins/facility/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/utils/FacilityABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.930049 Agently-3.2.2.4/Agently/plugins/request/
+-rw-r--r--   0 moxin      (501) staff       (20)     8057 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/Claude.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/ERNIE.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/Google.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/Kimi.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/MiniMax.py
+-rw-r--r--   0 moxin      (501) staff       (20)    13093 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/OAIClient.py
+-rw-r--r--   0 moxin      (501) staff       (20)    11446 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/OpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/ZhipuAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.931714 Agently-3.2.2.4/Agently/plugins/request/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/utils/RequestABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      162 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2728 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/utils/format.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.932509 Agently-3.2.2.4/Agently/plugins/storage/
+-rw-r--r--   0 moxin      (501) staff       (20)     3156 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/FileStorage.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.933043 Agently-3.2.2.4/Agently/plugins/storage/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/utils/StorageABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.933850 Agently-3.2.2.4/Agently/plugins/tool/
+-rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/Code.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5915 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/Web.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.934251 Agently-3.2.2.4/Agently/plugins/tool/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/utils/ToolABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      180 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/requirements.txt
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.938031 Agently-3.2.2.4/Agently/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/AliasManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/DataOps.py
+-rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/IdGenerator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/PluginManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/RuntimeCtx.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/StorageDelegate.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/ToolManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/check_version.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/load_json.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.938285 Agently-3.2.2.4/Agently.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      846 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)     3785 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      130 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/requires.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      846 2024-04-12 08:55:12.938569 Agently-3.2.2.4/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 08:55:12.938890 Agently-3.2.2.4/setup.cfg
+-rw-------   0 moxin      (501) staff       (20)      974 2024-04-12 08:55:08.000000 Agently-3.2.2.4/setup.py
```

### Comparing `Agently-3.2.2.3/Agently/Agent/Agent.py` & `Agently-3.2.2.4/Agently/Agent/Agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,18 @@
         self.agent_storage.table("agent_runtime_ctx").update_by_dict(self.agent_runtime_ctx.get()).save()
         return self
 
     def set_settings(self, settings_key: str, settings_value: any):
         self.settings.set(settings_key, settings_value)
         return self
 
+    def set_global_variable(self, variable_name: str, variable_value: any):
+        self.settings.set(f"global_variables.{ variable_name }", variable_value)
+        return self
+
     def set_agent_prompt(self, key: str, value: any):
         self.agent_runtime_ctx.set(f"prompt.{ key }", value)
         return self
 
     def get_agent_prompt(self, key: str):
         return self.agent_runtime_ctx.get(f"prompt.{ key }")
```

### Comparing `Agently-3.2.2.3/Agently/Agent/AgentFactory.py` & `Agently-3.2.2.4/Agently/Agent/AgentFactory.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,14 +48,18 @@
         self.plugin_manager.register(module_name, plugin_name, plugin)
         return self
 
     def set_settings(self, settings_key: str, settings_value: any):
         self.settings.set(settings_key, settings_value)
         return self
 
+    def set_global_variable(self, variable_name: str, variable_value: any):
+        self.settings.set(f"global_variables.{ variable_name }", variable_value)
+        return self
+
     def toggle_component(self, component_name: str, is_enabled: bool):
         self.set_settings(f"component_toggles.{ component_name }", is_enabled)
         return self
 
     def set_proxy(self, proxy_setting: any):
         self.set_settings("proxy", proxy_setting)
         return self
```

### Comparing `Agently-3.2.2.3/Agently/Facility/FacilityManager.py` & `Agently-3.2.2.4/Agently/Facility/FacilityManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Request/Request.py` & `Agently-3.2.2.4/Agently/Request/Request.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/WebSocket/WebSocket.py` & `Agently-3.2.2.4/Agently/WebSocket/WebSocket.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/Chunk.py` & `Agently-3.2.2.4/Agently/Workflow/Chunk.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/MainExecutor.py` & `Agently-3.2.2.4/Agently/Workflow/MainExecutor.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/Schema.py` & `Agently-3.2.2.4/Agently/Workflow/Schema.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/Workflow.py` & `Agently-3.2.2.4/Agently/Workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/lib/BreakingHub.py` & `Agently-3.2.2.4/Agently/Workflow/lib/BreakingHub.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/lib/ChunkExecutorABC.py` & `Agently-3.2.2.4/Agently/Workflow/lib/ChunkExecutorABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/lib/constants.py` & `Agently-3.2.2.4/Agently/Workflow/lib/constants.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/lib/painter.py` & `Agently-3.2.2.4/Agently/Workflow/lib/painter.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/utils/exec_tree.py` & `Agently-3.2.2.4/Agently/Workflow/utils/exec_tree.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/utils/find.py` & `Agently-3.2.2.4/Agently/Workflow/utils/find.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/utils/logger.py` & `Agently-3.2.2.4/Agently/Workflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/utils/runtime_supports.py` & `Agently-3.2.2.4/Agently/Workflow/utils/runtime_supports.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/yamlflow/preset_chunks/__init__.py` & `Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/Workflow/yamlflow/yamlflow.py` & `Agently-3.2.2.4/Agently/Workflow/yamlflow/yamlflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     if draw:
         return workflow.draw()
     else:
         return workflow.start()
 
 def start_yaml_from_path(workflow, yaml_path, *, draw):
     try:
-        with open(yaml_path, "r") as yaml_file:
+        with open(yaml_path, "r", encoding="utf-8") as yaml_file:
             yaml_dict = yaml.safe_load(yaml_file)
             return start_yaml(workflow, yaml_dict, draw=draw)
     except Exception as e:
         raise Exception(f"[Agently Workflow] Error occured when start YAML from path '{ yaml_path }'.\nError: { str(e) }")
 
 def start_yaml_from_str(workflow, yaml_str, *, draw):
     try:
```

### Comparing `Agently-3.2.2.3/Agently/__init__.py` & `Agently-3.2.2.4/Agently/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/_global.py` & `Agently-3.2.2.4/Agently/_global.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/__init__.py` & `Agently-3.2.2.4/Agently/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/Decorator.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/Decorator.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/EventListener.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/EventListener.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/OpenAIAssistant.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/OpenAIAssistant.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/ReplyReformer.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/ReplyReformer.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/Role.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/Role.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/Search.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/Search.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/Segment.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/Segment.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/Session.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/Session.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/Status.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/Status.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/Tool.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/Tool.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/UserInfo.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/UserInfo.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/YAMLLoader.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/YAMLLoader.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,26 +15,30 @@
             for key, value in target.items():
                 if key == "$type":
                     agently_tuple_list[0] = self.transform_to_agently_style(value, variables=variables)
                 elif key == "$desc":
                     agently_tuple_list[1] = self.transform_to_agently_style(value, variables=variables)
                 else:
                     result.update({ key: self.transform_to_agently_style(value, variables=variables) })
-            if agently_tuple_list[0] and agently_tuple_list[1]:
+            if agently_tuple_list[0] or agently_tuple_list[1]:
                 result = (agently_tuple_list[0], agently_tuple_list[1])
             return result
         if isinstance(target, list):
             result = []
             for item in target:
                 result.append(self.transform_to_agently_style(item, variables=variables))
             return result
         else:
             result = str(target)
             for key, value in variables.items():
                 result = result.replace("${" + str(key) + "}", str(value))
+            global_variables = self.agent.settings.get("global_variables")
+            if global_variables:
+                for key, value in global_variables.items():
+                    result = result.replace("${" + str(key) + "}", str(value))
             return result
 
     def load_yaml_prompt(self, *, path:str=None, yaml:str=None, use_agently_style:bool=True, variables:dict={}):
         # load yaml content
         yaml_dict = {}
         if variables:
             use_agently_style = True
```

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/__init__.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/agent_component/utils/ComponentABC.py` & `Agently-3.2.2.4/Agently/plugins/agent_component/utils/ComponentABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/facility/Embedding.py` & `Agently-3.2.2.4/Agently/plugins/facility/Embedding.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/facility/RoleManager.py` & `Agently-3.2.2.4/Agently/plugins/facility/RoleManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/facility/StatusManager.py` & `Agently-3.2.2.4/Agently/plugins/facility/StatusManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/facility/__init__.py` & `Agently-3.2.2.4/Agently/plugins/facility/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/Claude.py` & `Agently-3.2.2.4/Agently/plugins/request/Claude.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from .utils import RequestABC, to_prompt_structure, to_instruction, to_json_desc, find_json
+from .utils import RequestABC, to_prompt_structure, to_instruction, to_json_desc, find_json, format_request_messages
 from Agently.utils import RuntimeCtxNamespace
 import httpx
 import json
 
 class Claude(RequestABC):
     def __init__(self, request):
         self.request = request
         self.model_name = "Claude"
         self.model_settings = RuntimeCtxNamespace(f"model.{ self.model_name }", self.request.settings)
+        if not self.model_settings.get_trace_back("message_rules.no_multi_system_messages"):
+            self.model_settings.set("message_rules.no_multi_system_messages", False)
+        if not self.model_settings.get_trace_back("message_rules.strict_orders"):
+            self.model_settings.set("message_rules.strict_orders", True)
+        if not self.model_settings.get_trace_back("message_rules.no_multi_type_messages"):
+            self.model_settings.set("message_rules.no_multi_type_messages", False)
         self.default_options = {
             "model": "claude-3-sonnet-20240229",
             "max_tokens": 4096,
             "stream": True,
         }
     
     def construct_request_messages(self):
@@ -68,23 +74,28 @@
                     self.request.request_runtime_ctx.set("response:type", "JSON")
                 else:
                     prompt_dict["[OUTPUT REQUIERMENT]"] = str(prompt_output_data)
             prompt_text = to_prompt_structure(prompt_dict, end="[OUTPUT]:\n")
         request_messages.append({ "role": "user", "content": [{"type": "text", "text": prompt_text }] })
         return request_messages
 
+    
+
     def generate_request_data(self):
         options = self.model_settings.get_trace_back("options", {})
         return {
-            "messages": self.construct_request_messages(),
+            "messages": format_request_messages(self.construct_request_messages(), self.model_settings),
             "options": options,
         }
 
     async def request_model(self, request_data: dict):
         api_key = self.model_settings.get_trace_back("auth.api_key")
+        base_url = self.model_settings.get_trace_back("url", "https://api.anthropic.com/v1")
+        if base_url.endswith("/"):
+            base_url = base_url[:-1]
         proxy = self.request.settings.get_trace_back("proxy")
         messages = request_data["messages"]
         system_prompt = ""
         request_messages = []
         for message in messages:
             if message["role"] == "system":
                 system_prompt += f"{ message['content'][0]['text'] }\n"
@@ -107,15 +118,15 @@
         }
         client_params = {}
         if proxy:
             client_params["proxy"] = proxy
         async with httpx.AsyncClient(**client_params) as client:
             async with client.stream(
                 "POST",
-                "https://api.anthropic.com/v1/messages",
+                f"{ base_url }/messages",
                 **request_params
             ) as response:
                 async for chunk in response.aiter_lines():
                     yield chunk
 
     async def broadcast_response(self, response_generator):
         full_message = {}
```

### Comparing `Agently-3.2.2.3/Agently/plugins/request/ERNIE.py` & `Agently-3.2.2.4/Agently/plugins/request/ERNIE.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/Google.py` & `Agently-3.2.2.4/Agently/plugins/request/Google.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/Kimi.py` & `Agently-3.2.2.4/Agently/plugins/request/Kimi.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/MiniMax.py` & `Agently-3.2.2.4/Agently/plugins/request/MiniMax.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/OAIClient.py` & `Agently-3.2.2.4/Agently/plugins/request/OAIClient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from openai import AsyncOpenAI as OpenAIClient
-from .utils import RequestABC, to_prompt_structure, to_instruction, to_json_desc, find_json
+from .utils import RequestABC, to_prompt_structure, to_instruction, to_json_desc, find_json, format_request_messages
 from Agently.utils import RuntimeCtxNamespace
 import httpx
 import json
 
 class OAIClient(RequestABC):
     def __init__(self, request):
         self.request = request
@@ -72,66 +72,14 @@
                     self.request.request_runtime_ctx.set("response:type", "JSON")
                 else:
                     prompt_dict["[OUTPUT REQUIERMENT]"] = str(prompt_output_data)
             prompt_text = to_prompt_structure(prompt_dict, end="[OUTPUT]:\n")
         request_messages.append({ "role": "user", "content": [{"type": "text", "text": prompt_text }] })
         return request_messages
 
-    def format_request_messages(self, request_messages):
-        system_prompt = ""
-        system_messages = []
-        chat_messages = []
-        role_list = ["user", "assistant"]
-        current_role = 0
-        for message in request_messages:
-            if message["role"] == "system":
-                # no_multi_system_messages=True
-                if self.model_settings.get_trace_back("message_rules.no_multi_system_messages"):
-                    for content in message["content"]:
-                        if content["type"] == "text":
-                            system_prompt += f"{ content['text'] }\n"
-                # no_multi_system_messages=False
-                else:
-                    system_messages.append(message)
-            else:
-                # strict_orders=True
-                if self.model_settings.get_trace_back("message_rules.strict_orders"):
-                    if len(chat_messages) == 0 and message["role"] != "user":
-                        chat_messages.append({ "role": "user", "content": "What did we talked about?" })
-                        current_role = not current_role
-                    if message["role"] == role_list[current_role]:
-                        chat_messages.append(message)
-                        current_role = not current_role
-                    else:
-                        content = f"{ chat_messages[-1]['content'] }\n{ message['content'] }"
-                        chat_messages[-1]['content'] = content
-                # strict_orders=False
-                else:
-                    chat_messages.append(message)
-        # no_multi_system_messages=True
-        if self.model_settings.get_trace_back("message_rules.no_multi_system_messages") and system_prompt != "":
-            system_messages.append({
-                "role": "system",
-                "content": [{
-                    "type": "text",
-                    "text": system_prompt
-                }]
-            })
-        formatted_messages = system_messages.copy()
-        formatted_messages.extend(chat_messages)
-        # no_multi_type_messages=True
-        if self.model_settings.get_trace_back("message_rules.no_multi_type_messages"):
-            current_messages = formatted_messages.copy()
-            formatted_messages = []
-            for message in current_messages:
-                for item in message["content"]:
-                    if item["type"] == "text":
-                        formatted_messages.append({ "role": message["role"], "content": item["text"] })
-        return formatted_messages
-
     def construct_completion_prompt(self):
         # - init prompt
         completion_prompt = ""
         # - general instruction
         general_instruction_data = self.request.request_runtime_ctx.get_trace_back("prompt.general")
         if general_instruction_data:
             completion_prompt += f"[GENERAL INSTRUCTION]\n{ to_instruction(general_instruction_data) }\n"
@@ -214,15 +162,15 @@
         # collect options
         options = self.model_settings.get_trace_back("options", {})
         for key, value in self.default_options.items():
             if key not in options:
                 options.update({ key: value })
         if self.request_type == "chat":
             return {
-                "messages": self.format_request_messages(self.construct_request_messages()),
+                "messages": format_request_messages(self.construct_request_messages(), self.model_settings),
                 **options,
             }
         elif self.request_type == "completions":
             return {
                 "prompt": self.construct_completion_prompt(),
                 **options,
             }
```

### Comparing `Agently-3.2.2.3/Agently/plugins/request/OpenAI.py` & `Agently-3.2.2.4/Agently/plugins/request/OpenAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/ZhipuAI.py` & `Agently-3.2.2.4/Agently/plugins/request/ZhipuAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/__init__.py` & `Agently-3.2.2.4/Agently/plugins/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/utils/RequestABC.py` & `Agently-3.2.2.4/Agently/plugins/request/utils/RequestABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/request/utils/transform.py` & `Agently-3.2.2.4/Agently/plugins/request/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/storage/FileStorage.py` & `Agently-3.2.2.4/Agently/plugins/storage/FileStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import json
 from .utils import StorageABC
 
 class FileStorage(StorageABC):
     def __init__(self, db_name: str="default"):
         self.db_name = db_name
-        self.path = "./file_storage"
+        self.path = "./.Agently"
         if not os.path.exists(self.path):
             os.mkdir(self.path)
 
     def __load_from_file(self, table_name: str):
         if not os.path.exists(f"{ self.path }/{ self.db_name }/{ table_name }.data"):
             return {}
         else:
```

### Comparing `Agently-3.2.2.3/Agently/plugins/storage/__init__.py` & `Agently-3.2.2.4/Agently/plugins/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/storage/utils/StorageABC.py` & `Agently-3.2.2.4/Agently/plugins/storage/utils/StorageABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/tool/Code.py` & `Agently-3.2.2.4/Agently/plugins/tool/Code.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/tool/Web.py` & `Agently-3.2.2.4/Agently/plugins/tool/Web.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/plugins/tool/__init__.py` & `Agently-3.2.2.4/Agently/plugins/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/AliasManager.py` & `Agently-3.2.2.4/Agently/utils/AliasManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/DataOps.py` & `Agently-3.2.2.4/Agently/utils/DataOps.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/PluginManager.py` & `Agently-3.2.2.4/Agently/utils/PluginManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/RuntimeCtx.py` & `Agently-3.2.2.4/Agently/utils/RuntimeCtx.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/StorageDelegate.py` & `Agently-3.2.2.4/Agently/utils/StorageDelegate.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/ToolManager.py` & `Agently-3.2.2.4/Agently/utils/ToolManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/check_version.py` & `Agently-3.2.2.4/Agently/utils/check_version.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/load_json.py` & `Agently-3.2.2.4/Agently/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently/utils/transform.py` & `Agently-3.2.2.4/Agently/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.3/Agently.egg-info/PKG-INFO` & `Agently-3.2.2.4/Agently.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.3
+Version: 3.2.2.4
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.2.3/Agently.egg-info/SOURCES.txt` & `Agently-3.2.2.4/Agently.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 Agently/plugins/request/OAIClient.py
 Agently/plugins/request/OpenAI.py
 Agently/plugins/request/ZhipuAI.py
 Agently/plugins/request/__init__.py
 Agently/plugins/request/config.ini
 Agently/plugins/request/utils/RequestABC.py
 Agently/plugins/request/utils/__init__.py
+Agently/plugins/request/utils/format.py
 Agently/plugins/request/utils/transform.py
 Agently/plugins/storage/FileStorage.py
 Agently/plugins/storage/__init__.py
 Agently/plugins/storage/config.ini
 Agently/plugins/storage/utils/StorageABC.py
 Agently/plugins/storage/utils/__init__.py
 Agently/plugins/tool/Code.py
```

### Comparing `Agently-3.2.2.3/PKG-INFO` & `Agently-3.2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.3
+Version: 3.2.2.4
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Agently-3.2.2.3/setup.py` & `Agently-3.2.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 requirements = []
 for requirement in origin_requirements:
     if not requirement.startswith("#"):
         requirements.append(requirement)
 
 setuptools.setup(
     name = "Agently",
-    version = "3.2.2.3",
+    version = "3.2.2.4",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently, a framework to build applications based on language model powered intelligent agents.",
     long_description = "https://github.com/Maplemx/Agently",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
     packages = setuptools.find_packages(),
```

