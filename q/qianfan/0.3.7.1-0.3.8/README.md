# Comparing `tmp/qianfan-0.3.7.1.tar.gz` & `tmp/qianfan-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianfan-0.3.7.1.tar", max compression
+gzip compressed data, was "qianfan-0.3.8.tar", max compression
```

## Comparing `qianfan-0.3.7.1.tar` & `qianfan-0.3.8.tar`

### file list

```diff
@@ -1,160 +1,166 @@
--rw-r--r--   0        0        0     6443 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/README.pypi.md
--rw-r--r--   0        0        0     3668 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/pyproject.toml
--rw-r--r--   0        0        0     1578 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/__init__.py
--rw-r--r--   0        0        0      659 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/__init__.py
--rw-r--r--   0        0        0     2451 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/context.py
--rw-r--r--   0        0        0     4502 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/launcher.py
--rw-r--r--   0        0        0      847 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/runner/__init__.py
--rw-r--r--   0        0        0     1688 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/runner/base.py
--rw-r--r--   0        0        0     6028 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/runner/infer_runner.py
--rw-r--r--   0        0        0     6571 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/runner/qianfan_runner.py
--rw-r--r--   0        0        0     1460 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/space.py
--rw-r--r--   0        0        0      784 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/suggestor/__init__.py
--rw-r--r--   0        0        0     3370 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/suggestor/base.py
--rw-r--r--   0        0        0     3356 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/suggestor/random_suggestor.py
--rw-r--r--   0        0        0     3973 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/tune.py
--rw-r--r--   0        0        0     1357 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/autotuner/utils.py
--rw-r--r--   0        0        0      699 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/__init__.py
--rw-r--r--   0        0        0    15290 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/chat.py
--rw-r--r--   0        0        0     7120 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/completion.py
--rw-r--r--   0        0        0    14564 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/dataset.py
--rw-r--r--   0        0        0      790 2024-04-04 02:53:41.268825 qianfan-0.3.7.1/qianfan/common/client/embedding.py
--rw-r--r--   0        0        0     9595 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/evaluation.py
--rw-r--r--   0        0        0     6437 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/main.py
--rw-r--r--   0        0        0     4107 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/openai_adapter.py
--rw-r--r--   0        0        0    17018 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/plugin.py
--rw-r--r--   0        0        0    23840 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/trainer.py
--rw-r--r--   0        0        0     3265 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/txt2img.py
--rw-r--r--   0        0        0     9991 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/client/utils.py
--rw-r--r--   0        0        0        1 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/hub/__init__.py
--rw-r--r--   0        0        0     5823 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/hub/hub.py
--rw-r--r--   0        0        0     3512 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/hub/interface.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/persister/__init__.py
--rw-r--r--   0        0        0      963 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/persister/base.py
--rw-r--r--   0        0        0     2965 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/persister/persist.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/prompt/__init__.py
--rw-r--r--   0        0        0    23878 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/prompt/prompt.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/runnable/__init__.py
--rw-r--r--   0        0        0     6386 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/runnable/base.py
--rw-r--r--   0        0        0     3698 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/tool/baidu_search_tool.py
--rw-r--r--   0        0        0     7561 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/tool/base_tool.py
--rw-r--r--   0        0        0     2962 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/tool/duckduckgo_search_tool.py
--rw-r--r--   0        0        0     3312 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/common/tool/wikipedia_tool.py
--rw-r--r--   0        0        0     9582 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/config.py
--rw-r--r--   0        0        0    12267 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/consts.py
--rw-r--r--   0        0        0     1367 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/__init__.py
--rw-r--r--   0        0        0     2786 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/consts.py
--rw-r--r--   0        0        0     4363 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_operator.py
--rw-r--r--   0        0        0     1013 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/__init__.py
--rw-r--r--   0        0        0    27521 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/baidu_qianfan.py
--rw-r--r--   0        0        0     2701 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/base.py
--rw-r--r--   0        0        0    13584 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/bos.py
--rw-r--r--   0        0        0     9420 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/chunk_reader.py
--rw-r--r--   0        0        0     9532 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/file.py
--rw-r--r--   0        0        0    23618 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/data_source/utils.py
--rw-r--r--   0        0        0    58798 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/dataset.py
--rw-r--r--   0        0        0    14197 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/dataset_utils.py
--rw-r--r--   0        0        0     1139 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/__init__.py
--rw-r--r--   0        0        0     2237 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/base.py
--rw-r--r--   0        0        0     3942 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_character_repetition_filter.py
--rw-r--r--   0        0        0     4482 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_flagged_words.py
--rw-r--r--   0        0        0     2443 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_sentence_length_filter.py
--rw-r--r--   0        0        0     2504 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_special_characters.py
--rw-r--r--   0        0        0     4313 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_stopwords.py
--rw-r--r--   0        0        0     3085 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_word_number.py
--rw-r--r--   0        0        0     3910 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_word_repetition_filter.py
--rw-r--r--   0        0        0     4483 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/consts.py
--rw-r--r--   0        0        0     4693 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/utils.py
--rw-r--r--   0        0        0   136258 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/local_data_operators/word_list.py
--rw-r--r--   0        0        0     2832 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/process_interface.py
--rw-r--r--   0        0        0     4363 2024-04-04 02:53:41.272825 qianfan-0.3.7.1/qianfan/dataset/qianfan_data_operators.py
--rw-r--r--   0        0        0    10622 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/dataset/schema.py
--rw-r--r--   0        0        0    40452 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/dataset/table.py
--rw-r--r--   0        0        0     1302 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/dataset/table_utils.py
--rw-r--r--   0        0        0     2334 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/errors.py
--rw-r--r--   0        0        0      878 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/__init__.py
--rw-r--r--   0        0        0     2748 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/consts.py
--rw-r--r--   0        0        0    26228 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/evaluation_manager.py
--rw-r--r--   0        0        0     1325 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/evaluation_result.py
--rw-r--r--   0        0        0     4484 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/evaluator.py
--rw-r--r--   0        0        0     4379 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/local_evaluator.py
--rw-r--r--   0        0        0     2468 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/evaluation/opencompass_evaluator.py
--rw-r--r--   0        0        0       66 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/README.md
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/__init__.py
--rw-r--r--   0        0        0      200 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/langchain/__init__.py
--rw-r--r--   0        0        0      212 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/langchain/agents/__init__.py
--rw-r--r--   0        0        0    13709 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/openai/__init__.py
--rw-r--r--   0        0        0    18554 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/openai/adapter.py
--rw-r--r--   0        0        0     1602 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0     7804 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py
--rw-r--r--   0        0        0     1627 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py
--rw-r--r--   0        0        0     5365 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py
--rw-r--r--   0        0        0     4056 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py
--rw-r--r--   0        0        0     2577 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/fake_pyarrow_replacer.py
--rw-r--r--   0        0        0      742 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/model/__init__.py
--rw-r--r--   0        0        0      923 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/model/configs.py
--rw-r--r--   0        0        0      938 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/model/consts.py
--rw-r--r--   0        0        0    22871 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/model/model.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/py.typed
--rw-r--r--   0        0        0     1648 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/auth/__init__.py
--rw-r--r--   0        0        0     1656 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/auth/iam.py
--rw-r--r--   0        0        0    15255 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/auth/oauth.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/__init__.py
--rw-r--r--   0        0        0     4183 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/charge.py
--rw-r--r--   0        0        0     7503 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/consts.py
--rw-r--r--   0        0        0    30894 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/data.py
--rw-r--r--   0        0        0    16279 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/finetune.py
--rw-r--r--   0        0        0    23076 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/model.py
--rw-r--r--   0        0        0    19491 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/prompt.py
--rw-r--r--   0        0        0     5607 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/service.py
--rw-r--r--   0        0        0     4941 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/console/utils.py
--rw-r--r--   0        0        0     3779 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/http_client.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/images/__init__.py
--rw-r--r--   0        0        0    11411 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/images/image2text.py
--rw-r--r--   0        0        0    11777 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/images/text2image.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/__init__.py
--rw-r--r--   0        0        0    27287 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/base.py
--rw-r--r--   0        0        0    42166 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/chat_completion.py
--rw-r--r--   0        0        0    11545 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/completion.py
--rw-r--r--   0        0        0    10678 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/embedding.py
--rw-r--r--   0        0        0    13139 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/llm/plugin.py
--rw-r--r--   0        0        0    14096 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/requestor/__init__.py
--rw-r--r--   0        0        0    12834 2024-04-04 02:53:41.276825 qianfan-0.3.7.1/qianfan/resources/requestor/base.py
--rw-r--r--   0        0        0     3189 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/requestor/console_requestor.py
--rw-r--r--   0        0        0    21478 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/requestor/openapi_requestor.py
--rw-r--r--   0        0        0     9899 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/token_limiter.py
--rw-r--r--   0        0        0        0 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/tools/__init__.py
--rw-r--r--   0        0        0     4909 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/tools/tokenizer.py
--rw-r--r--   0        0        0     3580 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/tools/utils.py
--rw-r--r--   0        0        0     9199 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/resources/typing.py
--rw-r--r--   0        0        0     1141 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/__init__.py
--rw-r--r--   0        0        0    44551 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/actions.py
--rw-r--r--   0        0        0     6000 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/base.py
--rw-r--r--   0        0        0    38156 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/configs.py
--rw-r--r--   0        0        0     3600 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/consts.py
--rw-r--r--   0        0        0     3403 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/event.py
--rw-r--r--   0        0        0    11390 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/finetune.py
--rw-r--r--   0        0        0     9561 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/pipeline.py
--rw-r--r--   0        0        0     7772 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/post_pretrain.py
--rw-r--r--   0        0        0     1680 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/ppl.yaml
--rw-r--r--   0        0        0     4709 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/trainer/trainer.py
--rw-r--r--   0        0        0     1244 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/utils/__init__.py
--rw-r--r--   0        0        0     4647 2024-04-04 02:53:41.280825 qianfan-0.3.7.1/qianfan/utils/bos_uploader.py
--rw-r--r--   0        0        0      696 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/cache/__init__.py
--rw-r--r--   0        0        0      787 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/cache/base.py
--rw-r--r--   0        0        0      827 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/__init__.py
--rw-r--r--   0        0        0      730 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/compute.py
--rw-r--r--   0        0        0      812 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/functions.py
--rw-r--r--   0        0        0      869 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/ipc.py
--rw-r--r--   0        0        0      984 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/table.py
--rw-r--r--   0        0        0     1084 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/helper.py
--rw-r--r--   0        0        0     5670 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/logging.py
--rw-r--r--   0        0        0      734 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/pydantic/__init__.py
--rw-r--r--   0        0        0     7230 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/utils/utils.py
--rw-r--r--   0        0        0      900 2024-04-04 02:53:41.284825 qianfan-0.3.7.1/qianfan/version.py
--rw-r--r--   0        0        0    10341 1970-01-01 00:00:00.000000 qianfan-0.3.7.1/PKG-INFO
+-rw-r--r--   0        0        0     6443 2024-04-13 13:35:38.755281 qianfan-0.3.8/README.pypi.md
+-rw-r--r--   0        0        0     3772 2024-04-13 13:35:38.755281 qianfan-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1578 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/__init__.py
+-rw-r--r--   0        0        0     2451 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/context.py
+-rw-r--r--   0        0        0     4502 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/launcher.py
+-rw-r--r--   0        0        0      847 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/runner/__init__.py
+-rw-r--r--   0        0        0     1688 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/runner/base.py
+-rw-r--r--   0        0        0     6028 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/runner/infer_runner.py
+-rw-r--r--   0        0        0     6278 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/runner/qianfan_runner.py
+-rw-r--r--   0        0        0     1460 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/space.py
+-rw-r--r--   0        0        0      784 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/suggestor/__init__.py
+-rw-r--r--   0        0        0     3370 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/suggestor/base.py
+-rw-r--r--   0        0        0     3356 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/suggestor/random_suggestor.py
+-rw-r--r--   0        0        0     3973 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/tune.py
+-rw-r--r--   0        0        0     1357 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/autotuner/utils.py
+-rw-r--r--   0        0        0      699 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/__init__.py
+-rw-r--r--   0        0        0    15290 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/chat.py
+-rw-r--r--   0        0        0     7120 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/completion.py
+-rw-r--r--   0        0        0    14564 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/dataset.py
+-rw-r--r--   0        0        0      790 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/embedding.py
+-rw-r--r--   0        0        0     9595 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/evaluation.py
+-rw-r--r--   0        0        0     6437 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/main.py
+-rw-r--r--   0        0        0     4107 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/openai_adapter.py
+-rw-r--r--   0        0        0    17018 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/plugin.py
+-rw-r--r--   0        0        0    24762 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/trainer.py
+-rw-r--r--   0        0        0     3265 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/txt2img.py
+-rw-r--r--   0        0        0     9991 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/client/utils.py
+-rw-r--r--   0        0        0        1 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/hub/__init__.py
+-rw-r--r--   0        0        0     5823 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/hub/hub.py
+-rw-r--r--   0        0        0     3512 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/hub/interface.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/persister/__init__.py
+-rw-r--r--   0        0        0      963 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/persister/base.py
+-rw-r--r--   0        0        0     2982 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/persister/persist.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/prompt/__init__.py
+-rw-r--r--   0        0        0    30862 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/prompt/prompt.py
+-rw-r--r--   0        0        0     2215 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/prompt/template.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/runnable/__init__.py
+-rw-r--r--   0        0        0     7049 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/runnable/base.py
+-rw-r--r--   0        0        0     3698 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/tool/baidu_search_tool.py
+-rw-r--r--   0        0        0     7561 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/tool/base_tool.py
+-rw-r--r--   0        0        0     2962 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/tool/duckduckgo_search_tool.py
+-rw-r--r--   0        0        0     3312 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/common/tool/wikipedia_tool.py
+-rw-r--r--   0        0        0     9582 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/config.py
+-rw-r--r--   0        0        0    12267 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/consts.py
+-rw-r--r--   0        0        0     1367 2024-04-13 13:35:38.755281 qianfan-0.3.8/qianfan/dataset/__init__.py
+-rw-r--r--   0        0        0     2786 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/consts.py
+-rw-r--r--   0        0        0      600 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_insight/__init__.py
+-rw-r--r--   0        0        0     2369 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_insight/assets/index.html
+-rw-r--r--   0        0        0      841 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_insight/data_insight_utils.py
+-rw-r--r--   0        0        0     8768 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_insight/insight.py
+-rw-r--r--   0        0        0     4363 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_operator.py
+-rw-r--r--   0        0        0     1013 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/__init__.py
+-rw-r--r--   0        0        0    27521 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/baidu_qianfan.py
+-rw-r--r--   0        0        0     2701 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/base.py
+-rw-r--r--   0        0        0    13584 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/bos.py
+-rw-r--r--   0        0        0     9420 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/chunk_reader.py
+-rw-r--r--   0        0        0     9532 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/file.py
+-rw-r--r--   0        0        0    26192 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/data_source/utils.py
+-rw-r--r--   0        0        0    71978 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/dataset.py
+-rw-r--r--   0        0        0    17893 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/dataset_utils.py
+-rw-r--r--   0        0        0     1139 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/__init__.py
+-rw-r--r--   0        0        0     2237 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/base.py
+-rw-r--r--   0        0        0     3942 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_character_repetition_filter.py
+-rw-r--r--   0        0        0     4482 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_flagged_words.py
+-rw-r--r--   0        0        0     2443 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_sentence_length_filter.py
+-rw-r--r--   0        0        0     2504 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_special_characters.py
+-rw-r--r--   0        0        0     4313 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_stopwords.py
+-rw-r--r--   0        0        0     3085 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_word_number.py
+-rw-r--r--   0        0        0     3910 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/check_word_repetition_filter.py
+-rw-r--r--   0        0        0     4483 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/consts.py
+-rw-r--r--   0        0        0     4693 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/utils.py
+-rw-r--r--   0        0        0   136258 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/local_data_operators/word_list.py
+-rw-r--r--   0        0        0     2832 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/process_interface.py
+-rw-r--r--   0        0        0     4363 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/qianfan_data_operators.py
+-rw-r--r--   0        0        0    10622 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/schema.py
+-rw-r--r--   0        0        0     2010 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/summarization_method.py
+-rw-r--r--   0        0        0    49904 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/table.py
+-rw-r--r--   0        0        0     1302 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/dataset/table_utils.py
+-rw-r--r--   0        0        0     2334 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/errors.py
+-rw-r--r--   0        0        0      878 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/__init__.py
+-rw-r--r--   0        0        0     2748 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/consts.py
+-rw-r--r--   0        0        0    26228 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/evaluation_manager.py
+-rw-r--r--   0        0        0     1325 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/evaluation_result.py
+-rw-r--r--   0        0        0     4484 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/evaluator.py
+-rw-r--r--   0        0        0     4379 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/local_evaluator.py
+-rw-r--r--   0        0        0     2468 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/evaluation/opencompass_evaluator.py
+-rw-r--r--   0        0        0       66 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/langchain/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/langchain/agents/__init__.py
+-rw-r--r--   0        0        0    13709 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.759281 qianfan-0.3.8/qianfan/extensions/openai/__init__.py
+-rw-r--r--   0        0        0    18554 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/openai/adapter.py
+-rw-r--r--   0        0        0     1602 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0     7804 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py
+-rw-r--r--   0        0        0     1627 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py
+-rw-r--r--   0        0        0     5365 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py
+-rw-r--r--   0        0        0     4056 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py
+-rw-r--r--   0        0        0     2577 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/fake_pyarrow_replacer.py
+-rw-r--r--   0        0        0      742 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/model/__init__.py
+-rw-r--r--   0        0        0      923 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/model/configs.py
+-rw-r--r--   0        0        0      938 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/model/consts.py
+-rw-r--r--   0        0        0    23100 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/py.typed
+-rw-r--r--   0        0        0     1648 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/auth/__init__.py
+-rw-r--r--   0        0        0     1656 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/auth/iam.py
+-rw-r--r--   0        0        0    15255 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/auth/oauth.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/__init__.py
+-rw-r--r--   0        0        0     4183 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/charge.py
+-rw-r--r--   0        0        0     7533 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/consts.py
+-rw-r--r--   0        0        0    30894 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/data.py
+-rw-r--r--   0        0        0    16673 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/finetune.py
+-rw-r--r--   0        0        0    23132 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/model.py
+-rw-r--r--   0        0        0    19491 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/prompt.py
+-rw-r--r--   0        0        0     5607 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/service.py
+-rw-r--r--   0        0        0     4941 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/console/utils.py
+-rw-r--r--   0        0        0     3779 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/http_client.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/images/__init__.py
+-rw-r--r--   0        0        0    11411 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/images/image2text.py
+-rw-r--r--   0        0        0    11777 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/images/text2image.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/__init__.py
+-rw-r--r--   0        0        0    27287 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/base.py
+-rw-r--r--   0        0        0    42166 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/chat_completion.py
+-rw-r--r--   0        0        0    11545 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/completion.py
+-rw-r--r--   0        0        0    10678 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/embedding.py
+-rw-r--r--   0        0        0    13139 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/llm/plugin.py
+-rw-r--r--   0        0        0    14096 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/requestor/__init__.py
+-rw-r--r--   0        0        0    12846 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/requestor/base.py
+-rw-r--r--   0        0        0     3189 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/requestor/console_requestor.py
+-rw-r--r--   0        0        0    22243 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/requestor/openapi_requestor.py
+-rw-r--r--   0        0        0    10266 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/token_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/tools/__init__.py
+-rw-r--r--   0        0        0     4909 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/tools/tokenizer.py
+-rw-r--r--   0        0        0     3580 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/tools/utils.py
+-rw-r--r--   0        0        0     9199 2024-04-13 13:35:38.763281 qianfan-0.3.8/qianfan/resources/typing.py
+-rw-r--r--   0        0        0     1141 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/__init__.py
+-rw-r--r--   0        0        0    46962 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/actions.py
+-rw-r--r--   0        0        0     6000 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/base.py
+-rw-r--r--   0        0        0    38188 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/configs.py
+-rw-r--r--   0        0        0     3600 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/consts.py
+-rw-r--r--   0        0        0     3403 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/event.py
+-rw-r--r--   0        0        0    12166 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/finetune.py
+-rw-r--r--   0        0        0    10187 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/pipeline.py
+-rw-r--r--   0        0        0     8360 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/post_pretrain.py
+-rw-r--r--   0        0        0     1680 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/ppl.yaml
+-rw-r--r--   0        0        0     4843 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/trainer/trainer.py
+-rw-r--r--   0        0        0     1244 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/__init__.py
+-rw-r--r--   0        0        0     4647 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/bos_uploader.py
+-rw-r--r--   0        0        0      696 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/cache/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/cache/base.py
+-rw-r--r--   0        0        0      827 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/__init__.py
+-rw-r--r--   0        0        0      946 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/compute.py
+-rw-r--r--   0        0        0      812 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/functions.py
+-rw-r--r--   0        0        0      869 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/ipc.py
+-rw-r--r--   0        0        0      984 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/fake_pyarrow/table.py
+-rw-r--r--   0        0        0     1084 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/helper.py
+-rw-r--r--   0        0        0     5670 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/logging.py
+-rw-r--r--   0        0        0      734 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0     7230 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/utils/utils.py
+-rw-r--r--   0        0        0      900 2024-04-13 13:35:38.767281 qianfan-0.3.8/qianfan/version.py
+-rw-r--r--   0        0        0    10489 1970-01-01 00:00:00.000000 qianfan-0.3.8/PKG-INFO
```

### Comparing `qianfan-0.3.7.1/README.pypi.md` & `qianfan-0.3.8/README.pypi.md`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/pyproject.toml` & `qianfan-0.3.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qianfan"
-version = "0.3.7.1"
+version = "0.3.8"
 description = "文心千帆大模型平台 Python SDK"
 authors = []
 license = "Apache-2.0"
 readme = "README.pypi.md"
 exclude = [
     "qianfan/tests",
     "qianfan/docs",
@@ -34,14 +34,15 @@
     { version = "<1.22.0", python = ">=3.7 <3.8", optional = true },
     { version = ">=1.22.0", python = ">=3.8", optional = true }
 ]
 pyarrow = [
     { version = ">=14.0.1", python = ">=3.8", optional = true },
     { version = "<=12.0.1", python = ">=3.7 <3.8", optional = true }
 ]
+tabulate = { version = "*", optional = true }
 python-dateutil = { version = "^2.8.2", optional = true }
 rich = ">=13.0.0"
 typer = ">=0.9.0"
 pyyaml = "^6.0.1"
 prompt-toolkit = ">=3.0.38"
 torch = [
     { version = "<=1.13.1", python = "<3.8", optional = true},
@@ -82,19 +83,19 @@
 [tool.poetry.group.cookbook.dependencies]
 nbformat = {version = "^5.10.3", python = ">=3.8 <4"}
 aiohttp = {version = "^3.9.3", python = ">=3.8 <4"}
 papermill = {version = "*", python = ">=3.8 <4"}
 ipykernel = {version = "^6.29.4", python = ">=3.8 <4"}
 
 [tool.poetry.extras]
-dataset_base = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson"]
-langchain = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson", "langchain"]
-local_data_clean = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson", "ltp", "emoji", "sentencepiece", "torch"]
-openai = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson", "fastapi", "uvicorn"]
-extension = ["numpy", "pyarrow", "python-dateutil", "clevercsv", "ijson", "langchain", "ltp", "emoji", "sentencepiece", "torch", "fastapi", "uvicorn"]
+dataset_base = ["numpy", "pyarrow", "tabulate", "python-dateutil", "clevercsv", "ijson"]
+langchain = ["numpy", "pyarrow", "tabulate", "python-dateutil", "clevercsv", "ijson", "langchain"]
+local_data_clean = ["numpy", "pyarrow", "tabulate", "python-dateutil", "clevercsv", "ijson", "ltp", "emoji", "sentencepiece", "torch"]
+openai = ["numpy", "pyarrow", "tabulate", "python-dateutil", "clevercsv", "ijson", "fastapi", "uvicorn"]
+extension = ["numpy", "pyarrow", "tabulate", "python-dateutil", "clevercsv", "ijson", "langchain", "ltp", "emoji", "sentencepiece", "torch", "fastapi", "uvicorn"]
 
 [tool.ruff.lint]
 extend-select = ["PLW1514"]
 preview = true
 select = [
   "E",  # pycodestyle
   "F",  # pyflakes
```

### Comparing `qianfan-0.3.7.1/qianfan/__init__.py` & `qianfan-0.3.8/qianfan/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/__init__.py` & `qianfan-0.3.8/qianfan/autotuner/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/context.py` & `qianfan-0.3.8/qianfan/autotuner/context.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/launcher.py` & `qianfan-0.3.8/qianfan/autotuner/launcher.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/runner/__init__.py` & `qianfan-0.3.8/qianfan/autotuner/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/runner/base.py` & `qianfan-0.3.8/qianfan/autotuner/runner/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/runner/infer_runner.py` & `qianfan-0.3.8/qianfan/autotuner/runner/infer_runner.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/runner/qianfan_runner.py` & `qianfan-0.3.8/qianfan/autotuner/runner/qianfan_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,23 +162,14 @@
                 result["metrics"] = {
                     **eval_metrics,
                     **stat_metrics,
                 }
 
         await asyncio.gather(*[_eval(res) for res in result_list])
 
-        total_metrics = {
-            k: 0.0
-            for k in sample_metrics
-            if isinstance(sample_metrics[k], (float, int))
-        }
-        success_count = 0
-        for result in result_list:
-            for item in result["results"]:
-                if item["output"] is None:
-                    continue
-                success_count += 1
-                for k in total_metrics:
-                    total_metrics[k] += item["metrics"][k]
-        for k, v in total_metrics.items():
-            total_metrics[k] = v / success_count
+        metrics_ds = Dataset.create_from_pyobj(
+            [res["metrics"] for result in result_list for res in result["results"]]
+        )
+        total_metrics = self.evaluator.summarize(metrics_ds)
+        if total_metrics is None:
+            return {}
         return total_metrics
```

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/space.py` & `qianfan-0.3.8/qianfan/autotuner/space.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/suggestor/__init__.py` & `qianfan-0.3.8/qianfan/autotuner/suggestor/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/suggestor/base.py` & `qianfan-0.3.8/qianfan/autotuner/suggestor/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/suggestor/random_suggestor.py` & `qianfan-0.3.8/qianfan/autotuner/suggestor/random_suggestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/tune.py` & `qianfan-0.3.8/qianfan/autotuner/tune.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/autotuner/utils.py` & `qianfan-0.3.8/qianfan/autotuner/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/__init__.py` & `qianfan-0.3.8/qianfan/common/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/chat.py` & `qianfan-0.3.8/qianfan/common/client/chat.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/completion.py` & `qianfan-0.3.8/qianfan/common/client/completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/dataset.py` & `qianfan-0.3.8/qianfan/common/client/dataset.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/embedding.py` & `qianfan-0.3.8/qianfan/common/client/embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/evaluation.py` & `qianfan-0.3.8/qianfan/common/client/evaluation.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/main.py` & `qianfan-0.3.8/qianfan/common/client/main.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/openai_adapter.py` & `qianfan-0.3.8/qianfan/common/client/openai_adapter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/plugin.py` & `qianfan-0.3.8/qianfan/common/client/plugin.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/trainer.py` & `qianfan-0.3.8/qianfan/common/client/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,14 +321,21 @@
     "--list-train-type",
     "-l",
     callback=list_train_type,
     is_eager=True,
     help="Print supported train types.",
 )
 
+daemon_option = typer.Option(
+    None,
+    "--daemon",
+    "-d",
+    help="Run command as daemon.",
+)
+
 
 @trainer_app.command(
     "run",
     deprecated=True,
     help=(
         "Run a finetune trainer task. This command is deprecated and use command"
         " `finetune` instead."
@@ -338,18 +345,22 @@
 @credential_required
 def finetune(
     dataset_id: Optional[str] = typer.Option(None, help="Dataset id"),
     dataset_bos_path: Optional[str] = typer.Option(
         None,
         help="Dataset BOS path",
     ),
-    train_type: str = typer.Option(..., help="Train type"),
+    train_type: Optional[str] = typer.Option(None, help="Train type"),
     previous_task_id: Optional[str] = typer.Option(
         None, help="Task id of previous trainer output."
     ),
+    trainer_pipeline_file: Optional[str] = typer.Option(
+        None, help="Trainer pipeline file path"
+    ),
+    daemon: Optional[bool] = daemon_option,
     list_train_type: Optional[bool] = list_train_type_option,
     show_config_limit: Optional[str] = typer.Option(
         None,
         callback=show_config_limit,
         is_eager=True,
         help="Show config limit for specified train type.",
     ),
@@ -422,85 +433,95 @@
     ),
 ) -> None:
     """
     Run a finetune trainer job.
     """
     console = replace_logger_handler()
     callback = MyEventHandler(console=console)
-    ds = None
-    if dataset_id is not None:
-        ds = Dataset.load(qianfan_dataset_id=dataset_id, does_release=True)
-    deploy_config = None
-    if deploy_name is not None:
-        if deploy_endpoint_prefix is None:
-            print_error_msg("Deploy endpoint prefix is required")
-            raise typer.Exit(code=1)
-
-        deploy_config = DeployConfig(
-            name=deploy_name,
-            endpoint_prefix=deploy_endpoint_prefix,
-            description=deploy_description,
-            replicas=deploy_replicas,
-            pool_type=DeployPoolType[deploy_pool_type],
-            service_type=ServiceType[deploy_service_type],
-        )
 
-    trainer = LLMFinetune(
-        dataset=ds,
-        train_type=train_type,
-        event_handler=callback,
-        train_config=train_config_file,
-        deploy_config=deploy_config,
-        dataset_bos_path=dataset_bos_path,
-        previous_task_id=previous_task_id,
-    )
-
-    if trainer.train_action.train_config is None:
-        raise InternalError("Train config not found in trainer.")
-    if train_epoch is not None:
-        trainer.train_action.train_config.epoch = train_epoch
-    if train_batch_size is not None:
-        trainer.train_action.train_config.batch_size = train_batch_size
-    if train_learning_rate is not None:
-        trainer.train_action.train_config.learning_rate = train_learning_rate
-    if train_max_seq_len is not None:
-        trainer.train_action.train_config.max_seq_len = train_max_seq_len
-    if train_peft_type is not None:
-        trainer.train_action.train_config.peft_type = train_peft_type
-    if trainset_rate is not None:
-        trainer.train_action.train_config.trainset_rate = trainset_rate
-    if train_logging_steps is not None:
-        trainer.train_action.train_config.logging_steps = train_logging_steps
-    if train_warmup_ratio is not None:
-        trainer.train_action.train_config.warmup_ratio = train_warmup_ratio
-    if train_weight_decay is not None:
-        trainer.train_action.train_config.weight_decay = train_weight_decay
-    if train_lora_rank is not None:
-        trainer.train_action.train_config.lora_rank = train_lora_rank
-    if train_lora_all_linear is not None:
-        trainer.train_action.train_config.lora_all_linear = train_lora_all_linear
-
-    trainer.run()
-
-    console.log("Trainer finished!")
-    console.log(Pretty(trainer.output))
+    if trainer_pipeline_file is not None:
+        trainer = LLMFinetune.load(file=trainer_pipeline_file)
+        trainer.register_event_handler(callback)
+    else:
+        ds = None
+        if dataset_id is not None:
+            ds = Dataset.load(qianfan_dataset_id=dataset_id, does_release=True)
+        deploy_config = None
+        if deploy_name is not None:
+            if deploy_endpoint_prefix is None:
+                print_error_msg("Deploy endpoint prefix is required")
+                raise typer.Exit(code=1)
+
+            deploy_config = DeployConfig(
+                name=deploy_name,
+                endpoint_prefix=deploy_endpoint_prefix,
+                description=deploy_description,
+                replicas=deploy_replicas,
+                pool_type=DeployPoolType[deploy_pool_type],
+                service_type=ServiceType[deploy_service_type],
+            )
+        trainer = LLMFinetune(
+            dataset=ds,
+            train_type=train_type,
+            event_handler=callback,
+            train_config=train_config_file,
+            deploy_config=deploy_config,
+            dataset_bos_path=dataset_bos_path,
+            previous_task_id=previous_task_id,
+        )
+        if trainer.train_action.train_config is None:
+            raise InternalError("Train config not found in trainer.")
+        if train_epoch is not None:
+            trainer.train_action.train_config.epoch = train_epoch
+        if train_batch_size is not None:
+            trainer.train_action.train_config.batch_size = train_batch_size
+        if train_learning_rate is not None:
+            trainer.train_action.train_config.learning_rate = train_learning_rate
+        if train_max_seq_len is not None:
+            trainer.train_action.train_config.max_seq_len = train_max_seq_len
+        if train_peft_type is not None:
+            trainer.train_action.train_config.peft_type = train_peft_type
+        if trainset_rate is not None:
+            trainer.train_action.train_config.trainset_rate = trainset_rate
+        if train_logging_steps is not None:
+            trainer.train_action.train_config.logging_steps = train_logging_steps
+        if train_warmup_ratio is not None:
+            trainer.train_action.train_config.warmup_ratio = train_warmup_ratio
+        if train_weight_decay is not None:
+            trainer.train_action.train_config.weight_decay = train_weight_decay
+        if train_lora_rank is not None:
+            trainer.train_action.train_config.lora_rank = train_lora_rank
+        if train_lora_all_linear is not None:
+            trainer.train_action.train_config.lora_all_linear = train_lora_all_linear
+
+    if daemon:
+        trainer.start()
+        console.print(
+            f"trainer[{trainer.id}] started with pid:"
+            f" {trainer.info().get('process_id')}"
+        )
+        console.print(f"check running log in: {trainer.ppls[0]._get_log_path()}")
+    else:
+        trainer.run()
+        console.log("Trainer finished!")
+        console.log(Pretty(trainer.output))
 
     # wait a second for the log to be flushed
     time.sleep(0.1)
 
 
 @trainer_app.command()
 @credential_required
 def postpretrain(
     dataset_id: Optional[str] = typer.Option(None, help="Dataset id"),
     dataset_bos_path: Optional[str] = typer.Option(
         None,
         help="Dataset BOS path",
     ),
-    train_type: str = typer.Option(..., help="Train type"),
+    train_type: Optional[str] = typer.Option(None, help="Train type"),
     list_train_type: Optional[bool] = list_train_type_option,
     show_config_limit: Optional[str] = typer.Option(
         None,
         callback=show_config_limit,
         is_eager=True,
         help="Show config limit for specified train type.",
     ),
```

### Comparing `qianfan-0.3.7.1/qianfan/common/client/txt2img.py` & `qianfan-0.3.8/qianfan/common/client/txt2img.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/client/utils.py` & `qianfan-0.3.8/qianfan/common/client/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/hub/hub.py` & `qianfan-0.3.8/qianfan/common/hub/hub.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/hub/interface.py` & `qianfan-0.3.8/qianfan/common/hub/interface.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/persister/base.py` & `qianfan-0.3.8/qianfan/common/persister/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/persister/persist.py` & `qianfan-0.3.8/qianfan/common/persister/persist.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import glob
 from abc import ABC, abstractmethod
 from os import makedirs, path
 from typing import List, Type, TypeVar
 
 from qianfan.common.persister.base import Persistent
 from qianfan.consts import Consts
-from qianfan.utils.logging import log_info
+from qianfan.utils.logging import log_debug
 
 _T = TypeVar("_T", bound=Type["Persistent"])
 
 
 class Persister(ABC):
     @classmethod
     @abstractmethod
@@ -49,17 +49,17 @@
             makedirs(FileTmpPath)
 
     @classmethod
     def save(cls, p: Persistent) -> None:
         b = p.persist()
         f_path_dir = path.join(FileTmpPath, p._space())
         if not path.exists(f_path_dir):
-            makedirs(f_path_dir)
+            makedirs(f_path_dir, exist_ok=True)
         f_path = path.join(f_path_dir, p._identity())
-        log_info(f"save to {f_path}")
+        log_debug(f"save to {f_path}")
         with open(f_path, "wb") as f:
             f.write(b)
 
     @classmethod
     def load(cls, id: str, t: _T) -> Persistent:
         f_path_dir = path.join(FileTmpPath, t._space())
         if not path.exists(f_path_dir):
```

### Comparing `qianfan-0.3.7.1/qianfan/common/prompt/prompt.py` & `qianfan-0.3.8/qianfan/common/prompt/prompt.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,31 +8,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import copy
+import json
+import re
 import time
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, cast
 
 from qianfan.common.hub.interface import HubSerializable
 from qianfan.config import encoding
 from qianfan.consts import (
     PromptFrameworkType,
     PromptSceneType,
     PromptScoreStandard,
     PromptType,
 )
 from qianfan.errors import InvalidArgumentError, RequestError
 from qianfan.resources.console.prompt import Prompt as PromptResource
 from qianfan.resources.llm.completion import Completion
 from qianfan.resources.typing import Literal, QfResponse
-from qianfan.utils import log_warn
+
+if TYPE_CHECKING:
+    from qianfan.dataset import Dataset
+from qianfan.utils import log_info, log_warn
 
 
 @dataclass
 class PromptLabel(HubSerializable):
     """
     Class of prompt label
     """
@@ -541,14 +547,187 @@
             elif status == 3:  # failed
                 raise RequestError("Prompt optimization task failed.")
             time.sleep(1)
         optimized_prompt = resp["result"]["optimizeContent"]
 
         return Prompt(optimized_prompt, identifier=self.identifier)
 
+    def apo_by_sample(
+        self,
+        example: Optional["Dataset"] = None,
+        sample_prompt: Optional["Prompt"] = None,
+        feedback_prompt: Optional["Prompt"] = None,
+        update_prompt: Optional["Prompt"] = None,
+        iteration_round: int = 3,
+        infer_config: Dict[str, Any] = {"model": "ERNIE-Speed"},
+        optimize_config: Dict[str, Any] = {"model": "ERNIE-4.0-8K"},
+    ) -> "Prompt":
+        if iteration_round < 1:
+            raise ValueError("iteration_round must be greater than or equal to 1.")
+        if len(self.variables) > 0 and example is None:
+            raise ValueError("Example is required when there are variables in prompt.")
+
+        from qianfan.common.prompt.template import (
+            PROMPT_OPTIMIZE_FEEDBACK_TMPL,
+            PROMPT_OPTIMIZE_SAMPLE_TMPL,
+            PROMPT_OPTIMIZE_SAMPLE_WO_OUTPUT_TMPL,
+            PROMPT_OPTIMIZE_UPDATE_TMPL,
+        )
+        from qianfan.resources.llm.chat_completion import ChatCompletion
+
+        if sample_prompt is None:
+            if example is None:
+                sample_prompt = Prompt(
+                    PROMPT_OPTIMIZE_SAMPLE_WO_OUTPUT_TMPL, identifier="{{}}"
+                )
+            else:
+                sample_prompt = Prompt(PROMPT_OPTIMIZE_SAMPLE_TMPL, identifier="{{}}")
+        if feedback_prompt is None:
+            feedback_prompt = Prompt(PROMPT_OPTIMIZE_FEEDBACK_TMPL, identifier="{{}}")
+        if update_prompt is None:
+            update_prompt = Prompt(PROMPT_OPTIMIZE_UPDATE_TMPL, identifier="{{}}")
+
+        client = ChatCompletion()
+        left_identifier, right_identifier = PromptResource._split_identifier(
+            self.identifier
+        )
+        current_prompt = self
+
+        for _ in range(iteration_round):
+            sample_prompts: List[str]
+            # use prompt to generate sample output
+            if example is not None:
+                dataset_infer_config = copy.deepcopy(infer_config)
+                if "model" in infer_config:
+                    dataset_infer_config["service_model"] = infer_config["model"]
+                    del dataset_infer_config["model"]
+                if "endpoint" in infer_config:
+                    dataset_infer_config["service_endpoint"] = infer_config["endpoint"]
+                    del dataset_infer_config["endpoint"]
+                samples = example.test_using_llm(
+                    prompt_template=current_prompt, **dataset_infer_config
+                )
+                sample_prompts = [
+                    sample_prompt.render(
+                        input=json.dumps(
+                            {k: sample[k] for k in self.variables},
+                            ensure_ascii=False,
+                            indent=4,
+                        ),
+                        expect=sample["expected_output"],
+                        response=sample["llm_output"],
+                    )[0]
+                    for sample in samples.list()
+                ]
+            else:
+                model_output = ChatCompletion().do(
+                    messages=[{"role": "user", "content": current_prompt.render()[0]}],
+                    **infer_config,
+                )
+                assert isinstance(model_output, QfResponse)
+                sample_prompts = [
+                    sample_prompt.render(
+                        input=current_prompt.render()[0],
+                        expect="",
+                        response=model_output["result"],
+                    )[0]
+                ]
+            sample_str = "\n===\n".join(sample_prompts)
+            # put sample output into feedback prompt
+            feedback_input = feedback_prompt.render(
+                current_prompt=current_prompt.template,
+                samples=sample_str,
+            )[0]
+            log_info(f"Feedback input: {repr(feedback_input)}")
+            # get feedback from model
+            feedback = client.do(
+                messages=[
+                    {
+                        "role": "user",
+                        "content": feedback_input,
+                    }
+                ],
+                **optimize_config,
+            )
+            assert isinstance(feedback, QfResponse)
+            log_info(f"Feedback output: {repr(feedback['result'])}")
+            # use model to update prompt
+            update_input = update_prompt.render(
+                current_prompt=current_prompt.template,
+                samples=sample_str,
+                feedback=feedback["result"],
+                variables=" ".join(
+                    [
+                        f"{left_identifier}{var}{right_identifier}"
+                        for var in self.variables
+                    ]
+                ),
+            )[0]
+            log_info(f"Update input: {repr(update_input)}")
+            update_resp = client.do(
+                messages=[
+                    {
+                        "role": "user",
+                        "content": update_input,
+                    }
+                ],
+                **optimize_config,
+            )
+            assert isinstance(update_resp, QfResponse)
+            update = update_resp["result"]
+
+            log_info(f"Update output: {repr(update)}")
+
+            # update prompt
+            try:
+                new_prompt_tmpl = re.findall(
+                    "<START>(.*)<END>", update, re.MULTILINE | re.DOTALL
+                )[0]
+            except Exception:
+                new_prompt_tmpl = update
+            log_info(f"New prompt: {repr(new_prompt_tmpl)}")
+            current_prompt = Prompt(new_prompt_tmpl, identifier=self.identifier)
+        return current_prompt
+
+    def simplify(
+        self,
+        simplify_prompt: Optional["Prompt"] = None,
+        config: Dict[str, Any] = {"model": "ERNIE-4.0-8K"},
+    ) -> "Prompt":
+        from qianfan.common.prompt.template import PROMPT_SIMPLIFY_TMPL
+
+        if simplify_prompt is None:
+            simplify_prompt = Prompt(PROMPT_SIMPLIFY_TMPL, identifier="{{}}")
+
+        left_identifier, right_identifier = PromptResource._split_identifier(
+            self.identifier
+        )
+        client = Completion()
+        resp = client.do(
+            simplify_prompt.render(
+                current_prompt=self.template,
+                variables=" ".join(
+                    [
+                        f"{left_identifier}{var}{right_identifier}"
+                        for var in self.variables
+                    ]
+                ),
+            )[0],
+            **config,
+        )
+        assert isinstance(resp, QfResponse)
+        output = resp["result"]
+        try:
+            new_prompt_tmpl = re.findall(
+                "<START>(.*)<END>", output, re.MULTILINE | re.DOTALL
+            )[0]
+        except Exception:
+            new_prompt_tmpl = output
+        return Prompt(new_prompt_tmpl, identifier=self.identifier)
+
     @dataclass
     class PromptEvaluateResult(object):
         """
         Evaluation result of a prompt
         """
 
         prompt: "Prompt"
```

### Comparing `qianfan-0.3.7.1/qianfan/common/runnable/base.py` & `qianfan-0.3.8/qianfan/common/runnable/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 import json
 import os
 import pickle
-import platform
 import sys
 import threading
 from abc import ABC, abstractmethod
-from typing import (
-    Any,
-    Dict,
-    Generic,
-    Optional,
-    TypeVar,
-)
+from typing import Any, Dict, Generic, List, Optional, TypeVar
 
 import dill
 import multiprocess as multiprocessing
 import yaml
 
 from qianfan.config import encoding
 from qianfan.utils import utils
@@ -139,24 +132,48 @@
     def serialize(self, obj: Any) -> bytes:
         return dill.dumps(obj)
 
     def deserialize(self, data: bytes) -> Any:
         return dill.loads(data)
 
 
+class CompatSerializeHelper(SerializeHelper):
+    def __init__(self) -> None:
+        self.helpers: List[SerializeHelper] = [
+            JsonSerializeHelper(),
+            YamlSerializeHelper(),
+        ]
+
+    def serialize(self, obj: Any) -> bytes:
+        for helper in self.helpers:
+            try:
+                return helper.serialize(obj)
+            except Exception:
+                continue
+        raise Exception("serialize failed")
+
+    def deserialize(self, data: bytes) -> Any:
+        for helper in self.helpers:
+            try:
+                return helper.deserialize(data)
+            except Exception:
+                continue
+        raise Exception("deserialize failed")
+
+
 class ExecuteSerializable(Executable[Input, Output], Serializable):
     """
     set of executable and serializable. subclass implement it to support
     exec and dumps/loads.
     """
 
     process_id: str = ""
     process: Optional[multiprocessing.Process] = None
 
-    serialize_helper: SerializeHelper = JsonSerializeHelper()
+    serialize_helper: SerializeHelper = CompatSerializeHelper()
 
     def _get_specific_cache_path(self) -> str:
         cache_path = os.path.join(
             QianfanTrainerLocalCacheDir,
             utils.generate_letter_num_random_id(8),
         )
         if not os.path.exists(cache_path):
@@ -173,20 +190,20 @@
     def _start(self, **kwargs: Any) -> None:
         self.exec(**kwargs)
 
     def start(
         self, join_on_exited: bool = False, **kwargs: Any
     ) -> "ExecuteSerializable":
         def run_subprocess(pipe: multiprocessing.Pipe) -> None:
-            if platform.system() != "Windows":
-                os.setsid()  # type: ignore[attr-defined]
+            # if platform.system() != "Windows":
+            #     os.setsid()  # type: ignore[attr-defined]
             # redirect output
             log_path = self._get_log_path()
             with open(log_path, "a", encoding=encoding()) as f:
-                log_info(f"check trainer running log in {log_path}")
+                log_info(f"check running log in {log_path}")
                 sys.stdout = f
                 from qianfan.utils.logging import redirect_log_to_file
 
                 redirect_log_to_file(log_path)
 
             # start a thread for run
             main_t = threading.Thread(target=self._start, kwargs=kwargs)
```

### Comparing `qianfan-0.3.7.1/qianfan/common/tool/baidu_search_tool.py` & `qianfan-0.3.8/qianfan/common/tool/baidu_search_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/tool/base_tool.py` & `qianfan-0.3.8/qianfan/common/tool/base_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/tool/duckduckgo_search_tool.py` & `qianfan-0.3.8/qianfan/common/tool/duckduckgo_search_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/common/tool/wikipedia_tool.py` & `qianfan-0.3.8/qianfan/common/tool/wikipedia_tool.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/config.py` & `qianfan-0.3.8/qianfan/config.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/consts.py` & `qianfan-0.3.8/qianfan/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/__init__.py` & `qianfan-0.3.8/qianfan/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/consts.py` & `qianfan-0.3.8/qianfan/dataset/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/data_operator.py` & `qianfan-0.3.8/qianfan/dataset/data_operator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/data_source/__init__.py` & `qianfan-0.3.8/qianfan/dataset/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/data_source/baidu_qianfan.py` & `qianfan-0.3.8/qianfan/dataset/data_source/baidu_qianfan.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/data_source/base.py` & `qianfan-0.3.8/qianfan/dataset/data_source/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/data_source/bos.py` & `qianfan-0.3.8/qianfan/dataset/data_source/bos.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/data_source/chunk_reader.py` & `qianfan-0.3.8/qianfan/dataset/data_source/chunk_reader.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/data_source/file.py` & `qianfan-0.3.8/qianfan/dataset/data_source/file.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/data_source/utils.py` & `qianfan-0.3.8/qianfan/dataset/data_source/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,20 +15,21 @@
 utilities for data source
 """
 import datetime
 import hashlib
 import json
 import os
 import shutil
+import threading
 import uuid
 import zipfile
 from enum import Enum
 from pathlib import Path
 from time import sleep
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Type, Union
 
 import pyarrow
 import requests
 
 from qianfan.config import encoding, get_config
 from qianfan.dataset.consts import (
     QianfanDatasetCacheFileExtensionName,
@@ -77,14 +78,51 @@
 
     Jpg = "jpg"
     Jpeg = "jpeg"
     Png = "png"
     Bmp = "bmp"
 
 
+class TaskDispatcher:
+    def __init__(self, batch_size: int, task_number: int):
+        self.task_queue: List[Tuple[int, int]] = []
+        for batch_index in range(0, task_number, batch_size):
+            current_batch_size = min(task_number - batch_index, batch_size)
+            self.task_queue.append((batch_index, current_batch_size))
+
+        self.lock = threading.Lock()
+        self.current_task_queue_index = 0
+
+    def get_task(self) -> Optional[Tuple[int, int]]:
+        with self.lock:
+            if self.current_task_queue_index >= len(self.task_queue):
+                return None
+
+            task = self.task_queue[self.current_task_queue_index]
+            self.current_task_queue_index += 1
+            return task
+
+    def mapper_closure(
+        self, func: Callable[[int, int], Generator[Any, None, None]]
+    ) -> Callable[[], Generator[Tuple[int, Any], None, None]]:
+        def new_func() -> Generator[Tuple[int, Any], None, None]:
+            task_slice = self.get_task()
+            while task_slice:
+                batch_index, batch_size = task_slice[0], task_slice[1]
+                returned_data_list: List[Any] = []
+
+                for returned_data in func(batch_index, batch_size):
+                    returned_data_list.append(returned_data)
+
+                yield batch_index, returned_data_list
+                task_slice = self.get_task()
+
+        return new_func
+
+
 def _get_annotation_file_name(file_name: str) -> str:
     return file_name[: file_name.rfind(".")] + ".json"
 
 
 def _get_all_image_files_and_annotations_from_root(
     root: str, files: List[str]
 ) -> Tuple[List[str], List[Optional[Dict]]]:
@@ -237,31 +275,78 @@
     log_info("has got a memory-mapped table")
     return table
 
 
 def _create_map_arrow_file(
     path: str,
     mapper_closure: Callable,
+    batch_size: int,
+    task_number: int,
     **kwargs: Any,
 ) -> pyarrow.Table:
-    reader = MapperReader(mapper_closure=mapper_closure, **kwargs)
+    task_dispatcher = TaskDispatcher(batch_size, task_number)
+
+    reader = MapperReader(
+        mapper_closure=task_dispatcher.mapper_closure(mapper_closure), **kwargs
+    )
 
     tmp_folder_path, file_name = _construct_buffer_folder_path_and_file_name(
         QianfanMapperCacheDir, path
     )
     tmp_arrow_file_path = os.path.join(
         tmp_folder_path,
         f"{file_name}_{uuid.uuid4()}{QianfanDatasetCacheFileExtensionName}",
     )
 
     _write_table_to_arrow_file(tmp_arrow_file_path, reader)
     _remove_previous_folder_file(tmp_arrow_file_path)
     return _read_mmap_table_from_arrow_file(tmp_arrow_file_path)
 
 
+def _iterate_to_conduct_result(
+    mapper_closure: Callable,
+    batch_size: int,
+    task_number: int,
+    **kwargs: Any,
+) -> List[Any]:
+    task_dispatcher = TaskDispatcher(batch_size, task_number)
+
+    reader = MapperReader(
+        mapper_closure=task_dispatcher.mapper_closure(mapper_closure), **kwargs
+    )
+    result_list: List[Any] = []
+    for elem in reader:
+        for e in elem:
+            if e is None:
+                raise ValueError("cant return None")
+            if not isinstance(e, bool):
+                raise ValueError("returned value isn't bool")
+        result_list.extend(elem)
+
+    return result_list
+
+
+def _pure_iterate(
+    mapper_closure: Callable,
+    batch_size: int,
+    task_number: int,
+    **kwargs: Any,
+) -> None:
+    task_dispatcher = TaskDispatcher(batch_size, task_number)
+
+    reader = MapperReader(
+        mapper_closure=task_dispatcher.mapper_closure(mapper_closure), **kwargs
+    )
+
+    for _ in reader:
+        continue
+
+    return
+
+
 def _read_mmap_table_from_arrow_file(arrow_file_path: str) -> pyarrow.Table:
     log_info(f"start to get memory_map from {arrow_file_path}")
     with pyarrow.memory_map(arrow_file_path) as mmap_stream:
         return pyarrow.ipc.open_stream(mmap_stream).read_all()
 
 
 def _remove_previous_folder_file(path: str) -> None:
```

### Comparing `qianfan-0.3.7.1/qianfan/dataset/dataset.py` & `qianfan-0.3.8/qianfan/dataset/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,20 +11,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 dataset core concept, a wrap of data processing, data transmission and data validation
 """
 import functools
+import uuid
 from copy import deepcopy
 from time import sleep
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 import pyarrow
 from pyarrow import Table as PyarrowTable
+from tabulate import tabulate
 from typing_extensions import Self
 
 from qianfan import Completion, QfRole, get_config
 from qianfan.common import Prompt
 from qianfan.dataset.consts import (
     FirstTokenLatencyColumnName,
     LLMOutputColumnName,
@@ -48,20 +59,28 @@
     _check_and_generate_service,
     _check_online_data_process_result,
     _create_a_dataset_etl_task,
     _extract_string,
     _get_qianfan_schema,
     _list_cloud_data,
     _start_an_evaluation_task_for_model_batch_inference,
+    open_html_in_browser,
 )
 from qianfan.dataset.qianfan_data_operators import QianfanOperator
 from qianfan.dataset.schema import (
     QianfanSchema,
     Schema,
 )
+from qianfan.dataset.summarization_method import (
+    MaxMethod,
+    MeanMethod,
+    MinMethod,
+    QuantileMethod,
+    SummarizationMethod,
+)
 from qianfan.dataset.table import Table
 from qianfan.dataset.table_utils import _construct_packed_table_from_nest_sequence
 from qianfan.errors import ValidationError
 from qianfan.resources import Data, Model
 from qianfan.resources.console.consts import (
     DataTemplateType,
 )
@@ -509,14 +528,16 @@
         if new_ds.is_dataset_grouped():
             new_ds.pack()
 
         # 特判兼容原来的 replace_source 逻辑
         if replace_source is not None:
             log_warn('parameter "replace_source" has been set as deprecated')
 
+        new_ds._set_qianfan_default_io_column(source)
+
         if not replace_source:
             return new_ds
 
         self.inner_table = new_ds.inner_table
         self.inner_data_source_cache = new_ds.inner_data_source_cache
         self.inner_schema_cache = new_ds.inner_schema_cache
         return self
@@ -753,59 +774,109 @@
 
         return self.col_delete(QianfanDataGroupColumnName)
 
     # -------------------- Processable 相关 ----------------
     # 直接调用 Table 对象的接口方法
     # 这些接口不支持用在云端数据集上
     @_online_except_decorator
-    def map(self, op: Callable[[Any], Any], **kwargs: Any) -> Self:
+    def map(
+        self,
+        op: Callable[[Any], Any],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         map on dataset
 
         Args:
             op (Callable[[Any], Any]): handler used to map
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
             **kwargs (Any): other arguments
 
         Returns:
             Self: Dataset itself
         """
-        assert isinstance(self.inner_data_source_cache, FileDataSource)
-        return super().map(op, path=self.inner_data_source_cache.path, **kwargs)
+        if isinstance(self.inner_data_source_cache, FileDataSource):
+            if len(self) == 0:
+                return self
+
+            return super().map(
+                op,
+                should_create_new_obj,
+                path=self.inner_data_source_cache.path,
+                **kwargs,
+            )
+        else:
+            if not self.inner_table or len(self) == 0:
+                return self
+            return super().map(
+                op, should_create_new_obj, path=f"no_source_{uuid.uuid4()}"
+            )
 
     @_online_except_decorator
-    def filter(self, op: Callable[[Any], bool]) -> Self:
+    def filter(
+        self,
+        op: Callable[[Any], bool],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         filter on dataset
 
         Args:
             op (Callable[[Any], bool]): handler used to filter
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Dataset itself
         """
-        return super().filter(op)
+        if not self.inner_table or len(self) == 0:
+            return self
+        return super().filter(op, should_create_new_obj, **kwargs)
 
     @_online_except_decorator
-    def delete(self, index: Union[int, str]) -> Self:
+    def delete(
+        self,
+        index: Union[int, str],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         delete an element from dataset
 
         Args:
             index (Union[int, str]): element index to delete
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Dataset itself
         """
-        return super().delete(index)
+        return super().delete(index, should_create_new_obj, **kwargs)
 
     # 但是在云上数据集追加数据未来可以支持，本质是向数据集中导入新数据。
     # 目前不做修改，等待接口 ready
     @_online_except_decorator
     def append(
-        self, elem: Any, add_new_group: bool = False, is_grouped: bool = True
+        self,
+        elem: Any,
+        add_new_group: bool = False,
+        is_grouped: bool = True,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
     ) -> Self:
         """
         append element(s) to dataset
 
         Args:
             elem (Union[List[List[Dict]], List[Dict], Tuple[Dict], Dict]):
                 Elements added to dataset
@@ -817,27 +888,36 @@
                 Only used when dataset is grouped and elem is Sequence
                 and add_new_group was set True.
                 Default to True, all elements
                 will be in same group.
                 If it's True, each element will have
                 sequential incremental group id from last
                 available group id.
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
         Returns:
             Self: Dataset itself
         """
-        return super().append(elem, add_new_group, is_grouped)
+        return super().append(
+            elem, add_new_group, is_grouped, should_create_new_obj, **kwargs
+        )
 
     @_online_except_decorator
     def insert(
         self,
         elem: Any,
         index: Any,
         group_id: int = -1,
         add_new_group: bool = False,
         is_grouped: bool = True,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
     ) -> Self:
         """
         insert element(s) to dataset
 
         Args:
             elem (Union[List[List[Dict]], List[Dict], Tuple[Dict], Dict]):
                 Elements added to dataset
@@ -855,18 +935,25 @@
                 Only used when dataset is grouped and elem is Sequence
                 and add_new_group was set True.
                 Default to True, all elements
                 will be in same group.
                 If it's True, each element will have
                 sequential incremental group id from last
                 available group id.
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
         Returns:
             Self: Dataset itself
         """
-        return super().insert(elem, index, add_new_group, is_grouped)
+        return super().insert(
+            elem, index, add_new_group, is_grouped, should_create_new_obj, **kwargs
+        )
 
     def list(
         self,
         by: Optional[Union[slice, int, str, Sequence[int], Sequence[str]]] = None,
         **kwargs: Any,
     ) -> Any:
         """
@@ -910,14 +997,41 @@
                 err_msg = (
                     "can't get row number from data source:"
                     f" {type(self.inner_data_source_cache)}"
                 )
                 log_error(err_msg)
                 raise ValueError(err_msg)
 
+    @_online_except_decorator
+    def take_slice(
+        self,
+        start: int = 0,
+        end: int = -1,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        """
+        make a slice of dataset
+
+        Args:
+            start (int):
+                where the slice starts
+            end (int):
+                where the slice ends
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any):
+                other arguments
+        Returns:
+            Dataset: a sliced dataset
+        """
+        return super().take_slice(start, end, should_create_new_obj, **kwargs)
+
     def __getitem__(self, key: Any) -> Any:
         if (
             isinstance(key, int)
             or isinstance(key, slice)
             or (isinstance(key, (list, tuple)) and key and isinstance(key[0], int))
         ):
             return self.list(key)
@@ -932,78 +1046,129 @@
         else:
             err_msg = f"unsupported key type for deleting: {type(key)}"
             log_error(err_msg)
             raise TypeError(err_msg)
 
     # 列操作集
     @_online_except_decorator
-    def col_map(self, op: Callable[[Any], Any]) -> Self:
+    def col_map(
+        self,
+        op: Callable[[Any], Any],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         map on dataset's column
 
         Args:
             op (Callable[[Any], Any]): handler used to map
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Dataset itself
         """
-        return super().col_map(op)
+        return super().col_map(op, should_create_new_obj, **kwargs)
 
     @_online_except_decorator
-    def col_filter(self, op: Callable[[Any], bool]) -> Self:
+    def col_filter(
+        self,
+        op: Callable[[Any], bool],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         filter on dataset's column
 
         Args:
             op (Callable[[Any], bool]): handler used to filter
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Dataset itself
         """
-        return super().col_filter(op)
+        return super().col_filter(op, should_create_new_obj, **kwargs)
 
     @_online_except_decorator
-    def col_delete(self, index: Union[int, str]) -> Self:
+    def col_delete(
+        self,
+        index: Union[int, str],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         delete an column from dataset
 
         Args:
             index (str): column name to delete
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Dataset itself
         """
-        return super().col_delete(index)
+        return super().col_delete(index, should_create_new_obj, **kwargs)
 
     @_online_except_decorator
-    def col_append(self, elem: Any) -> Self:
+    def col_append(
+        self,
+        elem: Any,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         append a row to dataset
 
         Args:
             elem (Dict[str, List]): a dict containing element added to dataset, which
                 key as column name, value as column data
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
         Returns:
             Self: Dataset itself
         """
-        return super().col_append(elem)
+        return super().col_append(elem, should_create_new_obj, **kwargs)
 
     @_online_except_decorator
-    def col_insert(self, elem: Any, index: Any) -> Self:
+    def col_insert(
+        self,
+        elem: Any,
+        index: Any,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         append a row to dataset
 
         Args:
             elem (Dict[str, List]): dict containing element added to dataset
                 must has column name "name" and column data list "data"
             index (int): where to insert new column
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
         Returns:
             Self: Dataset itself
         """
-        return super().col_insert(elem, index)
+        return super().col_insert(elem, index, should_create_new_obj, **kwargs)
 
     # 等待接口 ready 才能对云端数据集做展示
     @_online_except_decorator
     def col_list(
         self,
         by: Optional[
             Union[slice, int, str, List[int], Tuple[int], List[str], Tuple[str]]
@@ -1051,14 +1216,35 @@
         Returns:
             int: column count。
 
         """
         return super().column_number()
 
     @_online_except_decorator
+    def select_columns(
+        self,
+        columns: List[str],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        """
+        select specific column in dataset
+
+        Args:
+            columns (List[str]):
+                column list
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
+        """
+        return super().select_columns(columns, should_create_new_obj, **kwargs)
+
+    @_online_except_decorator
     def pack(self, **kwargs: Any) -> bool:
         """
         pack all group into 1 row
         and make table array-like with single column
 
         Args:
             **kwargs (Any): other arguments
@@ -1086,14 +1272,39 @@
         """
         if isinstance(self.inner_data_source_cache, FileDataSource):
             return super().unpack(path=self.inner_data_source_cache.path, **kwargs)
         else:
             return super().unpack(**kwargs)
 
     @_online_except_decorator
+    def concat_table(
+        self,
+        concat_dataset: Union["Dataset", List["Dataset"]],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        """
+        concat content of operand dataset to caller dataset
+        this requires two datasets have identical fields
+
+        Args:
+            concat_dataset (Union["Dataset", List["Dataset"]]):
+                Dataset, or list of Dataset, which will be concat
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
+
+        Returns:
+            Dataset: concat Dataset
+        """
+        return super().concat_table(concat_dataset, should_create_new_obj, **kwargs)  # type: ignore
+
+    @_online_except_decorator
     def to_pydict(self) -> Dict:
         """
         convert dataset to dict
 
         Returns:
             Dict: a dict
         """
@@ -1177,19 +1388,19 @@
         """
 
         if model_version_id:
             return self._batch_inference_on_model(
                 model_version_id, output_prettified, **kwargs
             )
         elif service_model or service_endpoint:
-            return self._batch_inference_on_service(
-                service_model,
-                service_endpoint,
-                is_chat_service,
-                does_show_latency,
+            return self._batch_on_service_in_slice_mode(
+                service_model=service_model,
+                service_endpoint=service_endpoint,
+                is_chat_service=is_chat_service,
+                does_show_latency=does_show_latency,
                 **kwargs,
             )
         else:
             err_msg = "no sufficient argument has been passed"
             log_error(err_msg)
             raise ValueError(err_msg)
 
@@ -1238,26 +1449,62 @@
         """
 
         if model_version_id:
             return self._batch_inference_on_model(
                 model_version_id, output_prettified, **kwargs
             )
         elif service_model or service_endpoint:
-            return await self._async_batch_inference_on_service(
-                service_model,
-                service_endpoint,
-                is_chat_service,
-                does_show_latency,
+            return await self._async_batch_on_service_in_slice_mode(
+                service_model=service_model,
+                service_endpoint=service_endpoint,
+                is_chat_service=is_chat_service,
+                does_show_latency=does_show_latency,
                 **kwargs,
             )
         else:
             err_msg = "no sufficient argument has been passed"
             log_error(err_msg)
             raise ValueError(err_msg)
 
+    def _batch_on_service_in_slice_mode(
+        self, slice_size: int = -1, **kwargs: Any
+    ) -> "Dataset":
+        if slice_size <= 0:
+            return self._batch_inference_on_service(**kwargs)
+
+        result_ds_list: List[Dataset] = []
+
+        for i in range(0, len(self), slice_size):
+            start_index = i
+            end_index = min(i + slice_size - 1, len(self) - 1)
+            sliced_dataset = self.take_slice(start_index, end_index, True)
+
+            result_ds_list.append(sliced_dataset._batch_inference_on_service(**kwargs))
+
+        return result_ds_list[0].concat_table(result_ds_list[1:])
+
+    async def _async_batch_on_service_in_slice_mode(
+        self, slice_size: int = -1, **kwargs: Any
+    ) -> "Dataset":
+        if slice_size <= 0:
+            return await self._async_batch_inference_on_service(**kwargs)
+
+        result_ds_list: List[Dataset] = []
+
+        for i in range(0, len(self), slice_size):
+            start_index = i
+            end_index = min(i + slice_size - 1, len(self) - 1)
+            sliced_dataset = self.take_slice(start_index, end_index, True)
+
+            result_ds_list.append(
+                await sliced_dataset._async_batch_inference_on_service(**kwargs)
+            )
+
+        return result_ds_list[0].concat_table(result_ds_list[1:])
+
     def _batch_inference_on_model(
         self, model_version_id: str, output_prettified: bool, **kwargs: Any
     ) -> "Dataset":
         """
         create batch run using specific dataset on qianfan
         by evaluation ability of platform
 
@@ -1330,15 +1577,17 @@
 
         reference_column: Optional[str] = None
         if self.reference_column:
             table_dict[OldReferenceColumnName] = self.get_reference_data
             reference_column = OldReferenceColumnName
 
         if does_show_latency:
-            if len(first_token_latency_list) != 0:
+            if any(
+                [value != -1 and value != -1.0 for value in first_token_latency_list]
+            ):
                 table_dict[FirstTokenLatencyColumnName] = first_token_latency_list
             table_dict[RequestLatencyColumnName] = request_latency_list
 
         return Dataset.create_from_pyobj(
             table_dict,
             input_columns=self.input_columns,
             reference_column=reference_column,
@@ -1368,15 +1617,17 @@
         table_dict: Dict[str, Any] = {
             NewInputChatColumnName: input_list,
             LLMOutputColumnName: output_list,
             OldReferenceColumnName: reference_list,
         }
 
         if does_show_latency:
-            if len(first_token_latency_list) != 0:
+            if any(
+                [value != -1 and value != -1.0 for value in first_token_latency_list]
+            ):
                 table_dict[FirstTokenLatencyColumnName] = first_token_latency_list
             table_dict[RequestLatencyColumnName] = request_latency_list
 
         return Dataset.create_from_pyobj(
             table_dict,
             input_columns=[NewInputChatColumnName],
             reference_column=OldReferenceColumnName,
@@ -1643,7 +1894,148 @@
                     )
                 else:
                     reference_list.append(reference)
 
             input_chat_list.append(input_messages)
 
         return input_chat_list, reference_list
+
+    def show_as_table(self, show_in_browser: bool = False) -> None:
+        """
+        show dataset in browser or console
+
+        Args:
+            show_in_browser (bool):
+                whether show dataset in browser or console,
+                default to None.
+        """
+
+        if not show_in_browser:
+            from tabulate import tabulate
+
+            print(
+                tabulate(
+                    self.col_list(),
+                    showindex="always",
+                    headers="keys",
+                    tablefmt="simple",
+                    numalign="right",
+                )
+            )
+        else:
+            open_html_in_browser(self)
+
+    def show_overview_info(self) -> None:
+        """
+        show overall info in console
+        """
+
+        repetition_set: Dict[str, Dict[Any, int]] = {}
+        null_counter_set: Dict[str, int] = {}
+
+        packed_identifier = "_packed_identifier"
+
+        def _iterator(
+            entry: Union[List[Dict[str, Any]], Dict[str, Any], str], **kwargs: Any
+        ) -> None:
+            if isinstance(entry, (list, str)):
+                if (
+                    packed_identifier not in repetition_set
+                    and packed_identifier not in null_counter_set
+                ):
+                    repetition_set[packed_identifier] = {}
+                    null_counter_set[packed_identifier] = 0
+
+                if not entry:
+                    null_counter_set[packed_identifier] += 1
+                else:
+                    repetition_set[packed_identifier][entry] = (
+                        repetition_set[packed_identifier].get(entry, 0) + 1
+                    )
+            else:
+                for k, v in entry.items():
+                    if k not in null_counter_set and k not in repetition_set:
+                        repetition_set[k] = {}
+                        null_counter_set[k] = 0
+                    if not v:
+                        null_counter_set[v] += 1
+                    else:
+                        repetition_set[k][v] = repetition_set[k].get(v, 0) + 1
+
+        self.iterate(_iterator)
+
+        print(f"entry count: {len(self)}\n")
+
+        if packed_identifier not in null_counter_set:
+            column_fields = self.col_names()
+
+            reputation_result_data: List[float] = []
+            null_result_data: List[float] = []
+
+            for field in column_fields:
+                reputation_result_data.append(
+                    1 - (len(repetition_set[field]) / len(self))
+                )
+                null_result_data.append(null_counter_set[field] / len(self))
+
+            print(
+                tabulate(
+                    [self.col_names(), reputation_result_data, null_result_data],
+                    showindex=["reputation_ratio", "null_ratio"],
+                    headers="firstrow",
+                    tablefmt="simple",
+                    numalign="right",
+                )
+            )
+        else:
+            print(
+                tabulate(
+                    [
+                        "content",
+                        [1 - (len(repetition_set[packed_identifier]) / len(self))],
+                        [null_counter_set[packed_identifier] / len(self)],
+                    ],
+                    showindex=["reputation_ratio", "null_ratio"],
+                    headers="firstrow",
+                    tablefmt="simple",
+                    numalign="right",
+                )
+            )
+
+    def show_processed_statistics(
+        self, methods: List[SummarizationMethod] = [], **kwargs: Any
+    ) -> None:
+        """
+        show processed statistics data
+
+        Args:
+            methods (List[SummarizationMethod]):
+                statistic method list
+            **kwargs (Any):
+                other arguments
+        """
+        from tabulate import tabulate
+
+        if not methods or len(methods) == 0:
+            methods = [
+                MeanMethod(),
+                MinMethod(),
+                MaxMethod(),
+                QuantileMethod(q=0.2),
+                QuantileMethod(q=0.5),
+                QuantileMethod(q=0.8),
+                QuantileMethod(q=0.9),
+            ]
+
+        columns = [k for k, v in self.list(0).items() if isinstance(v, (int, float))]
+        result_data = [method.calculate(self, columns, **kwargs) for method in methods]
+        index_names = [method.name for method in methods]
+
+        print(
+            tabulate(
+                [columns, *result_data],
+                showindex=index_names,
+                headers="firstrow",
+                tablefmt="simple",
+                numalign="right",
+            )
+        )
```

### Comparing `qianfan-0.3.7.1/qianfan/dataset/dataset_utils.py` & `qianfan-0.3.8/qianfan/dataset/dataset_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 utilities dataset needs
 """
 import time
-from typing import Any, Dict, Iterator, List, Optional, Sequence, Tuple, Union
+import webbrowser
+from http.server import BaseHTTPRequestHandler, HTTPServer
+from typing import Any, BinaryIO, Dict, Iterator, List, Optional, Sequence, Tuple, Union
 
 import requests
 
 from qianfan import ChatCompletion, Completion, QfResponse, get_config
 from qianfan.common import Prompt
 from qianfan.dataset.data_source import DataSource, QianfanDataSource
 from qianfan.dataset.schema import (
@@ -36,14 +38,61 @@
     DataTemplateType,
     ETLTaskStatus,
     EvaluationTaskStatus,
 )
 from qianfan.utils import log_debug, log_error, log_info, log_warn
 from qianfan.utils.utils import generate_letter_num_random_id
 
+column_field_template = """
+      {{
+        title: `{0}`,
+        dataIndex: `{0}`,
+        key: `{0}`,
+      }},
+"""
+
+top_half_html = """
+<!DOCTYPE html>
+<html lang="en">
+<head>
+  <meta charset="UTF-8">
+  <meta name="viewport" content="width=device-width, initial-scale=1.0">
+  <title>Ant Design Table Example</title>
+  <!-- 引入 Ant Design 的 CSS 文件 -->
+  <link rel="stylesheet" href="https://cdn.bootcdn.net/ajax/libs/antd/4.18.0/antd.min.css">
+</head>
+<body>
+  <!-- 定义一个容器用于渲染表格 -->
+  <div id="app"></div>
+
+  <!-- 引入 Ant Design 的 JavaScript 文件 -->
+  <script src="https://cdn.bootcdn.net/ajax/libs/react/17.0.2/umd/react.production.min.js"></script>
+  <script src="https://cdn.bootcdn.net/ajax/libs/react-dom/17.0.2/umd/react-dom.production.min.js"></script>
+  <script src="https://cdn.bootcdn.net/ajax/libs/babel-standalone/6.26.0/babel.min.js"></script>
+  <script src="https://cdn.bootcdn.net/ajax/libs/antd/4.18.0/antd.min.js"></script>
+
+  <!-- 定义表格的列和数据 -->
+  <script type="text/babel">
+    const { Table } = antd;
+
+
+"""
+
+bottom_half_html = """
+
+    // 在容器中渲染表格
+    ReactDOM.render(
+      <Table columns={columns} dataSource={data} />,
+      document.getElementById('app')
+    );
+  </script>
+</body>
+</html>
+"""
+
 
 def _check_online_data_process_result(etl_id: str) -> Optional[Union[bool, int]]:
     """
     check etl task result using etl task id
 
     Args:
         etl_id (str):
@@ -150,24 +199,31 @@
     service: Union[ChatCompletion, Completion],
     input_list: Union[List[str], List[List[Dict[str, Any]]]],
     *args: Any,
     **kwargs: Any,
 ) -> Tuple[List[str], List[float], List[float]]:
     if "prompt_template" in kwargs:
         kwargs.pop("prompt_template")
+
+    if "access_key" in kwargs:
+        kwargs.pop("access_key")
+
+    if "secret_key" in kwargs:
+        kwargs.pop("secret_key")
+
     output_list: List[str] = []
-    request_latency_list: List[float] = []
-    first_token_latency_list: List[float] = []
+    request_latency_list: List[float] = [-1 for _ in range(len(input_list))]
+    first_token_latency_list: List[float] = [-1 for _ in range(len(input_list))]
     results = service.batch_do(input_list, *args, **kwargs).results()  # type: ignore
     for idx in range(len(results)):
         result = results[idx]
         if isinstance(result, QfResponse):
             output_list.append(result.body["result"])
             latencies = log_latency_info(result, idx)
-            request_latency_list.append(latencies[0])
+            request_latency_list[idx] = latencies[0]
         elif isinstance(result, Exception):
             log_warn(
                 "an exception has occurred during batch requesting and its"
                 f" result will be empty string. exception: {result}\ninput:"
                 f" {input_list[idx]}"
             )
             output_list.append("")
@@ -178,16 +234,16 @@
             total_latency: float = 0
             for r in result:
                 result_str += r.body["result"]
                 index += 1
                 latencies = log_latency_info(r, idx, index)
                 first_token_latency, total_latency = latencies[1], latencies[2]
             output_list.append(result_str)
-            request_latency_list.append(total_latency)
-            first_token_latency_list.append(first_token_latency)
+            request_latency_list[idx] = total_latency
+            first_token_latency_list[idx] = first_token_latency
 
     return output_list, request_latency_list, first_token_latency_list
 
 
 async def _async_batch_do_on_service(
     service: Union[ChatCompletion, Completion],
     input_list: Union[List[str], List[List[Dict[str, Any]]]],
@@ -379,21 +435,79 @@
             if column not in prompt_template.variables:
                 err_msg = f"input column {column} not in prompt template"
                 log_error(err_msg)
                 raise ValueError(err_msg)
 
     service: Union[ChatCompletion, Completion]
     if is_chat_service:
-        service = ChatCompletion(service_model, service_endpoint)
+        service = ChatCompletion(service_model, service_endpoint, **kwargs)
     else:
-        service = Completion(service_model, service_endpoint)
+        service = Completion(service_model, service_endpoint, **kwargs)
 
     return service
 
 
 def _extract_string(data: Union[str, Iterator[str]]) -> str:
     if isinstance(data, str):
         return data
     elif hasattr(data, "__iter__"):
         for item in data:
             return _extract_string(item)
     return ""
+
+
+def open_html_in_browser(ds: Any) -> None:
+    """
+    Display Dataset in a web browser without creating a temp file.
+
+    Instantiates a trivial http server and uses the webbrowser module to
+    open a URL to retrieve html from that server.
+
+    Args:
+        ds (Dataset):
+            Dataset need to be displayed
+    """
+
+    def _write_columns_field(bio: BinaryIO) -> None:
+        bio.write(bytes("\t\tconst columns = [\n", encoding="utf8"))
+        bio.write(bytes(column_field_template.format("index"), encoding="utf8"))
+        for field in ds.col_names():
+            bio.write(bytes(column_field_template.format(field), encoding="utf8"))
+        bio.write(bytes("\t\t];\n", encoding="utf8"))
+
+    def _write_column_data(bio: BinaryIO) -> None:
+        bio.write(bytes("\t\tconst data = [\n", encoding="utf8"))
+        index = 0
+
+        def _iterate(entry: Dict[str, Any], **kwargs: Any) -> None:
+            nonlocal index
+            index += 1
+
+            bio.write(bytes("\t\t\t{\n", encoding="utf8"))
+
+            bio.write(bytes("\t\t\t\tkey: `{}`,\n".format(index), encoding="utf8"))
+            bio.write(bytes("\t\t\t\tindex: `{}`,\n".format(index), encoding="utf8"))
+            for k, v in entry.items():
+                bio.write(bytes("\t\t\t\t{}: `{}`,\n".format(k, v), encoding="utf8"))
+
+            bio.write(bytes("\t\t\t},\n", encoding="utf8"))
+
+        ds.iterate(_iterate)
+        bio.write(bytes("\t\t];\n", encoding="utf8"))
+
+    browser = webbrowser.get(None)
+
+    class OneShotRequestHandler(BaseHTTPRequestHandler):
+        def do_GET(self) -> None:
+            self.send_response(200)
+            self.send_header("Content-type", "text/html")
+            self.end_headers()
+
+            self.wfile.write(bytes(top_half_html, encoding="utf8"))
+            _write_columns_field(self.wfile)
+            _write_column_data(self.wfile)
+            self.wfile.write(bytes(bottom_half_html, encoding="utf8"))
+
+    server = HTTPServer(("127.0.0.1", 0), OneShotRequestHandler)
+    browser.open("http://127.0.0.1:%s" % server.server_port)
+
+    server.handle_request()
```

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/__init__.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/base.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_character_repetition_filter.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_character_repetition_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_flagged_words.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_flagged_words.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_sentence_length_filter.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_sentence_length_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_special_characters.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_special_characters.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_stopwords.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_stopwords.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_word_number.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_word_number.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/check_word_repetition_filter.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/check_word_repetition_filter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/consts.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/utils.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/local_data_operators/word_list.py` & `qianfan-0.3.8/qianfan/dataset/local_data_operators/word_list.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/process_interface.py` & `qianfan-0.3.8/qianfan/dataset/process_interface.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/qianfan_data_operators.py` & `qianfan-0.3.8/qianfan/dataset/qianfan_data_operators.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/schema.py` & `qianfan-0.3.8/qianfan/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/dataset/table.py` & `qianfan-0.3.8/qianfan/dataset/table.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 wrapper for pyarrow.Table
 """
-import threading
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     List,
     Optional,
@@ -41,14 +40,16 @@
     Listable,
     Processable,
 )
 from qianfan.dataset.table_utils import _construct_table_from_nest_sequence
 from qianfan.utils import log_debug, log_error, log_info, log_warn
 from qianfan.utils.pydantic import BaseModel
 
+i = 0
+
 
 def _create_new_table_for_add(
     elem: Union[
         List[List[Dict]], List[Dict], Tuple[Dict], Dict, List[str], Tuple[str], str
     ],
     is_dataset_packed: bool = False,
     add_new_group: bool = False,
@@ -131,51 +132,14 @@
     return col_names == [QianfanDatasetPackColumnName]
 
 
 def _whether_dataset_is_grouped(col_names: List[str]) -> bool:
     return QianfanDataGroupColumnName in col_names
 
 
-class TaskDispatcher:
-    def __init__(self, batch_size: int, task_number: int):
-        self.task_queue: List[Tuple[int, int]] = []
-        for batch_index in range(0, task_number, batch_size):
-            current_batch_size = min(task_number - batch_index, batch_size)
-            self.task_queue.append((batch_index, current_batch_size))
-
-        self.lock = threading.Lock()
-        self.current_task_queue_index = 0
-
-    def get_task(self) -> Optional[Tuple[int, int]]:
-        with self.lock:
-            if self.current_task_queue_index >= len(self.task_queue):
-                return None
-
-            task = self.task_queue[self.current_task_queue_index]
-            self.current_task_queue_index += 1
-            return task
-
-    def mapper_closure(
-        self, func: Callable[[int, int], Generator[Any, None, None]]
-    ) -> Callable[[], Generator[Tuple[int, Any], None, None]]:
-        def new_func() -> Generator[Tuple[int, Any], None, None]:
-            task_slice = self.get_task()
-            while task_slice:
-                batch_index, batch_size = task_slice[0], task_slice[1]
-                returned_data_list: List[Any] = []
-
-                for returned_data in func(batch_index, batch_size):
-                    returned_data_list.append(returned_data)
-
-                yield batch_index, returned_data_list
-                task_slice = self.get_task()
-
-        return new_func
-
-
 class _PyarrowRowManipulator(BaseModel, Addable, Listable, Processable):
     """handler for processing of pyarrow table row"""
 
     class Config:
         arbitrary_types_allowed = True
 
     table: PyarrowTable
@@ -190,28 +154,28 @@
         self,
         elem: Union[List[Dict], Tuple[Dict], Dict],
         is_dataset_packed: bool = False,
         add_new_group: bool = False,
         is_grouped: bool = True,
         group_id: int = -1,
         **kwargs: Any,
-    ) -> Self:
+    ) -> PyarrowTable:
         """
         append element(s) to pyarrow table
 
         Args:
             elem (Union[List[Dict], Tuple[Dict], Dict]):
                 element(s) added to pyarrow table
             is_dataset_packed (bool): whether table is packed, default to False.
             add_new_group (bool): whether elem has new group id, default to False.
             is_grouped (bool): whether elem is grouped, default to True.
             group_id (int): new group id, default to -1.
             **kwargs (Any): optional arguments
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         return pyarrow.concat_tables(
             [
                 self.table,
                 _create_new_table_for_add(
                     elem,
@@ -230,29 +194,29 @@
         elem: Union[List[Dict], Tuple[Dict], Dict],
         index: int,
         is_dataset_packed: bool = False,
         add_new_group: bool = False,
         is_grouped: bool = True,
         group_id: int = -1,
         **kwargs: Any,
-    ) -> Self:
+    ) -> PyarrowTable:
         """
         insert element(s) to pyarrow table
 
         Args:
             elem (Union[List[Dict], Tuple[Dict], Dict]):
                 element(s) added to pyarrow table
             index (int): where to insert element(s).
             is_dataset_packed (bool): whether table is packed, default to False.
             add_new_group (bool): whether elem has new group id, default to False.
             is_grouped (bool): whether elem is grouped, default to True.
             group_id (int): new group id, default to -1.
             **kwargs (Any): optional arguments
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
         table_length = self.table.num_rows
         if index < 0 or index > table_length:
             err_msg = f"can't insert element at {index}"
             log_error(err_msg)
             raise ValueError(err_msg)
 
@@ -329,62 +293,64 @@
     def map(
         self,
         op: Callable[[Any], Any],
         batch_size: int = 10000,
         path: str = "./default_path",
         keep_original_order: bool = True,
         **kwargs: Any,
-    ) -> Self:
+    ) -> PyarrowTable:
         """
         map on pyarrow table's row
 
         Args:
             op (Callable[[Any], Any]): handler used to map
             batch_size (int): batch size of concurrent processing
             path (str): where to save temporary arrow file
             keep_original_order (bool): does table after mapping will keep
                 same order with OG Table, default to True
             **kwargs (Any): other arguments
 
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         # 构建出的新 table 会按照首行的 key 作为 columns
         # 现在处理都是按照单行为单位处理，
         # 这样子做的目的是确保每次处理时只会有一条数据被读入到内存中，
         # 防止一次性读入全部数据，丧失 Memory-Map 的含义
         # 后续需要优化成 Batch + 多线程的形式来优化数据集处理速度
 
         # 如果数据集是被 pack 起来的，则按照一行作为一个列表，传递给 op 函数
 
         # 创建一个任务分配器，来分配需要处理的区间
-        task_dispatcher = TaskDispatcher(batch_size, self.table.num_rows)
 
         if self._inner_table_is_packed():
 
             def _mapper_closure(
                 batch_index: int, batch_size: int
             ) -> Generator[Any, None, None]:
                 # 拿到一个区间任务并取出区间数据
                 rows = self.table.slice(batch_index, batch_size).to_pydict()[
                     QianfanDatasetPackColumnName
                 ]
 
                 # 开始处理并且放在结果集合里面
                 for row in rows:
                     returned_data = op(row)
+                    # 为了支持返回的是个迭代器的情况，需要特判
+                    # 这个逻辑应该是只会在 Packed 的情况下出现
+                    # 因为需要返回迭代器的情况是一条数据返回多条数据
+                    # 而会产生多条数据的情况有且仅有在原始数据集是 Packed 的情况
+                    if isinstance(returned_data, Generator):
+                        yield from returned_data
+                        continue
+
                     if not returned_data:
                         log_warn("a row has been deleted from table")
                         continue
-                    if not isinstance(returned_data, (list, str)):
-                        raise ValueError(
-                            "returned value isn't list or str, rather"
-                            f" {type(returned_data)}"
-                        )
 
                     yield returned_data
 
         else:
             is_grouped = self._inner_table_is_grouped()
 
             def _mapper_closure(
@@ -412,65 +378,118 @@
                     yield returned_data
 
         from qianfan.dataset.data_source.utils import _create_map_arrow_file
 
         return _create_map_arrow_file(
             path=path,
             **kwargs,
-            mapper_closure=task_dispatcher.mapper_closure(_mapper_closure),
+            mapper_closure=_mapper_closure,
+            batch_size=batch_size,
+            task_number=self.table.num_rows,
             keep_original_order=keep_original_order,
         )
 
-    def filter(self, op: Callable[[Any], bool]) -> Self:
+    def iterate(
+        self, op: Callable[[Any], None], batch_size: int = 10000, **kwargs: Any
+    ) -> None:
+        """
+        iterate on pyarrow table's row
+
+        Args:
+            op (Callable[[Any], None]): handler used to iterate
+            batch_size (int): batch size of concurrent processing
+            **kwargs (Any): other arguments
+        """
+        from qianfan.dataset.data_source.utils import _pure_iterate
+
+        if self._inner_table_is_packed():
+
+            def _iterate_closure(
+                batch_index: int, batch_size: int
+            ) -> Generator[None, None, None]:
+                # 拿到一个区间任务并取出区间数据
+                rows = self.table.slice(batch_index, batch_size).to_pydict()[
+                    QianfanDatasetPackColumnName
+                ]
+                for row in rows:
+                    op(row)
+                    yield None
+
+        else:
+
+            def _iterate_closure(
+                batch_index: int, batch_size: int
+            ) -> Generator[None, None, None]:
+                rows = self.table.slice(batch_index, batch_size).to_pylist()
+                for row in rows:
+                    input_dict = {key: val for key, val in row.items()}
+
+                    op(input_dict)
+                    yield None
+
+        _pure_iterate(_iterate_closure, batch_size, self.table.num_rows, **kwargs)
+
+    def filter(
+        self, op: Callable[[Any], bool], batch_size: int = 10000, **kwargs: Any
+    ) -> PyarrowTable:
         """
         filter on pyarrow table's row
 
         Args:
             op (Callable[[Any], bool]): handler used to filter
+            batch_size (int): batch size of concurrent processing
+            **kwargs (Any): other arguments
 
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
+        from qianfan.dataset.data_source.utils import _iterate_to_conduct_result
 
-        selection_masks: List[bool] = []
         if self._inner_table_is_packed():
-            for row_index in range(self.table.num_rows):
-                row = self.table.take([row_index]).to_pylist()[0][
+
+            def _filter_closure(
+                batch_index: int, batch_size: int
+            ) -> Generator[Any, None, None]:
+                # 拿到一个区间任务并取出区间数据
+                rows = self.table.slice(batch_index, batch_size).to_pydict()[
                     QianfanDatasetPackColumnName
                 ]
-                flag = op(row)
-                if flag is None:
-                    raise ValueError("cant return None")
-                if not isinstance(flag, bool):
-                    raise ValueError("returned value isn't bool")
+                for row in rows:
+                    flag = op(row)
+
+                    yield flag
 
-                selection_masks.append(flag)
         else:
-            for row_index in range(self.table.num_rows):
-                origin_data = self.table.take([row_index]).to_pylist()[0]
-                input_dict = {key: val for key, val in origin_data.items()}
-                flag = op(input_dict)
-                if flag is None:
-                    raise ValueError("cant return None")
-                if not isinstance(flag, bool):
-                    raise ValueError("returned value isn't bool")
 
-                selection_masks.append(flag)
+            def _filter_closure(
+                batch_index: int, batch_size: int
+            ) -> Generator[Any, None, None]:
+                rows = self.table.slice(batch_index, batch_size).to_pylist()
+                for row in rows:
+                    input_dict = {key: val for key, val in row.items()}
+
+                    flag = op(input_dict)
 
-        return self.table.filter(mask=selection_masks)
+                    yield flag
 
-    def delete(self, index: Union[int, str]) -> Self:
+        return self.table.filter(
+            _iterate_to_conduct_result(
+                _filter_closure, batch_size, self.table.num_rows, **kwargs
+            )
+        )
+
+    def delete(self, index: Union[int, str]) -> PyarrowTable:
         """
         delete an element from pyarrow table
 
         Args:
             index (Union[int, str]): element index to delete
 
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         if isinstance(index, str):
             raise ValueError("cannot delete row by str")
         table_length = self.table.num_rows
         if index < 0 or index >= table_length:
             raise OverflowError(f"index overflow, table length is {table_length}")
@@ -478,32 +497,50 @@
             return self.table.slice(1)
         elif index == table_length - 1:
             return self.table.slice(0, table_length - 1)
         return pyarrow.concat_tables(
             [self.table.slice(0, index), self.table.slice(index + 1)]
         )
 
+    def take_slice(self, start: int = 0, end: int = -1) -> PyarrowTable:
+        if start < 0:
+            err_msg = f"start index is smaller than 0: {start}"
+            log_error(err_msg)
+            raise ValueError(err_msg)
+
+        if end >= self.table.num_rows:
+            err_msg = (
+                f"end index {end} is bigger than table size: {self.table.num_rows}"
+            )
+            log_error(err_msg)
+            raise ValueError(err_msg)
+
+        if end < 0:
+            end = self.table.num_rows - 1
+
+        return self.table.slice(start, end - start + 1)
+
 
 class _PyarrowColumnManipulator(BaseModel, Addable, Listable, Processable):
     """handler for processing of pyarrow table column"""
 
     class Config:
         arbitrary_types_allowed = True
 
     table: PyarrowTable
 
-    def append(self, elem: Dict[str, List]) -> Self:
+    def append(self, elem: Dict[str, List]) -> PyarrowTable:
         """
         append a row to pyarrow table
 
         Args:
             elem (Dict[str, List]): dict containing element added to pyarrow table
                 key as column name, value as column data
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         if not isinstance(elem, dict):
             raise ValueError(f"element appended must be dict, not {type(elem)}")
 
         for name, data in elem.items():
             if name in self.table.column_names:
@@ -518,25 +555,25 @@
                     f" {len(data)}"
                 )
 
             self.table = self.table.append_column(name, [data])
 
         return self.table
 
-    def insert(self, elem: Dict[str, List], index: int) -> Self:
+    def insert(self, elem: Dict[str, List], index: int) -> PyarrowTable:
         """
         insert a row to pyarrow table
 
         Args:
             elem (Dict[str, List]): dict containing element added to pyarrow table
                 must has column name "name" and column data list "data"
             index (int): where to insert new column
 
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         col_length = self.table.num_columns
         if index < 0 or index > col_length:
             err_msg = f"can't insert column at {index}"
             log_error(err_msg)
             raise ValueError(err_msg)
@@ -571,86 +608,112 @@
             indices = by
         if isinstance(indices[0], str) and not set(indices).issubset(
             set(self.table.column_names)
         ):
             raise ValueError(f"contain not existed column name: {indices}")
         return self.table.select(list(indices)).to_pydict()
 
-    def map(self, op: Callable[[Any], Any]) -> Self:
+    def map(self, op: Callable[[Any], Any]) -> PyarrowTable:
         """
         map on pyarrow table's column
 
         Args:
             op (Callable[[Any], Any]): handler used to map
 
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         new_columns: Dict[str, List[Any]] = {}
         for i in range(self.table.num_columns):
             column = self.table.select([i]).to_pydict()
             ret_column = op(column)
             new_columns.update(ret_column)
 
         return pyarrow.Table.from_pydict(new_columns)
 
-    def filter(self, op: Callable[[Any], bool]) -> Self:
+    def filter(self, op: Callable[[Any], bool]) -> PyarrowTable:
         """
         filter on pyarrow table's column
 
         Args:
             op (Callable[[Any], bool]): handler used to filter
 
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         dropped_column_name = []
         for i in range(self.table.num_columns):
             column = self.table.select([i]).to_pydict()
             if not op(column):
                 dropped_column_name += list(column.keys())
 
         return self.table.drop_columns(dropped_column_name)
 
-    def delete(self, index: Union[int, str]) -> Self:
+    def delete(self, index: Union[int, str]) -> PyarrowTable:
         """
         delete an column from pyarrow table
 
         Args:
             index (str): column name to delete
 
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         if isinstance(index, int):
             raise ValueError("cannot delete column by int")
         return self.table.drop_columns(index)
 
-    def col_renames(self, new_names: List[str]) -> Self:
+    def col_renames(self, new_names: List[str]) -> PyarrowTable:
         """
         rename all dataset column
 
         Args:
             new_names (List[str]): All new names for columns
         Returns:
-            Self: a new pyarrow table
+            PyarrowTable: a new pyarrow table
         """
 
         if (
             _whether_dataset_is_grouped(self.table.column_names)
             and QianfanDataGroupColumnName not in new_names
         ):
             i = self.table.column_names.index(QianfanDataGroupColumnName)
             new_names.insert(i, QianfanDataGroupColumnName)
 
         return self.table.rename_columns(new_names)
 
+    def select_columns(self, columns: List[str]) -> PyarrowTable:
+        return self.table.select(columns)
+
+    def mean(self, column: str, skip_nulls: bool = True) -> float:
+        return pc.mean(self.table.column(column), skip_nulls=skip_nulls)
+
+    def quantile(
+        self,
+        column: str,
+        q: Union[List[float], float] = 0.5,
+        interpolation: str = "linear",
+        skip_nulls: bool = True,
+    ) -> List[float]:
+        return pc.quantile(
+            self.table.column(column),
+            q=q,
+            interpolation=interpolation,
+            skip_nulls=skip_nulls,
+        )
+
+    def min(self, column: str, skip_nulls: bool = True) -> Union[int, float]:
+        return pc.min(self.table.column(column), skip_nulls=skip_nulls)
+
+    def max(self, column: str, skip_nulls: bool = True) -> Union[int, float]:
+        return pc.max(self.table.column(column), skip_nulls=skip_nulls)
+
 
 class Table(Addable, Listable, Processable):
     """
     dataset representation on memory
     inherited from pyarrow.Table，implementing interface in process_interface.py
     """
 
@@ -703,14 +766,34 @@
             new_group_column_list.append(current_group_number)
 
         self.col_delete(QianfanDataGroupColumnName)
         self.col_append({QianfanDataGroupColumnName: new_group_column_list})
 
         return
 
+    def _create_new_obj(
+        self,
+        arrow_table: PyarrowTable,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        if not should_create_new_obj:
+            self.inner_table = arrow_table
+            return self
+
+        attr_dict = vars(self)
+        new_obj = self.__class__(inner_table=arrow_table)
+        for k, v in attr_dict.items():
+            if k == "inner_table":
+                continue
+
+            setattr(new_obj, k, v)
+
+        return new_obj
+
     def pack(
         self, batch_size: int = 10000, path: str = "./default_path", **kwargs: Any
     ) -> bool:
         """
         pack all group into 1 row
         and make table array-like with single column
 
@@ -742,16 +825,14 @@
             inner_index, [list(range(self.row_number()))]
         ).sort_by(QianfanDataGroupColumnName)
 
         # 用于合并由于切分数据集而导致被分割的同组元素的一个 Dict
         # 键是由下一个切片的开始索引
         merge_dict: Dict[int, Tuple[int, List[Dict[str, Any]]]] = {}
 
-        task_dispatcher = TaskDispatcher(batch_size, self.inner_table.num_rows)
-
         def _pack_closure(
             batch_index: int, batch_size: int
         ) -> Generator[Any, None, None]:
             # 当前组别的数据缓存
             group_data: List[Dict[str, Any]] = []
 
             rows = group_ordered_table.slice(batch_index, batch_size).to_pylist()
@@ -770,14 +851,17 @@
                     )
                     log_error(err_msg)
                     raise ValueError(err_msg)
 
                 rows[i].pop(inner_index)
                 rows[i].pop(QianfanDataGroupColumnName)
 
+                if "response" in rows[i] and isinstance(rows[i]["response"], str):
+                    rows[i]["response"] = [[rows[i]["response"]]]
+
                 # 当读完所有当前组的数据后，返回一次
                 if group_index != current_group_index:
                     if is_first_group_chunk:
                         is_first_group_chunk = False
                         if batch_index in merge_dict:
                             data_tuple = merge_dict[batch_index]
                             if data_tuple[0] == group_index:
@@ -802,15 +886,17 @@
                     yield group_data
 
         from qianfan.dataset.data_source.utils import _create_map_arrow_file
 
         self.inner_table = _create_map_arrow_file(
             path=path,
             **kwargs,
-            mapper_closure=task_dispatcher.mapper_closure(_pack_closure),
+            mapper_closure=_pack_closure,
+            batch_size=batch_size,
+            task_number=self.inner_table.num_rows,
         )
         return True
 
     def unpack(
         self, batch_size: int = 10000, path: str = "./default_path", **kwargs: Any
     ) -> bool:
         """
@@ -843,16 +929,14 @@
             isinstance(element, (list, tuple))
             and element
             and isinstance(element[0], dict)
         ):
             log_warn(f"dataset has element not supported: {element}")
             return False
 
-        task_dispatcher = TaskDispatcher(batch_size, self.inner_table.num_rows)
-
         def _unpack_closure(
             batch_index: int, batch_size: int
         ) -> Generator[Any, None, None]:
             rows = self.inner_table.slice(batch_index, batch_size).to_pydict()[
                 QianfanDatasetPackColumnName
             ]
             for i in range(len(rows)):
@@ -864,66 +948,110 @@
                     yield data
 
         from qianfan.dataset.data_source.utils import _create_map_arrow_file
 
         self.inner_table = _create_map_arrow_file(
             path=path,
             **kwargs,
-            mapper_closure=task_dispatcher.mapper_closure(_unpack_closure),
+            mapper_closure=_unpack_closure,
+            batch_size=batch_size,
+            task_number=self.inner_table.num_rows,
         )
         return True
 
     # 直接调用 Table 对象的接口方法都默认是在行上做处理
-    def map(self, op: Callable[[Any], Any], **kwargs: Any) -> Self:
+    def map(
+        self,
+        op: Callable[[Any], Any],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         map on pyarrow table's row
 
         Args:
             op (Callable[[Any], Any]): handler used to map
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
             **kwargs (Any): other arguments
 
         Returns:
             Self: Table itself
         """
         manipulator = self._row_op()
         if not callable(op):
             err_msg = "op has type {type}, rather than callable"
             log_error(err_msg)
             raise TypeError(err_msg)
 
-        self.inner_table = manipulator.map(op, **kwargs)  # noqa
-        return self
+        result_ds = manipulator.map(op, **kwargs)
+
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
-    def filter(self, op: Callable[[Any], bool]) -> Self:
+    def filter(
+        self,
+        op: Callable[[Any], bool],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         filter on pyarrow table's row
 
         Args:
             op (Callable[[Any], bool]): handler used to filter
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Table itself
         """
         manipulator = self._row_op()
-        self.inner_table = manipulator.filter(op)
-        return self
+        result_ds = manipulator.filter(op, **kwargs)
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
-    def delete(self, index: Union[int, str]) -> Self:
+    def delete(
+        self, index: Union[int, str], should_create_new_obj: bool = False, **kwargs: Any
+    ) -> Self:
         """
         delete an element from pyarrow table
 
         Args:
             index (Union[int, str]): element index to delete
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Table itself
         """
         manipulator = self._row_op()
-        self.inner_table = manipulator.delete(index)
-        return self
+        result_ds = manipulator.delete(index)
+        return self._create_new_obj(result_ds, should_create_new_obj)
+
+    def iterate(
+        self,
+        op: Callable[[Any], None],
+        **kwargs: Any,
+    ) -> None:
+        """
+        iterate on pyarrow table's row
+
+        Args:
+            op (Callable[[Any], bool]): handler used to iterate
+            **kwargs (Any): other arguments
+        """
+        manipulator = self._row_op()
+        manipulator.iterate(op, **kwargs)
 
     def _calculate_kwargs_for_add(
         self, add_new_group: bool = False, is_grouped: bool = True, group_id: int = -1
     ) -> Dict[str, Any]:
         kwargs: Dict[str, Any] = {}
         if self.is_dataset_grouped():
             if group_id != -1:
@@ -945,15 +1073,20 @@
             }
         elif self.is_dataset_packed():
             kwargs = {"is_dataset_packed": True}
 
         return kwargs
 
     def append(
-        self, elem: Any, add_new_group: bool = False, is_grouped: bool = True
+        self,
+        elem: Any,
+        add_new_group: bool = False,
+        is_grouped: bool = True,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
     ) -> Self:
         """
         append an element to pyarrow table
 
         Args:
             elem (Union[List[Dict], Tuple[Dict], Dict]): Elements added to pyarrow table
             add_new_group (bool):
@@ -964,31 +1097,38 @@
                 Only used when table is grouped and elem is Sequence
                 and add_new_group was set True.
                 Default to True, all elements
                 will be in same group.
                 If it's True, each element will have
                 sequential incremental group id from last
                 available group id.
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
         Returns:
             Self: Table itself
         """
         manipulator = self._row_op()
 
-        self.inner_table = manipulator.append(
+        result_ds = manipulator.append(
             elem, **self._calculate_kwargs_for_add(add_new_group, is_grouped)
         )
-        return self
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
     def insert(
         self,
         elem: Any,
         index: Any,
         group_id: int = -1,
         add_new_group: bool = False,
         is_grouped: bool = True,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
     ) -> Self:
         """
         insert an element to pyarrow table
 
         Args:
             elem (Union[List[Dict], Tuple[Dict], Dict]): Elements added to pyarrow table
             index (int): where to insert element(s)
@@ -1005,25 +1145,30 @@
                 Only used when table is grouped and elem is Sequence
                 and add_new_group was set True.
                 Default to True, all elements
                 will be in same group.
                 If it's True, each element will have
                 sequential incremental group id from last
                 available group id.
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
         Returns:
             Self: Table itself
         """
         manipulator = self._row_op()
 
-        self.inner_table = manipulator.insert(
+        result_ds = manipulator.insert(
             elem,
             index,
             **self._calculate_kwargs_for_add(add_new_group, is_grouped, group_id),
         )
-        return self
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
     def list(
         self, by: Optional[Union[slice, int, str, Sequence[int], Sequence[str]]] = None
     ) -> Any:
         """
         get element(s) from pyarrow table
 
@@ -1033,84 +1178,148 @@
                 return a python list of pyarrow table row
         Returns:
             Any: pyarrow table row list
         """
         manipulator = self._row_op()
         return manipulator.list(by)
 
-    def col_map(self, op: Callable[[Any], Any]) -> Self:
+    def take_slice(
+        self,
+        start: int = 0,
+        end: int = -1,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        manipulator = self._row_op()
+        result_ds = manipulator.take_slice(start, end)
+        return self._create_new_obj(result_ds, should_create_new_obj)
+
+    def col_map(
+        self,
+        op: Callable[[Any], Any],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         map on pyarrow table's column
 
         Args:
             op (Callable[[Any], Any]): handler used to map
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Table itself
         """
         manipulator = self._col_op()
-        self.inner_table = manipulator.map(op)  # noqa
-        return self
+        result_ds = manipulator.map(op)  # noqa
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
-    def col_filter(self, op: Callable[[Any], bool]) -> Self:
+    def col_filter(
+        self,
+        op: Callable[[Any], bool],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         filter on pyarrow table's column
 
         Args:
             op (Callable[[Any], bool]): handler used to filter
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Table itself
         """
         manipulator = self._col_op()
-        self.inner_table = manipulator.filter(op)
-        return self
+        result_ds = manipulator.filter(op)
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
-    def col_delete(self, index: Union[int, str]) -> Self:
+    def col_delete(
+        self,
+        index: Union[int, str],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         delete a column from pyarrow table
 
         Args:
             index (str): column name to delete
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
 
         Returns:
             Self: Table itself
         """
         manipulator = self._col_op()
-        self.inner_table = manipulator.delete(index)
-        return self
+        result_ds = manipulator.delete(index)
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
-    def col_append(self, elem: Any) -> Self:
+    def col_append(
+        self,
+        elem: Any,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         append a row to pyarrow table
 
         Args:
             elem (Dict[str, List]): dict containing element added to pyarrow table
                 key as column name, value as column data
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
+
         Returns:
             Self: Table itself
         """
         manipulator = self._col_op()
-        self.inner_table = manipulator.append(elem)
-        return self
+        result_ds = manipulator.append(elem)
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
-    def col_insert(self, elem: Any, index: Any) -> Self:
+    def col_insert(
+        self,
+        elem: Any,
+        index: Any,
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
         """
         append a row to pyarrow table
 
         Args:
             elem (Dict[str, List]): dict containing element added to pyarrow table
-                must has column name "name" and column data list "data"
+                must have column name "name" and column data list "data"
             index (int): where to insert new column
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
+
         Returns:
             Self: Table itself
         """
         manipulator = self._col_op()
-        self.inner_table = manipulator.insert(elem, index)
-        return self
+        result_ds = manipulator.insert(elem, index)
+        return self._create_new_obj(result_ds, should_create_new_obj)
 
     def col_list(
         self, by: Optional[Union[slice, int, str, Sequence[int], Sequence[str]]] = None
     ) -> Any:
         """
         get column(s) from pyarrow table
 
@@ -1142,14 +1351,81 @@
         Returns:
             Self: A brand-new Table with new name
         """
         manipulator = self._col_op()
         self.inner_table = manipulator.col_renames(new_names)
         return self
 
+    def select_columns(
+        self,
+        columns: List[str],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        manipulator = self._col_op()
+        result_ds = manipulator.select_columns(columns)
+        return self._create_new_obj(result_ds, should_create_new_obj)
+
+    def mean(self, column: str, skip_nulls: bool = True, **kwargs: Any) -> float:
+        manipulator = self._col_op()
+        return manipulator.mean(column, skip_nulls)
+
+    def quantile(
+        self,
+        column: str,
+        q: Union[List[float], float] = 0.5,
+        interpolation: str = "linear",
+        skip_nulls: bool = True,
+        **kwargs: Any,
+    ) -> List[float]:
+        manipulator = self._col_op()
+        return manipulator.quantile(column, q, interpolation, skip_nulls)
+
+    def min(
+        self, column: str, skip_nulls: bool = True, **kwargs: Any
+    ) -> Union[int, float]:
+        manipulator = self._col_op()
+        return manipulator.min(column, skip_nulls)
+
+    def max(
+        self, column: str, skip_nulls: bool = True, **kwargs: Any
+    ) -> Union[int, float]:
+        manipulator = self._col_op()
+        return manipulator.max(column, skip_nulls)
+
+    def concat_table(
+        self,
+        concat_table: Union[Self, List[Self]],
+        should_create_new_obj: bool = False,
+        **kwargs: Any,
+    ) -> Self:
+        """
+        concat content of operand Table to caller dataset
+        this requires two tables have identical fields
+
+        Args:
+            concat_table (Union[Self, List[Self]]):
+                Table, or list of Table, which will be concat
+            should_create_new_obj (bool):
+                should a new object be created when mapping terminates.
+                Default to False. In some cases, you may want to set
+                this value to True
+            **kwargs (Any): other arguments
+
+        Returns:
+            Self: concat Table
+        """
+        if not isinstance(concat_table, list):
+            concat_table = [concat_table]
+
+        result_ds = pyarrow.concat_tables(
+            [self.inner_table] + [table.inner_table for table in concat_table]
+        )
+        return self._create_new_obj(result_ds, should_create_new_obj)
+
     # 重写 get 和 del 的魔法方法
     def __getitem__(self, key: Any) -> Any:
         if isinstance(key, str) or (
             isinstance(key, Sequence) and isinstance(key[0], str)
         ):
             return self.col_list(key)
         return self.list(key)
```

### Comparing `qianfan-0.3.7.1/qianfan/dataset/table_utils.py` & `qianfan-0.3.8/qianfan/dataset/table_utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/errors.py` & `qianfan-0.3.8/qianfan/errors.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/evaluation/__init__.py` & `qianfan-0.3.8/qianfan/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/evaluation/consts.py` & `qianfan-0.3.8/qianfan/evaluation/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/evaluation/evaluation_manager.py` & `qianfan-0.3.8/qianfan/evaluation/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/evaluation/evaluation_result.py` & `qianfan-0.3.8/qianfan/evaluation/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/evaluation/evaluator.py` & `qianfan-0.3.8/qianfan/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/evaluation/local_evaluator.py` & `qianfan-0.3.8/qianfan/evaluation/local_evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/evaluation/opencompass_evaluator.py` & `qianfan-0.3.8/qianfan/evaluation/opencompass_evaluator.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py` & `qianfan-0.3.8/qianfan/extensions/langchain/agents/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/extensions/openai/adapter.py` & `qianfan-0.3.8/qianfan/extensions/openai/adapter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/__init__.py` & `qianfan-0.3.8/qianfan/extensions/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py` & `qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_chat_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py` & `qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_settings.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py` & `qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_text_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py` & `qianfan-0.3.8/qianfan/extensions/semantic_kernel/connectors/qianfan_text_embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/fake_pyarrow_replacer.py` & `qianfan-0.3.8/qianfan/fake_pyarrow_replacer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/model/__init__.py` & `qianfan-0.3.8/qianfan/model/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/model/configs.py` & `qianfan-0.3.8/qianfan/model/configs.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/model/consts.py` & `qianfan-0.3.8/qianfan/model/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/model/model.py` & `qianfan-0.3.8/qianfan/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     """model name"""
     service: Optional["Service"] = None
     """model service"""
     task_id: Optional[str]
     """train tkas id"""
     job_id: Optional[str]
     """train job id"""
+    step: Optional[int] = None
+    """checkpoint step"""
 
     def __init__(
         self,
         id: Optional[str] = None,
         version_id: Optional[str] = None,
         task_id: Optional[str] = None,
         job_id: Optional[str] = None,
@@ -235,18 +237,24 @@
                 break
             else:
                 raise InvalidArgumentError("invalid train task job to publish model")
         # 发布模型
         self.model_name = (
             name if name != "" else f"m_{generate_letter_num_random_id(12)}"
         )
+        model_version_meta: Dict[str, Any] = {
+            "taskId": self.job_id,
+            "iterationId": self.task_id,
+        }
+        if self.step:
+            model_version_meta["step"] = self.step
         model_publish_resp = ResourceModel.publish(
             is_new=True,
             model_name=self.model_name,
-            version_meta={"taskId": self.job_id, "iterationId": self.task_id},
+            version_meta=model_version_meta,
             **kwargs,
         )
         self.id = model_publish_resp["result"]["modelIDStr"]
         self.old_id = model_publish_resp["result"]["modelId"]
 
         if self.id is None:
             raise InvalidArgumentError("model id not found")
```

### Comparing `qianfan-0.3.7.1/qianfan/resources/__init__.py` & `qianfan-0.3.8/qianfan/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/auth/iam.py` & `qianfan-0.3.8/qianfan/resources/auth/iam.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/auth/oauth.py` & `qianfan-0.3.8/qianfan/resources/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/console/charge.py` & `qianfan-0.3.8/qianfan/resources/console/charge.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/console/consts.py` & `qianfan-0.3.8/qianfan/resources/console/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,16 @@
 
 
 class TrainMode(str, Enum):
     SFT = "SFT"
     """对应 LLMFinetune"""
     PostPretrain = "PostPretrain"
     """PostPretrain """
+    DPO = "DPO"
+    """DPO"""
 
 
 class TrainParameterScale(str, Enum):
     FullFineTuning = "FullFineTuning"
     PromptTuning = "PromptTuning"
     LoRA = "LoRA"
```

### Comparing `qianfan-0.3.7.1/qianfan/resources/console/data.py` & `qianfan-0.3.8/qianfan/resources/console/data.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/console/finetune.py` & `qianfan-0.3.8/qianfan/resources/console/finetune.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,34 +228,37 @@
         @console_api_request
         def create_task(
             cls,
             job_id: str,
             params_scale: Union[str, console_consts.TrainParameterScale],
             hyper_params: Dict[str, Any],
             dataset_config: Dict[str, Any],
-            incrementTaskId: Optional[str] = None,
+            increment_task_id: Optional[str] = None,
+            increment_checkpoint_step: Optional[int] = None,
             **kwargs: Any,
         ) -> QfRequest:
             """
             create a fine-tuning task.
 
             This function create a fine-tuning task associated with a
             specific job.
 
             Parameters:
-            name (str):
-                The name of job.
-            model (str):
-                The identifier of the fine-tuning job to be stopped.
-                e.g. "ERNIE-Speed"
-            train_mode (Union[str, console_consts.TrainMode]):
-                The train mode of the fine-tuning job, including "SFT",
-                "PostPreTrain" and so on.
-            description (Optional[str]):
-                The description of the fine-tuning job.
+            job_id (str):
+                The identifier of the fine-tuning job.
+            params_scale (Union[str, console_consts.TrainParameterScale]):
+                The parameter scale of the fine-tuning task.
+            hyper_params (Dict[str, Any]):
+                The hyper-parameters of the fine-tuning task.
+            dataset_config (Dict[str, Any]):
+                The dataset config of the fine-tuning task.
+            increment_task_id (Optional[str]):
+                The task id of the increment task.
+            increment_checkpoint_step (Optional[int]):
+                The checkpoint step for the increment task.
             kwargs:
                 Additional keyword arguments that can be passed to customize
                 the request.
 
             Note:
             The `@console_api_request` decorator is applied to this method, enabling
             it to send the generated QfRequest and return a QfResponse to the user.
@@ -272,16 +275,18 @@
                     params_scale.value
                     if isinstance(params_scale, console_consts.TrainParameterScale)
                     else params_scale
                 ),
                 "hyperParameterConfig": hyper_params,
                 "datasetConfig": dataset_config,
             }
-            if incrementTaskId is not None:
-                req.json_body["incrementTaskId"] = incrementTaskId
+            if increment_task_id is not None:
+                req.json_body["incrementTaskId"] = increment_task_id
+                if increment_checkpoint_step is not None:
+                    req.json_body["incrementCheckpointStep"] = increment_checkpoint_step
             return req
 
         @classmethod
         @console_api_request
         def job_list(
             cls,
             train_model: Optional[Union[str, console_consts.TrainMode]] = None,
```

### Comparing `qianfan-0.3.7.1/qianfan/resources/console/model.py` & `qianfan-0.3.8/qianfan/resources/console/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,16 @@
         This function allows for the publishing of a trained model to a model
         repository.
 
         Parameters:
           is_new (bool):
             A boolean indicating whether this is a new model to be published.
           version_meta (Dict[str, Any]):
-            Metadata for the model being published.
+            Metadata for the model being published, including description, jobId,
+            taskId, step.
           model_name (Optional[str]):
             The name of the model to be published (required when `is_new` is True).
           model_id (Optional[str]):
             The ID of the model to be published (required when `is_new` is False).
           tags (Optional[List[str]]):
             A list of tags associated with the model (optional).
           kwargs (Any):
```

### Comparing `qianfan-0.3.7.1/qianfan/resources/console/prompt.py` & `qianfan-0.3.8/qianfan/resources/console/prompt.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/console/service.py` & `qianfan-0.3.8/qianfan/resources/console/service.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/console/utils.py` & `qianfan-0.3.8/qianfan/resources/console/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/http_client.py` & `qianfan-0.3.8/qianfan/resources/http_client.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/images/image2text.py` & `qianfan-0.3.8/qianfan/resources/images/image2text.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/images/text2image.py` & `qianfan-0.3.8/qianfan/resources/images/text2image.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/llm/base.py` & `qianfan-0.3.8/qianfan/resources/llm/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/llm/chat_completion.py` & `qianfan-0.3.8/qianfan/resources/llm/chat_completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/llm/completion.py` & `qianfan-0.3.8/qianfan/resources/llm/completion.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/llm/embedding.py` & `qianfan-0.3.8/qianfan/resources/llm/embedding.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/llm/plugin.py` & `qianfan-0.3.8/qianfan/resources/llm/plugin.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/rate_limiter.py` & `qianfan-0.3.8/qianfan/resources/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/requestor/base.py` & `qianfan-0.3.8/qianfan/resources/requestor/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,15 @@
                 try:
                     body = await response.json()
                 except json.JSONDecodeError:
                     raise errors.RequestError(
                         "Got invalid json response from server, body:"
                         f" {response.content}"
                     )
-                resp = self._parse_async_response(body, response)
+                resp = await self._parse_async_response(body, response)
                 resp.statistic["request_latency"] = time.perf_counter() - start
                 resp.request = QfRequest.from_aiohttp(response.request_info)
                 resp.request.json_body = copy.deepcopy(request.json_body)
                 if "X-Ratelimit-Limit-Requests" in resp.headers:
                     await self._rate_limiter.async_reset_once(
                         float(resp.headers["X-Ratelimit-Limit-Requests"])
                     )
@@ -301,15 +301,15 @@
         """
         self._check_error(body)
         qf_response = QfResponse(
             code=resp.status_code, headers=dict(resp.headers), body=body
         )
         return qf_response
 
-    def _parse_async_response(
+    async def _parse_async_response(
         self, body: Dict[str, Any], resp: aiohttp.ClientResponse
     ) -> QfResponse:
         """
         parse async response to QfResponse
         """
         self._check_error(body)
```

### Comparing `qianfan-0.3.7.1/qianfan/resources/requestor/console_requestor.py` & `qianfan-0.3.8/qianfan/resources/requestor/console_requestor.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/requestor/openapi_requestor.py` & `qianfan-0.3.8/qianfan/resources/requestor/openapi_requestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     Iterator,
     Optional,
     TypeVar,
     Union,
 )
 from urllib.parse import urlparse
 
+import aiohttp
+import requests
+
 import qianfan.errors as errors
 from qianfan.config import get_config
 from qianfan.consts import APIErrorCode, Consts
 from qianfan.resources.auth.iam import iam_sign
 from qianfan.resources.auth.oauth import Auth
 from qianfan.resources.requestor.base import (
     BaseAPIRequestor,
@@ -200,15 +203,15 @@
                         continue
                     raise
                 raise errors.RequestError(
                     f"got unexpected stream response from server: {body_str}"
                 )
             body_str = body_str[len(Consts.STREAM_RESPONSE_PREFIX) :]
             json_body = json.loads(body_str)
-            parsed = self._parse_async_response(json_body, resp)
+            parsed = await self._parse_async_response(json_body, resp)
             parsed.request = QfRequest.from_aiohttp(resp.request_info)
             parsed.request.json_body = copy.deepcopy(request.json_body)
             yield data_postprocess(parsed)
 
     def _check_error(self, body: Dict[str, Any]) -> None:
         """
         check whether error_code in response body
@@ -227,14 +230,34 @@
             if error_code in {
                 APIErrorCode.APITokenExpired.value,
                 APIErrorCode.APITokenInvalid.value,
             }:
                 raise errors.AccessTokenExpiredError
             raise errors.APIError(error_code, err_msg, req_id)
 
+    def _parse_response(
+        self, body: Dict[str, Any], resp: requests.Response
+    ) -> QfResponse:
+        try:
+            return super()._parse_response(body, resp)
+        except errors.APIError as e:
+            if e.error_code == APIErrorCode.TPMLimitReached.value:
+                self._token_limiter.clear()
+            raise e
+
+    async def _parse_async_response(
+        self, body: Dict[str, Any], resp: aiohttp.ClientResponse
+    ) -> QfResponse:
+        try:
+            return await super()._parse_async_response(body, resp)
+        except errors.APIError as e:
+            if e.error_code == APIErrorCode.TPMLimitReached.value:
+                await self._async_token_limiter.clear()
+            raise e
+
     def _get_token_count_from_body(self, body: Dict[str, Any]) -> int:
         token_count = 0
         messages = body.get("messages", None)
         prompt = body.get("prompt", None)
 
         if messages and prompt:
             err_msg = "messages and prompt exist simultaneously"
```

### Comparing `qianfan-0.3.7.1/qianfan/resources/token_limiter.py` & `qianfan-0.3.8/qianfan/resources/token_limiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,23 @@
                     next_minute_dead_interval = 60 - self._last_check_timestamp.second
                     time.sleep(next_minute_dead_interval)
 
             err_msg = "get token from token limiter failed"
             log_error(err_msg)
             raise RuntimeError(err_msg)
 
+    def clear(self) -> bool:
+        if self._is_closed():
+            return True
+
+        with self._lock:
+            self._token_current = 0
+
+        return True
+
     def compensate(self, compensation: int) -> None:
         """
         justify the remaining token count in limiter
         when receive a response from server
         """
 
         if self._lock.acquire(timeout=1):
@@ -256,14 +265,23 @@
                     next_minute_dead_interval = 60 - self._last_check_timestamp.second
                     await asyncio.sleep(next_minute_dead_interval)
 
             err_msg = "get token from token limiter failed"
             log_error(err_msg)
             raise RuntimeError(err_msg)
 
+    async def clear(self) -> bool:
+        if self._is_closed():
+            return True
+
+        async with self._get_internal_async_lock():
+            self._token_current = 0
+
+        return True
+
     async def compensate(self, compensation: int) -> None:
         """
         justify the remaining token count in limiter
         when receive a response from server
         """
 
         lock = self._get_internal_async_lock()
```

### Comparing `qianfan-0.3.7.1/qianfan/resources/tools/tokenizer.py` & `qianfan-0.3.8/qianfan/resources/tools/tokenizer.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/tools/utils.py` & `qianfan-0.3.8/qianfan/resources/tools/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/resources/typing.py` & `qianfan-0.3.8/qianfan/resources/typing.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/trainer/__init__.py` & `qianfan-0.3.8/qianfan/trainer/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/trainer/actions.py` & `qianfan-0.3.8/qianfan/trainer/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,18 +239,20 @@
             "dataset_bos": self.bos_path,
             "output": self.result,
         }
         return meta
 
     @classmethod
     def _load_from_dict(cls, meta: Dict[str, Any]) -> "LoadDataSetAction":
-        return cls(
+        action = cls(
             id=meta.get("id"),
             dataset=meta.get("ds_id") or meta.get("dataset_bos"),
         )
+        action.result = meta.get("output")
+        return action
 
     @classmethod
     def load(cls, b: bytes) -> "LoadDataSetAction":
         meta = cls.serialize_helper.deserialize(b)
         assert isinstance(meta, dict)
         return cls._load_from_dict(meta)
 
@@ -294,14 +296,18 @@
     """train task id"""
     job_id: Optional[str] = None
     """train job id"""
     train_type: Optional[str] = ""
     """train_type"""
     is_incr: bool = False
     """if it's incremental train or not"""
+    _last_task_id: Optional[str] = None
+    """last task id"""
+    _last_task_step: Optional[int] = None
+    """last task step"""
     train_config: Optional[TrainConfig] = None
     """train config"""
     train_mode: console_consts.TrainMode
     """train mode"""
     job_name: str = ""
     """train task name"""
     task_description: Optional[str] = None
@@ -310,26 +316,35 @@
     """train job description"""
     _input: Optional[Dict[str, Any]] = None
     """train input"""
     result: Optional[Dict[str, Any]] = None
     """"train result"""
     train_model_name: Optional[str] = None
     """real name to start training"""
+    task_status: Optional[str] = None
+    """train task status, e.g. `Running`"""
+    progress: Optional[int] = 0
+    """training progress 0-100"""
+    vdl_link: Optional[str] = None
+    """visualdl link"""
+    log_link: Optional[str] = None
+    """log link"""
 
     def __init__(
         self,
         train_mode: console_consts.TrainMode,
         train_type: Optional[str] = None,
         train_config: Optional[TrainConfig] = None,
         task_id: Optional[str] = None,
         job_id: Optional[str] = None,
         peft_type: Optional[PeftType] = None,
         job_name: Optional[str] = None,
         task_description: Optional[str] = None,
         job_description: Optional[str] = None,
+        task_step: Optional[int] = None,
         **kwargs: Any,
     ) -> None:
         """
 
         Parameters:
             train_mode (Optional[console_consts.TrainMode], optional):
                 train mode, e.g. `SFT`, `PostPretrain`. Defaults to None.
@@ -350,24 +365,29 @@
                 train task name. Defaults to None.
             task_description (Optional[str], optional):
                 train task description. Defaults to None.
             job_description (Optional[str], optional):
                 train job description. Defaults to None.
         """
         super().__init__(**kwargs)
-        self.task_id = task_id
+        # for persist
+        self._init_job_id = job_id
+        self._init_task_id = task_id
+        self._last_task_id = task_id
+        self._last_task_step = task_step
         self.job_id = job_id
         self.train_mode = train_mode
         self.train_model_name = train_type
-        if self.task_id is not None:
+        if self._last_task_id is not None:
             # if incremental train
-            pre_task_detail = api.FineTune.V2.task_detail(task_id=self.task_id)
+            pre_task_detail = api.FineTune.V2.task_detail(task_id=self._last_task_id)
             # 获取增量任务的训练model
             if pre_task_detail.get("result") is not None:
                 self.train_type = pre_task_detail["result"]["model"]
+                self.job_id = pre_task_detail.get("result", {}).get("jobId")
                 self.train_mode = train_mode
             self.is_incr = True
         else:
             if train_type is None:
                 raise InvalidArgumentError("train_type must be specified")
             # 从基础模型开始训练
             self.train_type = train_type
@@ -541,34 +561,39 @@
         if "packing" in hyper_params_dict:
             hyper_params_dict["Packing"] = hyper_params_dict.pop("packing")
         ds_config = input["datasets"]
         log_debug(f"train with ds_config: { ds_config}")
         log_debug(f"train with hyper_params: { hyper_params_dict}")
         if self.is_incr:
             # 增量训练
-            kwargs["incrementTaskId"] = self.task_id
-            log_info(f"train with incrementTaskId: { self.task_id}")
+            kwargs["increment_task_id"] = self._last_task_id
+            if self._last_task_step:
+                kwargs["increment_checkpoint_step"] = self._last_task_step
+            log_info(
+                f"train with incrementTaskId: { self._last_task_id} with step:"
+                f" { self._last_task_step}"
+            )
         assert self.train_config.peft_type is not None
         create_task_resp = api.FineTune.V2.create_task(
             job_id=self.job_id,
             params_scale=self.train_config.peft_type,
             hyper_params=hyper_params_dict,
             dataset_config=ds_config,
             **kwargs,
         )
         self.task_id = str(create_task_resp["result"]["taskId"])
         log_debug(f"[train_action] create {self.train_mode} train task: {self.task_id}")
 
         # 获取job状态，是否训练完成
-        train_metrics = self._wait_model_trained(**kwargs)
+        train_output = self._wait_model_trained(**kwargs)
         self.result = {
             **input,
             "task_id": self.task_id,
             "job_id": self.job_id,
-            **train_metrics,
+            **train_output,
         }
         assert self.result is not None
         return self.result
 
     def _wait_model_trained(self, **kwargs: Dict) -> Dict[str, Any]:
         if self.task_id is None:
             raise InvalidArgumentError("task_id must not be None")
@@ -576,19 +601,25 @@
         while True:
             task_status_resp = api.FineTune.V2.task_detail(
                 task_id=self.task_id,
                 **kwargs,
             )
             task_status_result = task_status_resp.get("result", {})
             task_status = task_status_result.get("runStatus")
+            # 更新任务状态
+            self.task_status = task_status
 
             self.action_event(ActionState.Running, "train running", task_status_resp)
             if task_status == console_consts.TrainStatus.Finish:
                 output["metrics"] = task_status_result.get("metrics", {})
+                output["checkpoints"] = task_status_result.get("checkpointList", [])
                 log_info(f"[train_action] training task metrics: {output['metrics']}")
+                log_info(
+                    f"[train_action] training task checkpoints: {output['checkpoints']}"
+                )
                 break
             elif task_status in [
                 console_consts.TrainStatus.Fail,
                 console_consts.TrainStatus.Stop,
             ]:
                 log_error(
                     "[train_action] training job"
@@ -598,29 +629,30 @@
                 raise InternalError(
                     f"[train_action]training job {self.job_id}/{self.task_id} has ended"
                     f" with status: {task_status}"
                 )
             elif task_status == console_consts.TrainStatus.Running:
                 job_progress_str = task_status_result.get("runProgress")
                 job_progress = int(job_progress_str[:-1])
+                self.progress = job_progress
                 log_prefix = (
                     "sft"
                     if self.train_mode == console_consts.TrainMode.SFT
                     else "postPretrain"
                 )
+                self.log_link = f"https://console.bce.baidu.com/qianfan/train/{log_prefix}/{self.job_id}/{self.task_id}/detail/traininglog"
+                self.vdl_link = task_status_result.get("vdlLink", "")
                 log_info(
                     "[train_action] training ..."
                     f" job_name:{self.job_name} current status: {task_status},"
                     f" {job_progress}% check train task log in"
-                    f" https://console.bce.baidu.com/qianfan/train/{log_prefix}/{self.job_id}/{self.task_id}/detail/traininglog"
+                    f" {self.log_link}"
                 )
                 if job_progress >= 50:
-                    log_info(
-                        f" check vdl report in {task_status_result.get('vdlLink')}"
-                    )
+                    log_info(f" check vdl report in {self.vdl_link}")
                 time.sleep(get_config().TRAIN_STATUS_POLLING_INTERVAL)
             else:
                 raise InternalError(
                     f"[train_action] job: {self.job_name} task:"
                     f" {self.job_id}/{self.task_id} get unknown status: {task_status}"
                 )
         log_info(
@@ -705,46 +737,59 @@
         return self.serialize_helper.serialize(self._action_dict())
 
     def _action_dict(self) -> Dict[str, Any]:
         meta = {
             "id": self.id,
             "type": TrainAction.__name__,
             "init_params": {
-                "job_id": self.job_id,
-                "task_id": self.task_id,
+                "job_id": self._init_job_id,
+                "task_id": self._init_task_id,
                 "train_mode": (
                     self.train_mode
                     if isinstance(self.train_mode, str)
                     else self.train_mode.value
                 ),
                 "train_type": self.train_type,
                 "train_config": (
                     self.train_config.dict() if self.train_config is not None else {}
                 ),
                 "is_incr": self.is_incr,
                 "job_name": self.job_name,
                 "task_description": self.task_description,
                 "job_description": self.job_description,
             },
+            "job_id": self.job_id if hasattr(self, "job_id") else None,
+            "task_id": self.task_id if hasattr(self, "task_id") else None,
+            "status": self.task_status,
+            "progress": self.progress,
+            "vdl_link": self.vdl_link,
+            "log_link": self.log_link,
             "input": self._input,
             "output": self.result,
         }
         return meta
 
     @classmethod
     def _load_from_dict(cls, meta: Dict[str, Any]) -> "TrainAction":
         params = meta.get("init_params", {})
         if "train_config" in params:
             params["train_config"] = TrainConfig(**params["train_config"])
         action = cls(
+            id=meta.get("id"),
             **params,
         )
+        action.job_id = meta.get("job_id")
+        action.task_id = meta.get("task_id")
         action.is_incr = params.pop("is_incr", False)
         action._input = meta.get("input")
         action.result = meta.get("output")
+        action.task_status = meta.get("status")
+        action.progress = meta.get("progress")
+        action.vdl_link = meta.get("vdl_link")
+        action.log_link = meta.get("log_link")
         return action
 
 
 class ModelPublishAction(BaseAction[Dict[str, Any], Dict[str, Any]]):
     """
     Class for Model publish action, Commonly used after `TrainAction`.
 
@@ -828,18 +873,14 @@
         self.model = Model(task_id=self.task_id, job_id=self.job_id)
         return self._exec(**kwargs)
 
     def _action_dict(self) -> Dict[str, Any]:
         meta: Dict[str, Any] = {
             "id": self.id,
             "type": ModelPublishAction.__name__,
-            "init_params": {
-                "task_id": self.task_id,
-                "job_id": self.job_id,
-            },
             "input": {
                 "task_id": self.task_id,
                 "job_id": self.job_id,
             },
         }
         if self.model:
             meta["model_version_id"] = self.model.version_id
@@ -851,14 +892,15 @@
 
         return meta
 
     @classmethod
     def _load_from_dict(cls, meta: Dict[str, Any]) -> "BaseAction":
         params = meta.get("init_params", {})
         action = cls(
+            id=meta.get("id"),
             **params,
         )
         action._input = meta.get("input")  # type: ignore
         action.result = meta.get("output")
         action.model = Model(version_id=meta.get("model_version_id"))
         action.model.auto_complete_info()
         return action
@@ -1015,21 +1057,41 @@
             }
         return meta
 
     @classmethod
     def _load_from_dict(cls, meta: Dict[str, Any]) -> "BaseAction":
         deploy_config = meta.get("init_params", {}).get("deploy_config", {})
         action = cls(
-            DeployConfig(**deploy_config),
+            id=meta.get("id"),
+            deploy_config=DeployConfig(**deploy_config),
         )
         action._input = meta.get("input")
         action.result = meta.get("output")
         return action
 
 
+class BatchInferAction(BaseAction[Dict[str, Any], Dict[str, Any]]):
+    """BatchInferAction
+    Action for batch inference.
+    Sample:
+    input:
+        ```
+        {'model_id': "am-xxxx", 'model_version_id': "amv-xxxx"}
+        ```
+    output:
+        ```
+        {'infer_res': InferenceResult ...}
+        ```
+    """
+
+    # batch_inference_manager: Optional[BatchInferenceManager] = None
+    """batch inference manager for batch infer models or services."""
+    dataset: Optional[Dataset] = None
+
+
 class EvaluateAction(BaseAction[Dict[str, Any], Dict[str, Any]]):
     """EvaluateAction
     Action for evaluate models or services.
     Sample:
     input:
         ```
         {'model_id': "am-xxxx", 'model_version_id': "amv-xxxx"}
```

### Comparing `qianfan-0.3.7.1/qianfan/trainer/base.py` & `qianfan-0.3.8/qianfan/trainer/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/trainer/configs.py` & `qianfan-0.3.8/qianfan/trainer/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,34 +339,34 @@
     #     return TrainConfig
 
     TrainConfig = new_train_config_type  # type: ignore
     return TrainConfig
 
 
 def _update_default_config(model_info_list: List[Dict]) -> Dict:
-    model_info_mapping: Dict[str, Any] = {
+    train_mode_model_info_mappings: Dict[str, Any] = {
         console_consts.TrainMode.PostPretrain: {},
         console_consts.TrainMode.SFT: {},
+        console_consts.TrainMode.DPO: {},
     }
     for info in model_info_list:
         model = info["model"]
         for train_mode_info in info["supportTrainMode"]:
             train_mode = train_mode_info.get("trainMode")
-            if not model_info_mapping[train_mode].get(model, None):
-                model_info_mapping[train_mode][model] = {}
+            current = train_mode_model_info_mappings.get(train_mode, {})
+            if not current.get(model, None):
+                current[model] = {}
             for param_scale in train_mode_info["supportParameterScale"]:
                 default_fields = {}
                 param_scale_peft = param_scale["parameterScale"]
                 for params in param_scale["supportHyperParameterConfig"]:
                     field_name = camel_to_snake(params["key"])
                     default_fields[field_name] = params["default"]
-                model_info_mapping[train_mode][model][param_scale_peft] = TrainConfig(
-                    **default_fields
-                )
-    return model_info_mapping
+                current[model][param_scale_peft] = TrainConfig(**default_fields)
+    return train_mode_model_info_mappings
 
 
 def _parse_model_info_list(
     model_info_list: List[Dict], train_mode: console_consts.TrainMode
 ) -> Dict[str, ModelInfo]:
     """
     parse the supported fine-tune info list, update the train_limit
```

### Comparing `qianfan-0.3.7.1/qianfan/trainer/consts.py` & `qianfan-0.3.8/qianfan/trainer/consts.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/trainer/event.py` & `qianfan-0.3.8/qianfan/trainer/event.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/trainer/finetune.py` & `qianfan-0.3.8/qianfan/trainer/finetune.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, cast
 
 from qianfan.common.persister.persist import g_persister
-from qianfan.config import get_config
+from qianfan.config import encoding, get_config
 from qianfan.errors import InvalidArgumentError
 from qianfan.evaluation.evaluator import Evaluator
 from qianfan.model.configs import DeployConfig
 from qianfan.resources.console import consts as console_consts
 from qianfan.trainer.actions import (
     DeployAction,
     EvaluateAction,
@@ -216,14 +216,15 @@
             elif isinstance(ac, TrainAction):
                 self.train_action = ac
             elif isinstance(ac, ModelPublishAction):
                 self.model_publish = ac
             elif isinstance(ac, DeployAction):
                 self.deploy_action = ac
         self.ppls = [ppl]
+        self.result = [None]
         return self
 
     def run(self, **kwargs: Any) -> Trainer:
         """
         run a pipeline to run the fine-tune process.
 
         Parameters:
@@ -270,15 +271,18 @@
         action_name = action.__class__.__name__
         return action_mapping.get(action_name, {}).get(
             action.state, TrainStatus.Unknown
         )
 
     @property
     def output(self) -> Any:
-        return self.result[0]
+        if self.result[0]:
+            return self.result[0]
+        else:
+            return self.info()["actions"][-1]["output"]
 
     @classmethod
     def train_type_list(cls) -> Dict[str, ModelInfo]:
         return ModelInfoMapping
 
     @staticmethod
     def list() -> List["Trainer"]:
@@ -294,27 +298,42 @@
                     trainer_inst = Finetune(pipeline=task_ppl)
                     trainer_list.append(trainer_inst)
             except Exception as e:
                 raise e
         return trainer_list
 
     @staticmethod
-    def load(id: str) -> "Trainer":
-        task_ppl = g_persister.load(id, Pipeline)
+    def load(id: Optional[str] = None, file: Optional[str] = None) -> "Trainer":
+        if file is not None:
+            with open(file=file, mode="rb") as f:
+                task_ppl = Pipeline.load(f.read())
+        elif id:
+            task_ppl = cast(Pipeline, g_persister.load(id, Pipeline))
+        else:
+            raise InvalidArgumentError("invalid id or file to load")
         assert isinstance(task_ppl, Pipeline)
         if (
             task_ppl._case_init_params is not None
             and task_ppl._case_init_params.get("case_type") == Finetune.__name__
         ):
             trainer_inst = Finetune(pipeline=task_ppl)
             return trainer_inst
+
         raise InvalidArgumentError("pipeline not found {id} to load")
 
+    def save(self, file: Optional[str] = None) -> None:
+        if file:
+            with open(file=file, mode="w", encoding=encoding()) as f:
+                f.write(self.ppls[0].persist().decode(encoding=encoding()))
+        else:
+            g_persister.save(self.ppls[0])
+
     def info(self) -> Dict:
-        return self.ppls[0]._action_dict()
+        tmp = cast(Pipeline, g_persister.load(self.id, Pipeline))
+        return tmp._action_dict()
 
     @property
     def id(self) -> str:
         return self.ppls[0].id
 
 
 LLMFinetune = Finetune
```

### Comparing `qianfan-0.3.7.1/qianfan/trainer/pipeline.py` & `qianfan-0.3.8/qianfan/trainer/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
+import os
 import threading
+import time
 from typing import Any, Dict, Iterator, List, Optional, Sequence, Union
 
 from qianfan.common.persister.persist import g_persister
 from qianfan.errors import InternalError, InvalidArgumentError
 from qianfan.trainer.actions import (
     DeployAction,
     LoadDataSetAction,
@@ -86,15 +88,38 @@
         """
         Parameters:
             input: Optional[Dict[str, Any]] input of the pipeline.
             kwargs: additional keyword arguments.
         Return:
             Dict[str, Any]: The output of the pipeline.
         """
-        return self.exec_from(input, 0, **kwargs)
+        res: List[Any] = [{}]
+
+        def _exec_helper(res: List[Any]) -> None:
+            if len(res) == 0:
+                return
+            try:
+                res[0] = self.exec_from(input, 0, **kwargs)
+            except Exception as e:
+                res[0] = e
+
+        t = threading.Thread(target=_exec_helper, args=[res])
+        t.start()
+
+        while True:
+            g_persister.save(self)
+            if isinstance(res[0], Exception):
+                g_persister.save(self)
+                raise res[0]
+            if self._stop:
+                g_persister.save(self)
+                break
+            time.sleep(10)
+
+        return res[0]
 
     def exec_from(
         self,
         input: Optional[Dict[str, Any]] = None,
         start: Optional[Union[int, str]] = 0,
         **kwargs: Dict,
     ) -> Dict[str, Any]:
@@ -102,14 +127,15 @@
             start_idx = self.seq.index(start)
         elif isinstance(start, int):
             start_idx = start
         else:
             raise InvalidArgumentError(
                 "pipeline start must be index of sequence or key of action"
             )
+        self._stop = False
         g_persister.save(self)
         output: Dict[str, Any] = copy.deepcopy(input) if input is not None else {}
         for i, k in enumerate(self.seq):
             if self._stop:
                 break
             if i < start_idx:
                 continue
@@ -126,14 +152,15 @@
                     if isinstance(err, BaseException):
                         raise err
                     else:
                         raise InternalError(f"[get internal error: {err}")
 
         for next in self.post_actions:
             next.exec(copy.deepcopy(output), **kwargs)
+        self._stop = True
         return output
 
     def __getitem__(self, key: str) -> Optional[BaseAction]:
         """
         get action by key, which is the action id.
 
         Args:
@@ -196,26 +223,22 @@
 
     def _action_dict(self) -> Dict:
         meta: Dict[str, Any] = {
             "id": self.id,
             "current_action": self.current_action,
             # "output": self._last_output,
         }
-        # print("output:", self._last_output)
-        if self.process_id:
-            meta["process_id"] = self.process_id
+        meta["process_id"] = self.process_id if self.process_id else os.getpid()
         actions = []
         for action_id in self.seq:
             action_meta = self.actions[action_id]._action_dict()
             actions.append(action_meta)
         meta["actions"] = actions
         if self._case_init_params:
             meta["case_init_params"] = self._case_init_params
-        if self.process:
-            meta["process"] = self.process_id
         return meta
 
     @classmethod
     def load(cls, b: bytes) -> "Pipeline":
         meta = cls.serialize_helper.deserialize(b)
         assert isinstance(meta, dict)
         return cls._load_from_dict(meta)
@@ -235,14 +258,15 @@
             actions.append(action_obj)
         ppl = Pipeline(
             id=meta.get("id"),
             actions=actions,
             case_init_params=meta.get("case_init_params"),
         )
         assert isinstance(meta.get("current_action", ""), str)
+        ppl.process_id = meta.get("process_id", "")
         ppl.current_action = meta.get("current_action", "")
         return ppl
 
     @staticmethod
     def load_action(action_type: str, meta: Dict[str, Any]) -> Optional[BaseAction]:
         if action_type == TrainAction.__name__:
             return TrainAction._load_from_dict(meta)
```

### Comparing `qianfan-0.3.7.1/qianfan/trainer/post_pretrain.py` & `qianfan-0.3.8/qianfan/trainer/post_pretrain.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, cast
 
 from qianfan.common.persister.persist import g_persister
-from qianfan.config import get_config
+from qianfan.config import encoding, get_config
 from qianfan.dataset import Dataset
 from qianfan.errors import InvalidArgumentError
 from qianfan.resources.console import consts as console_consts
 from qianfan.trainer.actions import (
     LoadDataSetAction,
     TrainAction,
     action_mapping,
@@ -211,25 +211,38 @@
                     trainer_list.append(trainer_inst)
             except Exception as e:
                 raise e
 
         return trainer_list
 
     @staticmethod
-    def load(id: str) -> "Trainer":
-        task_ppl = g_persister.load(id, Pipeline)
+    def load(id: Optional[str] = None, file: Optional[str] = None) -> "Trainer":
+        if file is not None:
+            with open(file=file, mode="rb") as f:
+                task_ppl = Pipeline.load(f.read())
+        elif id:
+            task_ppl = cast(Pipeline, g_persister.load(id, Pipeline))
+        else:
+            raise InvalidArgumentError("invalid id or file to load")
         assert isinstance(task_ppl, Pipeline)
         if (
             task_ppl._case_init_params is not None
             and task_ppl._case_init_params.get("case_type") == PostPreTrain.__name__
         ):
             trainer_inst = PostPreTrain(pipeline=task_ppl)
             return trainer_inst
 
         raise InvalidArgumentError("pipeline not found {id} to load")
 
+    def save(self, file: Optional[str] = None) -> None:
+        if file:
+            with open(file=file, mode="w", encoding=encoding()) as f:
+                f.write(self.ppls[0].persist().decode(encoding=encoding()))
+        else:
+            g_persister.save(self.ppls[0])
+
     def info(self) -> Dict:
         return self.ppls[0]._action_dict()
 
     @property
     def id(self) -> str:
         return self.ppls[0].id
```

### Comparing `qianfan-0.3.7.1/qianfan/trainer/ppl.yaml` & `qianfan-0.3.8/qianfan/trainer/ppl.yaml`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/trainer/trainer.py` & `qianfan-0.3.8/qianfan/trainer/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,15 +141,19 @@
     @staticmethod
     @abstractmethod
     def list() -> List["Trainer"]:
         ...
 
     @staticmethod
     @abstractmethod
-    def load(id: str) -> "Trainer":
+    def load(id: Optional[str] = None, file: Optional[str] = None) -> "Trainer":
+        ...
+
+    @abstractmethod
+    def save(self, file: Optional[str] = None) -> None:
         ...
 
     def info(self) -> Dict:
         """
         Get the information of trainer.
         Returns:
             Dict: The dict of trainer info.
```

### Comparing `qianfan-0.3.7.1/qianfan/utils/__init__.py` & `qianfan-0.3.8/qianfan/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/utils/bos_uploader.py` & `qianfan-0.3.8/qianfan/utils/bos_uploader.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/utils/cache/__init__.py` & `qianfan-0.3.8/qianfan/utils/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/utils/cache/base.py` & `qianfan-0.3.8/qianfan/utils/cache/base.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/__init__.py` & `qianfan-0.3.8/qianfan/utils/fake_pyarrow/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/compute.py` & `qianfan-0.3.8/qianfan/utils/fake_pyarrow/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-fake pyarrow compute module
+fake pyarrow functions
 """
 
 from typing import Any
 
 
-def max(*args: Any, **kwargs: Any) -> Any:
+def concat_tables(*args: Any, **kwargs: Any) -> Any:
+    # do nothing
+    ...
+
+
+def memory_map(*args: Any, **kwargs: Any) -> Any:
     # do nothing
     ...
```

### Comparing `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/functions.py` & `qianfan-0.3.8/qianfan/utils/fake_pyarrow/ipc.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,21 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-fake pyarrow functions
+fake pyarrow ipc module
 """
 
 from typing import Any
 
 
-def concat_tables(*args: Any, **kwargs: Any) -> Any:
+def open_stream(*args: Any, **kwargs: Any) -> Any:
     # do nothing
     ...
 
 
-def memory_map(*args: Any, **kwargs: Any) -> Any:
+def new_stream(*args: Any, **kwargs: Any) -> Any:
+    # do nothing
+    ...
+
+
+class RecordBatchStreamWriter:
     # do nothing
     ...
```

### Comparing `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/ipc.py` & `qianfan-0.3.8/qianfan/utils/fake_pyarrow/table.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,26 +8,31 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
-fake pyarrow ipc module
+fake pyarrow.Table
 """
 
 from typing import Any
 
 
-def open_stream(*args: Any, **kwargs: Any) -> Any:
-    # do nothing
-    ...
+class Table:
+    """mock pyarrow.Table"""
 
+    @classmethod
+    def from_pydict(cls, *args: Any, **kwargs: Any) -> Any:
+        # do nothing
+        ...
+
+    @classmethod
+    def from_pylist(cls, *args: Any, **kwargs: Any) -> Any:
+        # do nothing
+        ...
 
-def new_stream(*args: Any, **kwargs: Any) -> Any:
-    # do nothing
-    ...
 
+class ChunkedArray:
+    """mock pyarrow.ChunkedArray"""
 
-class RecordBatchStreamWriter:
-    # do nothing
     ...
```

### Comparing `qianfan-0.3.7.1/qianfan/utils/fake_pyarrow/table.py` & `qianfan-0.3.8/qianfan/dataset/data_insight/data_insight_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,23 @@
-# Copyright (c) 2023 Baidu, Inc. All Rights Reserved.
+# Copyright (c) 2024 Baidu, Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """
-fake pyarrow.Table
+utilities of data insight
 """
+from typing import Any, Callable, Dict, Generator, List
 
-from typing import Any
-
-
-class Table:
-    """mock pyarrow.Table"""
-
-    @classmethod
-    def from_pydict(cls, *args: Any, **kwargs: Any) -> Any:
-        # do nothing
-        ...
-
-    @classmethod
-    def from_pylist(cls, *args: Any, **kwargs: Any) -> Any:
-        # do nothing
-        ...
-
-
-class ChunkedArray:
-    """mock pyarrow.ChunkedArray"""
 
-    ...
+def _get_generator(iteration_list: List[Dict[str, Any]], func: Callable) -> Generator:
+    for single in iteration_list:
+        yield func(single)
```

### Comparing `qianfan-0.3.7.1/qianfan/utils/helper.py` & `qianfan-0.3.8/qianfan/utils/helper.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/utils/logging.py` & `qianfan-0.3.8/qianfan/utils/logging.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/utils/pydantic/__init__.py` & `qianfan-0.3.8/qianfan/utils/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/utils/utils.py` & `qianfan-0.3.8/qianfan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/qianfan/version.py` & `qianfan-0.3.8/qianfan/version.py`

 * *Files identical despite different names*

### Comparing `qianfan-0.3.7.1/PKG-INFO` & `qianfan-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qianfan
-Version: 0.3.7.1
+Version: 0.3.8
 Summary: 文心千帆大模型平台 Python SDK
 Home-page: https://cloud.baidu.com/product/wenxinworkshop
 License: Apache-2.0
 Keywords: baidu,qianfan
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -41,14 +41,15 @@
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) ; extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension"
 Requires-Dist: python-dotenv (<=0.21.1) ; python_version < "3.8"
 Requires-Dist: python-dotenv (>=1.0) ; python_version >= "3.8"
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.24)
 Requires-Dist: rich (>=13.0.0)
 Requires-Dist: sentencepiece ; extra == "local-data-clean" or extra == "extension"
+Requires-Dist: tabulate ; extra == "dataset-base" or extra == "langchain" or extra == "local-data-clean" or extra == "openai" or extra == "extension"
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: torch (<=1.13.1) ; (python_version < "3.8") and (extra == "local-data-clean" or extra == "extension")
 Requires-Dist: torch ; (python_version >= "3.8") and (extra == "local-data-clean" or extra == "extension")
 Requires-Dist: typer (>=0.9.0)
 Requires-Dist: typing-extensions (>=4.0.0) ; python_full_version <= "3.10.0"
 Requires-Dist: uvicorn ; extra == "openai" or extra == "extension"
 Project-URL: Documentation, https://qianfan.readthedocs.io/en/stable/README.html
```

