# Comparing `tmp/Agently-3.2.2.4.tar.gz` & `tmp/Agently-3.3.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agently-3.2.2.4.tar", last modified: Fri Apr 12 08:55:12 2024, max compression
+gzip compressed data, was "Agently-3.3.0.0a6.tar", last modified: Sat Apr 13 09:29:57 2024, max compression
```

## Comparing `Agently-3.2.2.4.tar` & `Agently-3.3.0.0a6.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.938737 Agently-3.2.2.4/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.911229 Agently-3.2.2.4/Agently/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.912386 Agently-3.2.2.4/Agently/Agent/
--rw-r--r--   0 moxin      (501) staff       (20)    14256 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Agent/Agent.py
--rw-r--r--   0 moxin      (501) staff       (20)     2437 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Agent/AgentFactory.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Agent/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.912752 Agently-3.2.2.4/Agently/Facility/
--rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Facility/FacilityManager.py
--rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Facility/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.913810 Agently-3.2.2.4/Agently/Request/
--rw-r--r--   0 moxin      (501) staff       (20)     9783 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Request/Request.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Request/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.914234 Agently-3.2.2.4/Agently/WebSocket/
--rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/WebSocket/WebSocket.py
--rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/WebSocket/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.915678 Agently-3.2.2.4/Agently/Workflow/
--rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/Chunk.py
--rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/MainExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/Schema.py
--rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/Workflow.py
--rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.916254 Agently-3.2.2.4/Agently/Workflow/executors/
--rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/executors/StartExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/executors/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/executors/install.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.917381 Agently-3.2.2.4/Agently/Workflow/lib/
--rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/BreakingHub.py
--rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/ChunkExecutorABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/ChunkExecutorManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/Store.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/constants.py
--rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/lib/painter.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.918537 Agently-3.2.2.4/Agently/Workflow/utils/
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/exec_tree.py
--rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/find.py
--rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/logger.py
--rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/runtime_supports.py
--rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/utils/verify.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.919725 Agently-3.2.2.4/Agently/Workflow/yamlflow/
--rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.920561 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/
--rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/Print.py
--rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/Start.py
--rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
--rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     5728 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/Workflow/yamlflow/yamlflow.py
--rw-r--r--   0 moxin      (501) staff       (20)      527 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/_global.py
--rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/global_plugin_manager.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.920750 Agently-3.2.2.4/Agently/plugins/
--rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.925193 Agently-3.2.2.4/Agently/plugins/agent_component/
--rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Decorator.py
--rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/EventListener.py
--rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/OpenAIAssistant.py
--rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/ReplyReformer.py
--rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Role.py
--rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Search.py
--rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Segment.py
--rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Session.py
--rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Status.py
--rw-r--r--   0 moxin      (501) staff       (20)     8963 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/Tool.py
--rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/UserInfo.py
--rw-r--r--   0 moxin      (501) staff       (20)     3308 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/YAMLLoader.py
--rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.925489 Agently-3.2.2.4/Agently/plugins/agent_component/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/utils/ComponentABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/agent_component/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.927414 Agently-3.2.2.4/Agently/plugins/facility/
--rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/Embedding.py
--rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/RoleManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/StatusManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.927768 Agently-3.2.2.4/Agently/plugins/facility/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/utils/FacilityABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/facility/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.930049 Agently-3.2.2.4/Agently/plugins/request/
--rw-r--r--   0 moxin      (501) staff       (20)     8057 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/Claude.py
--rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/ERNIE.py
--rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/Google.py
--rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/Kimi.py
--rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/MiniMax.py
--rw-r--r--   0 moxin      (501) staff       (20)    13093 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/OAIClient.py
--rw-r--r--   0 moxin      (501) staff       (20)    11446 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/OpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/ZhipuAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.931714 Agently-3.2.2.4/Agently/plugins/request/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/utils/RequestABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      162 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     2728 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/utils/format.py
--rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/request/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.932509 Agently-3.2.2.4/Agently/plugins/storage/
--rw-r--r--   0 moxin      (501) staff       (20)     3156 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/FileStorage.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.933043 Agently-3.2.2.4/Agently/plugins/storage/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/utils/StorageABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/storage/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.933850 Agently-3.2.2.4/Agently/plugins/tool/
--rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/Code.py
--rw-r--r--   0 moxin      (501) staff       (20)     5915 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/Web.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.934251 Agently-3.2.2.4/Agently/plugins/tool/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/utils/ToolABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/plugins/tool/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      180 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/requirements.txt
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.938031 Agently-3.2.2.4/Agently/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/AliasManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/DataOps.py
--rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/IdGenerator.py
--rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/PluginManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/RuntimeCtx.py
--rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/StorageDelegate.py
--rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/ToolManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/check_version.py
--rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/load_json.py
--rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-12 08:54:36.000000 Agently-3.2.2.4/Agently/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-12 08:55:12.938285 Agently-3.2.2.4/Agently.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      846 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)     3785 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)      130 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/requires.txt
--rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-12 08:55:12.000000 Agently-3.2.2.4/Agently.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      846 2024-04-12 08:55:12.938569 Agently-3.2.2.4/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 08:55:12.938890 Agently-3.2.2.4/setup.cfg
--rw-------   0 moxin      (501) staff       (20)      974 2024-04-12 08:55:08.000000 Agently-3.2.2.4/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.608206 Agently-3.3.0.0a6/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.541693 Agently-3.3.0.0a6/Agently/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.542864 Agently-3.3.0.0a6/Agently/Agent/
+-rw-r--r--   0 moxin      (501) staff       (20)    14256 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Agent/Agent.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2437 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Agent/AgentFactory.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Agent/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.543395 Agently-3.3.0.0a6/Agently/Facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Facility/FacilityManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Facility/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.544841 Agently-3.3.0.0a6/Agently/Request/
+-rw-r--r--   0 moxin      (501) staff       (20)     9783 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Request/Request.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Request/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.545208 Agently-3.3.0.0a6/Agently/WebSocket/
+-rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/WebSocket/WebSocket.py
+-rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/WebSocket/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.546520 Agently-3.3.0.0a6/Agently/Workflow/
+-rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/Chunk.py
+-rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/MainExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/Schema.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/Workflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.547062 Agently-3.3.0.0a6/Agently/Workflow/executors/
+-rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/executors/StartExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/executors/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/executors/install.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.549071 Agently-3.3.0.0a6/Agently/Workflow/lib/
+-rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/BreakingHub.py
+-rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/ChunkExecutorABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/ChunkExecutorManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/Store.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/constants.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/painter.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.551755 Agently-3.3.0.0a6/Agently/Workflow/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/exec_tree.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/find.py
+-rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/logger.py
+-rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/runtime_supports.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/verify.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.552207 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/
+-rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.553832 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/Print.py
+-rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/Start.py
+-rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
+-rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5728 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/yamlflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)      569 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/_global.py
+-rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/global_plugin_manager.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.554032 Agently-3.3.0.0a6/Agently/plugins/
+-rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.577741 Agently-3.3.0.0a6/Agently/plugins/agent_component/
+-rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Decorator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/EventListener.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/OpenAIAssistant.py
+-rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/ReplyReformer.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Role.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Search.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Segment.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Session.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Status.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8963 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Tool.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/UserInfo.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3308 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/YAMLLoader.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.578150 Agently-3.3.0.0a6/Agently/plugins/agent_component/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/utils/ComponentABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.579956 Agently-3.3.0.0a6/Agently/plugins/facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/Embedding.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/RoleManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/StatusManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.580856 Agently-3.3.0.0a6/Agently/plugins/facility/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/utils/FacilityABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.584323 Agently-3.3.0.0a6/Agently/plugins/request/
+-rw-r--r--   0 moxin      (501) staff       (20)    11956 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/AzureOpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8057 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/Claude.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/ERNIE.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/Google.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/Kimi.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/MiniMax.py
+-rw-r--r--   0 moxin      (501) staff       (20)    13093 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/OAIClient.py
+-rw-r--r--   0 moxin      (501) staff       (20)    11670 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/OpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/ZhipuAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.584880 Agently-3.3.0.0a6/Agently/plugins/request/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/utils/RequestABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      162 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2728 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/utils/format.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.600946 Agently-3.3.0.0a6/Agently/plugins/storage/
+-rw-r--r--   0 moxin      (501) staff       (20)     3156 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/FileStorage.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.601511 Agently-3.3.0.0a6/Agently/plugins/storage/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/utils/StorageABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.602583 Agently-3.3.0.0a6/Agently/plugins/tool/
+-rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/Code.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5915 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/Web.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.602962 Agently-3.3.0.0a6/Agently/plugins/tool/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/utils/ToolABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-13 09:28:26.000000 Agently-3.3.0.0a6/Agently/requirements.txt
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.607517 Agently-3.3.0.0a6/Agently/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/AliasManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/DataOps.py
+-rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/IdGenerator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/PluginManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/RuntimeCtx.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/StorageDelegate.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/ToolManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/check_version.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/load_json.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.607753 Agently-3.3.0.0a6/Agently.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      913 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)     3824 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      163 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/requires.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      913 2024-04-13 09:29:57.608008 Agently-3.3.0.0a6/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-13 09:29:57.608244 Agently-3.3.0.0a6/setup.cfg
+-rw-------   0 moxin      (501) staff       (20)     1014 2024-04-13 09:24:41.000000 Agently-3.3.0.0a6/setup.py
```

### Comparing `Agently-3.2.2.4/Agently/Agent/Agent.py` & `Agently-3.3.0.0a6/Agently/Agent/Agent.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Agent/AgentFactory.py` & `Agently-3.3.0.0a6/Agently/Agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Facility/FacilityManager.py` & `Agently-3.3.0.0a6/Agently/Facility/FacilityManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Request/Request.py` & `Agently-3.3.0.0a6/Agently/Request/Request.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/WebSocket/WebSocket.py` & `Agently-3.3.0.0a6/Agently/WebSocket/WebSocket.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/Chunk.py` & `Agently-3.3.0.0a6/Agently/Workflow/Chunk.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/MainExecutor.py` & `Agently-3.3.0.0a6/Agently/Workflow/MainExecutor.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/Schema.py` & `Agently-3.3.0.0a6/Agently/Workflow/Schema.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/Workflow.py` & `Agently-3.3.0.0a6/Agently/Workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/lib/BreakingHub.py` & `Agently-3.3.0.0a6/Agently/Workflow/lib/BreakingHub.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/lib/ChunkExecutorABC.py` & `Agently-3.3.0.0a6/Agently/Workflow/lib/ChunkExecutorABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/lib/constants.py` & `Agently-3.3.0.0a6/Agently/Workflow/lib/constants.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/lib/painter.py` & `Agently-3.3.0.0a6/Agently/Workflow/lib/painter.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/utils/exec_tree.py` & `Agently-3.3.0.0a6/Agently/Workflow/utils/exec_tree.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/utils/find.py` & `Agently-3.3.0.0a6/Agently/Workflow/utils/find.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/utils/logger.py` & `Agently-3.3.0.0a6/Agently/Workflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/utils/runtime_supports.py` & `Agently-3.3.0.0a6/Agently/Workflow/utils/runtime_supports.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/yamlflow/preset_chunks/__init__.py` & `Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/Workflow/yamlflow/yamlflow.py` & `Agently-3.3.0.0a6/Agently/Workflow/yamlflow/yamlflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/__init__.py` & `Agently-3.3.0.0a6/Agently/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import nest_asyncio
 from .Request import Request
 from .Agent import AgentFactory
 from .Facility import FacilityManager
 from .WebSocket import WebSocketServer, WebSocketClient
 from .Workflow import Workflow, Schema as WorkflowSchema
 from ._global import global_plugin_manager, global_settings, global_storage, global_tool_manager, global_websocket_server
 from .utils import *
 
+nest_asyncio.apply()
+
 def create_agent(*args, **kwargs):
     return AgentFactory().create_agent(*args, **kwargs)
 
 facility = FacilityManager()
 lib = facility
 
 set_settings = global_settings.set
```

### Comparing `Agently-3.2.2.4/Agently/_global.py` & `Agently-3.3.0.0a6/Agently/_global.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/Decorator.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Decorator.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/EventListener.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/EventListener.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/OpenAIAssistant.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/OpenAIAssistant.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/ReplyReformer.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/ReplyReformer.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/Role.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Role.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/Search.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Search.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/Segment.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Segment.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/Session.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Session.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/Status.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Status.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/Tool.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Tool.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/UserInfo.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/UserInfo.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/YAMLLoader.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/YAMLLoader.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/agent_component/utils/ComponentABC.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/utils/ComponentABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/facility/Embedding.py` & `Agently-3.3.0.0a6/Agently/plugins/facility/Embedding.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/facility/RoleManager.py` & `Agently-3.3.0.0a6/Agently/plugins/facility/RoleManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/facility/StatusManager.py` & `Agently-3.3.0.0a6/Agently/plugins/facility/StatusManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/facility/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/facility/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/Claude.py` & `Agently-3.3.0.0a6/Agently/plugins/request/Claude.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/ERNIE.py` & `Agently-3.3.0.0a6/Agently/plugins/request/ERNIE.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/Google.py` & `Agently-3.3.0.0a6/Agently/plugins/request/Google.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/Kimi.py` & `Agently-3.3.0.0a6/Agently/plugins/request/Kimi.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/MiniMax.py` & `Agently-3.3.0.0a6/Agently/plugins/request/MiniMax.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/OAIClient.py` & `Agently-3.3.0.0a6/Agently/plugins/request/OAIClient.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/OpenAI.py` & `Agently-3.3.0.0a6/Agently/plugins/request/OpenAI.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,22 +206,25 @@
 
     async def broadcast_response_without_streaming(self, response):
         yield({ "event": "response:done", "data": response })
 
     async def broadcast_response_with_streaming(self, response_generator):
         response_message = {}
         async for part in response_generator:
-            delta = dict(part.choices[0].delta)
-            for key, value in delta.items():
-                if key not in response_message:
-                    response_message[key] = value or ""
-                else:
-                    response_message[key] += value or ""
-            yield({ "event": "response:delta_origin", "data": part })
-            yield({ "event": "response:delta", "data": part.choices[0].delta.content or "" })
+            if "choices" in dir(part) and isinstance(part.choices, list) and len(part.choices) > 0:
+                delta = dict(part.choices[0].delta)
+                for key, value in delta.items():
+                    if key not in response_message:
+                        response_message[key] = value or ""
+                    else:
+                        response_message[key] += value or ""
+                yield({ "event": "response:delta_origin", "data": part })
+                yield({ "event": "response:delta", "data": part.choices[0].delta.content or "" })
+            else:
+                yield({ "event": "response:delta_origin", "data": part })
         yield({ "event": "response:done_origin", "data": response_message })
         yield({ "event": "response:done", "data": response_message["content"] })
 
     async def broadcast_response(self, response_generator):
         if self.use_assistant and self.request_type == "chat":
             return self.broadcast_response_without_streaming(response_generator)
         elif self.request_type == "chat":
```

### Comparing `Agently-3.2.2.4/Agently/plugins/request/ZhipuAI.py` & `Agently-3.3.0.0a6/Agently/plugins/request/ZhipuAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/utils/RequestABC.py` & `Agently-3.3.0.0a6/Agently/plugins/request/utils/RequestABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/utils/format.py` & `Agently-3.3.0.0a6/Agently/plugins/request/utils/format.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/request/utils/transform.py` & `Agently-3.3.0.0a6/Agently/plugins/request/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/storage/FileStorage.py` & `Agently-3.3.0.0a6/Agently/plugins/storage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/storage/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/storage/utils/StorageABC.py` & `Agently-3.3.0.0a6/Agently/plugins/storage/utils/StorageABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/tool/Code.py` & `Agently-3.3.0.0a6/Agently/plugins/tool/Code.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/tool/Web.py` & `Agently-3.3.0.0a6/Agently/plugins/tool/Web.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/plugins/tool/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/AliasManager.py` & `Agently-3.3.0.0a6/Agently/utils/AliasManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/DataOps.py` & `Agently-3.3.0.0a6/Agently/utils/DataOps.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/PluginManager.py` & `Agently-3.3.0.0a6/Agently/utils/PluginManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/RuntimeCtx.py` & `Agently-3.3.0.0a6/Agently/utils/RuntimeCtx.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/StorageDelegate.py` & `Agently-3.3.0.0a6/Agently/utils/StorageDelegate.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/ToolManager.py` & `Agently-3.3.0.0a6/Agently/utils/ToolManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/check_version.py` & `Agently-3.3.0.0a6/Agently/utils/check_version.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/load_json.py` & `Agently-3.3.0.0a6/Agently/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently/utils/transform.py` & `Agently-3.3.0.0a6/Agently/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.4/Agently.egg-info/SOURCES.txt` & `Agently-3.3.0.0a6/Agently.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 Agently/plugins/facility/Embedding.py
 Agently/plugins/facility/RoleManager.py
 Agently/plugins/facility/StatusManager.py
 Agently/plugins/facility/__init__.py
 Agently/plugins/facility/config.ini
 Agently/plugins/facility/utils/FacilityABC.py
 Agently/plugins/facility/utils/__init__.py
+Agently/plugins/request/AzureOpenAI.py
 Agently/plugins/request/Claude.py
 Agently/plugins/request/ERNIE.py
 Agently/plugins/request/Google.py
 Agently/plugins/request/Kimi.py
 Agently/plugins/request/MiniMax.py
 Agently/plugins/request/OAIClient.py
 Agently/plugins/request/OpenAI.py
```

### Comparing `Agently-3.2.2.4/setup.py` & `Agently-3.3.0.0a6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,28 @@
     origin_requirements = f.read().splitlines()
 
 requirements = []
 for requirement in origin_requirements:
     if not requirement.startswith("#"):
         requirements.append(requirement)
 
+
 setuptools.setup(
     name = "Agently",
-    version = "3.2.2.4",
+    version = "3.3.0.0-alpha-6",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently, a framework to build applications based on language model powered intelligent agents.",
     long_description = "https://github.com/Maplemx/Agently",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
+    #packages = ["Agently"],
     packages = setuptools.find_packages(),
     package_data = {"": ["*.txt", "*.ini"]},
     install_requires= requirements,
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3',
+    python_requires=">=3.8",
 )
```

