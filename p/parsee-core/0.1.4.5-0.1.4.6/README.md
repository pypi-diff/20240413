# Comparing `tmp/parsee_core-0.1.4.5.tar.gz` & `tmp/parsee_core-0.1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsee_core-0.1.4.5.tar", max compression
+gzip compressed data, was "parsee_core-0.1.4.6.tar", max compression
```

## Comparing `parsee_core-0.1.4.5.tar` & `parsee_core-0.1.4.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1066 2024-03-21 12:33:53.103983 parsee_core-0.1.4.5/LICENSE
--rw-r--r--   0        0        0      529 2024-03-27 13:19:30.023928 parsee_core-0.1.4.5/parsee/__init__.py
--rw-r--r--   0        0        0     5174 2024-04-12 10:32:38.964069 parsee_core-0.1.4.5/parsee/cloud/api.py
--rw-r--r--   0        0        0     1093 2024-04-12 10:39:58.510402 parsee_core-0.1.4.5/parsee/cloud/cloud_image_fetcher.py
--rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.4.5/parsee/converters/__init__.py
--rw-r--r--   0        0        0     6063 2024-03-29 10:54:00.293459 parsee_core-0.1.4.5/parsee/converters/html_extraction.py
--rw-r--r--   0        0        0     3752 2024-04-12 10:39:58.514327 parsee_core-0.1.4.5/parsee/converters/image_creation.py
--rw-r--r--   0        0        0      399 2024-03-27 13:22:36.894150 parsee_core-0.1.4.5/parsee/converters/interfaces.py
--rw-r--r--   0        0        0     1806 2024-04-10 14:57:20.432097 parsee_core-0.1.4.5/parsee/converters/json_to_raw.py
--rw-r--r--   0        0        0     1069 2024-04-10 14:57:20.432511 parsee_core-0.1.4.5/parsee/converters/langchain.py
--rw-r--r--   0        0        0     3015 2024-04-10 14:57:20.432769 parsee_core-0.1.4.5/parsee/converters/main.py
--rw-r--r--   0        0        0     4324 2024-03-27 13:19:30.029388 parsee_core-0.1.4.5/parsee/converters/pdf_extraction.py
--rw-r--r--   0        0        0      491 2024-03-27 13:22:36.895882 parsee_core-0.1.4.5/parsee/converters/simple_text.py
--rw-r--r--   0        0        0     6680 2024-03-25 10:47:46.831244 parsee_core-0.1.4.5/parsee/datasets/dataset_dataclasses.py
--rw-r--r--   0        0        0     7820 2024-03-20 10:51:40.783264 parsee_core-0.1.4.5/parsee/datasets/evaluation/main.py
--rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.4.5/parsee/datasets/main.py
--rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.4.5/parsee/datasets/readers/disk_reader.py
--rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.4.5/parsee/datasets/readers/interfaces.py
--rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.4.5/parsee/datasets/writers/disk_writer.py
--rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.4.5/parsee/datasets/writers/interfaces.py
--rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.4.5/parsee/extraction/__init__.py
--rw-r--r--   0        0        0     4138 2024-04-11 14:09:13.370382 parsee_core-0.1.4.5/parsee/extraction/extractor_dataclasses.py
--rw-r--r--   0        0        0    29463 2024-04-11 11:20:23.988527 parsee_core-0.1.4.5/parsee/extraction/extractor_elements.py
--rw-r--r--   0        0        0     9472 2024-04-05 15:38:22.487342 parsee_core-0.1.4.5/parsee/extraction/final_structuring.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.5/parsee/extraction/models/__init__.py
--rw-r--r--   0        0        0     2062 2024-04-10 14:57:20.433864 parsee_core-0.1.4.5/parsee/extraction/models/helpers.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.5/parsee/extraction/models/llm_models/__init__.py
--rw-r--r--   0        0        0     2882 2024-04-10 14:57:20.434116 parsee_core-0.1.4.5/parsee/extraction/models/llm_models/anthropic_model.py
--rw-r--r--   0        0        0     2866 2024-04-10 14:57:20.434321 parsee_core-0.1.4.5/parsee/extraction/models/llm_models/chatgpt_model.py
--rw-r--r--   0        0        0      888 2024-04-10 14:57:20.434563 parsee_core-0.1.4.5/parsee/extraction/models/llm_models/llm_base_model.py
--rw-r--r--   0        0        0     1694 2024-04-10 14:57:20.434940 parsee_core-0.1.4.5/parsee/extraction/models/llm_models/ollama_model.py
--rw-r--r--   0        0        0      875 2024-04-10 14:57:20.435213 parsee_core-0.1.4.5/parsee/extraction/models/llm_models/prompts.py
--rw-r--r--   0        0        0     1971 2024-04-10 14:57:20.435485 parsee_core-0.1.4.5/parsee/extraction/models/llm_models/replicate_model.py
--rw-r--r--   0        0        0     7875 2024-03-19 14:15:12.265884 parsee_core-0.1.4.5/parsee/extraction/models/llm_models/structuring_schema.py
--rw-r--r--   0        0        0      985 2024-04-10 14:57:20.435851 parsee_core-0.1.4.5/parsee/extraction/models/model_dataclasses.py
--rw-r--r--   0        0        0     8163 2024-03-20 12:24:18.192932 parsee_core-0.1.4.5/parsee/extraction/models/model_loader.py
--rw-r--r--   0        0        0     4651 2024-04-12 11:29:47.420418 parsee_core-0.1.4.5/parsee/extraction/run.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.5/parsee/extraction/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.5/parsee/extraction/tasks/element_classification/__init__.py
--rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.4.5/parsee/extraction/tasks/element_classification/element_model.py
--rw-r--r--   0        0        0     2199 2024-04-10 14:57:20.436266 parsee_core-0.1.4.5/parsee/extraction/tasks/element_classification/element_model_llm.py
--rw-r--r--   0        0        0     8051 2024-04-10 14:57:20.436667 parsee_core-0.1.4.5/parsee/extraction/tasks/element_classification/features.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/__init__.py
--rw-r--r--   0        0        0     6108 2024-04-04 15:01:44.484913 parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/features.py
--rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/mapping_model.py
--rw-r--r--   0        0        0     2519 2024-04-10 14:57:20.436928 parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/mapping_model_llm.py
--rw-r--r--   0        0        0      894 2024-03-28 20:25:58.634238 parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/utils.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.5/parsee/extraction/tasks/meta_info_structuring/__init__.py
--rw-r--r--   0        0        0    13073 2024-04-10 14:57:20.437207 parsee_core-0.1.4.5/parsee/extraction/tasks/meta_info_structuring/features.py
--rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.4.5/parsee/extraction/tasks/meta_info_structuring/meta_info.py
--rw-r--r--   0        0        0     2641 2024-04-10 14:57:20.437514 parsee_core-0.1.4.5/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.5/parsee/extraction/tasks/questions/__init__.py
--rw-r--r--   0        0        0     6136 2024-04-10 14:57:20.437823 parsee_core-0.1.4.5/parsee/extraction/tasks/questions/features.py
--rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.4.5/parsee/extraction/tasks/questions/question_model.py
--rw-r--r--   0        0        0     4031 2024-04-10 14:57:20.438067 parsee_core-0.1.4.5/parsee/extraction/tasks/questions/question_model_llm.py
--rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.4.5/parsee/extraction/tasks/questions/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.4.5/parsee/storage/__init__.py
--rw-r--r--   0        0        0     2491 2024-04-12 10:17:23.380409 parsee_core-0.1.4.5/parsee/storage/in_memory_storage.py
--rw-r--r--   0        0        0     1212 2024-04-10 14:57:20.438565 parsee_core-0.1.4.5/parsee/storage/interfaces.py
--rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.4.5/parsee/storage/vector_stores/interfaces.py
--rw-r--r--   0        0        0     3204 2024-03-22 17:12:35.963569 parsee_core-0.1.4.5/parsee/storage/vector_stores/simple_faiss.py
--rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.4.5/parsee/templates/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-05 15:38:22.487748 parsee_core-0.1.4.5/parsee/templates/element_schema.py
--rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.4.5/parsee/templates/general_structuring_schema.py
--rw-r--r--   0        0        0     4019 2024-04-05 15:38:22.488067 parsee_core-0.1.4.5/parsee/templates/helpers.py
--rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.4.5/parsee/templates/job_template.py
--rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.4.5/parsee/templates/mappings.py
--rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.4.5/parsee/templates/template_from_json.py
--rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.4.5/parsee/utils/__init__.py
--rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.4.5/parsee/utils/constants.py
--rw-r--r--   0        0        0      781 2024-03-27 13:19:30.038637 parsee_core-0.1.4.5/parsee/utils/enums.py
--rw-r--r--   0        0        0     6632 2024-04-08 08:51:44.149915 parsee_core-0.1.4.5/parsee/utils/helper.py
--rw-r--r--   0        0        0     2030 2024-03-26 12:40:38.547700 parsee_core-0.1.4.5/parsee/utils/sample_items.py
--rw-r--r--   0        0        0      827 2024-04-12 10:47:01.739161 parsee_core-0.1.4.5/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 parsee_core-0.1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-21 12:33:53.103983 parsee_core-0.1.4.6/LICENSE
+-rw-r--r--   0        0        0      529 2024-03-27 13:19:30.023928 parsee_core-0.1.4.6/parsee/__init__.py
+-rw-r--r--   0        0        0     5174 2024-04-12 10:32:38.964069 parsee_core-0.1.4.6/parsee/cloud/api.py
+-rw-r--r--   0        0        0     1093 2024-04-12 10:39:58.510402 parsee_core-0.1.4.6/parsee/cloud/cloud_image_fetcher.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.4.6/parsee/converters/__init__.py
+-rw-r--r--   0        0        0     6063 2024-03-29 10:54:00.293459 parsee_core-0.1.4.6/parsee/converters/html_extraction.py
+-rw-r--r--   0        0        0     3752 2024-04-12 10:39:58.514327 parsee_core-0.1.4.6/parsee/converters/image_creation.py
+-rw-r--r--   0        0        0      399 2024-03-27 13:22:36.894150 parsee_core-0.1.4.6/parsee/converters/interfaces.py
+-rw-r--r--   0        0        0     1806 2024-04-10 14:57:20.432097 parsee_core-0.1.4.6/parsee/converters/json_to_raw.py
+-rw-r--r--   0        0        0     1069 2024-04-10 14:57:20.432511 parsee_core-0.1.4.6/parsee/converters/langchain.py
+-rw-r--r--   0        0        0     3015 2024-04-10 14:57:20.432769 parsee_core-0.1.4.6/parsee/converters/main.py
+-rw-r--r--   0        0        0     4324 2024-03-27 13:19:30.029388 parsee_core-0.1.4.6/parsee/converters/pdf_extraction.py
+-rw-r--r--   0        0        0      491 2024-03-27 13:22:36.895882 parsee_core-0.1.4.6/parsee/converters/simple_text.py
+-rw-r--r--   0        0        0     6680 2024-03-25 10:47:46.831244 parsee_core-0.1.4.6/parsee/datasets/dataset_dataclasses.py
+-rw-r--r--   0        0        0     7820 2024-03-20 10:51:40.783264 parsee_core-0.1.4.6/parsee/datasets/evaluation/main.py
+-rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.4.6/parsee/datasets/main.py
+-rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.4.6/parsee/datasets/readers/disk_reader.py
+-rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.4.6/parsee/datasets/readers/interfaces.py
+-rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.4.6/parsee/datasets/writers/disk_writer.py
+-rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.4.6/parsee/datasets/writers/interfaces.py
+-rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.4.6/parsee/extraction/__init__.py
+-rw-r--r--   0        0        0     4138 2024-04-11 14:09:13.370382 parsee_core-0.1.4.6/parsee/extraction/extractor_dataclasses.py
+-rw-r--r--   0        0        0    30049 2024-04-13 09:32:29.198541 parsee_core-0.1.4.6/parsee/extraction/extractor_elements.py
+-rw-r--r--   0        0        0     9472 2024-04-05 15:38:22.487342 parsee_core-0.1.4.6/parsee/extraction/final_structuring.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.6/parsee/extraction/models/__init__.py
+-rw-r--r--   0        0        0     2062 2024-04-10 14:57:20.433864 parsee_core-0.1.4.6/parsee/extraction/models/helpers.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.6/parsee/extraction/models/llm_models/__init__.py
+-rw-r--r--   0        0        0     2882 2024-04-10 14:57:20.434116 parsee_core-0.1.4.6/parsee/extraction/models/llm_models/anthropic_model.py
+-rw-r--r--   0        0        0     2866 2024-04-10 14:57:20.434321 parsee_core-0.1.4.6/parsee/extraction/models/llm_models/chatgpt_model.py
+-rw-r--r--   0        0        0      888 2024-04-10 14:57:20.434563 parsee_core-0.1.4.6/parsee/extraction/models/llm_models/llm_base_model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 14:57:20.434940 parsee_core-0.1.4.6/parsee/extraction/models/llm_models/ollama_model.py
+-rw-r--r--   0        0        0      875 2024-04-10 14:57:20.435213 parsee_core-0.1.4.6/parsee/extraction/models/llm_models/prompts.py
+-rw-r--r--   0        0        0     1971 2024-04-10 14:57:20.435485 parsee_core-0.1.4.6/parsee/extraction/models/llm_models/replicate_model.py
+-rw-r--r--   0        0        0     7875 2024-03-19 14:15:12.265884 parsee_core-0.1.4.6/parsee/extraction/models/llm_models/structuring_schema.py
+-rw-r--r--   0        0        0      985 2024-04-10 14:57:20.435851 parsee_core-0.1.4.6/parsee/extraction/models/model_dataclasses.py
+-rw-r--r--   0        0        0     8163 2024-03-20 12:24:18.192932 parsee_core-0.1.4.6/parsee/extraction/models/model_loader.py
+-rw-r--r--   0        0        0     4651 2024-04-12 11:29:47.420418 parsee_core-0.1.4.6/parsee/extraction/run.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.6/parsee/extraction/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.6/parsee/extraction/tasks/element_classification/__init__.py
+-rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.4.6/parsee/extraction/tasks/element_classification/element_model.py
+-rw-r--r--   0        0        0     2199 2024-04-10 14:57:20.436266 parsee_core-0.1.4.6/parsee/extraction/tasks/element_classification/element_model_llm.py
+-rw-r--r--   0        0        0     8051 2024-04-10 14:57:20.436667 parsee_core-0.1.4.6/parsee/extraction/tasks/element_classification/features.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/__init__.py
+-rw-r--r--   0        0        0     6108 2024-04-04 15:01:44.484913 parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/features.py
+-rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/mapping_model.py
+-rw-r--r--   0        0        0     2519 2024-04-10 14:57:20.436928 parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/mapping_model_llm.py
+-rw-r--r--   0        0        0      894 2024-03-28 20:25:58.634238 parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/utils.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.6/parsee/extraction/tasks/meta_info_structuring/__init__.py
+-rw-r--r--   0        0        0    13073 2024-04-10 14:57:20.437207 parsee_core-0.1.4.6/parsee/extraction/tasks/meta_info_structuring/features.py
+-rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.4.6/parsee/extraction/tasks/meta_info_structuring/meta_info.py
+-rw-r--r--   0        0        0     2641 2024-04-10 14:57:20.437514 parsee_core-0.1.4.6/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.6/parsee/extraction/tasks/questions/__init__.py
+-rw-r--r--   0        0        0     6371 2024-04-13 09:30:58.743777 parsee_core-0.1.4.6/parsee/extraction/tasks/questions/features.py
+-rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.4.6/parsee/extraction/tasks/questions/question_model.py
+-rw-r--r--   0        0        0     4031 2024-04-10 14:57:20.438067 parsee_core-0.1.4.6/parsee/extraction/tasks/questions/question_model_llm.py
+-rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.4.6/parsee/extraction/tasks/questions/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.4.6/parsee/storage/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-12 10:17:23.380409 parsee_core-0.1.4.6/parsee/storage/in_memory_storage.py
+-rw-r--r--   0        0        0     1212 2024-04-10 14:57:20.438565 parsee_core-0.1.4.6/parsee/storage/interfaces.py
+-rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.4.6/parsee/storage/vector_stores/interfaces.py
+-rw-r--r--   0        0        0     3204 2024-03-22 17:12:35.963569 parsee_core-0.1.4.6/parsee/storage/vector_stores/simple_faiss.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.4.6/parsee/templates/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-05 15:38:22.487748 parsee_core-0.1.4.6/parsee/templates/element_schema.py
+-rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.4.6/parsee/templates/general_structuring_schema.py
+-rw-r--r--   0        0        0     4019 2024-04-05 15:38:22.488067 parsee_core-0.1.4.6/parsee/templates/helpers.py
+-rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.4.6/parsee/templates/job_template.py
+-rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.4.6/parsee/templates/mappings.py
+-rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.4.6/parsee/templates/template_from_json.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.4.6/parsee/utils/__init__.py
+-rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.4.6/parsee/utils/constants.py
+-rw-r--r--   0        0        0      781 2024-03-27 13:19:30.038637 parsee_core-0.1.4.6/parsee/utils/enums.py
+-rw-r--r--   0        0        0     6632 2024-04-08 08:51:44.149915 parsee_core-0.1.4.6/parsee/utils/helper.py
+-rw-r--r--   0        0        0     2030 2024-03-26 12:40:38.547700 parsee_core-0.1.4.6/parsee/utils/sample_items.py
+-rw-r--r--   0        0        0      827 2024-04-13 09:35:28.948036 parsee_core-0.1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 parsee_core-0.1.4.6/PKG-INFO
```

### Comparing `parsee_core-0.1.4.5/LICENSE` & `parsee_core-0.1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/__init__.py` & `parsee_core-0.1.4.6/parsee/__init__.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/cloud/api.py` & `parsee_core-0.1.4.6/parsee/cloud/api.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/cloud/cloud_image_fetcher.py` & `parsee_core-0.1.4.6/parsee/cloud/cloud_image_fetcher.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/converters/html_extraction.py` & `parsee_core-0.1.4.6/parsee/converters/html_extraction.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/converters/image_creation.py` & `parsee_core-0.1.4.6/parsee/converters/image_creation.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/converters/json_to_raw.py` & `parsee_core-0.1.4.6/parsee/converters/json_to_raw.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/converters/langchain.py` & `parsee_core-0.1.4.6/parsee/converters/langchain.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/converters/main.py` & `parsee_core-0.1.4.6/parsee/converters/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/converters/pdf_extraction.py` & `parsee_core-0.1.4.6/parsee/converters/pdf_extraction.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/datasets/dataset_dataclasses.py` & `parsee_core-0.1.4.6/parsee/datasets/dataset_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/datasets/evaluation/main.py` & `parsee_core-0.1.4.6/parsee/datasets/evaluation/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/datasets/main.py` & `parsee_core-0.1.4.6/parsee/datasets/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/datasets/readers/disk_reader.py` & `parsee_core-0.1.4.6/parsee/datasets/readers/disk_reader.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/datasets/readers/interfaces.py` & `parsee_core-0.1.4.6/parsee/datasets/readers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/datasets/writers/disk_writer.py` & `parsee_core-0.1.4.6/parsee/datasets/writers/disk_writer.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/datasets/writers/interfaces.py` & `parsee_core-0.1.4.6/parsee/datasets/writers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/extractor_dataclasses.py` & `parsee_core-0.1.4.6/parsee/extraction/extractor_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/extractor_elements.py` & `parsee_core-0.1.4.6/parsee/extraction/extractor_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,14 +514,29 @@
         if contain_numbers:
             text = " ".join(text_pieces)
         else:
             text = ", ".join(text_pieces)
         text = re.sub(r' +', ' ', text)
         return "table: " + text
 
+    def get_text_and_surrounding_elements_text(self, elements: List[ExtractedEl]):
+
+        main_text = self.get_text_llm(True)
+
+        max_elements = 3
+
+        text_pieces = []
+        for a in range(self.source.element_index-1, max(-1, self.source.element_index-max_elements-1), -1):
+            if isinstance(elements[a], StructuredTable):
+                break
+            text_pieces.append(elements[a].get_text_llm(True))
+        text_pieces.reverse()
+        text_before = "\n".join(text_pieces)
+        return f"Table element - Text before table: {text_before}; {main_text}"
+
     def get_data_simplified(self):
         rows = []
 
         for row in self.rows:
             temp_row = []
             for cell_obj in row.final_values:
                 temp_row.append({"colspan": cell_obj.colspan, "val": cell_obj.val})
```

### Comparing `parsee_core-0.1.4.5/parsee/extraction/final_structuring.py` & `parsee_core-0.1.4.6/parsee/extraction/final_structuring.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/helpers.py` & `parsee_core-0.1.4.6/parsee/extraction/models/helpers.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/llm_models/anthropic_model.py` & `parsee_core-0.1.4.6/parsee/extraction/models/llm_models/anthropic_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/llm_models/chatgpt_model.py` & `parsee_core-0.1.4.6/parsee/extraction/models/llm_models/chatgpt_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/llm_models/llm_base_model.py` & `parsee_core-0.1.4.6/parsee/extraction/models/llm_models/llm_base_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/llm_models/ollama_model.py` & `parsee_core-0.1.4.6/parsee/extraction/models/llm_models/ollama_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/llm_models/prompts.py` & `parsee_core-0.1.4.6/parsee/extraction/models/llm_models/prompts.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/llm_models/replicate_model.py` & `parsee_core-0.1.4.6/parsee/extraction/models/llm_models/replicate_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/llm_models/structuring_schema.py` & `parsee_core-0.1.4.6/parsee/extraction/models/llm_models/structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/model_dataclasses.py` & `parsee_core-0.1.4.6/parsee/extraction/models/model_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/models/model_loader.py` & `parsee_core-0.1.4.6/parsee/extraction/models/model_loader.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/run.py` & `parsee_core-0.1.4.6/parsee/extraction/run.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/element_classification/element_model.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/element_classification/element_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/element_classification/element_model_llm.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/element_classification/element_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/element_classification/features.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/element_classification/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/features.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/mapping_model.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/mapping_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/mapping_model_llm.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/mapping_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/mappings/utils.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/mappings/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/meta_info_structuring/features.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/meta_info_structuring/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/meta_info_structuring/meta_info.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/meta_info_structuring/meta_info.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/questions/features.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/questions/features.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from parsee.extraction.models.llm_models.prompts import Prompt
 from parsee.extraction.models.llm_models.structuring_schema import get_prompt_schema_item
 from parsee.templates.general_structuring_schema import GeneralQueryItemSchema, StructuringItemSchema
 from parsee.extraction.tasks.questions.utils import MAIN_QUESTION_STR
 from parsee.extraction.extractor_dataclasses import ParseeMeta, ExtractedSource
 from parsee.utils.enums import DocumentType, SearchStrategy
 from parsee.storage.interfaces import StorageManager
-from parsee.extraction.extractor_elements import StandardDocumentFormat, ExtractedEl
+from parsee.extraction.extractor_elements import StandardDocumentFormat, ExtractedEl, StructuredTable
 
 
 class GeneralQueriesPromptBuilder:
 
     storage: StorageManager
 
     def __init__(self, storage: StorageManager):
@@ -38,18 +38,18 @@
         if schema_item.searchStrategy == SearchStrategy.VECTOR:
             return self.storage.vector_store.find_closest_elements(document, schema_item.title, schema_item.keywords, False)
         elif schema_item.searchStrategy == SearchStrategy.START:
             return document.elements
         else:
             raise NotImplemented
 
-    def get_elements_text(self, elements: List[ExtractedEl]):
-        llm_text = "This is the available data to answer the question (in the following, if tables have empty cells, they are omitted):\n"
+    def get_elements_text(self, elements: List[ExtractedEl], document: StandardDocumentFormat):
+        llm_text = "This is the available data to answer the question (in the following, if tables have empty cells, they are omitted, if a cell spans several columns, values might be repeated for each cell):\n"
         for el in elements:
-            llm_text += f"[{el.source.element_index}]: {el.get_text_llm(True)}\n"
+            llm_text += f"[{el.source.element_index}]: {el.get_text_and_surrounding_elements_text(document.elements) if isinstance(el, StructuredTable) else el.get_text_llm(True)}\n"
         return llm_text
 
     def build_prompt(self, structuring_item: GeneralQueryItemSchema, meta_items: List[StructuringItemSchema], document: StandardDocumentFormat, relevant_elements_custom: Optional[List[ExtractedEl]] = None, multimodal: bool = False, max_images: Optional[int] = None, max_image_size: Optional[int] = None) -> Prompt:
 
         elements = self.get_relevant_elements(structuring_item, document) if relevant_elements_custom is None else relevant_elements_custom
 
         if not multimodal:
@@ -80,9 +80,9 @@
             for meta_item in relevant_meta_items:
                 meta_prompt_item = get_prompt_schema_item(meta_item)
                 main_question += f"\n({meta_item.id}): {meta_item.title} {meta_item.additionalInfo} {meta_prompt_item.get_possible_values_str()}"
 
         prompt = Prompt(general_info, main_question,
                         'Please at the end of each answer also provide the numbers of the text fragments you used to answer in square brackets.' if not multimodal else "",
                         full_example,
-                        self.get_elements_text(elements) if not multimodal else self.storage.image_creator.get_images(document, elements, max_images, max_image_size))
+                        self.get_elements_text(elements, document) if not multimodal else self.storage.image_creator.get_images(document, elements, max_images, max_image_size))
         return prompt
```

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/questions/question_model.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/questions/question_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/questions/question_model_llm.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/questions/question_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/extraction/tasks/questions/utils.py` & `parsee_core-0.1.4.6/parsee/extraction/tasks/questions/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/storage/in_memory_storage.py` & `parsee_core-0.1.4.6/parsee/storage/in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/storage/interfaces.py` & `parsee_core-0.1.4.6/parsee/storage/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/storage/vector_stores/simple_faiss.py` & `parsee_core-0.1.4.6/parsee/storage/vector_stores/simple_faiss.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/templates/element_schema.py` & `parsee_core-0.1.4.6/parsee/templates/element_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/templates/general_structuring_schema.py` & `parsee_core-0.1.4.6/parsee/templates/general_structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/templates/helpers.py` & `parsee_core-0.1.4.6/parsee/templates/helpers.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/templates/job_template.py` & `parsee_core-0.1.4.6/parsee/templates/job_template.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/templates/mappings.py` & `parsee_core-0.1.4.6/parsee/templates/mappings.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/utils/enums.py` & `parsee_core-0.1.4.6/parsee/utils/enums.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/utils/helper.py` & `parsee_core-0.1.4.6/parsee/utils/helper.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/parsee/utils/sample_items.py` & `parsee_core-0.1.4.6/parsee/utils/sample_items.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.5/pyproject.toml` & `parsee_core-0.1.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsee-core"
-version = "0.1.4.5"
+version = "0.1.4.6"
 description = ""
 authors = ["Parsee.ai <info@parsee.ai>"]
 homepage = "https://parsee.ai"
 packages = [{include = "parsee"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
```

### Comparing `parsee_core-0.1.4.5/PKG-INFO` & `parsee_core-0.1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsee-core
-Version: 0.1.4.5
+Version: 0.1.4.6
 Summary: 
 Home-page: https://parsee.ai
 Author: Parsee.ai
 Author-email: info@parsee.ai
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

