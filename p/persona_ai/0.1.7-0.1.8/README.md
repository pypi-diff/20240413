# Comparing `tmp/persona_ai-0.1.7.tar.gz` & `tmp/persona_ai-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persona_ai-0.1.7.tar", max compression
+gzip compressed data, was "persona_ai-0.1.8.tar", max compression
```

## Comparing `persona_ai-0.1.7.tar` & `persona_ai-0.1.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0    11250 2024-04-11 10:00:15.400629 persona_ai-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/code_runners/__init__.py
--rw-r--r--   0        0        0     1239 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/code_runners/base.py
--rw-r--r--   0        0        0     2363 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/code_runners/local.py
--rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/constants.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/conversation_listeners/__init__.py
--rw-r--r--   0        0        0     5963 2024-04-11 11:06:54.667592 persona_ai-0.1.7/persona_ai/conversation_listeners/terminal.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/conversations/__init__.py
--rw-r--r--   0        0        0     3214 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/conversations/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/domain/__init__.py
--rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/domain/conversations.py
--rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/domain/events.py
--rw-r--r--   0        0        0     1172 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/domain/repositories.py
--rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/domain/roles.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/domain/schemas/__init__.py
--rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/domain/schemas/crud.py
--rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/domain/tasks.py
--rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/domain/utils.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/infrastructure/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      758 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/infrastructure/repositories/base.py
--rw-r--r--   0        0        0     1967 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/infrastructure/repositories/in_memory.py
--rw-r--r--   0        0        0     2884 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/infrastructure/repositories/mongo.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/initializers/__init__.py
--rw-r--r--   0        0        0     4362 2024-04-11 10:13:24.751773 persona_ai-0.1.7/persona_ai/initializers/env_configurator.py
--rw-r--r--   0        0        0     1012 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/initializers/persona_configuration.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/models/__init__.py
--rw-r--r--   0        0        0      870 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/models/base.py
--rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/models/code_bison.py
--rw-r--r--   0        0        0    10057 2024-04-11 14:30:12.657119 persona_ai-0.1.7/persona_ai/models/gemini.py
--rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/models/text_bison.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/moderation/__init__.py
--rw-r--r--   0        0        0     2907 2024-04-11 14:00:13.990403 persona_ai-0.1.7/persona_ai/moderation/ai_moderator.py
--rw-r--r--   0        0        0     7345 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/moderation/base.py
--rw-r--r--   0        0        0     4475 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/moderation/history_moderator.py
--rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/moderation/history_moderator_fc.py
--rw-r--r--   0        0        0     5580 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/moderation/react_moderator.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/personas/__init__.py
--rw-r--r--   0        0        0     6678 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/personas/agent.py
--rw-r--r--   0        0        0     4221 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/personas/assistant.py
--rw-r--r--   0        0        0     6504 2024-04-11 10:53:55.133342 persona_ai-0.1.7/persona_ai/personas/base.py
--rw-r--r--   0        0        0     3805 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/personas/coder.py
--rw-r--r--   0        0        0    13267 2024-04-11 11:05:25.442988 persona_ai-0.1.7/persona_ai/personas/party.py
--rw-r--r--   0        0        0     3023 2024-04-11 14:30:55.936715 persona_ai-0.1.7/persona_ai/personas/technician.py
--rw-r--r--   0        0        0      760 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/personas/terminal.py
--rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/agent.jinja2
--rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/assistant.jinja2
--rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/coder.jinja2
--rw-r--r--   0        0        0     1194 2024-04-11 15:04:24.559375 persona_ai-0.1.7/persona_ai/prompt_templates/history_moderator.jinja2
--rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/history_moderator_fc.jinja2
--rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/react_json_moderator.jinja2
--rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/react_moderator.jinja2
--rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/refiner.jinja2
--rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
--rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
--rw-r--r--   0        0        0      102 2024-04-11 14:33:38.412861 persona_ai-0.1.7/persona_ai/prompt_templates/technician.jinja2
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/prompts/__init__.py
--rw-r--r--   0        0        0      238 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/prompts/base.py
--rw-r--r--   0        0        0     2207 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/prompts/jinja.py
--rw-r--r--   0        0        0      588 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/prompts/text.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/refiners/__init__.py
--rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/refiners/request_refiner.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/task_manager/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/task_manager/base.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/tools/__init__.py
--rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/tools/base.py
--rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/tools/functional.py
--rw-r--r--   0        0        0      730 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/tools/manager.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/transport/__init__.py
--rw-r--r--   0        0        0     3477 2024-04-11 13:57:49.665513 persona_ai-0.1.7/persona_ai/transport/local/local_messagebus.py
--rw-r--r--   0        0        0     4022 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/transport/messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/transport/rabbitmq/__init__.py
--rw-r--r--   0        0        0    10002 2024-04-11 10:00:15.400629 persona_ai-0.1.7/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
--rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/utils/__init__.py
--rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/utils/crypto.py
--rw-r--r--   0        0        0      750 2024-04-08 06:52:52.049183 persona_ai-0.1.7/persona_ai/utils/extractors.py
--rw-r--r--   0        0        0     1139 2024-04-11 16:07:12.885667 persona_ai-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    12755 1970-01-01 00:00:00.000000 persona_ai-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    11250 2024-04-11 10:00:15.400629 persona_ai-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/code_runners/__init__.py
+-rw-r--r--   0        0        0     1239 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/code_runners/base.py
+-rw-r--r--   0        0        0     2363 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/code_runners/local.py
+-rw-r--r--   0        0        0      153 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/constants.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/conversation_listeners/__init__.py
+-rw-r--r--   0        0        0     6058 2024-04-13 08:46:20.890471 persona_ai-0.1.8/persona_ai/conversation_listeners/terminal_conversation_listener.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/conversations/__init__.py
+-rw-r--r--   0        0        0     3214 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/conversations/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/__init__.py
+-rw-r--r--   0        0        0     6372 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/conversations.py
+-rw-r--r--   0        0        0      767 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/events.py
+-rw-r--r--   0        0        0     1172 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/domain/repositories.py
+-rw-r--r--   0        0        0       82 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/roles.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/schemas/__init__.py
+-rw-r--r--   0        0        0      600 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/schemas/crud.py
+-rw-r--r--   0        0        0     2759 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/tasks.py
+-rw-r--r--   0        0        0      146 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/domain/utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/infrastructure/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      758 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/infrastructure/repositories/base.py
+-rw-r--r--   0        0        0     1967 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/infrastructure/repositories/in_memory.py
+-rw-r--r--   0        0        0     2884 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/infrastructure/repositories/mongo.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/initializers/__init__.py
+-rw-r--r--   0        0        0     4362 2024-04-11 10:13:24.751773 persona_ai-0.1.8/persona_ai/initializers/env_configurator.py
+-rw-r--r--   0        0        0     1012 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/initializers/persona_configuration.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/models/__init__.py
+-rw-r--r--   0        0        0      870 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/models/base.py
+-rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/models/code_bison.py
+-rw-r--r--   0        0        0    10057 2024-04-13 08:21:54.496495 persona_ai-0.1.8/persona_ai/models/gemini.py
+-rw-r--r--   0        0        0     2591 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/models/text_bison.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/moderation/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-13 08:48:32.646648 persona_ai-0.1.8/persona_ai/moderation/ai_moderator.py
+-rw-r--r--   0        0        0     7345 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/moderation/base.py
+-rw-r--r--   0        0        0     4478 2024-04-13 08:29:21.845098 persona_ai-0.1.8/persona_ai/moderation/history_moderator.py
+-rw-r--r--   0        0        0     4759 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/moderation/history_moderator_fc.py
+-rw-r--r--   0        0        0     5580 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/moderation/react_moderator.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/personas/__init__.py
+-rw-r--r--   0        0        0     6678 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/personas/agent.py
+-rw-r--r--   0        0        0     4221 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/personas/assistant.py
+-rw-r--r--   0        0        0     6504 2024-04-11 10:53:55.133342 persona_ai-0.1.8/persona_ai/personas/base.py
+-rw-r--r--   0        0        0     3805 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/personas/coder.py
+-rw-r--r--   0        0        0    13267 2024-04-11 11:05:25.442988 persona_ai-0.1.8/persona_ai/personas/party.py
+-rw-r--r--   0        0        0     3023 2024-04-11 14:30:55.936715 persona_ai-0.1.8/persona_ai/personas/technician.py
+-rw-r--r--   0        0        0      760 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/personas/terminal.py
+-rw-r--r--   0        0        0      860 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/agent.jinja2
+-rw-r--r--   0        0        0      413 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/assistant.jinja2
+-rw-r--r--   0        0        0     1009 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/coder.jinja2
+-rw-r--r--   0        0        0     1194 2024-04-11 15:04:24.559375 persona_ai-0.1.8/persona_ai/prompt_templates/history_moderator.jinja2
+-rw-r--r--   0        0        0     1062 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/history_moderator_fc.jinja2
+-rw-r--r--   0        0        0     1776 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/react_json_moderator.jinja2
+-rw-r--r--   0        0        0     1083 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/react_moderator.jinja2
+-rw-r--r--   0        0        0      330 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/refiner.jinja2
+-rw-r--r--   0        0        0      946 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2
+-rw-r--r--   0        0        0      841 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2
+-rw-r--r--   0        0        0      102 2024-04-11 14:33:38.412861 persona_ai-0.1.8/persona_ai/prompt_templates/technician.jinja2
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/prompts/__init__.py
+-rw-r--r--   0        0        0      238 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/prompts/base.py
+-rw-r--r--   0        0        0     2207 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/prompts/jinja.py
+-rw-r--r--   0        0        0      588 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/prompts/text.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/refiners/__init__.py
+-rw-r--r--   0        0        0     1786 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/refiners/request_refiner.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/task_manager/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/task_manager/base.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/tools/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/tools/base.py
+-rw-r--r--   0        0        0     1746 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/tools/functional.py
+-rw-r--r--   0        0        0      730 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/tools/manager.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/transport/__init__.py
+-rw-r--r--   0        0        0     3477 2024-04-11 13:57:49.665513 persona_ai-0.1.8/persona_ai/transport/local/local_messagebus.py
+-rw-r--r--   0        0        0     4022 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/transport/messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/transport/rabbitmq/__init__.py
+-rw-r--r--   0        0        0    10002 2024-04-11 10:00:15.400629 persona_ai-0.1.8/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py
+-rw-r--r--   0        0        0        0 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/utils/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-08 06:52:52.049183 persona_ai-0.1.8/persona_ai/utils/crypto.py
+-rw-r--r--   0        0        0      911 2024-04-13 08:45:38.530414 persona_ai-0.1.8/persona_ai/utils/extractors.py
+-rw-r--r--   0        0        0     1164 2024-04-13 09:10:47.190812 persona_ai-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    12749 1970-01-01 00:00:00.000000 persona_ai-0.1.8/PKG-INFO
```

### Comparing `persona_ai-0.1.7/README.md` & `persona_ai-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/code_runners/base.py` & `persona_ai-0.1.8/persona_ai/code_runners/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/code_runners/local.py` & `persona_ai-0.1.8/persona_ai/code_runners/local.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/conversation_listeners/terminal.py` & `persona_ai-0.1.8/persona_ai/conversation_listeners/terminal_conversation_listener.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from persona_ai.domain.conversations import Message, Blob
 from persona_ai.domain.events import Event
 from persona_ai.domain.tasks import TaskStatus
 from persona_ai.domain.utils import create_id
 from persona_ai.initializers.persona_configuration import PersonaAI
 from persona_ai.task_manager.base import TaskManager
 from persona_ai.transport.messagebus import ConversationListener
+from persona_ai.utils.extractors import markdown_to_text
 
 LINE = "-----------------------------------------------------------"
 
 
 class TerminalConversationListener(ConversationListener):
     """
     A conversation listener that prints messages and events to the terminal.
@@ -86,15 +87,16 @@
         print()
         cprint(f"Message from {message.sender_name}", "yellow")
 
         if message.body.blobs is not None:
             for blob in message.body.blobs:
                 self._print_blob(blob)
 
-        cprint(f"{message.get_text()}", "white")
+        text = markdown_to_text(message.get_text())
+        cprint(f"{text}", "white")
         print()
 
     def _print_iteration(self, event: Event):
         cprint(LINE, "white")
         task = self.task_manager.get_by_id(event.body["task_id"])
         if task is None:
             cprint(" *** Task not found *** ", "red")
```

### Comparing `persona_ai-0.1.7/persona_ai/conversations/manager.py` & `persona_ai-0.1.8/persona_ai/conversations/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/domain/conversations.py` & `persona_ai-0.1.8/persona_ai/domain/conversations.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/domain/events.py` & `persona_ai-0.1.8/persona_ai/domain/events.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/domain/repositories.py` & `persona_ai-0.1.8/persona_ai/domain/repositories.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/domain/schemas/crud.py` & `persona_ai-0.1.8/persona_ai/domain/schemas/crud.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/domain/tasks.py` & `persona_ai-0.1.8/persona_ai/domain/tasks.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/infrastructure/repositories/base.py` & `persona_ai-0.1.8/persona_ai/infrastructure/repositories/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/infrastructure/repositories/in_memory.py` & `persona_ai-0.1.8/persona_ai/infrastructure/repositories/in_memory.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/infrastructure/repositories/mongo.py` & `persona_ai-0.1.8/persona_ai/infrastructure/repositories/mongo.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/initializers/env_configurator.py` & `persona_ai-0.1.8/persona_ai/initializers/env_configurator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/initializers/persona_configuration.py` & `persona_ai-0.1.8/persona_ai/initializers/persona_configuration.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/models/base.py` & `persona_ai-0.1.8/persona_ai/models/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/models/code_bison.py` & `persona_ai-0.1.8/persona_ai/models/code_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/models/gemini.py` & `persona_ai-0.1.8/persona_ai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/models/text_bison.py` & `persona_ai-0.1.8/persona_ai/models/text_bison.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/moderation/ai_moderator.py` & `persona_ai-0.1.8/persona_ai/moderation/ai_moderator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from persona_ai.domain.tasks import Task
 from persona_ai.initializers.persona_configuration import PersonaAI
 from persona_ai.models.base import GenAIModel
 from persona_ai.moderation.base import Moderator, ModerationResult, Rule
 from persona_ai.prompts.base import Prompt
 from persona_ai.tools.base import ToolDefinition
 from persona_ai.transport.messagebus import Participant
+from persona_ai.utils.extractors import markdown_to_text
 
 logger = logging.getLogger(__name__)
 
 
 class AIModerator(ABC, Moderator):
     """
     AI moderator.
@@ -61,26 +62,25 @@
         prompt = self._render_prompt(
             allowed_participants=allowed_participants,
             conversation_history=conversation_history,
             init_message=task.init_message,
             task=task,
         )
 
-        print("***")
-        print(prompt)
-        print("***")
-
         response = self.model.generate(
             prompt,
             tools=tools,
             **self._get_generation_kwargs(),
         )
 
         logger.debug("Model response: %s", response)
 
+        if response.text:
+            response.text = markdown_to_text(response.text.strip())
+
         return self._process_response(allowed_participants, response, task)
 
     def _get_generation_kwargs(self):
         return {}
 
     @abstractmethod
     def _process_response(
```

### Comparing `persona_ai-0.1.7/persona_ai/moderation/base.py` & `persona_ai-0.1.8/persona_ai/moderation/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/moderation/history_moderator.py` & `persona_ai-0.1.8/persona_ai/moderation/history_moderator.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Parse the output the history moderator selector using regular expressions.
     It retrieves the assistant id and reasoning process.
     """
 
     def parse(self, text: str) -> HistoryModeratorOutput:
         thought_pattern = r"Thought:\s*(.+)"
         participant_pattern = r"Participant:\s*(.+)"
-        assistant_question_pattern = r"Participant Input:\s*(.+)"
+        assistant_question_pattern = r"Participant Question:\s*(.+)"
 
         thought_match = re.search(thought_pattern, text)
         participant_match = re.search(participant_pattern, text)
         participant_question_match = re.search(
             assistant_question_pattern, text, re.DOTALL
         )
```

### Comparing `persona_ai-0.1.7/persona_ai/moderation/history_moderator_fc.py` & `persona_ai-0.1.8/persona_ai/moderation/history_moderator_fc.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/moderation/react_moderator.py` & `persona_ai-0.1.8/persona_ai/moderation/react_moderator.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/personas/agent.py` & `persona_ai-0.1.8/persona_ai/personas/agent.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/personas/assistant.py` & `persona_ai-0.1.8/persona_ai/personas/assistant.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/personas/base.py` & `persona_ai-0.1.8/persona_ai/personas/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/personas/coder.py` & `persona_ai-0.1.8/persona_ai/personas/coder.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/personas/party.py` & `persona_ai-0.1.8/persona_ai/personas/party.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/personas/technician.py` & `persona_ai-0.1.8/persona_ai/personas/technician.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/personas/terminal.py` & `persona_ai-0.1.8/persona_ai/personas/terminal.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompt_templates/agent.jinja2` & `persona_ai-0.1.8/persona_ai/prompt_templates/agent.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompt_templates/coder.jinja2` & `persona_ai-0.1.8/persona_ai/prompt_templates/coder.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompt_templates/history_moderator.jinja2` & `persona_ai-0.1.8/persona_ai/prompt_templates/history_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompt_templates/history_moderator_fc.jinja2` & `persona_ai-0.1.8/persona_ai/prompt_templates/history_moderator_fc.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompt_templates/react_json_moderator.jinja2` & `persona_ai-0.1.8/persona_ai/prompt_templates/react_json_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompt_templates/react_moderator.jinja2` & `persona_ai-0.1.8/persona_ai/prompt_templates/react_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2` & `persona_ai-0.1.8/persona_ai/prompt_templates/request_and_history_function_calling_mediator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2` & `persona_ai-0.1.8/persona_ai/prompt_templates/request_and_history_function_calling_moderator.jinja2`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompts/jinja.py` & `persona_ai-0.1.8/persona_ai/prompts/jinja.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/prompts/text.py` & `persona_ai-0.1.8/persona_ai/prompts/text.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/refiners/request_refiner.py` & `persona_ai-0.1.8/persona_ai/refiners/request_refiner.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/task_manager/base.py` & `persona_ai-0.1.8/persona_ai/task_manager/base.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/tools/functional.py` & `persona_ai-0.1.8/persona_ai/tools/functional.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/tools/manager.py` & `persona_ai-0.1.8/persona_ai/tools/manager.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/transport/local/local_messagebus.py` & `persona_ai-0.1.8/persona_ai/transport/local/local_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/transport/messagebus.py` & `persona_ai-0.1.8/persona_ai/transport/messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py` & `persona_ai-0.1.8/persona_ai/transport/rabbitmq/rabbitmq_messagebus.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/utils/crypto.py` & `persona_ai-0.1.8/persona_ai/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `persona_ai-0.1.7/persona_ai/utils/extractors.py` & `persona_ai-0.1.8/persona_ai/utils/extractors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import re
 
+from strip_markdown import strip_markdown
+
 
 def extract_json(data: str) -> str:
     """Extract JSON delimited from ```json ... ``` from a string."""
 
     data = data.strip()
     if data.startswith("{") and data.endswith("}"):
         return data
@@ -22,7 +24,12 @@
 
 
 def extract_python_code(data: str) -> str:
     """Extract Python code delimited from ```python ... ``` from a string."""
     python = re.search(r"```python(.*?)```", data, re.DOTALL)
     if python:
         return python.group(1)
+
+
+def markdown_to_text(markdown: str) -> str:
+    """Convert markdown to text."""
+    return strip_markdown(markdown)
```

### Comparing `persona_ai-0.1.7/pyproject.toml` & `persona_ai-0.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "persona_ai"
-version = "0.1.7"
+version = "0.1.8"
 description = "Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes"
 authors = ["Bruno Fortunato <bruno.fortunato@applica.guru>"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0"
+python = ">=3.10,<4.0"
 pydantic = "^2.6.4"
 python-dotenv = "^1.0.1"
 Jinja2 = "^3.1.3"
 termcolor = "^2.4.0"
 shortuuid = "^1.0.13"
 google-cloud-aiplatform = "^1.47.0"
 google-api-python-client = "^2.125.0"
 pymongo = "^4.6.3"
 pika = "^1.3.2"
 pycryptodome = "^3.20.0"
 pywhatkit = "^5.4"
+strip-markdown = "^1.3"
 
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^7.2.6"
 jupyter = "^1.0.0"
 
 [build-system]
```

### Comparing `persona_ai-0.1.7/PKG-INFO` & `persona_ai-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: persona_ai
-Version: 0.1.7
+Version: 0.1.8
 Summary: Persona is a groundbreaking distributed AI agent system utilizing Google Vertex AI's premier Large Language Models such as Gemini-pro, Text-Bison, and Code-Bison. Developed by Applica Software Guru, Persona is engineered for scalable, high-performance, and intelligent operations across various data sets and applications. It harnesses the power of Google's Vertex AI to deliver unmatched insights and automation capabilities, setting new standards in AI-driven analytics and decision-making processes
 License: MIT
 Author: Bruno Fortunato
 Author-email: bruno.fortunato@applica.guru
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: google-api-python-client (>=2.125.0,<3.0.0)
 Requires-Dist: google-cloud-aiplatform (>=1.47.0,<2.0.0)
 Requires-Dist: pika (>=1.3.2,<2.0.0)
 Requires-Dist: pycryptodome (>=3.20.0,<4.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pywhatkit (>=5.4,<6.0)
 Requires-Dist: shortuuid (>=1.0.13,<2.0.0)
+Requires-Dist: strip-markdown (>=1.3,<2.0)
 Requires-Dist: termcolor (>=2.4.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Introduction
 
 ****Welcome to the exciting world of Persona AI, a cutting-edge framework designed for the development of generative
 artificial intelligence applications that span multiple modes of interaction. Persona AI leverages the power of Google
```

