# Comparing `tmp/LangTorch-1.0.0.tar.gz` & `tmp/LangTorch-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LangTorch-1.0.0.tar", last modified: Sun Mar 31 16:27:52 2024, max compression
+gzip compressed data, was "LangTorch-1.0.1.tar", last modified: Sat Apr 13 15:08:10 2024, max compression
```

## Comparing `LangTorch-1.0.0.tar` & `LangTorch-1.0.1.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.428460 LangTorch-1.0.0/
--rw-rw-rw-   0        0        0     6593 2024-03-31 16:27:52.428460 LangTorch-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5898 2024-03-31 09:58:48.000000 LangTorch-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-31 16:27:52.428460 LangTorch-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1499 2024-03-30 17:16:20.000000 LangTorch-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:51.875227 LangTorch-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:51.913994 LangTorch-1.0.0/src/LangTorch.egg-info/
--rw-rw-rw-   0        0        0     6593 2024-03-31 16:27:51.000000 LangTorch-1.0.0/src/LangTorch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2906 2024-03-31 16:27:51.000000 LangTorch-1.0.0/src/LangTorch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 16:27:51.000000 LangTorch-1.0.0/src/LangTorch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2024-03-31 16:27:51.000000 LangTorch-1.0.0/src/LangTorch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-31 16:27:51.000000 LangTorch-1.0.0/src/LangTorch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.010639 LangTorch-1.0.0/src/langtorch/
--rw-rw-rw-   0        0        0     9127 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/_VariableFunctions.py
--rw-rw-rw-   0        0        0      483 2024-03-06 17:07:38.000000 LangTorch-1.0.0/src/langtorch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.098163 LangTorch-1.0.0/src/langtorch/api/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:39:23.000000 LangTorch-1.0.0/src/langtorch/api/TODO_anthropic_parallel_processor.py
--rw-rw-rw-   0        0        0      542 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/api/TODO_assistant.py
--rw-rw-rw-   0        0        0     7008 2023-11-17 20:54:26.000000 LangTorch-1.0.0/src/langtorch/api/TODO_gcp_parallel_processor.py
--rw-rw-rw-   0        0        0      108 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/api/__init__.py
--rw-rw-rw-   0        0        0     1107 2024-01-14 23:17:01.000000 LangTorch-1.0.0/src/langtorch/api/api_threading.py
--rw-rw-rw-   0        0        0    12575 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/api/call.py
--rw-rw-rw-   0        0        0    10822 2024-03-23 23:19:27.000000 LangTorch-1.0.0/src/langtorch/api/openai_parallel_processor.py
--rw-rw-rw-   0        0        0     9670 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/api/parallel_processor_utils.py
--rw-rw-rw-   0        0        0     6523 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/api/tools.py
--rw-rw-rw-   0        0        0     1097 2023-11-17 20:54:26.000000 LangTorch-1.0.0/src/langtorch/api/utils.py
--rw-rw-rw-   0        0        0     8104 2024-03-21 19:09:07.000000 LangTorch-1.0.0/src/langtorch/autograd.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.115247 LangTorch-1.0.0/src/langtorch/conf/
--rw-rw-rw-   0        0        0     2526 2024-03-20 14:29:47.000000 LangTorch-1.0.0/src/langtorch/conf/__init__.py
--rw-rw-rw-   0        0        0      491 2023-11-17 20:54:26.000000 LangTorch-1.0.0/src/langtorch/conf/new_session_template.yaml
--rw-rw-rw-   0        0        0        0 2023-11-06 19:21:02.000000 LangTorch-1.0.0/src/langtorch/conf/overrides.yaml
--rw-rw-rw-   0        0        0     5231 2024-03-06 17:07:08.000000 LangTorch-1.0.0/src/langtorch/decorators.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.175880 LangTorch-1.0.0/src/langtorch/grammars/
--rw-rw-rw-   0        0        0        0 2023-10-26 10:38:18.000000 LangTorch-1.0.0/src/langtorch/grammars/__init__.py
--rw-rw-rw-   0        0        0     4522 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/grammars/formatters.py
--rw-rw-rw-   0        0        0     4454 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/grammars/langtorch_default_parser.py
--rw-rw-rw-   0        0        0     5186 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/grammars/pandoc.py
--rw-rw-rw-   0        0        0     1090 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/grammars/parsers.py
--rw-rw-rw-   0        0        0     6102 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/grammars/text_content_ast.py
--rw-rw-rw-   0        0        0     2269 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/grammars/utils.py
--rw-rw-rw-   0        0        0     6718 2024-03-31 08:22:35.000000 LangTorch-1.0.0/src/langtorch/main.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.202164 LangTorch-1.0.0/src/langtorch/methods/
--rw-rw-rw-   0        0        0       78 2023-11-05 01:06:54.000000 LangTorch-1.0.0/src/langtorch/methods/__init__.py
--rw-rw-rw-   0        0        0     2707 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/methods/chain_of_density.py
--rw-rw-rw-   0        0        0      587 2023-11-17 20:54:26.000000 LangTorch-1.0.0/src/langtorch/methods/chain_of_thought.py
--rw-rw-rw-   0        0        0     2279 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/methods/embeddings.py
--rw-rw-rw-   0        0        0        0 2023-10-28 13:28:13.000000 LangTorch-1.0.0/src/langtorch/methods/prompts.yaml
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.211173 LangTorch-1.0.0/src/langtorch/optim/
--rw-rw-rw-   0        0        0        0 2023-11-05 08:27:58.000000 LangTorch-1.0.0/src/langtorch/optim/__init__.py
--rw-rw-rw-   0        0        0     2199 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/optim/optimizer.py
--rw-rw-rw-   0        0        0      574 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/semalg_utils.py
--rw-rw-rw-   0        0        0     3280 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/semantic_algebra.py
--rw-rw-rw-   0        0        0    15334 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/session.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.247737 LangTorch-1.0.0/src/langtorch/tensors/
--rw-rw-rw-   0        0        0      180 2023-11-09 16:31:32.000000 LangTorch-1.0.0/src/langtorch/tensors/__init__.py
--rw-rw-rw-   0        0        0     1873 2024-03-29 20:45:29.000000 LangTorch-1.0.0/src/langtorch/tensors/chattensor.py
--rw-rw-rw-   0        0        0     3586 2024-03-20 14:29:46.000000 LangTorch-1.0.0/src/langtorch/tensors/codetensor.py
--rw-rw-rw-   0        0        0        0 2023-10-28 04:37:19.000000 LangTorch-1.0.0/src/langtorch/tensors/langtorchtensor.py
--rw-rw-rw-   0        0        0     1151 2024-03-20 14:29:47.000000 LangTorch-1.0.0/src/langtorch/tensors/markdowntensor.py
--rw-rw-rw-   0        0        0    36397 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tensors/texttensor.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.296965 LangTorch-1.0.0/src/langtorch/texts/
--rw-rw-rw-   0        0        0      182 2024-03-25 15:58:05.000000 LangTorch-1.0.0/src/langtorch/texts/__init__.py
--rw-rw-rw-   0        0        0     1459 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/texts/chat.py
--rw-rw-rw-   0        0        0      390 2024-03-25 18:15:28.000000 LangTorch-1.0.0/src/langtorch/texts/code.py
--rw-rw-rw-   0        0        0     2106 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/texts/markdown.py
--rw-rw-rw-   0        0        0      100 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/texts/markup.py
--rw-rw-rw-   0        0        0      419 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/texts/string.py
--rw-rw-rw-   0        0        0    34799 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/texts/text.py
--rw-rw-rw-   0        0        0      240 2024-03-29 21:00:57.000000 LangTorch-1.0.0/src/langtorch/texts/thread.py
--rw-rw-rw-   0        0        0      411 2023-11-17 20:54:25.000000 LangTorch-1.0.0/src/langtorch/torch_utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.309118 LangTorch-1.0.0/src/langtorch/tt/
--rw-rw-rw-   0        0        0      184 2024-03-06 08:14:15.000000 LangTorch-1.0.0/src/langtorch/tt/__init__.py
--rw-rw-rw-   0        0        0    30603 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/functional.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.317119 LangTorch-1.0.0/src/langtorch/tt/modules/
--rw-rw-rw-   0        0        0       66 2024-03-06 16:57:20.000000 LangTorch-1.0.0/src/langtorch/tt/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.319117 LangTorch-1.0.0/src/langtorch/tt/modules/from_t/
--rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.0/src/langtorch/tt/modules/from_t/__init__.py
--rw-rw-rw-   0        0        0        0 2023-10-28 06:28:14.000000 LangTorch-1.0.0/src/langtorch/tt/modules/from_t/transformers_automodel.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.336747 LangTorch-1.0.0/src/langtorch/tt/modules/to_t/
--rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_t/__init__.py
--rw-rw-rw-   0        0        0     1451 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_t/distance.py
--rw-rw-rw-   0        0        0      471 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_t/embedding.py
--rw-rw-rw-   0        0        0     1312 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_t/tokenizer.py
-drwxrwxrwx   0        0        0        0 2024-03-31 16:27:52.427447 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/
--rw-rw-rw-   0        0        0      372 2024-03-31 06:22:28.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/__init__.py
--rw-rw-rw-   0        0        0    22247 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/activation.py
--rw-rw-rw-   0        0        0     3259 2024-03-13 19:07:50.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/assistantmodule.py
--rw-rw-rw-   0        0        0      144 2024-03-06 08:14:15.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/chatmodule.py
--rw-rw-rw-   0        0        0      614 2024-03-11 15:48:53.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/codemodule.py
--rw-rw-rw-   0        0        0    13348 2024-03-06 08:14:15.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/conv.py
--rw-rw-rw-   0        0        0     1623 2024-03-14 00:05:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/linear.py
--rw-rw-rw-   0        0        0     2579 2024-03-31 05:57:25.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/loss.py
--rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/pooling.py
--rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/rnn.py
--rw-rw-rw-   0        0        0     7201 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/textmodule.py
--rw-rw-rw-   0        0        0        0 2023-09-25 19:20:23.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/transformer.py
--rw-rw-rw-   0        0        0     2009 2024-03-31 08:18:44.000000 LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/transformers.py
--rw-rw-rw-   0        0        0     1270 2024-02-28 12:31:38.000000 LangTorch-1.0.0/src/langtorch/types.py
--rw-rw-rw-   0        0        0     8337 2024-03-27 03:29:29.000000 LangTorch-1.0.0/src/langtorch/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.773488 LangTorch-1.0.1/
+-rw-rw-rw-   0        0        0     6463 2024-04-13 15:08:10.773488 LangTorch-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5758 2024-03-31 16:29:32.000000 LangTorch-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 15:08:10.773488 LangTorch-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2024-04-13 15:05:24.000000 LangTorch-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.065155 LangTorch-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.101951 LangTorch-1.0.1/src/LangTorch.egg-info/
+-rw-rw-rw-   0        0        0     6463 2024-04-13 15:08:09.000000 LangTorch-1.0.1/src/LangTorch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2950 2024-04-13 15:08:10.000000 LangTorch-1.0.1/src/LangTorch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 15:08:09.000000 LangTorch-1.0.1/src/LangTorch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2024-04-13 15:08:09.000000 LangTorch-1.0.1/src/LangTorch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-13 15:08:09.000000 LangTorch-1.0.1/src/LangTorch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.203655 LangTorch-1.0.1/src/langtorch/
+-rw-rw-rw-   0        0        0     9127 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/_VariableFunctions.py
+-rw-rw-rw-   0        0        0      483 2024-03-06 17:07:38.000000 LangTorch-1.0.1/src/langtorch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.311002 LangTorch-1.0.1/src/langtorch/api/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:39:23.000000 LangTorch-1.0.1/src/langtorch/api/TODO_anthropic_parallel_processor.py
+-rw-rw-rw-   0        0        0      542 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/api/TODO_assistant.py
+-rw-rw-rw-   0        0        0     7008 2023-11-17 20:54:26.000000 LangTorch-1.0.1/src/langtorch/api/TODO_gcp_parallel_processor.py
+-rw-rw-rw-   0        0        0      108 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/api/__init__.py
+-rw-rw-rw-   0        0        0     1107 2024-01-14 23:17:01.000000 LangTorch-1.0.1/src/langtorch/api/api_threading.py
+-rw-rw-rw-   0        0        0    12599 2024-04-05 11:21:04.000000 LangTorch-1.0.1/src/langtorch/api/call.py
+-rw-rw-rw-   0        0        0    10822 2024-03-23 23:19:27.000000 LangTorch-1.0.1/src/langtorch/api/openai_parallel_processor.py
+-rw-rw-rw-   0        0        0     9670 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/api/parallel_processor_utils.py
+-rw-rw-rw-   0        0        0     6523 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/api/tools.py
+-rw-rw-rw-   0        0        0     1097 2023-11-17 20:54:26.000000 LangTorch-1.0.1/src/langtorch/api/utils.py
+-rw-rw-rw-   0        0        0     8104 2024-03-21 19:09:07.000000 LangTorch-1.0.1/src/langtorch/autograd.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.331697 LangTorch-1.0.1/src/langtorch/conf/
+-rw-rw-rw-   0        0        0     2526 2024-03-20 14:29:47.000000 LangTorch-1.0.1/src/langtorch/conf/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-11-17 20:54:26.000000 LangTorch-1.0.1/src/langtorch/conf/new_session_template.yaml
+-rw-rw-rw-   0        0        0        0 2023-11-06 19:21:02.000000 LangTorch-1.0.1/src/langtorch/conf/overrides.yaml
+-rw-rw-rw-   0        0        0     5231 2024-03-06 17:07:08.000000 LangTorch-1.0.1/src/langtorch/decorators.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.403557 LangTorch-1.0.1/src/langtorch/grammars/
+-rw-rw-rw-   0        0        0        0 2023-10-26 10:38:18.000000 LangTorch-1.0.1/src/langtorch/grammars/__init__.py
+-rw-rw-rw-   0        0        0     4522 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/grammars/formatters.py
+-rw-rw-rw-   0        0        0     4454 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/grammars/langtorch_default_parser.py
+-rw-rw-rw-   0        0        0     5186 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/grammars/pandoc.py
+-rw-rw-rw-   0        0        0     1090 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/grammars/parsers.py
+-rw-rw-rw-   0        0        0     6102 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/grammars/text_content_ast.py
+-rw-rw-rw-   0        0        0     2269 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/grammars/utils.py
+-rw-rw-rw-   0        0        0     8043 2024-04-13 15:03:44.000000 LangTorch-1.0.1/src/langtorch/main.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.442226 LangTorch-1.0.1/src/langtorch/methods/
+-rw-rw-rw-   0        0        0       78 2023-11-05 01:06:54.000000 LangTorch-1.0.1/src/langtorch/methods/__init__.py
+-rw-rw-rw-   0        0        0     2704 2024-03-31 16:48:02.000000 LangTorch-1.0.1/src/langtorch/methods/chain_of_density.py
+-rw-rw-rw-   0        0        0      587 2023-11-17 20:54:26.000000 LangTorch-1.0.1/src/langtorch/methods/chain_of_thought.py
+-rw-rw-rw-   0        0        0     2279 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/methods/embeddings.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 13:28:13.000000 LangTorch-1.0.1/src/langtorch/methods/prompts.yaml
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.455790 LangTorch-1.0.1/src/langtorch/optim/
+-rw-rw-rw-   0        0        0        0 2023-11-05 08:27:58.000000 LangTorch-1.0.1/src/langtorch/optim/__init__.py
+-rw-rw-rw-   0        0        0     2199 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/optim/optimizer.py
+-rw-rw-rw-   0        0        0      574 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/semalg_utils.py
+-rw-rw-rw-   0        0        0     3280 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/semantic_algebra.py
+-rw-rw-rw-   0        0        0    15346 2024-04-05 11:21:12.000000 LangTorch-1.0.1/src/langtorch/session.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.505865 LangTorch-1.0.1/src/langtorch/tensors/
+-rw-rw-rw-   0        0        0      180 2023-11-09 16:31:32.000000 LangTorch-1.0.1/src/langtorch/tensors/__init__.py
+-rw-rw-rw-   0        0        0     1873 2024-03-29 20:45:29.000000 LangTorch-1.0.1/src/langtorch/tensors/chattensor.py
+-rw-rw-rw-   0        0        0     3586 2024-03-20 14:29:46.000000 LangTorch-1.0.1/src/langtorch/tensors/codetensor.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 04:37:19.000000 LangTorch-1.0.1/src/langtorch/tensors/langtorchtensor.py
+-rw-rw-rw-   0        0        0     1151 2024-03-20 14:29:47.000000 LangTorch-1.0.1/src/langtorch/tensors/markdowntensor.py
+-rw-rw-rw-   0        0        0    37201 2024-04-04 00:50:53.000000 LangTorch-1.0.1/src/langtorch/tensors/texttensor.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.579140 LangTorch-1.0.1/src/langtorch/texts/
+-rw-rw-rw-   0        0        0      182 2024-03-25 15:58:05.000000 LangTorch-1.0.1/src/langtorch/texts/__init__.py
+-rw-rw-rw-   0        0        0     1459 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/texts/chat.py
+-rw-rw-rw-   0        0        0      390 2024-03-25 18:15:28.000000 LangTorch-1.0.1/src/langtorch/texts/code.py
+-rw-rw-rw-   0        0        0     2106 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/texts/markdown.py
+-rw-rw-rw-   0        0        0      100 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/texts/markup.py
+-rw-rw-rw-   0        0        0      419 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/texts/string.py
+-rw-rw-rw-   0        0        0    36118 2024-04-07 13:08:34.000000 LangTorch-1.0.1/src/langtorch/texts/text.py
+-rw-rw-rw-   0        0        0      240 2024-03-29 21:00:57.000000 LangTorch-1.0.1/src/langtorch/texts/thread.py
+-rw-rw-rw-   0        0        0      411 2023-11-17 20:54:25.000000 LangTorch-1.0.1/src/langtorch/torch_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.604461 LangTorch-1.0.1/src/langtorch/tt/
+-rw-rw-rw-   0        0        0      184 2024-03-06 08:14:15.000000 LangTorch-1.0.1/src/langtorch/tt/__init__.py
+-rw-rw-rw-   0        0        0    30603 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/tt/functional.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.613964 LangTorch-1.0.1/src/langtorch/tt/modules/
+-rw-rw-rw-   0        0        0       66 2024-03-06 16:57:20.000000 LangTorch-1.0.1/src/langtorch/tt/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.615979 LangTorch-1.0.1/src/langtorch/tt/modules/from_t/
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.1/src/langtorch/tt/modules/from_t/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:28:14.000000 LangTorch-1.0.1/src/langtorch/tt/modules/from_t/transformers_automodel.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.654388 LangTorch-1.0.1/src/langtorch/tt/modules/to_t/
+-rw-rw-rw-   0        0        0        0 2023-10-28 06:26:06.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_t/__init__.py
+-rw-rw-rw-   0        0        0     1451 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_t/distance.py
+-rw-rw-rw-   0        0        0      471 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_t/embedding.py
+-rw-rw-rw-   0        0        0     1312 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_t/tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-04-13 15:08:10.772488 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/
+-rw-rw-rw-   0        0        0      372 2024-03-31 06:22:28.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/__init__.py
+-rw-rw-rw-   0        0        0    22263 2024-04-09 18:19:04.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/activation.py
+-rw-rw-rw-   0        0        0     3259 2024-03-13 19:07:50.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/assistantmodule.py
+-rw-rw-rw-   0        0        0      144 2024-03-06 08:14:15.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/chatmodule.py
+-rw-rw-rw-   0        0        0      614 2024-03-11 15:48:53.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/codemodule.py
+-rw-rw-rw-   0        0        0    13348 2024-03-06 08:14:15.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/conv.py
+-rw-rw-rw-   0        0        0     1623 2024-03-14 00:05:44.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/linear.py
+-rw-rw-rw-   0        0        0     2579 2024-03-31 05:57:25.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/loss.py
+-rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/pooling.py
+-rw-rw-rw-   0        0        0      883 2024-03-31 16:49:04.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/retriever.py
+-rw-rw-rw-   0        0        0        9 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/rnn.py
+-rw-rw-rw-   0        0        0     7201 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/textmodule.py
+-rw-rw-rw-   0        0        0        0 2023-09-25 19:20:23.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/transformer.py
+-rw-rw-rw-   0        0        0     2009 2024-03-31 08:18:44.000000 LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/transformers.py
+-rw-rw-rw-   0        0        0     1270 2024-02-28 12:31:38.000000 LangTorch-1.0.1/src/langtorch/types.py
+-rw-rw-rw-   0        0        0     8337 2024-03-27 03:29:29.000000 LangTorch-1.0.1/src/langtorch/utils.py
```

### Comparing `LangTorch-1.0.0/PKG-INFO` & `LangTorch-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,68 @@
 Metadata-Version: 2.1
 Name: LangTorch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Framework for intuitive LLM application development with tensors.
 Home-page: https://github.com/AdamSobieszek/LangTorch
 Author: Adam Sobieszek
 Author-email: contact@langtorch.org
 Keywords: LangTorch,PyTorch,LLM,Language Models,Chat,Chains
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 70%; height: auto; vertical-align: middle;"> </div>
+#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;"> </div>
 
 [![PyPI version](https://badge.fury.io/py/langtorch.svg)](https://badge.fury.io/py/langtorch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/AdamSobieszek.svg?style=social&label=Follow%20%40AdamSobieszek)](https://twitter.com/AdamSobieszek)
 [![GitHub star chart](https://img.shields.io/github/stars/AdamSobieszek/langtorch?style=social)](https://star-history.com/#AdamSobieszek/langtorch)
 
 [//]: # ([![]&#40;https://dcbadge.vercel.app/api/server/6adMQxSpJS?compact=true&style=flat&#41;]&#40;https://discord.gg/6adMQxSpJS&#41;)
 
 
-LangTorch is a Python package designed to simplify the development of LLM applications by leveraging familiar PyTorch concepts. While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications, by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more, thanks to TextTensors -- which are like torch Tensors but with text data as entries, offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
+LangTorch is a Python package that accelerates development of complex language model applications by leveraging familiar PyTorch concepts.
+
+While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more.
+> Powered by **TextTensors** â€” "torch Tensors but with text data as entries" â€” offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
 
 ## Installation
 
 ```bash
 pip install langtorch
 ```
 
 ## Overview
-[README (1).md](..%2FSamouwielbienie%20v2%2FLas2020%2F0%2FREADME%20%281%29.md)
-- **Create more with less**: Instead of providing wrapper classes for users to memorize, LangTorch introduces flexible objects that, while governed by simple rules, enable all kinds of text formatting, templating and LLM operations. This lets developers think about what they want to build, instead of how the classes were named.
-- - **Unified Approach**: TextTensors let you structure geometrically and handle in parallel text entries, that without any additional classes can represent strings, documents, prompt templates, completion dictionaries, chat histories, markup languages, chunks, retrieval queries, tokens, embeddings...
-- **You probably already know LangTorch**: LangTorch components subclass their numerical PyTorch counterparts, which lets users apply their existing coding skills to building novel LLM app architectures. This includes **TextModules** - a subclass of torch.nn.Module working on TextTensors and able to perform template completions, prompt injections, local and API LLM inference, create embedding, performing operations on embeddings in retrieval and so on.
+
+- **No useless classes**:
+
+	Instead of providing wrapper classes for users to memorize, LangTorch introduces fewer, more flexible objects that enable all kinds of text formatting, templating and LLM operations.
+
+- **Unified Approach**: 
+
+	 TextTensors let you structure geometrically and handle in parallel text entries that can represent:
+	> strings, documents, prompt templates, completion dictionaries, chat histories, markup languages, chunks, retrieval queries, tokens, embeddings and so on
+
+- **You probably already know LangTorch**: 
+
+	LangTorch components subclass their numerical PyTorch counterparts, which lets users apply their existing coding skills to building novel LLM app architectures.
+
+- **Other goodies like TextModules**
+
+	a subclass of torch.nn.Module working on TextTensors and able to perform:
+	> template completions, prompt injections, local and API LLM inference, create embedding, performing operations on embeddings in retrieval and so on, and so on
+
 - Honestly just go to https://langtorch.org there is much more information there!
 
-## Code Examples Speak for Themselves
+## Code Examples
 
 The examples are introduced on the main documentation page, but even without much introduction you can see how compact some pretty complex operations can be implemented with LangTorch.
 
 ### TextTensors act both as texts and embeddings
 
 ```python  
 import torch  
@@ -60,16 +78,20 @@
 tensor([[0.6923, 0.6644, 0.6317, 0.5749],
 	    [0.5457, 0.7728, 0.5387, 0.7036]])
 Content:
 [[Yes], 
  [No ]]
 ```
 
+
 LangTorch code looks weird at first, why? Since the utility of Tensors, as used in Torch, relies on their ability to calculate simultaneously products of several weights. The corresponding, and most used, feature in LangTorch allows several prompts to be formatted on several inputs, by defining the multiplication of text entries `text1*text2` similarly to `text1.format(**text2)`
 
+
+### Chains
+
 The multiplication operation lets us build chains of TextModules with a simple `torch.nn.Sequential`:
 
 ```python
 chain = torch.nn.Sequential(
     TextModule("Translate this equation to natural language: {}"),
     CoT,
     OpenAI("gpt-4")
@@ -77,14 +99,16 @@
     OpenAI("gpt-4", T=0)
 )
 
 input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
 output_tensor = chain(input_tensor)
 ```
 
+
+
 ### Retrieval & RAG from scratch
 
 The code below is a complete working implementation of a cosine similarity-based retriever:
 
 ```python
 class Retriever(TextModule):  
     def __init__(self, documents: TextTensor):  
@@ -125,8 +149,8 @@
 assistant_response = rag_chat(user_query)
 ```
 
 Go to https://langtorch.org to understand these RAGs-to-riches code shenanigans.
 
 ## License
 
-LangTorch is MIT licensed. See the [LICENSE](#) file for details.
+LangTorch is available under the [MIT license](https://opensource.org/licenses/MIT).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `LangTorch-1.0.0/README.md` & `LangTorch-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,51 @@
-#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 70%; height: auto; vertical-align: middle;"> </div>
+#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;"> </div>
 
 [![PyPI version](https://badge.fury.io/py/langtorch.svg)](https://badge.fury.io/py/langtorch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/AdamSobieszek.svg?style=social&label=Follow%20%40AdamSobieszek)](https://twitter.com/AdamSobieszek)
 [![GitHub star chart](https://img.shields.io/github/stars/AdamSobieszek/langtorch?style=social)](https://star-history.com/#AdamSobieszek/langtorch)
 
 [//]: # ([![]&#40;https://dcbadge.vercel.app/api/server/6adMQxSpJS?compact=true&style=flat&#41;]&#40;https://discord.gg/6adMQxSpJS&#41;)
 
 
-LangTorch is a Python package designed to simplify the development of LLM applications by leveraging familiar PyTorch concepts. While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications, by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more, thanks to TextTensors -- which are like torch Tensors but with text data as entries, offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
+LangTorch is a Python package that accelerates development of complex language model applications by leveraging familiar PyTorch concepts.
+
+While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more.
+> Powered by **TextTensors** — "torch Tensors but with text data as entries" — offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
 
 ## Installation
 
 ```bash
 pip install langtorch
 ```
 
 ## Overview
-[README (1).md](..%2FSamouwielbienie%20v2%2FLas2020%2F0%2FREADME%20%281%29.md)
-- **Create more with less**: Instead of providing wrapper classes for users to memorize, LangTorch introduces flexible objects that, while governed by simple rules, enable all kinds of text formatting, templating and LLM operations. This lets developers think about what they want to build, instead of how the classes were named.
-- - **Unified Approach**: TextTensors let you structure geometrically and handle in parallel text entries, that without any additional classes can represent strings, documents, prompt templates, completion dictionaries, chat histories, markup languages, chunks, retrieval queries, tokens, embeddings...
-- **You probably already know LangTorch**: LangTorch components subclass their numerical PyTorch counterparts, which lets users apply their existing coding skills to building novel LLM app architectures. This includes **TextModules** - a subclass of torch.nn.Module working on TextTensors and able to perform template completions, prompt injections, local and API LLM inference, create embedding, performing operations on embeddings in retrieval and so on.
+
+- **No useless classes**:
+
+	Instead of providing wrapper classes for users to memorize, LangTorch introduces fewer, more flexible objects that enable all kinds of text formatting, templating and LLM operations.
+
+- **Unified Approach**: 
+
+	 TextTensors let you structure geometrically and handle in parallel text entries that can represent:
+	> strings, documents, prompt templates, completion dictionaries, chat histories, markup languages, chunks, retrieval queries, tokens, embeddings and so on
+
+- **You probably already know LangTorch**: 
+
+	LangTorch components subclass their numerical PyTorch counterparts, which lets users apply their existing coding skills to building novel LLM app architectures.
+
+- **Other goodies like TextModules**
+
+	a subclass of torch.nn.Module working on TextTensors and able to perform:
+	> template completions, prompt injections, local and API LLM inference, create embedding, performing operations on embeddings in retrieval and so on, and so on
+
 - Honestly just go to https://langtorch.org there is much more information there!
 
-## Code Examples Speak for Themselves
+## Code Examples
 
 The examples are introduced on the main documentation page, but even without much introduction you can see how compact some pretty complex operations can be implemented with LangTorch.
 
 ### TextTensors act both as texts and embeddings
 
 ```python  
 import torch  
@@ -43,16 +61,20 @@
 tensor([[0.6923, 0.6644, 0.6317, 0.5749],
 	    [0.5457, 0.7728, 0.5387, 0.7036]])
 Content:
 [[Yes], 
  [No ]]
 ```
 
+
 LangTorch code looks weird at first, why? Since the utility of Tensors, as used in Torch, relies on their ability to calculate simultaneously products of several weights. The corresponding, and most used, feature in LangTorch allows several prompts to be formatted on several inputs, by defining the multiplication of text entries `text1*text2` similarly to `text1.format(**text2)`
 
+
+### Chains
+
 The multiplication operation lets us build chains of TextModules with a simple `torch.nn.Sequential`:
 
 ```python
 chain = torch.nn.Sequential(
     TextModule("Translate this equation to natural language: {}"),
     CoT,
     OpenAI("gpt-4")
@@ -60,14 +82,16 @@
     OpenAI("gpt-4", T=0)
 )
 
 input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
 output_tensor = chain(input_tensor)
 ```
 
+
+
 ### Retrieval & RAG from scratch
 
 The code below is a complete working implementation of a cosine similarity-based retriever:
 
 ```python
 class Retriever(TextModule):  
     def __init__(self, documents: TextTensor):  
@@ -108,8 +132,8 @@
 assistant_response = rag_chat(user_query)
 ```
 
 Go to https://langtorch.org to understand these RAGs-to-riches code shenanigans.
 
 ## License
 
-LangTorch is MIT licensed. See the [LICENSE](#) file for details.
+LangTorch is available under the [MIT license](https://opensource.org/licenses/MIT).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `LangTorch-1.0.0/setup.py` & `LangTorch-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="LangTorch",
-    version="1.0.0",
+    version="1.0.1",
     description="Framework for intuitive LLM application development with tensors.",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="Adam Sobieszek",
     author_email="contact@langtorch.org",
     url="https://github.com/AdamSobieszek/LangTorch",
     packages=find_packages(where="src"),
```

### Comparing `LangTorch-1.0.0/src/LangTorch.egg-info/PKG-INFO` & `LangTorch-1.0.1/src/LangTorch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,68 @@
 Metadata-Version: 2.1
 Name: LangTorch
-Version: 1.0.0
+Version: 1.0.1
 Summary: Framework for intuitive LLM application development with tensors.
 Home-page: https://github.com/AdamSobieszek/LangTorch
 Author: Adam Sobieszek
 Author-email: contact@langtorch.org
 Keywords: LangTorch,PyTorch,LLM,Language Models,Chat,Chains
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 70%; height: auto; vertical-align: middle;"> </div>
+#  <div style="text-align: center;"> <img src="./langtorch_banner.png" alt="LangTorch Logo" style="max-width: 40rem; width: 100%; height: auto; vertical-align: middle;"> </div>
 
 [![PyPI version](https://badge.fury.io/py/langtorch.svg)](https://badge.fury.io/py/langtorch)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/AdamSobieszek.svg?style=social&label=Follow%20%40AdamSobieszek)](https://twitter.com/AdamSobieszek)
 [![GitHub star chart](https://img.shields.io/github/stars/AdamSobieszek/langtorch?style=social)](https://star-history.com/#AdamSobieszek/langtorch)
 
 [//]: # ([![]&#40;https://dcbadge.vercel.app/api/server/6adMQxSpJS?compact=true&style=flat&#41;]&#40;https://discord.gg/6adMQxSpJS&#41;)
 
 
-LangTorch is a Python package designed to simplify the development of LLM applications by leveraging familiar PyTorch concepts. While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications, by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more, thanks to TextTensors -- which are like torch Tensors but with text data as entries, offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
+LangTorch is a Python package that accelerates development of complex language model applications by leveraging familiar PyTorch concepts.
+
+While existing frameworks focus on connecting language models to other services, LangTorch aims to change the way you approach creating LLM applications by introducing a unified framework for working with texts, chats, templates, LLMs, API calls and more.
+> Powered by **TextTensors** â€” "torch Tensors but with text data as entries" â€” offering a flexible way to structure and transform text data and embeddings with seamless parallelization. 
 
 ## Installation
 
 ```bash
 pip install langtorch
 ```
 
 ## Overview
-[README (1).md](..%2FSamouwielbienie%20v2%2FLas2020%2F0%2FREADME%20%281%29.md)
-- **Create more with less**: Instead of providing wrapper classes for users to memorize, LangTorch introduces flexible objects that, while governed by simple rules, enable all kinds of text formatting, templating and LLM operations. This lets developers think about what they want to build, instead of how the classes were named.
-- - **Unified Approach**: TextTensors let you structure geometrically and handle in parallel text entries, that without any additional classes can represent strings, documents, prompt templates, completion dictionaries, chat histories, markup languages, chunks, retrieval queries, tokens, embeddings...
-- **You probably already know LangTorch**: LangTorch components subclass their numerical PyTorch counterparts, which lets users apply their existing coding skills to building novel LLM app architectures. This includes **TextModules** - a subclass of torch.nn.Module working on TextTensors and able to perform template completions, prompt injections, local and API LLM inference, create embedding, performing operations on embeddings in retrieval and so on.
+
+- **No useless classes**:
+
+	Instead of providing wrapper classes for users to memorize, LangTorch introduces fewer, more flexible objects that enable all kinds of text formatting, templating and LLM operations.
+
+- **Unified Approach**: 
+
+	 TextTensors let you structure geometrically and handle in parallel text entries that can represent:
+	> strings, documents, prompt templates, completion dictionaries, chat histories, markup languages, chunks, retrieval queries, tokens, embeddings and so on
+
+- **You probably already know LangTorch**: 
+
+	LangTorch components subclass their numerical PyTorch counterparts, which lets users apply their existing coding skills to building novel LLM app architectures.
+
+- **Other goodies like TextModules**
+
+	a subclass of torch.nn.Module working on TextTensors and able to perform:
+	> template completions, prompt injections, local and API LLM inference, create embedding, performing operations on embeddings in retrieval and so on, and so on
+
 - Honestly just go to https://langtorch.org there is much more information there!
 
-## Code Examples Speak for Themselves
+## Code Examples
 
 The examples are introduced on the main documentation page, but even without much introduction you can see how compact some pretty complex operations can be implemented with LangTorch.
 
 ### TextTensors act both as texts and embeddings
 
 ```python  
 import torch  
@@ -60,16 +78,20 @@
 tensor([[0.6923, 0.6644, 0.6317, 0.5749],
 	    [0.5457, 0.7728, 0.5387, 0.7036]])
 Content:
 [[Yes], 
  [No ]]
 ```
 
+
 LangTorch code looks weird at first, why? Since the utility of Tensors, as used in Torch, relies on their ability to calculate simultaneously products of several weights. The corresponding, and most used, feature in LangTorch allows several prompts to be formatted on several inputs, by defining the multiplication of text entries `text1*text2` similarly to `text1.format(**text2)`
 
+
+### Chains
+
 The multiplication operation lets us build chains of TextModules with a simple `torch.nn.Sequential`:
 
 ```python
 chain = torch.nn.Sequential(
     TextModule("Translate this equation to natural language: {}"),
     CoT,
     OpenAI("gpt-4")
@@ -77,14 +99,16 @@
     OpenAI("gpt-4", T=0)
 )
 
 input_tensor = TextTensor(["170*32 =", "4*20 =", "123*45/10 =", "2**10*5 ="])
 output_tensor = chain(input_tensor)
 ```
 
+
+
 ### Retrieval & RAG from scratch
 
 The code below is a complete working implementation of a cosine similarity-based retriever:
 
 ```python
 class Retriever(TextModule):  
     def __init__(self, documents: TextTensor):  
@@ -125,8 +149,8 @@
 assistant_response = rag_chat(user_query)
 ```
 
 Go to https://langtorch.org to understand these RAGs-to-riches code shenanigans.
 
 ## License
 
-LangTorch is MIT licensed. See the [LICENSE](#) file for details.
+LangTorch is available under the [MIT license](https://opensource.org/licenses/MIT).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `LangTorch-1.0.0/src/LangTorch.egg-info/SOURCES.txt` & `LangTorch-1.0.1/src/LangTorch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,11 +71,12 @@
 src/langtorch/tt/modules/to_tt/assistantmodule.py
 src/langtorch/tt/modules/to_tt/chatmodule.py
 src/langtorch/tt/modules/to_tt/codemodule.py
 src/langtorch/tt/modules/to_tt/conv.py
 src/langtorch/tt/modules/to_tt/linear.py
 src/langtorch/tt/modules/to_tt/loss.py
 src/langtorch/tt/modules/to_tt/pooling.py
+src/langtorch/tt/modules/to_tt/retriever.py
 src/langtorch/tt/modules/to_tt/rnn.py
 src/langtorch/tt/modules/to_tt/textmodule.py
 src/langtorch/tt/modules/to_tt/transformer.py
 src/langtorch/tt/modules/to_tt/transformers.py
```

### Comparing `LangTorch-1.0.0/src/langtorch/_VariableFunctions.py` & `LangTorch-1.0.1/src/langtorch/_VariableFunctions.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/api/TODO_assistant.py` & `LangTorch-1.0.1/src/langtorch/api/TODO_assistant.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/api/TODO_gcp_parallel_processor.py` & `LangTorch-1.0.1/src/langtorch/api/TODO_gcp_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/api/api_threading.py` & `LangTorch-1.0.1/src/langtorch/api/api_threading.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/api/call.py` & `LangTorch-1.0.1/src/langtorch/api/call.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,16 @@
         """
 
     if tools is not None:
         for i, tool in enumerate(tools):
             if isinstance(tool, str):
                 try:
                     tools[i] = json.loads(tool)
-                except json.JSONDecodeError:
-                    raise ValueError(f"Tool {tool} is not a valid JSON string object.")
+                except json.JSONDecodeError as e:
+                    raise ValueError(f"Tool {tool} is not a valid JSON string object.") from e
             if not "type" in tools[i]:
                 tools[i] = {"type": "function", "function": tools[i]}
 
     params = {"temperature": temperature,
               "top_p": top_p,
               "n": n,
               "stop": stop,
@@ -180,16 +180,16 @@
     if len(system_messages) == 1:
         system_messages = system_messages * len(prompts)
     request_strings = chat_strings(prompts, system_messages, model, **kwargs)
 
     if api_key is None:
         try:
             api_key = os.environ["OPENAI_API_KEY"]
-        except KeyError:
-            raise KeyError('No OpenAI API key. Set os.environ["OPENAI_API_KEY"] = YOUR KEY')
+        except KeyError as e:
+            raise KeyError('No OpenAI API key. Set os.environ["OPENAI_API_KEY"] = YOUR KEY') from e
     ids, uncached_request_strings = session.request("openai", "chat", request_strings, cache)
 
     if request_strings:
         job = execute_api_requests_in_parallel(
             ids=ids,
             request_strings=uncached_request_strings,
             request_url="https://api.openai.com/v1/chat/completions",
```

### Comparing `LangTorch-1.0.0/src/langtorch/api/openai_parallel_processor.py` & `LangTorch-1.0.1/src/langtorch/api/openai_parallel_processor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/api/parallel_processor_utils.py` & `LangTorch-1.0.1/src/langtorch/api/parallel_processor_utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/api/tools.py` & `LangTorch-1.0.1/src/langtorch/api/tools.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/api/utils.py` & `LangTorch-1.0.1/src/langtorch/api/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/autograd.py` & `LangTorch-1.0.1/src/langtorch/autograd.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/conf/__init__.py` & `LangTorch-1.0.1/src/langtorch/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/decorators.py` & `LangTorch-1.0.1/src/langtorch/decorators.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/grammars/formatters.py` & `LangTorch-1.0.1/src/langtorch/grammars/formatters.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/grammars/langtorch_default_parser.py` & `LangTorch-1.0.1/src/langtorch/grammars/langtorch_default_parser.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/grammars/pandoc.py` & `LangTorch-1.0.1/src/langtorch/grammars/pandoc.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/grammars/parsers.py` & `LangTorch-1.0.1/src/langtorch/grammars/parsers.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/grammars/text_content_ast.py` & `LangTorch-1.0.1/src/langtorch/grammars/text_content_ast.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/grammars/utils.py` & `LangTorch-1.0.1/src/langtorch/grammars/utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/main.py` & `LangTorch-1.0.1/src/langtorch/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,51 @@
 import sys
 
 import langtorch.semantic_algebra
 
 sys.path.append("..")
 import langtorch
-from langtorch import TextTensor, String, Text
+from langtorch import TextTensor, String, Text,  Activation
 from langtorch.tt.functional import dropout
 from langtorch import Session
 import numpy as np
 import torch
 from langtorch import TextModule
 from langtorch import Chat, ChatML
 
+from langtorch import TextTensor, TextModule, OpenAI
+import torch
+# Without any additional classes we can implement a retriever and RAG module
+
+
+
+
+
+llm = Activation(model="gpt-3.5-turbo", T=0.9, tools=[{"type": "function",
+                  "function": {
+                    "name": "get_current_weather",
+                    "description": "Get the current weather in a given location",
+                    "parameters": {
+                      "type": "object",
+                      "properties": {
+                        "location": {
+                          "type": "string",
+                          "description": "The city and state, e.g. San Francisco, CA"
+                        },
+                        "unit": {
+                          "type": "string",
+                          "enum": ["celsius", "fahrenheit"]
+                        }
+                      },
+                      "required": ["location"]
+                    }}}], tool_choice="auto")
+
+
+print(llm(TextTensor("What is the current weather in San Francisco?")).item().items())
+# Outputs: [('assistant', ('tool_call', '{"id": "call_6bII1dQHLYWiar5W1eSRDCQu", "type": "function", "function": {"name": "get_current_weather", "arguments": "{\\"location\\":\\"San Francisco\\"}"}}'))]
 
 class ChatML(Chat):
     language = 'chatml'
     allowed_keys = ["user", "assistant", "system"]
 
     def __str__(self):
         formatted = "\n".join(f"<|im_start|>{k}\n{Text(v)}<|im_end|>" for k, v in self.items())
@@ -27,23 +57,23 @@
     ("assistant", "Hi! How can I help you today?"),
     ("user", "Tell me about {thing}."),
     ("system", "Hello!"),
     ("assistant", "Hi! How can I help you today?"),
     ("user", "Tell me about {thing}.")
 )
 # Use iloc to make sure you format the right message
-input = [1,1,1,1,1,1,1,1,1,1,1]
+input = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
 for i, m in enumerate([chat_template]):
     if "system" in m.keys():
         _ = m.loc["system"].values()[-1]
-        print("sys",_)
+        print("sys", _)
         m = m.loc[["user", "assistant"]]
     if np.all([key in ["user", "assistant"] for key in m.keys()]):
-        input[i] = [(k, str(Text(v, parse=False))) for k,v in m.items()]
-        print('>', input[i] )
+        input[i] = [(k, str(Text(v, parse=False))) for k, v in m.items()]
+        print('>', input[i])
     elif "user" not in m.keys() or "assistant" not in m.keys():
         # NOT STRICT
         input[i] = [("user", str(m))]
     else:
         raise ValueError(
             f"Invalid input to OpenAI Chat. Ambigous input: some but not all items in TextTensor entries have keys 'user' or 'assistant'. Change the input into a valid chat, or the input was a single user message remove these keys or use entry.add_key_('user'): \nentry.items()=={m.items()}")
```

### Comparing `LangTorch-1.0.0/src/langtorch/methods/chain_of_density.py` & `LangTorch-1.0.1/src/langtorch/methods/chain_of_density.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .. import TextTensor, TextModule, ActivationGPT, Text
+from .. import TextTensor, TextModule, Activation, Text
 
 
 class CoDModule(TextModule):
     def __init__(self, iterations=5):
         # Base CoD prompt template
         self.template = """
         Article: {*}
```

### Comparing `LangTorch-1.0.0/src/langtorch/methods/chain_of_thought.py` & `LangTorch-1.0.1/src/langtorch/methods/chain_of_thought.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/methods/embeddings.py` & `LangTorch-1.0.1/src/langtorch/methods/embeddings.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/optim/optimizer.py` & `LangTorch-1.0.1/src/langtorch/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/semalg_utils.py` & `LangTorch-1.0.1/src/langtorch/semalg_utils.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/semantic_algebra.py` & `LangTorch-1.0.1/src/langtorch/semantic_algebra.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/session.py` & `LangTorch-1.0.1/src/langtorch/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,16 @@
                         self._responses[key] = [m.decode('utf-8') for m in
                                                 dataset[:]] if dataset.dtype == np.object_ else torch.from_numpy(
                             dataset[:])
 
         if self._session_file and os.path.exists(self._session_file) and not new_session_file:
             try:
                 _config = OmegaConf.merge(_config, OmegaConf.load(self._session_file))
-            except Exception as E:
-                print(f"Error loading session from {self._session_file}: {E}")
+            except Exception as e:
+                print(f"Error loading session from {self._session_file}: {e}")
 
         if not getattr(_config, "tensor_savepath", None):
             _config.tensor_savepath = "" if self._session_file is None else os.path.join(
                 os.path.dirname(os.path.abspath(self._session_file)), "saved_tensors.pt")
 
         if _config.tensor_savepath and os.path.exists(_config.tensor_savepath):
             self._tensors = torch.load(_config.tensor_savepath)
@@ -302,18 +302,18 @@
         # If the attribute name corresponds to an id in the tensors list, return that tensors
         if not hasattr(self._config, name) and name in [m["id"] for m in self._config["tensors"]]:
             return self.tensors[name]
 
         # Return the attribute from the configuration
         try:
             attr = self._config[name]
-        except KeyError:
+        except KeyError as e:
             logging.warning(f"getattr {name}, but session attributes are: {self._config.keys()}")
 
-            raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'")
+            raise AttributeError(f"'{type(self).__name__}' object has no attribute '{name}'") from e
 
         return attr
 
     def get_hash(self, *args):
         """
         Generates hash converted to base64 from a list of string requests.
         This serves as a unique ID for an api request for caching purposes.
```

### Comparing `LangTorch-1.0.0/src/langtorch/tensors/chattensor.py` & `LangTorch-1.0.1/src/langtorch/tensors/chattensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tensors/codetensor.py` & `LangTorch-1.0.1/src/langtorch/tensors/codetensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tensors/markdowntensor.py` & `LangTorch-1.0.1/src/langtorch/tensors/markdowntensor.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tensors/texttensor.py` & `LangTorch-1.0.1/src/langtorch/tensors/texttensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,29 @@
                 is_gradient: bool = False, is_param: bool = False, **kwargs):
         embedding = None
         if metadata is None:
             metadata = dict()
         for attr in ["content", "embedding"]:
             if not attr in metadata:
                 metadata[attr] = eval(attr)
-        # TODO create from dict of tensors
+
+        def dict_to_tt(cls, d, parse): # TODO create from dict of tensors
+            if not d:
+                return None
+            def item_to_tt(cls, k,v, parse):
+                content = cls.input_formatter(cls.content_to_object_array(v,  parse=parse))
+                content = np.array([(k, v) for v in content.flat], dtype=object).reshape(content.shape)
+                return cls.__new__(cls, content, parse=parse)
+
+            content = item_to_tt(cls, d.items()[0][0], d.items()[0][1], parse=parse)
+            for k, v in d.items()[1:]:
+                content += item_to_tt(cls, k, v, parse=parse)
+            return content
+
+        
         # Set content to be an object array with cls.text_class entries
         metadata["content"] = cls.content_to_object_array(metadata["content"], parse=parse)
         # Apply input formatter
         metadata["content"] = cls.input_formatter(metadata["content"])
 
         tensor = super().__new__(cls, torch.arange(metadata["content"].size, dtype=torch.float32).reshape(
             metadata["content"].shape), **kwargs)
@@ -131,17 +145,20 @@
         super().__init__()
 
     def __hash__(self):
         return id(self)
 
     @classmethod
     def content_to_object_array(cls, input, **kwargs):
-        return input.content if isinstance(input, TextTensor) \
-            else np.array(input, dtype=object) if isinstance(input, Text) \
-            else chararray_to_TextArray(input, cls._ttype, **kwargs)
+        try:
+            return input.content if isinstance(input, TextTensor) \
+                else np.array(input, dtype=object) if isinstance(input, Text) \
+                else chararray_to_TextArray(input, cls._ttype, **kwargs)
+        except Exception as e:
+            raise ValueError(f"Could not convert input to TextTensor content. Failed to convert input to an array:\n{e}")
 
     @property
     def content(self):
         return self._content
 
     @content.setter
     def content(self, content):
```

### Comparing `LangTorch-1.0.0/src/langtorch/texts/chat.py` & `LangTorch-1.0.1/src/langtorch/texts/chat.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/texts/markdown.py` & `LangTorch-1.0.1/src/langtorch/texts/markdown.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/texts/text.py` & `LangTorch-1.0.1/src/langtorch/texts/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         return [self.__class__(m, parse=False) for m in self._content]
 
     @content.setter
     def content(self, content):
         if isinstance(content, tuple) and len(content) == 2 and (
                 isinstance(content[0], str) and isinstance(content[1], str)):
             AttributeError(
-                f"When setting the .content attribute, passing a tuple of strings is ambiguous. Pass either a list with a (key, value) tuple or a list with two strings."
+                f"When setting the .content attribute, passing a tuple of two strings is ambiguous. Pass a list with a tuple [(key, value)] or a list of strings [value, value]."
             )
 
         if isinstance(content, list):
             content = tuple(content)
         assert isinstance(content, tuple)
         self._content = self._to_ast(content, parser=False, is_tuple=True)
 
@@ -497,14 +497,15 @@
         modes = ["auto", "words", "sentances", "paragraphs"]  # TODO maybe use spliters from other packages
         assert mode in modes, f"Mode must be one of {modes}"
         if mode != "auto":
             raise NotImplementedError("Other modes are not yet implemented")
         from langtorch import TextTensor
         return TextTensor(str(self).split() if sep == "" else str(self).split(sep), parse=False)
 
+
     def __getitem__(self, index):
         if isinstance(index, str):
             return self.loc[index]
         return self.iloc[index]
 
     def __or__(self, other):
         return
@@ -512,24 +513,50 @@
     def __len__(self):
         return len(str(self.content))
 
     def __iter__(self):
         for s in self.content:
             yield s
 
+    # def _handle_other(self, other, method):
+    #     if isinstance(other, str) and not isinstance(other, Text):
+    #         return other
+    #     elif isinstance(other, Text):
+    #         return other.content
+    #     elif is_TextTensor(other):
+    #         if len(other.flat) == 1:
+    #             return self.__class__(*self.content, *other.item().content, parse=False)
+    #         else:
+    #             return other.__class__([getattr(self, method)(t) for t in other.flat], ttype=self.__class__, parse=False)
+    #     else:
+    #         return other
+
     def __add__(self, other):
         if isinstance(other, str) and not isinstance(other, Text):
             return self.__class__(*self.content, other, parse=False)
         elif isinstance(other, Text):
             return self.__class__(*self.content, *other.content, parse=False)
+        elif is_TextTensor(other):
+            if len(other.flat) == 1:
+                return self.__class__(*self.content, *other.item().content, parse=False)
+            else:
+                return other.__class__([self + t for t in other.flat], ttype=self.__class__, parse=False)
         else:
-            raise TypeError(f'Cannot add {type(other)}')
+            try:
+                return self.__class__(*self.content, other, parse=False)
+            except ValueError as e:
+                raise ValueError(f"Cannot add other={other} to Text. Failed to create a Text instance from other.") from e
 
     def __mul__(self, other):
-        if not isinstance(other, Text):
+        if is_TextTensor(other):
+            if len(other.flat) == 1:
+                other =  other.item()
+            else:
+                return other.__class__([self * t for t in other.flat], ttype=self.__class__, parse=False)
+        elif not isinstance(other, Text):
             try:
                 other = Text(other)
             except ParseException:
                 other = Text(other, parse=False)
 
         def flatten_keys(parent_key, value, sep='.'):
             if isinstance(value, tuple):
```

### Comparing `LangTorch-1.0.0/src/langtorch/tt/functional.py` & `LangTorch-1.0.1/src/langtorch/tt/functional.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_t/distance.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_t/distance.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_t/tokenizer.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_t/tokenizer.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/activation.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/activation.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                  T: float = 0.8,
                  tools: Optional[List[dict]] = None,
                  parse_output=False,
                  *args, **kwargs):
         super(OpenAI, self).__init__()
         self.system_message = str(system_message)
         self.model = model
-        self.backwad_prompt = backward_prompt
+        self.backward_prompt = backward_prompt
         self.keep_history = True if keep_history or kwargs.get('echo', False) else False
         if not 'temperature' in kwargs:
             kwargs['temperature'] = T
         cache = cache | (kwargs['temperature'] == .0)
         self.cache = cache
         self.kwargs = kwargs
 
@@ -116,20 +116,20 @@
                 m = m.loc[["user", "assistant"]]
             if np.all([key in ["user", "assistant"] for key in m.keys()]):
                 input[i] = m.items()
             elif "user" not in m.keys() or "assistant" not in m.keys():
                 # NOT STRICT
                 input[i] = [("user", str(m))]
                 logging.debug(
-                    f"A text without 'exculsively assistant' ot 'user' keys was passed to OpenAI Chat. Assuming the whole Text is a user message: = '{str(m)[:25]}'... ")
+                    f"A text without exclusively 'assistant' ot 'user' keys was passed to OpenAI Chat. Assuming the whole Text is one user message: = '{str(m)[:25]}'... ")
             else:
                 raise ValueError(
-                    f"Invalid input to OpenAI Chat. Ambigous input: some but not all items in TextTensor entries have keys 'user' or 'assistant'. Change the input into a valid chat, or the input was a single user message remove these keys or use entry.add_key_('user'): \nentry.items()=={m.items()}")
+                    f"Invalid input to OpenAI Chat. Ambiguous input: some but not all items in TextTensor entries have keys 'user' or 'assistant'. Change the input into a valid chat, or the input was a single user message remove these keys or use entry.add_key_('user'): \nentry.items()=={m.items()}")
         logging.debug(f"Chat api input: {input}")
-        logging.debug(f"Chat api system messages: {system_messages}")
+        logging.debug(f"Chat api unique system messages: {set(system_messages)}")
 
         result = chat(input, system_messages, model=self.model, cache=self.cache, as_str=True, tools=self.tool_jsons,
                       **self.kwargs)
 
         assert result is not None
         if not self.keep_history:
             return TextTensor(result, parse=self.parse_output).reshape(shape)
```

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/assistantmodule.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/assistantmodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/codemodule.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/codemodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/conv.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/conv.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/linear.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/linear.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/loss.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/loss.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/textmodule.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/textmodule.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/tt/modules/to_tt/transformers.py` & `LangTorch-1.0.1/src/langtorch/tt/modules/to_tt/transformers.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/types.py` & `LangTorch-1.0.1/src/langtorch/types.py`

 * *Files identical despite different names*

### Comparing `LangTorch-1.0.0/src/langtorch/utils.py` & `LangTorch-1.0.1/src/langtorch/utils.py`

 * *Files identical despite different names*

