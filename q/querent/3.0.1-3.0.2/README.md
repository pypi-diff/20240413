# Comparing `tmp/querent-3.0.1.tar.gz` & `tmp/querent-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querent-3.0.1.tar", last modified: Sat Apr  6 14:19:49 2024, max compression
+gzip compressed data, was "querent-3.0.2.tar", last modified: Sat Apr 13 07:50:58 2024, max compression
```

## Comparing `querent-3.0.1.tar` & `querent-3.0.2.tar`

### file list

```diff
@@ -1,267 +1,267 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.556272 querent-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-06 14:13:26.000000 querent-3.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)    17135 2024-04-06 14:19:49.556272 querent-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-06 14:13:26.000000 querent-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.476271 querent-3.0.1/querent/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-06 14:13:26.000000 querent-3.0.1/querent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.480271 querent-3.0.1/querent/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-06 14:13:26.000000 querent-3.0.1/querent/callback/event_callback_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-06 14:13:26.000000 querent-3.0.1/querent/callback/event_callback_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.484271 querent-3.0.1/querent/channel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-06 14:13:26.000000 querent-3.0.1/querent/channel/channel_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.484271 querent-3.0.1/querent/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.488271 querent-3.0.1/querent/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.488271 querent-3.0.1/querent/collectors/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/aws/aws_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.488271 querent-3.0.1/querent/collectors/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/azure/azure_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/collector_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/collector_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/collector_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/collector_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.488271 querent-3.0.1/querent/collectors/drive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/drive/google_drive_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/dropbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/dropbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/dropbox/dropbox_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/email/email_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/email/imap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/fs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/fs/fs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/gcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/gcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/gcs/gcs_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.492271 querent-3.0.1/querent/collectors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/github/github_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/collectors/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/jira/jira_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/collectors/news/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/news/news_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/collectors/slack/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/slack/slack_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/collectors/webscaper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/webscaper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-06 14:13:26.000000 querent-3.0.1/querent/collectors/webscaper/web_scraper_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/common_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.496271 querent-3.0.1/querent/common/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/errors/metric_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/common/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/collected_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/collector_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/engine_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/file_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/ingested_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/ingested_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/ingested_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/ingested_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/querent_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/querent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/resource_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/types/workflow_config_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-06 14:13:26.000000 querent-3.0.1/querent/common/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/config/collector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/collector/collector_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/config/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/core/gpt_llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/core/llm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/core/opensource_llm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.504271 querent-3.0.1/querent/config/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/engine/engine_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/graph_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/ingestor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/ingestor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/ingestor/ingestor_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/logger/logger_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/metric/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/resource/resource_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/config/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-06 14:13:26.000000 querent-3.0.1/querent/config/workflow/workflow_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.508272 querent-3.0.1/querent/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.512272 querent-3.0.1/querent/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/bert_ner_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/fixed_entities_set_opensourcellm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16808 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    21403 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/gpt_llm_gpt_ner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-06 14:13:26.000000 querent-3.0.1/querent/core/transformers/relationship_extraction_llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.512272 querent-3.0.1/querent/dal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/dal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.512272 querent-3.0.1/querent/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/gnn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.516271 querent-3.0.1/querent/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/graph_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/shacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-06 14:13:26.000000 querent-3.0.1/querent/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.516271 querent-3.0.1/querent/ingestors/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.516271 querent-3.0.1/querent/ingestors/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/audio/audio_ingestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/base_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/code/code_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/csv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/csv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/csv/csv_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/doc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/doc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/doc/doc_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/email/email_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/email/email_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/github/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/github/github_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.520272 querent-3.0.1/querent/ingestors/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/html/html_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/images/image_ingestor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/ingestor_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/ingestor_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/json/json_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/pdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/pdfs/pdf_ingestor_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/ppt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/ppt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/ppt/ppt_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/texts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/texts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/texts/text_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/video/video_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.524272 querent-3.0.1/querent/ingestors/xlsx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/xlsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/xlsx/xlsx_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.528272 querent-3.0.1/querent/ingestors/xml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-06 14:13:26.000000 querent-3.0.1/querent/ingestors/xml/xml_ingestor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.528272 querent-3.0.1/querent/insights/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.528272 querent-3.0.1/querent/kg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.532272 querent-3.0.1/querent/kg/ner_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/attn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/contextual_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/dependency_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/filter_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/fixed_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/fixed_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/ner_helperfunctions/ner_llm_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/querent_kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.536272 querent-3.0.1/querent/kg/rel_helperfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/contextual_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/embedding_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/filter_semantic_triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/fixed_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/openai_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/openllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/questionanswer_llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/rag_retriever.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/rel_normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-06 14:13:26.000000 querent-3.0.1/querent/kg/rel_helperfunctions/triple_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.544272 querent-3.0.1/querent/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/custom_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-06 14:13:26.000000 querent-3.0.1/querent/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.548272 querent-3.0.1/querent/metric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.548272 querent-3.0.1/querent/metric/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/adapters/promethus_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/base_metric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/metric_logging_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-06 14:13:26.000000 querent-3.0.1/querent/metric/metric_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.548272 querent-3.0.1/querent/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-06 14:13:26.000000 querent-3.0.1/querent/processors/async_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-06 14:13:26.000000 querent-3.0.1/querent/processors/text_cleanup_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-06 14:13:26.000000 querent-3.0.1/querent/processors/text_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.552272 querent-3.0.1/querent/querent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/querent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/resource_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/querent/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.552272 querent-3.0.1/querent/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.552272 querent-3.0.1/querent/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/gcs_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/milvus_vectorevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/neo4j_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/postgres_graphevent_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-06 14:13:26.000000 querent-3.0.1/querent/storage/s3-data-management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.552272 querent-3.0.1/querent/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-06 14:13:26.000000 querent-3.0.1/querent/tools/web_page_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.556272 querent-3.0.1/querent/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:13:26.000000 querent-3.0.1/querent/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-06 14:13:26.000000 querent-3.0.1/querent/utils/webpage_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.556272 querent-3.0.1/querent/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 14:13:26.000000 querent-3.0.1/querent/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-06 14:13:26.000000 querent-3.0.1/querent/workflow/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-06 14:13:26.000000 querent-3.0.1/querent/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:19:49.556272 querent-3.0.1/querent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17135 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 14:19:49.000000 querent-3.0.1/querent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 14:19:49.556272 querent-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-06 14:13:26.000000 querent-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.845642 querent-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-13 07:45:05.000000 querent-3.0.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-13 07:50:58.845642 querent-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-04-13 07:45:05.000000 querent-3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.773641 querent-3.0.2/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-13 07:45:05.000000 querent-3.0.2/querent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.773641 querent-3.0.2/querent/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-13 07:45:05.000000 querent-3.0.2/querent/callback/event_callback_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-13 07:45:05.000000 querent-3.0.2/querent/callback/event_callback_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-13 07:45:05.000000 querent-3.0.2/querent/channel/channel_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/collectors/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/aws/aws_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.777641 querent-3.0.2/querent/collectors/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/azure/azure_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/collector_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/collector_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/collector_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/collector_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/drive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/drive/google_drive_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/dropbox/dropbox_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/email/email_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/email/imap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/fs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/fs/fs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/gcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/gcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/gcs/gcs_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.781641 querent-3.0.2/querent/collectors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/github/github_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.785641 querent-3.0.2/querent/collectors/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/jira/jira_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.785641 querent-3.0.2/querent/collectors/news/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/news/news_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.785641 querent-3.0.2/querent/collectors/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/slack/slack_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.785641 querent-3.0.2/querent/collectors/webscaper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/webscaper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-13 07:45:05.000000 querent-3.0.2/querent/collectors/webscaper/web_scraper_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.789641 querent-3.0.2/querent/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/common_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.789641 querent-3.0.2/querent/common/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/errors/metric_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.793641 querent-3.0.2/querent/common/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/collected_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/collector_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/engine_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/file_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/ingested_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/ingested_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/ingested_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/ingested_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/querent_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/querent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/resource_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/types/workflow_config_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-13 07:45:05.000000 querent-3.0.2/querent/common/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.793641 querent-3.0.2/querent/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.797641 querent-3.0.2/querent/config/collector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/collector/collector_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.797641 querent-3.0.2/querent/config/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/core/gpt_llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/core/llm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/core/opensource_llm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.797641 querent-3.0.2/querent/config/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/engine/engine_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/graph_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.797641 querent-3.0.2/querent/config/ingestor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/ingestor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/ingestor/ingestor_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/config/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/logger/logger_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/config/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/metric/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/config/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/resource/resource_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/config/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-13 07:45:05.000000 querent-3.0.2/querent/config/workflow/workflow_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.801641 querent-3.0.2/querent/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.805641 querent-3.0.2/querent/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13746 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/bert_ner_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/fixed_entities_set_opensourcellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16808 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21403 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/gpt_llm_gpt_ner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-04-13 07:45:05.000000 querent-3.0.2/querent/core/transformers/relationship_extraction_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.805641 querent-3.0.2/querent/dal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/dal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.805641 querent-3.0.2/querent/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/gnn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.809641 querent-3.0.2/querent/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/graph_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/shacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-13 07:45:05.000000 querent-3.0.2/querent/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/audio/audio_ingestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/base_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4538 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/code/code_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/csv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/csv/csv_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.813641 querent-3.0.2/querent/ingestors/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/doc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/doc/doc_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/email/email_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/email/email_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/github/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/github/github_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/html/html_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/images/image_ingestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/ingestor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/ingestor_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/json/json_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.817641 querent-3.0.2/querent/ingestors/pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/pdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/pdfs/pdf_ingestor_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/ppt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/ppt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/ppt/ppt_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/texts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/texts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/texts/text_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/video/video_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/xlsx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/xlsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/xlsx/xlsx_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/ingestors/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-13 07:45:05.000000 querent-3.0.2/querent/ingestors/xml/xml_ingestor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/insights/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/insights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.821642 querent-3.0.2/querent/kg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.825641 querent-3.0.2/querent/kg/ner_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/attn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/contextual_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/dependency_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/filter_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6118 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/fixed_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/fixed_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/ner_helperfunctions/ner_llm_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/querent_kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.829642 querent-3.0.2/querent/kg/rel_helperfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/contextual_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/embedding_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/filter_semantic_triples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/fixed_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/opeai_ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/openai_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/openllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/questionanswer_llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/rag_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/rel_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-13 07:45:05.000000 querent-3.0.2/querent/kg/rel_helperfunctions/triple_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.833642 querent-3.0.2/querent/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/custom_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-13 07:45:05.000000 querent-3.0.2/querent/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.833642 querent-3.0.2/querent/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.837642 querent-3.0.2/querent/metric/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/adapters/promethus_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/base_metric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/metric_logging_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-13 07:45:05.000000 querent-3.0.2/querent/metric/metric_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.837642 querent-3.0.2/querent/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 07:45:05.000000 querent-3.0.2/querent/processors/async_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-13 07:45:05.000000 querent-3.0.2/querent/processors/text_cleanup_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-13 07:45:05.000000 querent-3.0.2/querent/processors/text_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.837642 querent-3.0.2/querent/querent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/querent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/resource_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/querent/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.837642 querent-3.0.2/querent/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.841642 querent-3.0.2/querent/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/gcs_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/milvus_vectorevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/neo4j_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/postgres_graphevent_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-13 07:45:05.000000 querent-3.0.2/querent/storage/s3-data-management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.841642 querent-3.0.2/querent/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10882 2024-04-13 07:45:05.000000 querent-3.0.2/querent/tools/web_page_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.841642 querent-3.0.2/querent/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 07:45:05.000000 querent-3.0.2/querent/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-13 07:45:05.000000 querent-3.0.2/querent/utils/webpage_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.845642 querent-3.0.2/querent/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 07:45:05.000000 querent-3.0.2/querent/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-13 07:45:05.000000 querent-3.0.2/querent/workflow/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-13 07:45:05.000000 querent-3.0.2/querent/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 07:50:58.845642 querent-3.0.2/querent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-13 07:50:58.000000 querent-3.0.2/querent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 07:50:58.845642 querent-3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-13 07:45:05.000000 querent-3.0.2/setup.py
```

### Comparing `querent-3.0.1/LICENCE` & `querent-3.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/PKG-INFO` & `querent-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.1
+Version: 3.0.2
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -57,15 +57,15 @@
 Requires-Dist: jsonschema==4.17.3
 Requires-Dist: kombu==5.2.4
 Requires-Dist: llama_cpp_python==0.2.15
 Requires-Dist: lxml==4.9.2
 Requires-Dist: newspaper3k==0.2.8
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.24.3
-Requires-Dist: Pillow==10.0.1
+Requires-Dist: Pillow==10.3.0
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: PyJWT==2.4.0
 Requires-Dist: pytest==7.3.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: redis==5.0.3
 Requires-Dist: regex==2023.5.5
 Requires-Dist: sentence-transformers==2.2.2
@@ -97,15 +97,14 @@
 Requires-Dist: azure-storage-blob==12.19.0
 Requires-Dist: moviepy==1.0.3
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: dropbox==11.36.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: google-api-python-client==2.105.0
 Requires-Dist: requests_html==0.10.0
-Requires-Dist: rapidocr-onnxruntime==1.3.9
 Requires-Dist: pybase64==1.3.1
 Requires-Dist: pdfminer==20191125
 Requires-Dist: unidecode==1.3.7
 Requires-Dist: psutil==5.9.8
 Requires-Dist: langchain-community==0.0.25
 Requires-Dist: langchain==0.1.11
 Requires-Dist: openai==1.13.3
```

### Comparing `querent-3.0.1/README.md` & `querent-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/__init__.py` & `querent-3.0.2/querent/__init__.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/callback/event_callback_dispatcher.py` & `querent-3.0.2/querent/callback/event_callback_dispatcher.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/callback/event_callback_interface.py` & `querent-3.0.2/querent/callback/event_callback_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/channel/channel_interface.py` & `querent-3.0.2/querent/channel/channel_interface.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/aws/aws_collector.py` & `querent-3.0.2/querent/collectors/aws/aws_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/azure/azure_collector.py` & `querent-3.0.2/querent/collectors/azure/azure_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/collector_errors.py` & `querent-3.0.2/querent/collectors/collector_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/collector_factory.py` & `querent-3.0.2/querent/collectors/collector_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/collector_resolver.py` & `querent-3.0.2/querent/collectors/collector_resolver.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/drive/google_drive_collector.py` & `querent-3.0.2/querent/collectors/drive/google_drive_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/dropbox/dropbox_collector.py` & `querent-3.0.2/querent/collectors/dropbox/dropbox_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/email/email_collector.py` & `querent-3.0.2/querent/collectors/email/email_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/email/imap.py` & `querent-3.0.2/querent/collectors/email/imap.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/fs/fs_collector.py` & `querent-3.0.2/querent/collectors/fs/fs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/gcs/gcs_collector.py` & `querent-3.0.2/querent/collectors/gcs/gcs_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/github/github_collector.py` & `querent-3.0.2/querent/collectors/github/github_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/jira/jira_collector.py` & `querent-3.0.2/querent/collectors/jira/jira_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/news/news_collector.py` & `querent-3.0.2/querent/collectors/news/news_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/slack/slack_collector.py` & `querent-3.0.2/querent/collectors/slack/slack_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/collectors/webscaper/web_scraper_collector.py` & `querent-3.0.2/querent/collectors/webscaper/web_scraper_collector.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/common_errors.py` & `querent-3.0.2/querent/common/common_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/errors/metric_errors.py` & `querent-3.0.2/querent/common/errors/metric_errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/types/collected_bytes.py` & `querent-3.0.2/querent/common/types/collected_bytes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/types/file_buffer.py` & `querent-3.0.2/querent/common/types/file_buffer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/types/ingested_code.py` & `querent-3.0.2/querent/common/types/ingested_code.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/types/ingested_images.py` & `querent-3.0.2/querent/common/types/ingested_images.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/types/ingested_messages.py` & `querent-3.0.2/querent/common/types/ingested_messages.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/types/ingested_tokens.py` & `querent-3.0.2/querent/common/types/ingested_tokens.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/types/querent_queue.py` & `querent-3.0.2/querent/common/types/querent_queue.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/common/uri.py` & `querent-3.0.2/querent/common/uri.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/collector/collector_config.py` & `querent-3.0.2/querent/config/collector/collector_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/config.py` & `querent-3.0.2/querent/config/config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/core/gpt_llm_config.py` & `querent-3.0.2/querent/config/core/gpt_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/core/llm_config.py` & `querent-3.0.2/querent/config/core/llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/core/opensource_llm_config.py` & `querent-3.0.2/querent/config/core/opensource_llm_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/engine/engine_config.py` & `querent-3.0.2/querent/config/engine/engine_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/graph_config.py` & `querent-3.0.2/querent/config/graph_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/ingestor/ingestor_config.py` & `querent-3.0.2/querent/config/ingestor/ingestor_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/metric/prometheus.py` & `querent-3.0.2/querent/config/metric/prometheus.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/resource/resource_config.py` & `querent-3.0.2/querent/config/resource/resource_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/config/workflow/workflow_config.py` & `querent-3.0.2/querent/config/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/core/base_engine.py` & `querent-3.0.2/querent/core/base_engine.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/core/transformers/bert_ner_opensourcellm.py` & `querent-3.0.2/querent/core/transformers/bert_ner_opensourcellm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/core/transformers/fixed_entities_set_opensourcellm.py` & `querent-3.0.2/querent/core/transformers/fixed_entities_set_opensourcellm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py` & `querent-3.0.2/querent/core/transformers/gpt_llm_bert_ner_or_fixed_entities_set_ner.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/core/transformers/gpt_llm_gpt_ner.py` & `querent-3.0.2/querent/core/transformers/gpt_llm_gpt_ner.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/core/transformers/relationship_extraction_llm.py` & `querent-3.0.2/querent/core/transformers/relationship_extraction_llm.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/graph/errors.py` & `querent-3.0.2/querent/graph/errors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/graph/graph.py` & `querent-3.0.2/querent/graph/graph.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/graph/graph_namespace.py` & `querent-3.0.2/querent/graph/graph_namespace.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/graph/ontology.py` & `querent-3.0.2/querent/graph/ontology.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/graph/schema.py` & `querent-3.0.2/querent/graph/schema.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/graph/shacl.py` & `querent-3.0.2/querent/graph/shacl.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/graph/subject.py` & `querent-3.0.2/querent/graph/subject.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/graph/utils.py` & `querent-3.0.2/querent/graph/utils.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/audio/audio_ingestors.py` & `querent-3.0.2/querent/ingestors/audio/audio_ingestors.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/base_ingestor.py` & `querent-3.0.2/querent/ingestors/base_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/code/code_ingestor.py` & `querent-3.0.2/querent/ingestors/code/code_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/csv/csv_ingestor.py` & `querent-3.0.2/querent/ingestors/csv/csv_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/doc/doc_ingestor.py` & `querent-3.0.2/querent/ingestors/doc/doc_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/email/email_ingestor.py` & `querent-3.0.2/querent/ingestors/email/email_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/email/email_reader.py` & `querent-3.0.2/querent/ingestors/email/email_reader.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/github/github_ingestor.py` & `querent-3.0.2/querent/ingestors/github/github_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/html/html_ingestor.py` & `querent-3.0.2/querent/ingestors/html/html_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/images/image_ingestor.py` & `querent-3.0.2/querent/ingestors/images/image_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/ingestor_factory.py` & `querent-3.0.2/querent/ingestors/ingestor_factory.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/ingestor_manager.py` & `querent-3.0.2/querent/ingestors/ingestor_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/json/json_ingestor.py` & `querent-3.0.2/querent/ingestors/json/json_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/pdfs/pdf_ingestor_v1.py` & `querent-3.0.2/querent/ingestors/pdfs/pdf_ingestor_v1.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/ppt/ppt_ingestor.py` & `querent-3.0.2/querent/ingestors/ppt/ppt_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/texts/text_ingestor.py` & `querent-3.0.2/querent/ingestors/texts/text_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/video/video_ingestor.py` & `querent-3.0.2/querent/ingestors/video/video_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/xlsx/xlsx_ingestor.py` & `querent-3.0.2/querent/ingestors/xlsx/xlsx_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/ingestors/xml/xml_ingestor.py` & `querent-3.0.2/querent/ingestors/xml/xml_ingestor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/ner_helperfunctions/attn_scores.py` & `querent-3.0.2/querent/kg/ner_helperfunctions/attn_scores.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/ner_helperfunctions/contextual_embeddings.py` & `querent-3.0.2/querent/kg/ner_helperfunctions/contextual_embeddings.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/ner_helperfunctions/dependency_parsing.py` & `querent-3.0.2/querent/kg/ner_helperfunctions/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/ner_helperfunctions/filter_triples.py` & `querent-3.0.2/querent/kg/ner_helperfunctions/filter_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/ner_helperfunctions/fixed_entities.py` & `querent-3.0.2/querent/kg/ner_helperfunctions/fixed_entities.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/ner_helperfunctions/fixed_predicate.py` & `querent-3.0.2/querent/kg/ner_helperfunctions/fixed_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/ner_helperfunctions/ner_llm_transformer.py` & `querent-3.0.2/querent/kg/ner_helperfunctions/ner_llm_transformer.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/querent_kg.py` & `querent-3.0.2/querent/kg/querent_kg.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/contextual_predicate.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/contextual_predicate.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/embedding_store.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/embedding_store.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/filter_semantic_triples.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/filter_semantic_triples.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/fixed_relationships.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/fixed_relationships.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/gpt_pydantic_classes.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/openai_functions.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/openai_functions.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/questionanswer_llama2.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/questionanswer_llama2.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/rag_retriever.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/rag_retriever.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/rel_normalize.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/rel_normalize.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/kg/rel_helperfunctions/triple_to_json.py` & `querent-3.0.2/querent/kg/rel_helperfunctions/triple_to_json.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/logging/filters.py` & `querent-3.0.2/querent/logging/filters.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/logging/handlers.py` & `querent-3.0.2/querent/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/logging/logger.py` & `querent-3.0.2/querent/logging/logger.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/metric/adapters/promethus_adapter.py` & `querent-3.0.2/querent/metric/adapters/promethus_adapter.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/metric/metric_logging_handler.py` & `querent-3.0.2/querent/metric/metric_logging_handler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/metric/metric_registry.py` & `querent-3.0.2/querent/metric/metric_registry.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/processors/text_cleanup_processor.py` & `querent-3.0.2/querent/processors/text_cleanup_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/processors/text_processor.py` & `querent-3.0.2/querent/processors/text_processor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/querent/auto_scaler.py` & `querent-3.0.2/querent/querent/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/querent/querent.py` & `querent-3.0.2/querent/querent/querent.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/querent/resource_manager.py` & `querent-3.0.2/querent/querent/resource_manager.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/storage/gcs_query.py` & `querent-3.0.2/querent/storage/gcs_query.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/storage/milvus_vectorevent_storage.py` & `querent-3.0.2/querent/storage/milvus_vectorevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/storage/neo4j_graphevent_storage.py` & `querent-3.0.2/querent/storage/neo4j_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/storage/postgres_graphevent_storage.py` & `querent-3.0.2/querent/storage/postgres_graphevent_storage.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/storage/s3-data-management.py` & `querent-3.0.2/querent/storage/s3-data-management.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/tools/web_page_extractor.py` & `querent-3.0.2/querent/tools/web_page_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/utils/webpage_extractor.py` & `querent-3.0.2/querent/utils/webpage_extractor.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/workflow/_helpers.py` & `querent-3.0.2/querent/workflow/_helpers.py`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent/workflow/workflow.py` & `querent-3.0.2/querent/workflow/workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,32 +16,59 @@
 
 from querent.logging.logger import setup_logger
 logger = setup_logger(__name__, "Workflows")
 
 async def start_workflow(config_dict: dict):
     # Start the workflow
     workflow_config = config_dict.get("workflow")
-    engine_params = workflow_config.get("config").get("engine_params", None)
+    engine_params = workflow_config.get("config", None)
     is_engine_params = False
     try:
         if engine_params is not None:
-            engine_params = json.loads(engine_params)
+            engine_params_json = {}
+            
+            if engine_params.get("fixed_entities") is not None:
+                engine_params_json["fixed_entities"] = [x for x in engine_params.get("fixed_entities").split(",")]
+            
+            if engine_params.get("sample_entities") is not None:
+                engine_params_json["sample_entities"] = [x for x in engine_params.get("fixed_entities").split(",")]
+            
+            if engine_params.get("ner_model_name") is not None:
+                engine_params_json["ner_model_name"] = engine_params.get("ner_model_name")
+            
+            if engine_params.get("enable_filtering") is not None:
+                engine_params_json["enable_filtering"] = engine_params.get("enable_filtering")
+            
+            engine_params_json["filter_params"] = {
+                "score_threshold": float(engine_params.get("score_threshold")) if engine_params.get("score_threshold") is not None else None,
+                "attention_score_threshold": float(engine_params.get("attention_score_threshold")) if engine_params.get("attention_score_threshold") is not None else None,
+                "similarity_threshold": float(engine_params.get("similarity_threshold")) if engine_params.get("similarity_threshold") is not None else None,
+                "min_cluster_size": int(engine_params.get("min_cluster_size")) if engine_params.get("min_cluster_size") is not None else None,
+                "min_samples": int(engine_params.get("min_samples")) if engine_params.get("min_samples") is not None else None,
+                "cluster_persistence_threshold": float(engine_params.get("cluster_persistence_threshold")) if engine_params.get("cluster_persistence_threshold") is not None else None,
+            }
+
+            if engine_params.get("is_confined_search") is not None:
+                engine_params_json["is_confined_search"] = engine_params.get("is_confined_search")
+
+            if engine_params.get("user_context") is not None:
+                engine_params_json["user_context"] = engine_params.get("user_context")
             is_engine_params = True
     except Exception as e:
         logger.error("Got error while loading engine params: ", e)
     workflow = WorkflowConfig(config_source=workflow_config)
     collector_configs = config_dict.get("collectors", [])
     collectors = []
     for collector_config in collector_configs:
         collectors.append(CollectorConfig(config_source=collector_config).resolve())
     engine_configs = config_dict.get("engines", [])
     engines = []
     for engine_config in engine_configs:
         if is_engine_params:
-            engine_config.update(engine_params)
+            engine_config.update(engine_params_json)
         engine_config_source = engine_config.get("config", {})
         if engine_config["name"] == "knowledge_graph_using_openai":
             engine_config.update({"openai_api_key": engine_config["config"]["openai_api_key"]})
             engines.append(GPTConfig(config_source=engine_config))
         elif engine_config["name"] == "knowledge_graph_using_llama2_v1":
             engines.append(LLM_Config(config_source=engine_config))
     config_dict["engines"] = engines
```

### Comparing `querent-3.0.1/querent.egg-info/PKG-INFO` & `querent-3.0.2/querent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querent
-Version: 3.0.1
+Version: 3.0.2
 Summary: The Asynchronous Data Dynamo and Graph Neural Network Catalyst
 Home-page: https://github.com/Querent-ai/querent-ai
 Author: Querent AI
 License: Business Source License 1.1
 Project-URL: Documentation, https://github.com/Querent-ai/querent-ai/docs
 Project-URL: Issue Tracker, https://github.com/Querent-ai/querent-ai/issues
 Keywords: Graph Neural Network,Scalability,Data-Driven Insights,GNN,Async,Knowledge Graphs,KG,Large Language Models,asyncio,Insights,aysnchronous,LLM,transformers,pytorch,Llama-index,AI,Artificial Intelligence,Neo4j,Queues,QuiAssisstant,Collectors,Data,Data Science,Data Engineering,Data Analysis,Data Analytics,News,NLP,Natural Language Processing,Text,Text Analysis,Deep Learning,Graphs,Graph Theory,Graph Algorithms,Graph Analytics,Graph Databases,Graph Processing,Graph Mining,Graph Neural Networks,GNN,GNNs,Graph Neural Network
@@ -57,15 +57,15 @@
 Requires-Dist: jsonschema==4.17.3
 Requires-Dist: kombu==5.2.4
 Requires-Dist: llama_cpp_python==0.2.15
 Requires-Dist: lxml==4.9.2
 Requires-Dist: newspaper3k==0.2.8
 Requires-Dist: nltk==3.8.1
 Requires-Dist: numpy==1.24.3
-Requires-Dist: Pillow==10.0.1
+Requires-Dist: Pillow==10.3.0
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: PyJWT==2.4.0
 Requires-Dist: pytest==7.3.2
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: redis==5.0.3
 Requires-Dist: regex==2023.5.5
 Requires-Dist: sentence-transformers==2.2.2
@@ -97,15 +97,14 @@
 Requires-Dist: azure-storage-blob==12.19.0
 Requires-Dist: moviepy==1.0.3
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: dropbox==11.36.2
 Requires-Dist: requests==2.31.0
 Requires-Dist: google-api-python-client==2.105.0
 Requires-Dist: requests_html==0.10.0
-Requires-Dist: rapidocr-onnxruntime==1.3.9
 Requires-Dist: pybase64==1.3.1
 Requires-Dist: pdfminer==20191125
 Requires-Dist: unidecode==1.3.7
 Requires-Dist: psutil==5.9.8
 Requires-Dist: langchain-community==0.0.25
 Requires-Dist: langchain==0.1.11
 Requires-Dist: openai==1.13.3
```

### Comparing `querent-3.0.1/querent.egg-info/SOURCES.txt` & `querent-3.0.2/querent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querent-3.0.1/querent.egg-info/requires.txt` & `querent-3.0.2/querent.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 jsonschema==4.17.3
 kombu==5.2.4
 llama_cpp_python==0.2.15
 lxml==4.9.2
 newspaper3k==0.2.8
 nltk==3.8.1
 numpy==1.24.3
-Pillow==10.0.1
+Pillow==10.3.0
 pydantic==2.6.4
 PyJWT==2.4.0
 pytest==7.3.2
 python-dotenv==1.0.0
 redis==5.0.3
 regex==2023.5.5
 sentence-transformers==2.2.2
@@ -56,15 +56,14 @@
 azure-storage-blob==12.19.0
 moviepy==1.0.3
 python-docx==1.1.0
 dropbox==11.36.2
 requests==2.31.0
 google-api-python-client==2.105.0
 requests_html==0.10.0
-rapidocr-onnxruntime==1.3.9
 pybase64==1.3.1
 pdfminer==20191125
 unidecode==1.3.7
 psutil==5.9.8
 langchain-community==0.0.25
 langchain==0.1.11
 openai==1.13.3
```

### Comparing `querent-3.0.1/setup.py` & `querent-3.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "jsonschema==4.17.3",
     "kombu==5.2.4",
     "llama_cpp_python==0.2.15",
     "lxml==4.9.2",
     "newspaper3k==0.2.8",
     "nltk==3.8.1",
     "numpy==1.24.3",
-    "Pillow==10.0.1",
+    "Pillow==10.3.0",
     "pydantic==2.6.4",
     "PyJWT==2.4.0",
     "pytest==7.3.2",
     "python-dotenv==1.0.0",
     "redis==5.0.3",
     "regex==2023.5.5",
     "sentence-transformers==2.2.2",
@@ -63,15 +63,14 @@
     "azure-storage-blob==12.19.0",
     "moviepy==1.0.3",
     "python-docx==1.1.0",
     "dropbox==11.36.2",
     "requests==2.31.0",
     "google-api-python-client==2.105.0",
     "requests_html==0.10.0",
-    "rapidocr-onnxruntime==1.3.9",
     "pybase64==1.3.1",
     "pdfminer==20191125",
     "unidecode==1.3.7",
     "psutil==5.9.8",
     "langchain-community==0.0.25",
     "langchain==0.1.11",
     "openai==1.13.3",
@@ -80,15 +79,15 @@
 ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="querent",
-    version="3.0.1",
+    version="3.0.2",
     author="Querent AI",
     description="The Asynchronous Data Dynamo and Graph Neural Network Catalyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Querent-ai/querent-ai",
     project_urls={
         "Documentation": "https://github.com/Querent-ai/querent-ai/docs",
```

