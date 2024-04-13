# Comparing `tmp/inseq-0.5.0.tar.gz` & `tmp/inseq-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inseq-0.5.0.tar", max compression
+gzip compressed data, was "inseq-0.6.0.tar", last modified: Sat Apr 13 13:30:19 2024, max compression
```

## Comparing `inseq-0.5.0.tar` & `inseq-0.6.0.tar`

### file list

```diff
@@ -1,53 +1,107 @@
--rw-r--r--   0        0        0    10899 2023-12-05 11:54:40.310294 inseq-0.5.0/LICENSE
--rw-r--r--   0        0        0    15605 2023-12-07 01:28:44.048738 inseq-0.5.0/README.md
--rw-r--r--   0        0        0     1080 2023-12-05 11:54:40.321160 inseq-0.5.0/inseq/__init__.py
--rw-r--r--   0        0        0      418 2023-12-05 11:54:40.321275 inseq-0.5.0/inseq/attr/__init__.py
--rw-r--r--   0        0        0     3231 2023-12-05 11:54:40.321339 inseq-0.5.0/inseq/attr/attribution_decorators.py
--rw-r--r--   0        0        0     1401 2023-12-05 11:54:40.321426 inseq-0.5.0/inseq/attr/feat/__init__.py
--rw-r--r--   0        0        0     6448 2023-12-05 11:54:40.321507 inseq-0.5.0/inseq/attr/feat/attribution_utils.py
--rw-r--r--   0        0        0    36293 2023-12-05 11:54:40.321617 inseq-0.5.0/inseq/attr/feat/feature_attribution.py
--rw-r--r--   0        0        0    11461 2023-12-05 11:54:40.321728 inseq-0.5.0/inseq/attr/feat/gradient_attribution.py
--rw-r--r--   0        0        0     5759 2023-12-05 11:54:40.321810 inseq-0.5.0/inseq/attr/feat/internals_attribution.py
--rw-r--r--   0        0        0      366 2023-12-05 11:54:40.321899 inseq-0.5.0/inseq/attr/feat/ops/__init__.py
--rw-r--r--   0        0        0     8487 2023-12-05 11:54:40.321985 inseq-0.5.0/inseq/attr/feat/ops/discretized_integrated_gradients.py
--rw-r--r--   0        0        0    12629 2023-12-05 11:54:40.322065 inseq-0.5.0/inseq/attr/feat/ops/lime.py
--rw-r--r--   0        0        0    13429 2023-12-05 11:54:40.322146 inseq-0.5.0/inseq/attr/feat/ops/monotonic_path_builder.py
--rw-r--r--   0        0        0    20563 2023-12-05 11:54:40.322235 inseq-0.5.0/inseq/attr/feat/ops/sequential_integrated_gradients.py
--rw-r--r--   0        0        0     5317 2023-12-05 11:54:40.322314 inseq-0.5.0/inseq/attr/feat/perturbation_attribution.py
--rw-r--r--   0        0        0    23562 2023-12-05 11:54:40.322443 inseq-0.5.0/inseq/attr/step_functions.py
--rw-r--r--   0        0        0        0 2023-12-05 11:54:40.322527 inseq-0.5.0/inseq/commands/__init__.py
--rw-r--r--   0        0        0     7524 2023-12-05 11:54:40.322613 inseq-0.5.0/inseq/commands/attribute.py
--rw-r--r--   0        0        0     3371 2023-12-05 11:54:40.322671 inseq-0.5.0/inseq/commands/attribute_dataset.py
--rw-r--r--   0        0        0     1691 2023-12-05 11:54:40.322730 inseq-0.5.0/inseq/commands/base.py
--rw-r--r--   0        0        0      857 2023-12-05 11:54:40.322786 inseq-0.5.0/inseq/commands/cli.py
--rw-r--r--   0        0        0     1769 2023-12-05 11:54:40.322873 inseq-0.5.0/inseq/data/__init__.py
--rw-r--r--   0        0        0     3464 2023-12-05 11:54:40.322939 inseq-0.5.0/inseq/data/aggregation_functions.py
--rw-r--r--   0        0        0    38509 2023-12-05 11:54:40.323037 inseq-0.5.0/inseq/data/aggregator.py
--rw-r--r--   0        0        0    36537 2023-12-05 11:54:40.323179 inseq-0.5.0/inseq/data/attribution.py
--rw-r--r--   0        0        0     8094 2023-12-05 11:54:40.323258 inseq-0.5.0/inseq/data/batch.py
--rw-r--r--   0        0        0     7408 2023-12-05 11:54:40.323325 inseq-0.5.0/inseq/data/data_utils.py
--rw-r--r--   0        0        0    16482 2023-12-05 11:54:40.323407 inseq-0.5.0/inseq/data/viz.py
--rw-r--r--   0        0        0     2712 2023-12-05 11:54:40.323535 inseq-0.5.0/inseq/models/__init__.py
--rw-r--r--   0        0        0    29629 2023-12-05 11:54:40.323633 inseq-0.5.0/inseq/models/attribution_model.py
--rw-r--r--   0        0        0     9671 2023-12-05 11:54:40.323732 inseq-0.5.0/inseq/models/decoder_only.py
--rw-r--r--   0        0        0    12996 2023-12-05 11:54:40.323802 inseq-0.5.0/inseq/models/encoder_decoder.py
--rw-r--r--   0        0        0    21512 2023-12-05 11:54:40.323893 inseq-0.5.0/inseq/models/huggingface_model.py
--rw-r--r--   0        0        0     3478 2023-12-05 11:54:40.323972 inseq-0.5.0/inseq/models/model_config.py
--rw-r--r--   0        0        0       45 2023-12-05 11:54:40.324022 inseq-0.5.0/inseq/models/model_config.yaml
--rw-r--r--   0        0        0      483 2023-12-05 11:54:40.324081 inseq-0.5.0/inseq/models/model_decorators.py
--rw-r--r--   0        0        0     3066 2023-12-05 11:54:40.324173 inseq-0.5.0/inseq/utils/__init__.py
--rw-r--r--   0        0        0    15706 2023-12-05 11:54:40.324270 inseq-0.5.0/inseq/utils/alignment_utils.py
--rw-r--r--   0        0        0    11731 2023-12-05 11:54:40.324357 inseq-0.5.0/inseq/utils/argparse.py
--rw-r--r--   0        0        0     1589 2023-12-05 11:54:40.324416 inseq-0.5.0/inseq/utils/cache.py
--rw-r--r--   0        0        0     8079 2023-12-05 11:54:40.324490 inseq-0.5.0/inseq/utils/contrast_utils.py
--rw-r--r--   0        0        0     1753 2023-12-05 11:54:40.324547 inseq-0.5.0/inseq/utils/errors.py
--rw-r--r--   0        0        0     1072 2023-12-05 11:54:40.324599 inseq-0.5.0/inseq/utils/id_utils.py
--rw-r--r--   0        0        0      938 2023-12-05 11:54:40.324656 inseq-0.5.0/inseq/utils/import_utils.py
--rw-r--r--   0        0        0    15419 2023-12-05 11:54:40.324738 inseq-0.5.0/inseq/utils/misc.py
--rw-r--r--   0        0        0     1278 2023-12-05 11:54:40.324798 inseq-0.5.0/inseq/utils/registry.py
--rw-r--r--   0        0        0    18715 2023-12-05 11:54:40.324880 inseq-0.5.0/inseq/utils/serialization.py
--rw-r--r--   0        0        0     9420 2023-12-05 11:54:40.324994 inseq-0.5.0/inseq/utils/torch_utils.py
--rw-r--r--   0        0        0     4367 2023-12-05 11:54:40.325064 inseq-0.5.0/inseq/utils/typing.py
--rw-r--r--   0        0        0     4305 2023-12-05 11:54:40.325137 inseq-0.5.0/inseq/utils/viz_utils.py
--rw-r--r--   0        0        0     6641 2023-12-07 01:29:58.968080 inseq-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    18598 1970-01-01 00:00:00.000000 inseq-0.5.0/PKG-INFO
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.810013 inseq-0.6.0/
+-rw-r--r--   0 gsarti     (501) staff       (20)      328 2024-02-19 21:32:33.000000 inseq-0.6.0/.dockerignore
+-rw-r--r--   0 gsarti     (501) staff       (20)      424 2023-12-05 11:54:40.000000 inseq-0.6.0/.editorconfig
+-rw-r--r--   0 gsarti     (501) staff       (20)    13880 2024-02-19 21:32:33.000000 inseq-0.6.0/.gitignore
+-rw-r--r--   0 gsarti     (501) staff       (20)     1070 2024-02-19 21:32:33.000000 inseq-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 gsarti     (501) staff       (20)      514 2023-12-17 17:43:31.000000 inseq-0.6.0/.readthedocs.yaml
+-rw-r--r--   0 gsarti     (501) staff       (20)      279 2024-04-13 13:07:56.000000 inseq-0.6.0/CHANGELOG.md
+-rw-r--r--   0 gsarti     (501) staff       (20)     1717 2023-12-15 15:31:48.000000 inseq-0.6.0/CITATION.cff
+-rw-r--r--   0 gsarti     (501) staff       (20)     3375 2024-02-19 21:32:33.000000 inseq-0.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 gsarti     (501) staff       (20)     1266 2024-02-19 21:32:33.000000 inseq-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 gsarti     (501) staff       (20)    10899 2023-12-05 11:54:40.000000 inseq-0.6.0/LICENSE
+-rw-r--r--   0 gsarti     (501) staff       (20)      208 2024-02-19 21:32:33.000000 inseq-0.6.0/MANIFEST.in
+-rw-r--r--   0 gsarti     (501) staff       (20)    38648 2024-04-13 13:30:19.809745 inseq-0.6.0/PKG-INFO
+-rw-r--r--   0 gsarti     (501) staff       (20)    22276 2024-04-13 12:28:33.000000 inseq-0.6.0/README.md
+-rw-r--r--   0 gsarti     (501) staff       (20)     1223 2024-02-19 21:32:33.000000 inseq-0.6.0/SECURITY.md
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.782979 inseq-0.6.0/inseq/
+-rw-r--r--   0 gsarti     (501) staff       (20)     1080 2023-12-05 11:54:40.000000 inseq-0.6.0/inseq/__init__.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.784480 inseq-0.6.0/inseq/attr/
+-rw-r--r--   0 gsarti     (501) staff       (20)      418 2023-12-05 11:54:40.000000 inseq-0.6.0/inseq/attr/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     3252 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/attr/attribution_decorators.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.787067 inseq-0.6.0/inseq/attr/feat/
+-rw-r--r--   0 gsarti     (501) staff       (20)     1587 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     6621 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/attr/feat/attribution_utils.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    38327 2024-03-07 12:14:41.000000 inseq-0.6.0/inseq/attr/feat/feature_attribution.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    11545 2024-02-21 09:34:53.000000 inseq-0.6.0/inseq/attr/feat/gradient_attribution.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     6188 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/attr/feat/internals_attribution.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.792995 inseq-0.6.0/inseq/attr/feat/ops/
+-rw-r--r--   0 gsarti     (501) staff       (20)      470 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/ops/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     8474 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/attr/feat/ops/discretized_integrated_gradients.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    12629 2023-12-15 15:31:48.000000 inseq-0.6.0/inseq/attr/feat/ops/lime.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    13416 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/attr/feat/ops/monotonic_path_builder.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     5290 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/ops/reagent.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.794949 inseq-0.6.0/inseq/attr/feat/ops/reagent_core/
+-rw-r--r--   0 gsarti     (501) staff       (20)      467 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/ops/reagent_core/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     8470 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/ops/reagent_core/importance_score_evaluator.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     5443 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/ops/reagent_core/rationalizer.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     5887 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/ops/reagent_core/stopping_condition_evaluator.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     4178 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/ops/reagent_core/token_replacer.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     4004 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/ops/reagent_core/token_sampler.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    20550 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/attr/feat/ops/sequential_integrated_gradients.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    22437 2024-03-14 08:35:48.000000 inseq-0.6.0/inseq/attr/feat/ops/value_zeroing.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    14697 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/attr/feat/perturbation_attribution.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    23946 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/attr/step_functions.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.795938 inseq-0.6.0/inseq/commands/
+-rw-r--r--   0 gsarti     (501) staff       (20)        0 2023-12-05 11:54:40.000000 inseq-0.6.0/inseq/commands/__init__.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.796570 inseq-0.6.0/inseq/commands/attribute/
+-rw-r--r--   0 gsarti     (501) staff       (20)      324 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/attribute/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     3605 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/attribute/attribute.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     6507 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/attribute/attribute_args.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.798069 inseq-0.6.0/inseq/commands/attribute_context/
+-rw-r--r--   0 gsarti     (501) staff       (20)      412 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/attribute_context/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    11831 2024-04-04 13:26:28.000000 inseq-0.6.0/inseq/commands/attribute_context/attribute_context.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    16464 2024-04-04 13:26:28.000000 inseq-0.6.0/inseq/commands/attribute_context/attribute_context_args.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    22733 2024-04-04 13:26:28.000000 inseq-0.6.0/inseq/commands/attribute_context/attribute_context_helpers.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     6617 2024-03-20 10:33:50.000000 inseq-0.6.0/inseq/commands/attribute_context/attribute_context_viz_helpers.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.798738 inseq-0.6.0/inseq/commands/attribute_dataset/
+-rw-r--r--   0 gsarti     (501) staff       (20)      101 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/attribute_dataset/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     1940 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/attribute_dataset/attribute_dataset.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     1711 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/attribute_dataset/attribute_dataset_args.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     1718 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/base.py
+-rw-r--r--   0 gsarti     (501) staff       (20)      992 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/commands/cli.py
+-rw-r--r--   0 gsarti     (501) staff       (20)      739 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/commands/commands_utils.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.801322 inseq-0.6.0/inseq/data/
+-rw-r--r--   0 gsarti     (501) staff       (20)     1769 2023-12-05 11:54:40.000000 inseq-0.6.0/inseq/data/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     3451 2024-02-27 16:28:56.000000 inseq-0.6.0/inseq/data/aggregation_functions.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    36690 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/data/aggregator.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    37704 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/data/attribution.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     8081 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/data/batch.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     7614 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/data/data_utils.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    16714 2024-03-07 12:14:41.000000 inseq-0.6.0/inseq/data/viz.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.803956 inseq-0.6.0/inseq/models/
+-rw-r--r--   0 gsarti     (501) staff       (20)     2706 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/models/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    30284 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/models/attribution_model.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     9679 2024-04-04 13:26:28.000000 inseq-0.6.0/inseq/models/decoder_only.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    12977 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/models/encoder_decoder.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    22271 2024-04-04 13:26:28.000000 inseq-0.6.0/inseq/models/huggingface_model.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     4349 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/models/model_config.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     3701 2024-04-04 13:26:28.000000 inseq-0.6.0/inseq/models/model_config.yaml
+-rw-r--r--   0 gsarti     (501) staff       (20)      483 2023-12-05 11:54:40.000000 inseq-0.6.0/inseq/models/model_decorators.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.808100 inseq-0.6.0/inseq/utils/
+-rw-r--r--   0 gsarti     (501) staff       (20)     3428 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/utils/__init__.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    15731 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/utils/alignment_utils.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    20326 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/utils/argparse.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     1589 2023-12-05 11:54:40.000000 inseq-0.6.0/inseq/utils/cache.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     8134 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/utils/contrast_utils.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     1746 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/utils/errors.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     4832 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/utils/hooks.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     1072 2024-02-28 16:26:34.000000 inseq-0.6.0/inseq/utils/id_utils.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     1040 2024-04-13 12:28:33.000000 inseq-0.6.0/inseq/utils/import_utils.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    15612 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/utils/misc.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     1278 2023-12-05 11:54:40.000000 inseq-0.6.0/inseq/utils/registry.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    18703 2024-02-17 15:31:56.000000 inseq-0.6.0/inseq/utils/serialization.py
+-rw-r--r--   0 gsarti     (501) staff       (20)    15549 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/utils/torch_utils.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     5505 2024-02-28 16:18:15.000000 inseq-0.6.0/inseq/utils/typing.py
+-rw-r--r--   0 gsarti     (501) staff       (20)     4305 2023-12-05 11:54:40.000000 inseq-0.6.0/inseq/utils/viz_utils.py
+drwxr-xr-x   0 gsarti     (501) staff       (20)        0 2024-04-13 13:30:19.808386 inseq-0.6.0/inseq.egg-info/
+-rw-r--r--   0 gsarti     (501) staff       (20)    38648 2024-04-13 13:30:19.000000 inseq-0.6.0/inseq.egg-info/PKG-INFO
+-rw-r--r--   0 gsarti     (501) staff       (20)     2823 2024-04-13 13:30:19.000000 inseq-0.6.0/inseq.egg-info/SOURCES.txt
+-rw-r--r--   0 gsarti     (501) staff       (20)        1 2024-04-13 13:30:19.000000 inseq-0.6.0/inseq.egg-info/dependency_links.txt
+-rw-r--r--   0 gsarti     (501) staff       (20)       50 2024-04-13 13:30:19.000000 inseq-0.6.0/inseq.egg-info/entry_points.txt
+-rw-r--r--   0 gsarti     (501) staff       (20)      977 2024-04-13 13:30:19.000000 inseq-0.6.0/inseq.egg-info/requires.txt
+-rw-r--r--   0 gsarti     (501) staff       (20)        6 2024-04-13 13:30:19.000000 inseq-0.6.0/inseq.egg-info/top_level.txt
+-rw-r--r--   0 gsarti     (501) staff       (20)     5755 2024-04-13 13:20:24.000000 inseq-0.6.0/pyproject.toml
+-rw-r--r--   0 gsarti     (501) staff       (20)     7089 2024-04-13 12:28:33.000000 inseq-0.6.0/requirements-dev.txt
+-rw-r--r--   0 gsarti     (501) staff       (20)     1958 2024-04-13 12:28:33.000000 inseq-0.6.0/requirements.txt
+-rw-r--r--   0 gsarti     (501) staff       (20)       38 2024-04-13 13:30:19.810063 inseq-0.6.0/setup.cfg
+-rw-r--r--   0 gsarti     (501) staff       (20)     8394 2024-04-13 13:18:17.000000 inseq-0.6.0/v0.6.md
```

### Comparing `inseq-0.5.0/LICENSE` & `inseq-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inseq-0.5.0/inseq/__init__.py` & `inseq-0.6.0/inseq/__init__.py`

 * *Files identical despite different names*

### Comparing `inseq-0.5.0/inseq/attr/attribution_decorators.py` & `inseq-0.6.0/inseq/attr/attribution_decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Decorators for attribution methods."""
 
 import logging
+from collections.abc import Sequence
 from functools import wraps
-from typing import Any, Callable, List, Optional, Sequence
+from typing import Any, Callable, Optional
 
 from ..data.data_utils import TensorWrapper
 
 logger = logging.getLogger(__name__)
 
 
 def set_hook(f: Callable[[Any], Any]) -> Callable[[Any], Any]:
@@ -51,15 +52,15 @@
 
 
 def batched(f: Callable[..., Any]) -> Callable[..., Any]:
     """Decorator that enables batching of the args."""
 
     @wraps(f)
     def batched_wrapper(self, *args, batch_size: Optional[int] = None, **kwargs):
-        def get_batched(bs: Optional[int], seq: Sequence[Any]) -> List[List[Any]]:
+        def get_batched(bs: Optional[int], seq: Sequence[Any]) -> list[list[Any]]:
             if isinstance(seq, str):
                 seq = [seq]
             if isinstance(seq, list):
                 return [seq[i : i + bs] for i in range(0, len(seq), bs)]  # noqa
             if isinstance(seq, tuple):
                 return list(zip(*[get_batched(bs, s) for s in seq]))
             elif isinstance(seq, TensorWrapper):
```

### Comparing `inseq-0.5.0/inseq/attr/feat/__init__.py` & `inseq-0.6.0/inseq/attr/feat/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     SaliencyAttribution,
     SequentialIntegratedGradientsAttribution,
 )
 from .internals_attribution import AttentionWeightsAttribution, InternalsAttributionRegistry
 from .perturbation_attribution import (
     LimeAttribution,
     OcclusionAttribution,
+    PerturbationAttributionRegistry,
+    ReagentAttribution,
+    ValueZeroingAttribution,
 )
 
 __all__ = [
     "FeatureAttribution",
     "extract_args",
     "list_feature_attribution_methods",
     "join_token_ids",
@@ -35,8 +38,11 @@
     "LayerGradientXActivationAttribution",
     "LayerDeepLiftAttribution",
     "InternalsAttributionRegistry",
     "AttentionWeightsAttribution",
     "OcclusionAttribution",
     "LimeAttribution",
     "SequentialIntegratedGradientsAttribution",
+    "ValueZeroingAttribution",
+    "PerturbationAttributionRegistry",
+    "ReagentAttribution",
 ]
```

### Comparing `inseq-0.5.0/inseq/attr/feat/attribution_utils.py` & `inseq-0.6.0/inseq/attr/feat/attribution_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
 import math
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
-
-import torch
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 from ...utils import extract_signature_args, get_aligned_idx
 from ...utils.typing import (
     OneOrMoreAttributionSequences,
     OneOrMoreIdSequences,
     OneOrMoreTokenSequences,
     SingleScorePerStepTensor,
+    StepAttributionTensor,
     TextInput,
     TokenWithId,
 )
 from ..step_functions import get_step_scores_args
 
 if TYPE_CHECKING:
     from ...models import AttributionModel
@@ -47,15 +46,15 @@
     ]
 
 
 def check_attribute_positions(
     max_length: int,
     attr_pos_start: Optional[int] = None,
     attr_pos_end: Optional[int] = None,
-) -> Tuple[int, int]:
+) -> tuple[int, int]:
     r"""Checks whether the combination of start/end positions for attribution is valid.
 
     Args:
         max_length (:obj:`int`): The maximum length of sequences in the batch.
         attr_pos_start (:obj:`int`, `optional`): The initial position for performing
             sequence attribution. Defaults to 1 (0 is the default BOS token).
         attr_pos_end (:obj:`int`, `optional`): The final position for performing sequence
@@ -86,16 +85,16 @@
     return attr_pos_start, attr_pos_end
 
 
 def join_token_ids(
     tokens: OneOrMoreTokenSequences,
     ids: OneOrMoreIdSequences,
     contrast_tokens: Optional[OneOrMoreTokenSequences] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
-) -> List[TokenWithId]:
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
+) -> list[TokenWithId]:
     """Joins tokens and ids into a list of TokenWithId objects."""
     if contrast_tokens is None:
         contrast_tokens = tokens
     # 1:1 alignment between target and contrast tokens
     if contrast_targets_alignments is None:
         contrast_targets_alignments = [[(idx, idx) for idx, _ in enumerate(seq)] for seq in tokens]
     sequences = []
@@ -112,18 +111,18 @@
         sequences.append(curr_seq)
     return sequences
 
 
 def extract_args(
     attribution_method: "FeatureAttribution",
     attributed_fn: Callable[..., SingleScorePerStepTensor],
-    step_scores: List[str],
-    default_args: List[str],
+    step_scores: list[str],
+    default_args: list[str],
     **kwargs,
-) -> Tuple[Dict[str, Any], Dict[str, Any], Dict[str, Any]]:
+) -> tuple[dict[str, Any], dict[str, Any], dict[str, Any]]:
     attribution_args = kwargs.pop("attribution_args", {})
     attributed_fn_args = kwargs.pop("attributed_fn_args", {})
     step_scores_args = kwargs.pop("step_scores_args", {})
     extra_attribution_args, attribution_unused_args = attribution_method.get_attribution_args(**kwargs)
     extra_attributed_fn_args, attributed_fn_unused_args = extract_signature_args(
         kwargs, attributed_fn, exclude_args=default_args, return_remaining=True
     )
@@ -139,21 +138,21 @@
     attribution_args.update(extra_attribution_args)
     attributed_fn_args.update(extra_attributed_fn_args)
     step_scores_args.update(extra_step_scores_args)
     return attribution_args, attributed_fn_args, step_scores_args
 
 
 def get_source_target_attributions(
-    attr: Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]],
+    attr: Union[StepAttributionTensor, tuple[StepAttributionTensor, StepAttributionTensor]],
     is_encoder_decoder: bool,
-) -> Tuple[torch.Tensor, torch.Tensor]:
-    if is_encoder_decoder:
-        if isinstance(attr, tuple) and len(attr) > 1:
-            return attr[0], attr[1]
-        elif isinstance(attr, tuple) and len(attr) == 1:
-            return attr[0], None
+    has_sequence_scores: bool = False,
+) -> tuple[Optional[StepAttributionTensor], Optional[StepAttributionTensor]]:
+    if isinstance(attr, tuple):
+        if is_encoder_decoder:
+            if has_sequence_scores:
+                return (attr[0], attr[1], attr[2])
+            else:
+                return (attr[0], attr[1]) if len(attr) > 1 else (attr[0], None)
         else:
-            return attr, None
-    elif isinstance(attr, tuple):
-        return None, attr[0]
+            return (None, None, attr[0]) if has_sequence_scores else (None, attr[0])
     else:
-        return None, attr
+        return (attr, None) if is_encoder_decoder else (None, attr)
```

### Comparing `inseq-0.5.0/inseq/attr/feat/feature_attribution.py` & `inseq-0.6.0/inseq/attr/feat/feature_attribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """Feature attribution methods registry.
 
 Todo:
     * 🟡: Allow custom arguments for model loading in the :class:`FeatureAttribution` :meth:`load` method.
 """
 import logging
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import torch
 from jaxtyping import Int
 
 from ...data import (
     DecoderOnlyBatch,
     EncoderDecoderBatch,
@@ -110,14 +110,15 @@
         self.forward_batch_embeds: bool = True
         self.target_layer = None
         self.use_baselines: bool = False
         self.use_attention_weights: bool = False
         self.use_hidden_states: bool = False
         self.use_predicted_target: bool = True
         self.use_model_config: bool = False
+        self.is_final_step_method: bool = False
         if hook_to_model:
             self.hook(**kwargs)
 
     @classmethod
     def load(
         cls,
         method_name: str,
@@ -169,20 +170,20 @@
         targets: FeatureAttributionInput,
         attr_pos_start: Optional[int] = None,
         attr_pos_end: Optional[int] = None,
         show_progress: bool = True,
         pretty_progress: bool = True,
         output_step_attributions: bool = False,
         attribute_target: bool = False,
-        step_scores: List[str] = [],
+        step_scores: list[str] = [],
         include_eos_baseline: bool = False,
         attributed_fn: Union[str, Callable[..., SingleScorePerStepTensor], None] = None,
-        attribution_args: Dict[str, Any] = {},
-        attributed_fn_args: Dict[str, Any] = {},
-        step_scores_args: Dict[str, Any] = {},
+        attribution_args: dict[str, Any] = {},
+        attributed_fn_args: dict[str, Any] = {},
+        step_scores_args: dict[str, Any] = {},
     ) -> FeatureAttributionOutput:
         r"""Prepares inputs and performs attribution.
 
         Wraps the attribution method :meth:`~inseq.attr.feat.FeatureAttribution.attribute` method
         and the :meth:`~inseq.models.InputFormatter.prepare_inputs_for_attribution` method.
 
         Args:
@@ -268,23 +269,52 @@
         if self.use_model_config and self.attribution_model.is_distributed:
             raise RuntimeError(
                 "Distributed models are incompatible with attribution methods requiring access to models' internals "
                 "for storing or intervention purposes. Please use a non-distributed model with the current attribution"
                 " method."
             )
 
+    @staticmethod
+    def _build_multistep_output_from_single_step(
+        single_step_output: FeatureAttributionStepOutput,
+        attr_pos_start: int,
+        attr_pos_end: int,
+    ) -> list[FeatureAttributionStepOutput]:
+        if single_step_output.step_scores:
+            raise ValueError("step_scores are not supported for final step attribution methods.")
+        num_seq = len(single_step_output.prefix)
+        steps = []
+        for pos_idx in range(attr_pos_start, attr_pos_end):
+            step_output = single_step_output.clone_empty()
+            step_output.source = single_step_output.source
+            step_output.prefix = [single_step_output.prefix[seq_idx][:pos_idx] for seq_idx in range(num_seq)]
+            step_output.target = (
+                single_step_output.target
+                if pos_idx == attr_pos_end - 1
+                else [[single_step_output.prefix[seq_idx][pos_idx]] for seq_idx in range(num_seq)]
+            )
+            if single_step_output.source_attributions is not None:
+                step_output.source_attributions = single_step_output.source_attributions[:, :, pos_idx - 1]
+            if single_step_output.target_attributions is not None:
+                step_output.target_attributions = single_step_output.target_attributions[:, :pos_idx, pos_idx - 1]
+            single_step_output.step_scores = {}
+            if single_step_output.sequence_scores is not None:
+                step_output.sequence_scores = single_step_output.sequence_scores
+            steps.append(step_output)
+        return steps
+
     def format_contrastive_targets(
         self,
         target_sequences: TextSequences,
         target_tokens: OneOrMoreTokenSequences,
-        attributed_fn_args: Dict[str, Any],
-        step_scores_args: Dict[str, Any],
+        attributed_fn_args: dict[str, Any],
+        step_scores_args: dict[str, Any],
         attr_pos_start: int,
         attr_pos_end: int,
-    ) -> Tuple[Optional[DecoderOnlyBatch], Optional[List[List[Tuple[int, int]]]], Dict[str, Any], Dict[str, Any]]:
+    ) -> tuple[Optional[DecoderOnlyBatch], Optional[list[list[tuple[int, int]]]], dict[str, Any], dict[str, Any]]:
         contrast_batch, contrast_targets_alignments = None, None
         contrast_targets = attributed_fn_args.get("contrast_targets", None)
         if contrast_targets is None:
             contrast_targets = step_scores_args.get("contrast_targets", None)
         contrast_targets_alignments = attributed_fn_args.get("contrast_targets_alignments", None)
         if contrast_targets_alignments is None:
             contrast_targets_alignments = step_scores_args.get("contrast_targets_alignments", None)
@@ -323,18 +353,18 @@
         attributed_fn: Callable[..., SingleScorePerStepTensor],
         attr_pos_start: Optional[int] = None,
         attr_pos_end: Optional[int] = None,
         show_progress: bool = True,
         pretty_progress: bool = True,
         output_step_attributions: bool = False,
         attribute_target: bool = False,
-        step_scores: List[str] = [],
-        attribution_args: Dict[str, Any] = {},
-        attributed_fn_args: Dict[str, Any] = {},
-        step_scores_args: Dict[str, Any] = {},
+        step_scores: list[str] = [],
+        attribution_args: dict[str, Any] = {},
+        attributed_fn_args: dict[str, Any] = {},
+        step_scores_args: dict[str, Any] = {},
     ) -> FeatureAttributionOutput:
         r"""Performs the feature attribution procedure using the specified attribution method.
 
         Args:
             batch (:class:`~inseq.data.EncoderDecoderBatch` or :class:`~inseq.data.DecoderOnlyBatch`): The batch of
                 sequences to attribute.
             attributed_fn (:obj:`Callable[..., SingleScorePerStepTensor]`): The function of model
@@ -412,25 +442,27 @@
         else:
             iter_pos_end = attr_pos_end
         pbar = get_progress_bar(
             sequences=sequences,
             target_lengths=targets_lengths,
             method_name=self.method_name,
             show=show_progress,
-            pretty=pretty_progress,
+            pretty=False if self.is_final_step_method else pretty_progress,
             attr_pos_start=attr_pos_start,
-            attr_pos_end=attr_pos_end,
+            attr_pos_end=1 if self.is_final_step_method else attr_pos_end,
         )
         whitespace_indexes = find_char_indexes(sequences.targets, " ")
         attribution_outputs = []
 
         start = datetime.now()
 
         # Attribution loop for generation
         for step in range(attr_pos_start, iter_pos_end):
+            if self.is_final_step_method and step != iter_pos_end - 1:
+                continue
             tgt_ids, tgt_mask = batch.get_step_target(step, with_attention=True)
             step_output = self.filtered_attribute_step(
                 batch[:step],
                 target_ids=tgt_ids.unsqueeze(1),
                 attributed_fn=attributed_fn,
                 target_attention_mask=tgt_mask.unsqueeze(1),
                 attribute_target=attribute_target,
@@ -446,41 +478,46 @@
                 batch[:step],
                 self.attribution_model.convert_ids_to_tokens(tgt_ids.unsqueeze(1), skip_special_tokens=False),
                 tgt_ids.detach().to("cpu"),
                 contrast_batch=contrast_batch,
                 contrast_targets_alignments=contrast_targets_alignments,
             )
             attribution_outputs.append(step_output)
-            if pretty_progress:
+            if pretty_progress and not self.is_final_step_method:
                 tgt_tokens = batch.target_tokens
                 skipped_prefixes = tok2string(self.attribution_model, tgt_tokens, end=attr_pos_start)
                 attributed_sentences = tok2string(self.attribution_model, tgt_tokens, attr_pos_start, step + 1)
                 unattributed_suffixes = tok2string(self.attribution_model, tgt_tokens, step + 1, attr_pos_end)
                 skipped_suffixes = tok2string(self.attribution_model, tgt_tokens, start=attr_pos_end)
                 update_progress_bar(
                     pbar,
                     skipped_prefixes,
                     attributed_sentences,
                     unattributed_suffixes,
                     skipped_suffixes,
                     whitespace_indexes,
                     show=show_progress,
-                    pretty=pretty_progress,
+                    pretty=True,
                 )
             else:
-                update_progress_bar(pbar, show=show_progress, pretty=pretty_progress)
+                update_progress_bar(pbar, show=show_progress, pretty=False)
         end = datetime.now()
-        close_progress_bar(pbar, show=show_progress, pretty=pretty_progress)
+        close_progress_bar(pbar, show=show_progress, pretty=False if self.is_final_step_method else pretty_progress)
         batch.detach().to("cpu")
+        if self.is_final_step_method:
+            attribution_outputs = self._build_multistep_output_from_single_step(
+                attribution_outputs[0],
+                attr_pos_start=attr_pos_start,
+                attr_pos_end=iter_pos_end,
+            )
         out = FeatureAttributionOutput(
             sequence_attributions=FeatureAttributionSequenceOutput.from_step_attributions(
                 attributions=attribution_outputs,
                 tokenized_target_sentences=target_tokens_with_ids,
-                pad_id=self.attribution_model.pad_token,
-                has_bos_token=self.attribution_model.is_encoder_decoder,
+                pad_token=self.attribution_model.pad_token,
                 attr_pos_end=attr_pos_end,
             ),
             step_attributions=attribution_outputs if output_step_attributions else None,
             info={
                 "attribution_method": self.method_name,
                 "attr_pos_start": attr_pos_start,
                 "attr_pos_end": attr_pos_end,
@@ -497,18 +534,18 @@
     def filtered_attribute_step(
         self,
         batch: Union[DecoderOnlyBatch, EncoderDecoderBatch],
         target_ids: Int[torch.Tensor, "batch_size 1"],
         attributed_fn: Callable[..., SingleScorePerStepTensor],
         target_attention_mask: Optional[Int[torch.Tensor, "batch_size 1"]] = None,
         attribute_target: bool = False,
-        step_scores: List[str] = [],
-        attribution_args: Dict[str, Any] = {},
-        attributed_fn_args: Dict[str, Any] = {},
-        step_scores_args: Dict[str, Any] = {},
+        step_scores: list[str] = [],
+        attribution_args: dict[str, Any] = {},
+        attributed_fn_args: dict[str, Any] = {},
+        step_scores_args: dict[str, Any] = {},
     ) -> FeatureAttributionStepOutput:
         r"""Performs a single attribution step for all the sequences in the batch that
         still have valid target_ids, as identified by the target_attention_mask.
         Finished sentences are temporarily filtered out to make the attribution step
         faster and then reinserted before returning.
 
         Args:
@@ -577,39 +614,39 @@
                 attribution_args = {**attribution_args, **hidden_states_dict}
         # Perform attribution step
         step_output = self.attribute_step(
             attribute_main_args,
             attribution_args,
         )
         # Format step scores arguments and calculate step scores
-        for step_score in step_scores:
+        for score in step_scores:
             step_fn_args = self.attribution_model.formatter.format_step_function_args(
                 attribution_model=self.attribution_model,
                 forward_output=output,
                 target_ids=target_ids,
                 is_attributed_fn=False,
                 batch=batch,
             )
-            step_fn_extra_args = get_step_scores_args([step_score], step_scores_args)
-            step_output.step_scores[step_score] = get_step_scores(step_score, step_fn_args, step_fn_extra_args)
+            step_fn_extra_args = get_step_scores_args([score], step_scores_args)
+            step_output.step_scores[score] = get_step_scores(score, step_fn_args, step_fn_extra_args).to("cpu")
         # Reinsert finished sentences
         if target_attention_mask is not None and is_filtered:
-            step_output.remap_from_filtered(target_attention_mask, orig_batch)
+            step_output.remap_from_filtered(target_attention_mask, orig_batch, self.is_final_step_method)
         step_output = step_output.detach().to("cpu")
         return step_output
 
-    def get_attribution_args(self, **kwargs) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+    def get_attribution_args(self, **kwargs) -> tuple[dict[str, Any], dict[str, Any]]:
         if hasattr(self, "method") and hasattr(self.method, "attribute"):
             return extract_signature_args(kwargs, self.method.attribute, self.ignore_extra_args, return_remaining=True)
         return {}, {}
 
     def attribute_step(
         self,
-        attribute_fn_main_args: Dict[str, Any],
-        attribution_args: Dict[str, Any] = {},
+        attribute_fn_main_args: dict[str, Any],
+        attribution_args: dict[str, Any] = {},
     ) -> FeatureAttributionStepOutput:
         r"""Performs a single attribution step for the specified attribution arguments.
 
         Args:
             attribute_fn_main_args (:obj:`dict`): Main arguments used for the attribution method. These are built from
                 model inputs at the current step of the feature attribution process.
             attribution_args (:obj:`dict`, `optional`): Additional arguments to pass to the attribution method.
@@ -659,14 +696,14 @@
 
 class DummyAttribution(FeatureAttribution):
     """Dummy attribution method that returns empty attributions."""
 
     method_name = "dummy"
 
     def attribute_step(
-        self, attribute_fn_main_args: Dict[str, Any], attribution_args: Dict[str, Any] = {}
+        self, attribute_fn_main_args: dict[str, Any], attribution_args: dict[str, Any] = {}
     ) -> FeatureAttributionStepOutput:
         return FeatureAttributionStepOutput(
             source_attributions=None,
             target_attributions=None,
             step_scores={},
         )
```

### Comparing `inseq-0.5.0/inseq/attr/feat/gradient_attribution.py` & `inseq-0.6.0/inseq/attr/feat/gradient_attribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Gradient-based feature attribution methods."""
 
 import logging
-from typing import Any, Dict
+from typing import Any
 
 from captum.attr import (
     DeepLift,
     GradientShap,
     InputXGradient,
     IntegratedGradients,
     LayerDeepLift,
@@ -61,16 +61,16 @@
         if self.attribute_batch_ids and not self.forward_batch_embeds:
             self.target_layer = None
         else:
             self.attribution_model.remove_interpretable_embeddings()
 
     def attribute_step(
         self,
-        attribute_fn_main_args: Dict[str, Any],
-        attribution_args: Dict[str, Any] = {},
+        attribute_fn_main_args: dict[str, Any],
+        attribution_args: dict[str, Any] = {},
     ) -> GranularFeatureAttributionStepOutput:
         r"""Performs a single attribution step for the specified attribution arguments.
 
         Args:
             attribute_fn_main_args (:obj:`dict`): Main arguments used for the attribution method. These are built from
                 model inputs at the current step of the feature attribution process.
             attribution_args (:obj:`dict`, `optional`): Additional arguments to pass to the attribution method.
@@ -91,16 +91,16 @@
             and self.method.has_convergence_delta()
         ):
             attr, deltas = attr
         source_attributions, target_attributions = get_source_target_attributions(
             attr, self.attribution_model.is_encoder_decoder
         )
         return GranularFeatureAttributionStepOutput(
-            source_attributions=source_attributions,
-            target_attributions=target_attributions,
+            source_attributions=source_attributions if source_attributions is not None else None,
+            target_attributions=target_attributions if target_attributions is not None else None,
             step_scores={"deltas": deltas} if deltas is not None else None,
         )
 
 
 class DeepLiftAttribution(GradientAttributionRegistry):
     """DeepLIFT attribution method.
```

### Comparing `inseq-0.5.0/inseq/attr/feat/internals_attribution.py` & `inseq-0.6.0/inseq/attr/feat/internals_attribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Attention-based feature attribution methods."""
 
 import logging
-from typing import Any, Dict, Optional
+from typing import Any, Optional
 
+import torch
 from captum._utils.typing import TensorOrTupleOfTensorsGeneric
-from captum.attr._utils.attribution import Attribution
 
 from ...data import MultiDimensionalFeatureAttributionStepOutput
 from ...utils import Registry
-from ...utils.typing import MultiLayerMultiUnitScoreTensor
+from ...utils.typing import InseqAttribution, MultiLayerMultiUnitScoreTensor
 from .feature_attribution import FeatureAttribution
 
 logger = logging.getLogger(__name__)
 
 
 class InternalsAttributionRegistry(FeatureAttribution, Registry):
     r"""Model Internals-based attribution method registry."""
@@ -34,15 +34,15 @@
 
 
 class AttentionWeightsAttribution(InternalsAttributionRegistry):
     """The basic attention attribution method, which retrieves the attention weights from the model."""
 
     method_name = "attention"
 
-    class AttentionWeights(Attribution):
+    class AttentionWeights(InseqAttribution):
         @staticmethod
         def has_convergence_delta() -> bool:
             return False
 
         def attribute(
             self,
             inputs: TensorOrTupleOfTensorsGeneric,
@@ -70,27 +70,35 @@
                     Tensor of cross-attention weights computed during the forward pass with shape
                     :obj:`(batch_size, n_layers, n_heads, source_seq_len, target_seq_len)`.
 
             Returns:
                 :class:`~inseq.data.MultiDimensionalFeatureAttributionStepOutput`: A step output containing attention
                 weights for each layer and head, with shape :obj:`(batch_size, seq_len, n_layers, n_heads)`.
             """
-            # We adopt the format [batch_size, sequence_length, num_layers, num_heads]
+            # We adopt the format [batch_size, sequence_length, sequence_length, num_layers, num_heads]
             # for consistency with other multi-unit methods (e.g. gradient attribution)
-            decoder_self_attentions = decoder_self_attentions[..., -1, :].clone().permute(0, 3, 1, 2)
+            decoder_self_attentions = decoder_self_attentions.to("cpu").clone().permute(0, 4, 3, 1, 2)
+            decoder_self_attentions = torch.where(
+                decoder_self_attentions == 0,
+                (torch.ones_like(decoder_self_attentions) * float("nan")),
+                decoder_self_attentions,
+            )
             if self.forward_func.is_encoder_decoder:
                 sequence_scores = {}
                 if len(inputs) > 1:
                     target_attributions = decoder_self_attentions
                 else:
                     target_attributions = None
                     sequence_scores["decoder_self_attentions"] = decoder_self_attentions
-                sequence_scores["encoder_self_attentions"] = encoder_self_attentions.clone().permute(0, 3, 4, 1, 2)
+                sequence_scores["encoder_self_attentions"] = (
+                    encoder_self_attentions.to("cpu").clone().permute(0, 4, 3, 1, 2)
+                )
+                cross_attentions = cross_attentions.to("cpu").clone().permute(0, 4, 3, 1, 2)
                 return MultiDimensionalFeatureAttributionStepOutput(
-                    source_attributions=cross_attentions[..., -1, :].clone().permute(0, 3, 1, 2),
+                    source_attributions=cross_attentions,
                     target_attributions=target_attributions,
                     sequence_scores=sequence_scores,
                     _num_dimensions=2,  # num_layers, num_heads
                 )
             else:
                 return MultiDimensionalFeatureAttributionStepOutput(
                     source_attributions=None,
@@ -100,15 +108,17 @@
 
     def __init__(self, attribution_model, **kwargs):
         super().__init__(attribution_model)
         # Attention weights will be passed to the attribute_step method
         self.use_attention_weights = True
         # Does not rely on predicted output (i.e. decoding strategy agnostic)
         self.use_predicted_target = False
+        # Needs only the final generation step to extract scores
+        self.is_final_step_method = True
         self.method = self.AttentionWeights(attribution_model)
 
     def attribute_step(
         self,
-        attribute_fn_main_args: Dict[str, Any],
-        attribution_args: Dict[str, Any],
+        attribute_fn_main_args: dict[str, Any],
+        attribution_args: dict[str, Any],
     ) -> MultiDimensionalFeatureAttributionStepOutput:
         return self.method.attribute(**attribute_fn_main_args, **attribution_args)
```

### Comparing `inseq-0.5.0/inseq/attr/feat/ops/discretized_integrated_gradients.py` & `inseq-0.6.0/inseq/attr/feat/ops/discretized_integrated_gradients.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 # LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 # OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 from pathlib import Path
-from typing import Any, Callable, List, Tuple, Union
+from typing import Any, Callable, Union
 
 import torch
 from captum._utils.common import (
     _expand_additional_forward_args,
     _expand_target,
     _format_additional_forward_args,
     _format_output,
@@ -47,15 +47,15 @@
         super().__init__(forward_func, multiply_by_inputs)
         self.path_builder = None
 
     def load_monotonic_path_builder(
         self,
         model_name: str,
         vocabulary_embeddings: VocabularyEmbeddingsTensor,
-        special_tokens: List[int],
+        special_tokens: list[int],
         cache_dir: Path = INSEQ_ARTIFACTS_CACHE / "dig_knn",
         embedding_scaling: int = 1,
         **kwargs,
     ) -> None:
         """Loads the Discretized Integrated Gradients (DIG) path builder."""
         self.path_builder = MonotonicPathBuilder.load(
             model_name,
@@ -63,15 +63,15 @@
             special_tokens=special_tokens,
             cache_dir=cache_dir,
             embedding_scaling=embedding_scaling,
             **kwargs,
         )
 
     @staticmethod
-    def get_inputs_baselines(scaled_features_tpl: Tuple[Tensor, ...], n_steps: int) -> Tuple[Tensor, ...]:
+    def get_inputs_baselines(scaled_features_tpl: tuple[Tensor, ...], n_steps: int) -> tuple[Tensor, ...]:
         # Baseline and inputs are reversed in the path builder
         # For every element in the batch, the first embedding of the sub-tensor
         # of shape (n_steps x embedding_dim) is the baseline, the last is the input.
         n_examples = scaled_features_tpl[0].shape[0] // n_steps
         baselines = tuple(
             torch.cat(
                 [features[i, :, :].unsqueeze(0) for i in range(0, n_steps * n_examples, n_steps)],
@@ -92,15 +92,15 @@
         baselines: BaselineType = None,
         target: TargetType = None,
         additional_forward_args: Any = None,
         n_steps: int = 50,
         method: str = "greedy",
         internal_batch_size: Union[None, int] = None,
         return_convergence_delta: bool = False,
-    ) -> Union[TensorOrTupleOfTensorsGeneric, Tuple[TensorOrTupleOfTensorsGeneric, Tensor]]:
+    ) -> Union[TensorOrTupleOfTensorsGeneric, tuple[TensorOrTupleOfTensorsGeneric, Tensor]]:
         n_examples = inputs[0].shape[0]
         # Keeps track whether original input is a tuple or not before
         # converting it into a tuple.
         is_inputs_tuple = _is_tuple(inputs)
 
         inputs, baselines = _format_input_baseline(inputs, baselines)
 
@@ -142,19 +142,19 @@
                 target=target,
             )
             return _format_output(is_inputs_tuple, attributions), delta
         return _format_output(is_inputs_tuple, attributions)
 
     def _attribute(
         self,
-        scaled_features_tpl: Tuple[Tensor, ...],
+        scaled_features_tpl: tuple[Tensor, ...],
         target: TargetType = None,
         additional_forward_args: Any = None,
         n_steps: int = 50,
-    ) -> Tuple[Tensor, ...]:
+    ) -> tuple[Tensor, ...]:
         additional_forward_args = _format_additional_forward_args(additional_forward_args)
         input_additional_args = (
             _expand_additional_forward_args(additional_forward_args, n_steps)
             if additional_forward_args is not None
             else None
         )
         expanded_target = _expand_target(target, n_steps)
```

### Comparing `inseq-0.5.0/inseq/attr/feat/ops/lime.py` & `inseq-0.6.0/inseq/attr/feat/ops/lime.py`

 * *Files identical despite different names*

### Comparing `inseq-0.5.0/inseq/attr/feat/ops/monotonic_path_builder.py` & `inseq-0.6.0/inseq/attr/feat/ops/monotonic_path_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """Monotonic path builder for Discretized Integrated Gradients (DIG)."""
 
 import logging
 import os
 from enum import Enum
 from itertools import islice
 from pathlib import Path
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, Optional, Union
 
 import torch
 from jaxtyping import Float, Int
 
 from ....utils import is_joblib_available, is_scikitlearn_available
 
 if is_joblib_available():
@@ -52,15 +52,15 @@
 
 class UnknownPathBuildingStrategy(Exception):
     """Raised when a strategy for pathbuilding is not valid."""
 
     def __init__(
         self,
         strategy: str,
-        *args: Tuple[Any],
+        *args: tuple[Any],
     ) -> None:
         """Initialize the exception."""
         super().__init__(
             (
                 f"Unknown strategy: {strategy}.\nAvailable strategies: "
                 f"{','.join([s.value for s in PathBuildingStrategies])}"
             ),
@@ -71,15 +71,15 @@
 class MonotonicPathBuilder:
     """Build monotonic paths between two token embeddings."""
 
     def __init__(
         self,
         vocabulary_embeddings: VocabularyEmbeddingsTensor,
         knn_graph: "csr_matrix",
-        special_tokens: List[int] = [],
+        special_tokens: list[int] = [],
     ) -> None:
         """Initialize the monotonic path builder."""
         self.vocabulary_embeddings = vocabulary_embeddings
         self.knn_graph = knn_graph
         self.special_tokens = special_tokens
 
     @staticmethod
@@ -108,15 +108,15 @@
         n_neighbors: int = 50,
         mode: str = "distance",
         n_jobs: int = -1,
         save_cache: bool = True,
         overwrite_cache: bool = False,
         cache_dir: Path = INSEQ_ARTIFACTS_CACHE / "path_knn",
         vocabulary_embeddings: Optional[VocabularyEmbeddingsTensor] = None,
-        special_tokens: List[int] = [],
+        special_tokens: list[int] = [],
         embedding_scaling: int = 1,
     ) -> "MonotonicPathBuilder":
         """Load a cached monotonic path builder from a model name, or compute it if it does not exist."""
         cache_filename = os.path.join(cache_dir, f"{model_name.replace('/', '__')}_{n_neighbors}.pkl")
         if vocabulary_embeddings is None:
             logger.warning(
                 "Since no token embeddings are passed, a cached file is expected. "
@@ -184,15 +184,15 @@
 
     def find_path(
         self,
         word_idx: int,
         baseline_idx: int,
         n_steps: Optional[int] = 30,
         strategy: Optional[str] = "greedy",
-    ) -> List[int]:
+    ) -> list[int]:
         """Find a monotonic path from a word to a baseline."""
         # if word_idx is a special token copy it and return
         if word_idx in self.special_tokens:
             return [word_idx] * (n_steps - 1)
         word_path = [word_idx]
         for _ in range(n_steps - 2):
             word_path.append(
@@ -203,15 +203,15 @@
                     strategy=strategy,
                     n_steps=n_steps,
                 )
             )
         return word_path
 
     def build_monotonic_path_embedding(
-        self, word_path: List[int], baseline_idx: int, n_steps: int = 30
+        self, word_path: list[int], baseline_idx: int, n_steps: int = 30
     ) -> Float[torch.Tensor, "n_steps embed_size"]:
         """Build a monotonic path embedding from a word path."""
         baseline_vec = self.vocabulary_embeddings[baseline_idx]
         monotonic_embs = [self.vocabulary_embeddings[word_path[0]]]
         for idx in range(len(word_path) - 1):
             monotonic_embs.append(
                 self.make_monotonic_vec(
@@ -227,15 +227,15 @@
         assert self.check_monotonic(monotonic_embs), "The embeddings are not monotonic"
         return torch.stack(monotonic_embs)
 
     def get_closest_word(
         self,
         word_idx: int,
         baseline_idx: int,
-        word_path: List[int],
+        word_path: list[int],
         strategy: str = "greedy",
         n_steps: int = 30,
     ) -> int:
         """Get the closest word to the current word in the path."""
         # If (for some reason) we do select the ref_idx as the previous anchor word,
         # then all further anchor words should be ref_idx
         if word_idx == baseline_idx:
```

### Comparing `inseq-0.5.0/inseq/attr/feat/ops/sequential_integrated_gradients.py` & `inseq-0.6.0/inseq/attr/feat/ops/sequential_integrated_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
 # LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 # OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 import typing
-from typing import Any, Callable, List, Tuple, Union
+from typing import Any, Callable, Union
 
 import torch
 from captum._utils.common import (
     _expand_additional_forward_args,
     _expand_target,
     _format_additional_forward_args,
     _format_output,
@@ -134,30 +134,30 @@
         target: TargetType = None,
         additional_forward_args: Any = None,
         n_steps: int = 50,
         method: str = "gausslegendre",
         internal_batch_size: Union[None, int] = None,
         *,
         return_convergence_delta: Literal[True],
-    ) -> Tuple[TensorOrTupleOfTensorsGeneric, Tensor]:
+    ) -> tuple[TensorOrTupleOfTensorsGeneric, Tensor]:
         ...
 
     def attribute(  # type: ignore
         self,
         inputs: TensorOrTupleOfTensorsGeneric,
         baselines: BaselineType = None,
         target: TargetType = None,
         additional_forward_args: Any = None,
         n_steps: int = 50,
         method: str = "gausslegendre",
         internal_batch_size: Union[None, int] = None,
         return_convergence_delta: bool = False,
     ) -> Union[
         TensorOrTupleOfTensorsGeneric,
-        Tuple[TensorOrTupleOfTensorsGeneric, Tensor],
+        tuple[TensorOrTupleOfTensorsGeneric, Tensor],
     ]:
         r"""
         This method attributes the output of the model with given target index
         (in case it is provided, otherwise it assumes that output is a
         scalar) to the inputs of the model using the approach described above.
 
         In addition to that it also returns, if `return_convergence_delta` is
@@ -363,23 +363,23 @@
                 target=target,
             )
             return _format_output(is_inputs_tuple, attributions), delta
         return _format_output(is_inputs_tuple, attributions)
 
     def _attribute(
         self,
-        inputs: Tuple[Tensor, ...],
-        baselines: Tuple[Union[Tensor, int, float], ...],
+        inputs: tuple[Tensor, ...],
+        baselines: tuple[Union[Tensor, int, float], ...],
         target: TargetType = None,
         additional_forward_args: Any = None,
         n_steps: int = 50,
         method: str = "gausslegendre",
         idx: int = None,
-        step_sizes_and_alphas: Union[None, Tuple[List[float], List[float]]] = None,
-    ) -> Tuple[Tensor, ...]:
+        step_sizes_and_alphas: Union[None, tuple[list[float], list[float]]] = None,
+    ) -> tuple[Tensor, ...]:
         if step_sizes_and_alphas is None:
             # retrieve step size and scaling factor for specified
             # approximation method
             step_sizes_func, alphas_func = approximation_parameters(method)
             step_sizes, alphas = step_sizes_func(n_steps), alphas_func(n_steps)
         else:
             step_sizes, alphas = step_sizes_and_alphas
```

### Comparing `inseq-0.5.0/inseq/attr/step_functions.py` & `inseq-0.6.0/inseq/attr/step_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Protocol, Tuple, Union
+from inspect import signature
+from typing import TYPE_CHECKING, Any, Optional, Protocol, Union
 
 import torch
 import torch.nn.functional as F
 from transformers.modeling_outputs import ModelOutput
 
 from ..data import FeatureAttributionInput
 from ..data.aggregation_functions import DEFAULT_ATTRIBUTION_AGGREGATE_DICT
@@ -80,43 +81,43 @@
     ) -> SingleScorePerStepTensor:
         ...
 
 
 def logit_fn(args: StepFunctionArgs) -> SingleScorePerStepTensor:
     """Compute the logit of the target_ids from the model's output logits."""
     logits = args.attribution_model.output2logits(args.forward_output)
-    target_ids = args.target_ids.reshape(logits.shape[0], 1)
+    target_ids = args.target_ids.reshape(logits.shape[0], 1).to(logits.device)
     return logits.gather(-1, target_ids).squeeze(-1)
 
 
 def probability_fn(args: StepFunctionArgs, logprob: bool = False) -> SingleScorePerStepTensor:
     """Compute the probabilty of target_ids from the model's output logits."""
     logits = args.attribution_model.output2logits(args.forward_output)
-    target_ids = args.target_ids.reshape(logits.shape[0], 1)
+    target_ids = args.target_ids.reshape(logits.shape[0], 1).to(logits.device)
     logits = logits.softmax(dim=-1) if not logprob else logits.log_softmax(dim=-1)
     # Extracts the ith score from the softmax output over the vocabulary (dim -1 of the logits)
     # where i is the value of the corresponding index in target_ids.
     return logits.gather(-1, target_ids).squeeze(-1)
 
 
 def entropy_fn(args: StepFunctionArgs) -> SingleScorePerStepTensor:
     """Compute the entropy of the model's output distribution."""
     logits = args.attribution_model.output2logits(args.forward_output)
-    entropy = torch.zeros(logits.size(0))
+    entropy = torch.zeros(logits.size(0)).to(logits.device)
     for i in range(logits.size(0)):
         entropy[i] = torch.distributions.Categorical(logits=logits[i]).entropy()
     return entropy
 
 
 def crossentropy_fn(args: StepFunctionArgs) -> SingleScorePerStepTensor:
     """Compute the cross entropy between the target_ids and the logits.
     See: https://github.com/ZurichNLP/nmtscore/blob/master/src/nmtscore/models/m2m100.py#L99.
     """
     logits = args.attribution_model.output2logits(args.forward_output)
-    return F.cross_entropy(logits, args.target_ids, reduction="none").squeeze(-1)
+    return F.cross_entropy(logits, args.target_ids.to(logits.device), reduction="none").squeeze(-1)
 
 
 def perplexity_fn(args: StepFunctionArgs) -> SingleScorePerStepTensor:
     """Compute perplexity of the target_ids from the logits.
     Perplexity is the weighted branching factor. If we have a perplexity of 100, it means that whenever the model is
     trying to guess the next word it is as confused as if it had to pick between 100 words.
     Reference: https://chiaracampagnola.io/2020/05/17/perplexity-in-language-models/.
@@ -125,15 +126,15 @@
 
 
 @contrast_fn_docstring()
 def contrast_logits_fn(
     args: StepFunctionArgs,
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     contrast_force_inputs: bool = False,
 ):
     """Returns the logit of a generation target given contrastive context or target prediction alternative.
     If only ``contrast_targets`` are specified, the logit of the contrastive prediction is computed given same
     context. The logit for the same token given contrastive source/target preceding context can also be computed
     using ``contrast_sources`` without specifying ``contrast_targets``.
     """
@@ -148,15 +149,15 @@
 
 
 @contrast_fn_docstring()
 def contrast_prob_fn(
     args: StepFunctionArgs,
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     logprob: bool = False,
     contrast_force_inputs: bool = False,
 ):
     """Returns the probability of a generation target given contrastive context or target prediction alternative.
     If only ``contrast_targets`` are specified, the probability of the contrastive prediction is computed given same
     context. The probability for the same token given contrastive source/target preceding context can also be computed
     using ``contrast_sources`` without specifying ``contrast_targets``.
@@ -172,39 +173,39 @@
 
 
 @contrast_fn_docstring()
 def pcxmi_fn(
     args: StepFunctionArgs,
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     contrast_force_inputs: bool = False,
 ) -> SingleScorePerStepTensor:
     """Compute the pointwise conditional cross-mutual information (P-CXMI) of target ids given original and contrastive
     input options. The P-CXMI is defined as the negative log-ratio between the conditional probability of the target
     given the original input and the conditional probability of the target given the contrastive input, as defined
     by `Yin et al. (2021) <https://arxiv.org/abs/2109.07446>`__.
     """
     original_probs = probability_fn(args)
     contrast_probs = contrast_prob_fn(
         args=args,
         contrast_sources=contrast_sources,
         contrast_targets=contrast_targets,
         contrast_targets_alignments=contrast_targets_alignments,
         contrast_force_inputs=contrast_force_inputs,
-    )
+    ).to(original_probs.device)
     return -torch.log2(torch.div(original_probs, contrast_probs))
 
 
 @contrast_fn_docstring()
 def kl_divergence_fn(
     args: StepFunctionArgs,
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     top_k: int = 0,
     top_p: float = 1.0,
     min_tokens_to_keep: int = 1,
     contrast_force_inputs: bool = False,
 ) -> SingleScorePerStepTensor:
     """Compute the pointwise Kullback-Leibler divergence of target ids given original and contrastive input options.
     The KL divergence is the expectation of the log difference between the probabilities of regular (P) and contrastive
@@ -232,15 +233,15 @@
         contrast_targets_alignments=contrast_targets_alignments,
         return_contrastive_target_ids=False,
         return_contrastive_batch=True,
     )
     c_forward_output = args.attribution_model.get_forward_output(
         contrast_inputs.batch, use_embeddings=args.attribution_model.is_encoder_decoder
     )
-    contrast_logits: torch.Tensor = args.attribution_model.output2logits(c_forward_output)
+    contrast_logits: torch.Tensor = args.attribution_model.output2logits(c_forward_output).to(original_logits.device)
     filtered_original_logits, filtered_contrast_logits = filter_logits(
         original_logits=original_logits,
         contrast_logits=contrast_logits,
         top_p=top_p,
         top_k=top_k,
         min_tokens_to_keep=min_tokens_to_keep,
     )
@@ -255,15 +256,15 @@
 
 
 @contrast_fn_docstring()
 def contrast_prob_diff_fn(
     args: StepFunctionArgs,
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     logprob: bool = False,
     contrast_force_inputs: bool = False,
 ):
     """Returns the difference between next step probability for a candidate generation target vs. a contrastive
     alternative. Can be used as attribution target to answer the question: "Which features were salient in the
     choice of picking the selected token rather than its contrastive alternative?". Follows the implementation
     of `Yin and Neubig (2022) <https://aclanthology.org/2022.emnlp-main.14>`__. Can also be used to compute the
@@ -274,46 +275,46 @@
     contrast_probs = contrast_prob_fn(
         args=args,
         contrast_sources=contrast_sources,
         contrast_targets=contrast_targets,
         contrast_targets_alignments=contrast_targets_alignments,
         logprob=logprob,
         contrast_force_inputs=contrast_force_inputs,
-    )
+    ).to(model_probs.device)
     return model_probs - contrast_probs
 
 
 @contrast_fn_docstring()
 def contrast_logits_diff_fn(
     args: StepFunctionArgs,
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     contrast_force_inputs: bool = False,
 ):
     """Equivalent to ``contrast_prob_diff_fn`` but for logits. The original target function used in
     `Yin and Neubig (2022) <https://aclanthology.org/2022.emnlp-main.14>`__
     """
     model_logits = logit_fn(args)
     contrast_logits = contrast_logits_fn(
         args=args,
         contrast_sources=contrast_sources,
         contrast_targets=contrast_targets,
         contrast_targets_alignments=contrast_targets_alignments,
         contrast_force_inputs=contrast_force_inputs,
-    )
+    ).to(model_logits.device)
     return model_logits - contrast_logits
 
 
 @contrast_fn_docstring()
 def in_context_pvi_fn(
     args: StepFunctionArgs,
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     contrast_force_inputs: bool = False,
 ):
     """Returns the in-context pointwise V-usable information as defined by `Lu et al. (2023)
     <https://arxiv.org/abs/2310.12300>`__. In-context PVI is a variant of P-CXMI that captures the amount of usable
     information in a given contextual example, i.e. how much context information contributes to model's prediction.
     In-context PVI was used by `Lu et al. (2023) <https://arxiv.org/abs/2310.12300>`__ to estimate example difficulty
     for a given model, and by `Prasad et al. (2023) <https://arxiv.org/abs/2304.10703>`__ to measure the
@@ -325,15 +326,15 @@
     contrast_logprob = contrast_prob_fn(
         args=args,
         contrast_sources=contrast_sources,
         contrast_targets=contrast_targets,
         contrast_targets_alignments=contrast_targets_alignments,
         logprob=True,
         contrast_force_inputs=contrast_force_inputs,
-    )
+    ).to(orig_logprob.device)
     return -orig_logprob + contrast_logprob
 
 
 def mc_dropout_prob_avg_fn(
     args: StepFunctionArgs,
     n_mcd_steps: int = 5,
     logprob: bool = False,
@@ -357,15 +358,15 @@
     noisy_probs = []
     for _ in range(n_mcd_steps):
         aux_batch = args.attribution_model.formatter.convert_args_to_batch(args)
         aux_output = args.attribution_model.get_forward_output(
             aux_batch, use_embeddings=args.attribution_model.is_encoder_decoder
         )
         args.forward_output = aux_output
-        noisy_prob = probability_fn(args, logprob=logprob)
+        noisy_prob = probability_fn(args, logprob=logprob).to(orig_prob.device)
         noisy_probs.append(noisy_prob)
     # Z-score the original based on the mean and standard deviation of MC dropout predictions
     return (orig_prob - torch.stack(noisy_probs).mean(0)).div(torch.stack(noisy_probs).std(0))
 
 
 def top_p_size_fn(
     args: StepFunctionArgs,
@@ -373,15 +374,15 @@
 ):
     """Returns the number of tokens that have cumulative probability above :obj:`top_p` in the model's output logits.
 
     Args:
         top_p (:obj:`float`): The cumulative probability threshold to use for filtering the logits.
     """
     logits: torch.Tensor = args.attribution_model.output2logits(args.forward_output)
-    indices_to_remove = top_p_logits_mask(logits, top_p, 1)
+    indices_to_remove = top_p_logits_mask(logits, top_p, 1).to(logits.device)
     logits = logits.masked_select(~indices_to_remove)[None, ...]
     return torch.tensor(logits.size(-1))[None, ...]
 
 
 STEP_SCORES_MAP = {
     "logit": logit_fn,
     "probability": probability_fn,
@@ -414,59 +415,58 @@
     check_is_step_function(score_identifier)
     return STEP_SCORES_MAP[score_identifier]
 
 
 def get_step_scores(
     score_identifier: str,
     step_fn_args: StepFunctionArgs,
-    step_fn_extra_args: Dict[str, Any] = {},
+    step_fn_extra_args: dict[str, Any] = {},
 ) -> SingleScorePerStepTensor:
     """Returns step scores for the target tokens in the batch."""
     return get_step_function(score_identifier)(step_fn_args, **step_fn_extra_args)
 
 
 def get_step_scores_args(
-    score_identifiers: List[str], kwargs: Dict[str, Any], default_args: Optional[Dict[str, Any]] = None
-) -> Dict[str, Any]:
+    score_identifiers: list[str], kwargs: dict[str, Any], default_args: Optional[dict[str, Any]] = None
+) -> dict[str, Any]:
     step_scores_args = {}
     for step_fn_id in score_identifiers:
         step_fn = get_step_function(step_fn_id)
         step_scores_args.update(
             **extract_signature_args(
                 kwargs,
                 step_fn,
                 exclude_args=default_args,
                 return_remaining=False,
             )
         )
     return step_scores_args
 
 
-def list_step_functions() -> List[str]:
+def list_step_functions() -> list[str]:
     """Lists identifiers for all available step scores. One or more step scores identifiers can be passed to the
     :meth:`~inseq.models.AttributionModel.attribute` method either to compute scores while attributing (``step_scores``
     parameter), or as target function for the attribution, if supported by the attribution method (``attributed_fn``
     parameter).
     """
     return list(STEP_SCORES_MAP.keys())
 
 
 def register_step_function(
     fn: StepFunction,
     identifier: str,
-    aggregate_map: Optional[Dict[str, str]] = None,
+    aggregate_map: Optional[dict[str, str]] = None,
     overwrite: bool = False,
 ) -> None:
     """Registers a function to be used to compute step scores and store them in the
     :class:`~inseq.data.attribution.FeatureAttributionOutput` object. Registered step functions can also be used as
     attribution targets by gradient-based feature attribution methods.
 
     Args:
-        fn (:obj:`callable`): The function to be used to compute step scores. Default parameters (use kwargs to capture
-        unused ones when defining your function):
+        fn (:obj:`callable`): The function to be used to compute step scores. Default parameters (use kwargs to capture unused ones when defining your function):
 
             - :obj:`attribution_model`: an :class:`~inseq.models.AttributionModel` instance, corresponding to the model
                 used for computing the score.
 
             - :obj:`forward_output`: the output of the forward pass from the attribution model.
 
             - :obj:`encoder_input_ids`, :obj:`decoder_input_ids`, :obj:`encoder_input_embeds`,
@@ -496,7 +496,11 @@
         logger.warning(f"Overwriting {identifier} step function.")
     STEP_SCORES_MAP[identifier] = fn
     if isinstance(aggregate_map, dict):
         for agg_name, aggregation_fn_identifier in aggregate_map.items():
             if agg_name not in DEFAULT_ATTRIBUTION_AGGREGATE_DICT["step_scores"]:
                 DEFAULT_ATTRIBUTION_AGGREGATE_DICT["step_scores"][agg_name] = {}
             DEFAULT_ATTRIBUTION_AGGREGATE_DICT["step_scores"][agg_name][identifier] = aggregation_fn_identifier
+
+
+def is_contrastive_step_function(step_fn_id: str) -> bool:
+    return "contrast_targets" in signature(get_step_function(step_fn_id)).parameters
```

### Comparing `inseq-0.5.0/inseq/commands/base.py` & `inseq-0.6.0/inseq/commands/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import dataclasses
 from abc import ABC, abstractstaticmethod
 from argparse import Namespace
-from typing import Any, Iterable, NewType, Union
+from collections.abc import Iterable
+from typing import Any, NewType, Union
 
 from ..utils import InseqArgumentParser
 
 DataClassType = NewType("DataClassType", Any)
 OneOrMoreDataClasses = Union[DataClassType, Iterable[DataClassType]]
```

### Comparing `inseq-0.5.0/inseq/commands/cli.py` & `inseq-0.6.0/inseq/commands/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Adapted from https://github.com/huggingface/transformers/blob/main/src/transformers/commands/transformers_cli.py."""
 import sys
 
 from ..utils import InseqArgumentParser
 from .attribute import AttributeCommand
+from .attribute_context import AttributeContextCommand
 from .attribute_dataset import AttributeDatasetCommand
+from .base import BaseCLICommand
 
-COMMANDS = [AttributeCommand, AttributeDatasetCommand]
+COMMANDS: list[BaseCLICommand] = [AttributeCommand, AttributeDatasetCommand, AttributeContextCommand]
 
 
 def main():
     parser = InseqArgumentParser(prog="Inseq CLI tool", usage="inseq <COMMAND> [<ARGS>]")
     command_parser = parser.add_subparsers(title="Inseq CLI command helpers")
 
     for command_type in COMMANDS:
```

### Comparing `inseq-0.5.0/inseq/data/__init__.py` & `inseq-0.6.0/inseq/data/__init__.py`

 * *Files identical despite different names*

### Comparing `inseq-0.5.0/inseq/data/aggregation_functions.py` & `inseq-0.6.0/inseq/data/aggregation_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from abc import abstractmethod
-from typing import List, Tuple, Union
+from typing import Union
 
 import torch
 from torch.linalg import vector_norm
 
 from ..utils import Registry, available_classes
 from ..utils.typing import (
     ScoreTensor,
@@ -33,15 +33,15 @@
     def __init__(self):
         self.takes_single_tensor: bool = True
         self.takes_sequence_scores: bool = False
 
     @abstractmethod
     def __call__(
         self,
-        scores: Union[torch.Tensor, Tuple[torch.Tensor, ...]],
+        scores: Union[torch.Tensor, tuple[torch.Tensor, ...]],
         dim: int,
         **kwargs,
     ) -> ScoreTensor:
         pass
 
 
 class MeanAggregationFunction(AggregationFunction):
@@ -108,10 +108,10 @@
             "kl_divergence": "sum",
             "mc_dropout_prob_avg": "prod",
         }
     },
 }
 
 
-def list_aggregation_functions() -> List[str]:
+def list_aggregation_functions() -> list[str]:
     """Lists identifiers for all available aggregation functions."""
     return available_classes(AggregationFunction)
```

### Comparing `inseq-0.5.0/inseq/data/aggregator.py` & `inseq-0.6.0/inseq/data/aggregator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Callable, List, Optional, Sequence, Tuple, Type, TypeVar, Union
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Callable, Optional, TypeVar, Union
 
 import torch
 
 from ..utils import (
     Registry,
     aggregate_contiguous,
     aggregate_token_pair,
     aggregate_token_sequence,
     available_classes,
     extract_signature_args,
+    validate_indices,
 )
 from ..utils import normalize as normalize_fn
-from ..utils.typing import IndexSpan, TokenWithId
+from ..utils.typing import IndexSpan, OneOrMoreIndices, TokenWithId
 from .aggregation_functions import AggregationFunction
 from .data_utils import TensorWrapper
 
 if TYPE_CHECKING:
     from .attribution import FeatureAttributionSequenceOutput
 
 
@@ -121,15 +123,15 @@
         """
         pass
 
 
 def _get_aggregators_from_id(
     aggregator: str,
     aggregate_fn: Optional[str] = None,
-) -> Tuple[Type[Aggregator], Optional[AggregationFunction]]:
+) -> tuple[type[Aggregator], Optional[AggregationFunction]]:
     if aggregator in available_classes(Aggregator):
         aggregator = Aggregator.available_classes()[aggregator]
     elif aggregator in available_classes(AggregationFunction):
         if aggregate_fn is not None:
             raise ValueError(
                 "If aggregator is a string identifying an aggregation function, aggregate_fn should not be provided."
             )
@@ -151,19 +153,19 @@
     aggregate_fn = AggregationFunction.available_classes()[aggregate_fn]()
     return aggregator, aggregate_fn
 
 
 class AggregatorPipeline:
     def __init__(
         self,
-        aggregators: List[Union[str, Type[Aggregator]]],
-        aggregate_fn: Optional[List[Union[str, Callable]]] = None,
+        aggregators: list[Union[str, type[Aggregator]]],
+        aggregate_fn: Optional[list[Union[str, Callable]]] = None,
     ):
-        self.aggregators: List[Type[Aggregator]] = []
-        self.aggregate_fn: List[Callable] = []
+        self.aggregators: list[type[Aggregator]] = []
+        self.aggregate_fn: list[Callable] = []
         if aggregate_fn is not None:
             if len(aggregate_fn) != len(aggregators):
                 raise ValueError(
                     "If custom aggregate_fn are provided, their number should match the number of aggregators."
                 )
         for idx in range(len(aggregators)):
             curr_aggregator = aggregators[idx]
@@ -192,24 +194,24 @@
             )
         if do_post_aggregation_checks:
             for aggregator in self.aggregators:
                 aggregator.end_aggregation_hook(tensors, **kwargs)
         return tensors
 
 
-AggregatorInput = Union[AggregatorPipeline, Type[Aggregator], str, Sequence[Union[str, Type[Aggregator]]], None]
+AggregatorInput = Union[AggregatorPipeline, type[Aggregator], str, Sequence[Union[str, type[Aggregator]]], None]
 
 
-def list_aggregators() -> List[str]:
+def list_aggregators() -> list[str]:
     """Lists identifiers for all available aggregators."""
     return available_classes(Aggregator)
 
 
 class AggregableMixin(ABC):
-    _aggregator: Union[AggregatorPipeline, Type[Aggregator]]
+    _aggregator: Union[AggregatorPipeline, type[Aggregator]]
 
     def aggregate(
         self: AggregableMixinClass,
         aggregator: AggregatorInput = None,
         aggregate_fn: Union[str, Sequence[str], None] = None,
         do_pre_aggregation_checks: bool = True,
         do_post_aggregation_checks: bool = True,
@@ -300,15 +302,15 @@
         return attr.__class__(**aggregated_sequence_attribution_fields)
 
     @classmethod
     def _process_attribution_scores(
         cls,
         attr: "FeatureAttributionSequenceOutput",
         aggregate_fn: AggregationFunction,
-        select_idx: Union[int, Tuple[int, int], List[int], None] = None,
+        select_idx: Optional[OneOrMoreIndices] = None,
         normalize: bool = True,
         **kwargs,
     ):
         fn_kwargs = extract_signature_args(kwargs, aggregate_fn)
         # If select_idx is a single int, no aggregation is performed
         do_aggregate = not isinstance(select_idx, int)
         has_source = attr.source_attributions is not None
@@ -361,29 +363,29 @@
         return attr.target
 
     @classmethod
     def aggregate_source_attributions(
         cls,
         attr: "FeatureAttributionSequenceOutput",
         aggregate_fn: AggregationFunction,
-        select_idx: Union[int, Tuple[int, int], List[int], None] = None,
+        select_idx: Optional[OneOrMoreIndices] = None,
         normalize: bool = True,
         **kwargs,
     ):
         if attr.source_attributions is None:
             return attr.source_attributions
         scores = cls._process_attribution_scores(attr, aggregate_fn, select_idx, normalize, **kwargs)
         return scores[0] if attr.target_attributions is not None else scores
 
     @classmethod
     def aggregate_target_attributions(
         cls,
         attr: "FeatureAttributionSequenceOutput",
         aggregate_fn: AggregationFunction,
-        select_idx: Union[int, Tuple[int, int], List[int], None] = None,
+        select_idx: Optional[OneOrMoreIndices] = None,
         normalize: bool = True,
         **kwargs,
     ):
         if attr.target_attributions is None:
             return attr.target_attributions
         scores = cls._process_attribution_scores(attr, aggregate_fn, select_idx, normalize, **kwargs)
         return scores[1] if attr.source_attributions is not None else scores
@@ -393,15 +395,15 @@
         return attr.step_scores
 
     @classmethod
     def aggregate_sequence_scores(
         cls,
         attr: "FeatureAttributionSequenceOutput",
         aggregate_fn: AggregationFunction,
-        select_idx: Union[int, Tuple[int, int], List[int], None] = None,
+        select_idx: Optional[OneOrMoreIndices] = None,
         **kwargs,
     ):
         if aggregate_fn.takes_sequence_scores:
             return attr.sequence_scores
         fn_kwargs = extract_signature_args(kwargs, aggregate_fn)
         new_sequence_scores = {}
         for scores_id, seq_scores in attr.sequence_scores.items():
@@ -434,62 +436,28 @@
             for step_score in attr.step_scores.values():
                 assert len(step_score) == attr.attr_pos_end - attr.attr_pos_start
 
     @staticmethod
     def _filter_scores(
         scores: torch.Tensor,
         dim: int = -1,
-        indices: Union[int, Tuple[int, int], List[int], None] = None,
+        indices: Optional[OneOrMoreIndices] = None,
     ) -> torch.Tensor:
-        n_units = scores.shape[dim]
-
-        if hasattr(indices, "__iter__"):
-            if len(indices) == 0:
-                raise RuntimeError("At least two indices must be specified for aggregation.")
-            if len(indices) == 1:
-                indices = indices[0]
-
+        indexed = scores.index_select(dim, validate_indices(scores, dim, indices).to(scores.device))
         if isinstance(indices, int):
-            if indices not in range(-n_units, n_units):
-                raise IndexError(f"Index out of range. Scores only have {n_units} units.")
-            indices = indices if indices >= 0 else n_units + indices
-            return scores.select(dim, torch.tensor(indices, device=scores.device))
-        else:
-            if indices is None:
-                indices = (0, n_units)
-                logger.info("No indices specified for extraction. Using all units by default.")
-
-            # Convert negative indices to positive indices
-            if hasattr(indices, "__iter__"):
-                indices = type(indices)([h_idx if h_idx >= 0 else n_units + h_idx for h_idx in indices])
-            if not hasattr(indices, "__iter__") or (
-                len(indices) == 2 and isinstance(indices, tuple) and indices[0] >= indices[1]
-            ):
-                raise RuntimeError(
-                    "A (start, end) tuple of indices representing a span, a list of individual indices"
-                    " or a single index must be specified for select_idx."
-                )
-            max_idx_val = n_units if isinstance(indices, list) else n_units + 1
-            if not all(h in range(-n_units, max_idx_val) for h in indices):
-                raise IndexError("One or more index out of range. Scores only have {n_units} units.")
-            if len(set(indices)) != len(indices):
-                raise IndexError("Duplicate indices are not allowed.")
-            if isinstance(indices, tuple):
-                scores = scores.index_select(dim, torch.arange(indices[0], indices[1]))
-            else:
-                scores = scores.index_select(dim, torch.tensor(indices, device=scores.device))
-            return scores
+            return indexed.squeeze(dim)
+        return indexed
 
     @staticmethod
     def _aggregate_scores(
-        scores: Union[torch.Tensor, Tuple[torch.Tensor, ...]],
+        scores: Union[torch.Tensor, tuple[torch.Tensor, ...]],
         aggregate_fn: AggregationFunction,
         dim: int = -1,
         **kwargs,
-    ) -> Union[torch.Tensor, Tuple[torch.Tensor, ...]]:
+    ) -> Union[torch.Tensor, tuple[torch.Tensor, ...]]:
         if isinstance(scores, tuple) and aggregate_fn.takes_single_tensor:
             return tuple(aggregate_fn(score, dim=dim, **kwargs) for score in scores)
         return aggregate_fn(scores, dim=dim, **kwargs)
 
 
 class ContiguousSpanAggregator(SequenceAttributionAggregator):
     """Reduces sequence attributions across one or more contiguous spans.
@@ -542,15 +510,15 @@
             for multiple contiguous spans.
         """
         source_spans = cls.format_spans(source_spans)
         target_spans = cls.format_spans(target_spans)
         return super().aggregate(attr, source_spans=source_spans, target_spans=target_spans, **kwargs)
 
     @staticmethod
-    def format_spans(spans) -> List[Tuple[int, int]]:
+    def format_spans(spans) -> list[tuple[int, int]]:
         if not spans:
             return spans
         return [spans] if isinstance(spans[0], int) else spans
 
     @classmethod
     def validate_spans(cls, span_sequence: "FeatureAttributionSequenceOutput", spans: Optional[IndexSpan] = None):
         if not spans:
@@ -575,15 +543,15 @@
         # First aggregate alongside the y-axis
         scores_aggregated_y = aggregate_contiguous(scores, y_spans, aggregate_fn, aggregate_dim=1)
         # Then aggregate alonside the x-axis
         scores_aggregated_x = aggregate_contiguous(scores_aggregated_y, x_spans, aggregate_fn, aggregate_dim=0)
         return scores_aggregated_x
 
     @staticmethod
-    def _relativize_target_spans(spans: List[Tuple[int, int]], start: int):
+    def _relativize_target_spans(spans: list[tuple[int, int]], start: int):
         if start != 0 and spans:
             # Remove target spans referring to the unattributed prefix, rescale remaining spans to relative idxs
             # of the generated sequences and set 0 if the span starts before the generation begins.
             spans = [(s[0] - start if s[0] > start else 0, s[1] - start) for s in spans if s[1] > start]
         return spans
 
     @staticmethod
@@ -687,57 +655,57 @@
     Args:
         attr (:class:`~inseq.data.FeatureAttributionSequenceOutput`): The attribution object to aggregate.
         aggregate_fn (:obj:`Callable`, optional): Function to aggregate over the subwords.
             Defaults to the highest absolute value score across the aggregated span, with original sign
             preserved (e.g. [0.3, -0.7, 0.1] -> -0.7).
         aggregate_source (bool, optional): Whether to aggregate over the source sequence. Defaults to True.
         aggregate_target (bool, optional): Whether to aggregate over the target sequence. Defaults to True.
-        special_symbol (str, optional): Symbol used to identify subwords. Defaults to '▁', used by SentencePiece.
-            If is_suffix_symbol=True, then this symbol is used to identify parts to be aggregated (e.g. # in WordPiece,
-            ['phen', '##omen', '##al']). Otherwise, it identifies the roots that should be preserved (e.g. ▁ in
-            SentencePiece, ['▁phen', 'omen', 'al']).
+        special_chars (str or tuple of str, optional): One or more characters used to identify subword boundaries.
+            Defaults to '▁', used by SentencePiece. If is_suffix_symbol=True, then this symbol is used to identify
+            parts to be aggregated (e.g. # in WordPiece, ['phen', '##omen', '##al']). Otherwise, it identifies the
+            roots that should be preserved (e.g. ▁ in SentencePiece, ['▁phen', 'omen', 'al']).
         is_suffix_symbol (bool, optional): Whether the special symbol is used to identify suffixes or prefixes.
             Defaults to False.
     """
 
     aggregator_name = "subwords"
 
     @classmethod
     def aggregate(
         cls,
         attr: "FeatureAttributionSequenceOutput",
         aggregate_source: bool = True,
         aggregate_target: bool = True,
-        special_symbol: str = "▁",
+        special_chars: Union[str, tuple[str, ...]] = "▁",
         is_suffix_symbol: bool = False,
         **kwargs,
     ):
         source_spans = []
         target_spans = []
         if aggregate_source:
-            source_spans = cls.get_spans(attr.source, special_symbol, is_suffix_symbol)
+            source_spans = cls.get_spans(attr.source, special_chars, is_suffix_symbol)
         if aggregate_target:
-            target_spans = cls.get_spans(attr.target, special_symbol, is_suffix_symbol)
+            target_spans = cls.get_spans(attr.target, special_chars, is_suffix_symbol)
         return super().aggregate(attr, source_spans=source_spans, target_spans=target_spans, **kwargs)
 
     @staticmethod
-    def get_spans(tokens: List[TokenWithId], special_symbol: str, is_suffix_symbol: bool):
+    def get_spans(tokens: list[TokenWithId], special_chars: Union[str, tuple[str, ...]], is_suffix_symbol: bool):
         spans = []
         last_prefix_idx = 0
-        has_special_symbol = any(sym in token.token for token in tokens for sym in special_symbol)
-        if not has_special_symbol:
+        has_special_chars = any(sym in token.token for token in tokens for sym in special_chars)
+        if not has_special_chars:
             logger.warning(
-                f"ATTENTION: The {special_symbol} symbol is currently used for subword aggregation, but no instances "
-                "have been detected in the sequence. Change the special symbols using e.g. special_symbol=('Ġ', 'Ċ')"
+                f"The {special_chars} character is currently used for subword aggregation, but no instances "
+                "have been detected in the sequence. Change the special symbols using e.g. special_chars=('Ġ', 'Ċ')"
                 ", and set is_suffix_symbol=True if they are used as suffix word separators (e.g. Hello</w> world</w>)"
             )
             return spans
         for curr_idx, token in enumerate(tokens):
             # Suffix if token start with special suffix symbol, or if it doesn't have the special prefix symbol.
-            is_suffix = token.token.startswith(special_symbol) == is_suffix_symbol
+            is_suffix = token.token.startswith(special_chars) == is_suffix_symbol
             if is_suffix:
                 if curr_idx == len(tokens) - 1 and curr_idx - last_prefix_idx > 1:
                     spans.append((last_prefix_idx, curr_idx))
                 continue
             if curr_idx - last_prefix_idx > 1:
                 spans.append((last_prefix_idx, curr_idx))
             last_prefix_idx = curr_idx
```

### Comparing `inseq-0.5.0/inseq/data/attribution.py` & `inseq-0.6.0/inseq/data/attribution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 from copy import deepcopy
 from dataclasses import dataclass, field
 from os import PathLike
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Type, Union
+from typing import TYPE_CHECKING, Any, Callable, Optional, Union
 
 import torch
 
 from ..utils import (
     drop_padding,
     get_sequences_from_batched_steps,
     json_advanced_dump,
     json_advanced_load,
+    pad_with_nan,
     pretty_dict,
     remap_from_filtered,
 )
 from ..utils.typing import (
     MultipleScoresPerSequenceTensor,
     MultipleScoresPerStepTensor,
     OneOrMoreTokenWithIdSequences,
@@ -68,15 +69,15 @@
             input_embeds=attribution_model.embed(encodings.input_ids, as_targets=as_targets),
             baseline_embeds=attribution_model.embed(encodings.baseline_ids, as_targets=as_targets),
         )
         batch = Batch(encodings, embeddings)
     return batch
 
 
-def merge_attributions(attributions: List["FeatureAttributionOutput"]) -> "FeatureAttributionOutput":
+def merge_attributions(attributions: list["FeatureAttributionOutput"]) -> "FeatureAttributionOutput":
     """Merges multiple :class:`~inseq.data.FeatureAttributionOutput` objects into a single one.
 
     Merging is allowed only if the two outputs match on the fields specified in ``_merge_match_info_fields``.
 
     Args:
         attributions (:obj:`list` of :class:`~inseq.data.FeatureAttributionOutput`): The FeatureAttributionOutput
             objects to be merged.
@@ -132,24 +133,24 @@
             step of the target for every token in the target prefix.
         step_scores (:obj:`dict[str, SingleScorePerStepTensor]`, optional): Dictionary of step scores
             produced alongside attributions (one per generation step).
         sequence_scores (:obj:`dict[str, MultipleScoresPerStepTensor]`, optional): Dictionary of sequence
             scores produced alongside attributions (n per generation step, as for attributions).
     """
 
-    source: List[TokenWithId]
-    target: List[TokenWithId]
+    source: list[TokenWithId]
+    target: list[TokenWithId]
     source_attributions: Optional[SequenceAttributionTensor] = None
     target_attributions: Optional[SequenceAttributionTensor] = None
-    step_scores: Optional[Dict[str, SingleScoresPerSequenceTensor]] = None
-    sequence_scores: Optional[Dict[str, MultipleScoresPerSequenceTensor]] = None
+    step_scores: Optional[dict[str, SingleScoresPerSequenceTensor]] = None
+    sequence_scores: Optional[dict[str, MultipleScoresPerSequenceTensor]] = None
     attr_pos_start: int = 0
     attr_pos_end: Optional[int] = None
-    _aggregator: Union[str, List[str], None] = None
-    _dict_aggregate_fn: Optional[Dict[str, str]] = None
+    _aggregator: Union[str, list[str], None] = None
+    _dict_aggregate_fn: Optional[dict[str, str]] = None
 
     def __post_init__(self):
         if self._dict_aggregate_fn is None:
             self._dict_aggregate_fn = {}
         default_aggregate_fn = DEFAULT_ATTRIBUTION_AGGREGATE_DICT
         default_aggregate_fn.update(self._dict_aggregate_fn)
         self._dict_aggregate_fn = default_aggregate_fn
@@ -173,20 +174,19 @@
                 : len(sources[seq_id]), : len(targets[seq_id]), ...
             ]
         return remove_pad_fn
 
     @classmethod
     def from_step_attributions(
         cls,
-        attributions: List["FeatureAttributionStepOutput"],
-        tokenized_target_sentences: Optional[List[List[TokenWithId]]] = None,
-        pad_id: Optional[Any] = None,
-        has_bos_token: bool = True,
+        attributions: list["FeatureAttributionStepOutput"],
+        tokenized_target_sentences: list[list[TokenWithId]],
+        pad_token: Optional[Any] = None,
         attr_pos_end: Optional[int] = None,
-    ) -> List["FeatureAttributionSequenceOutput"]:
+    ) -> list["FeatureAttributionSequenceOutput"]:
         """Converts a list of :class:`~inseq.data.attribution.FeatureAttributionStepOutput` objects containing multiple
         examples outputs per step into a list of :class:`~inseq.data.attribution.FeatureAttributionSequenceOutput` with
         every object containing all step outputs for an individual example.
 
         Raises:
             `ValueError`: If the number of sequences in the attributions is not the same for all input sequences.
 
@@ -194,71 +194,69 @@
             `List[FeatureAttributionSequenceOutput]`: List of
             :class:`~inseq.data.attribution.FeatureAttributionSequenceOutput` objects.
         """
         attr = attributions[0]
         num_sequences = len(attr.prefix)
         if not all(len(attr.prefix) == num_sequences for attr in attributions):
             raise ValueError("All the attributions must include the same number of sequences.")
-        seq_attributions = []
-        sources = None
-        if attr.source_attributions is not None:
-            sources = [drop_padding(attr.source[seq_id], pad_id) for seq_id in range(num_sequences)]
-        targets = [
-            drop_padding([a.target[seq_id][0] for a in attributions], pad_id) for seq_id in range(num_sequences)
-        ]
-        if tokenized_target_sentences is None:
-            tokenized_target_sentences = targets
-        if has_bos_token:
-            tokenized_target_sentences = [tok_seq[1:] for tok_seq in tokenized_target_sentences]
-        tokenized_target_sentences = [
-            drop_padding(tokenized_target_sentences[seq_id], pad_id) for seq_id in range(num_sequences)
-        ]
-        if attr_pos_end is None:
-            attr_pos_end = max([len(t) for t in tokenized_target_sentences])
-        pos_start = [
-            min(len(tokenized_target_sentences[seq_id]), attr_pos_end) - len(targets[seq_id])
-            for seq_id in range(num_sequences)
-        ]
-        for seq_id in range(num_sequences):
-            source = tokenized_target_sentences[seq_id][: pos_start[seq_id]] if sources is None else sources[seq_id]
-            seq_attributions.append(
-                attr.get_sequence_cls(
-                    source=source,
-                    target=tokenized_target_sentences[seq_id],
-                    attr_pos_start=pos_start[seq_id],
-                    attr_pos_end=attr_pos_end,
+        seq_attributions: list[FeatureAttributionSequenceOutput] = []
+        sources = []
+        targets = []
+        pos_start = []
+        for seq_idx in range(num_sequences):
+            if attr.source_attributions is not None:
+                sources.append(drop_padding(attr.source[seq_idx], pad_token))
+            curr_target = [a.target[seq_idx][0] for a in attributions]
+            targets.append(drop_padding(curr_target, pad_token))
+            if all(attr.prefix[seq_idx][0] == pad_token for seq_idx in range(num_sequences)):
+                tokenized_target_sentences[seq_idx] = tokenized_target_sentences[seq_idx][:1] + drop_padding(
+                    tokenized_target_sentences[seq_idx][1:], pad_token
                 )
+            else:
+                tokenized_target_sentences[seq_idx] = drop_padding(tokenized_target_sentences[seq_idx], pad_token)
+        if attr_pos_end is None:
+            attr_pos_end = max(len(t) for t in tokenized_target_sentences)
+        for seq_idx in range(num_sequences):
+            # If the model is decoder-only, the source is the input prefix
+            curr_pos_start = min(len(tokenized_target_sentences[seq_idx]), attr_pos_end) - len(targets[seq_idx])
+            pos_start.append(curr_pos_start)
+            source = tokenized_target_sentences[seq_idx][:curr_pos_start] if not sources else sources[seq_idx]
+            curr_seq_attribution: FeatureAttributionSequenceOutput = attr.get_sequence_cls(
+                source=source,
+                target=tokenized_target_sentences[seq_idx],
+                attr_pos_start=pos_start[seq_idx],
+                attr_pos_end=attr_pos_end,
             )
+            seq_attributions.append(curr_seq_attribution)
         if attr.source_attributions is not None:
             source_attributions = get_sequences_from_batched_steps([att.source_attributions for att in attributions])
             for seq_id in range(num_sequences):
                 # Remove padding from tensor
                 filtered_source_attribution = source_attributions[seq_id][
                     : len(sources[seq_id]), : len(targets[seq_id]), ...
                 ]
                 seq_attributions[seq_id].source_attributions = filtered_source_attribution
         if attr.target_attributions is not None:
-            target_attributions = get_sequences_from_batched_steps([att.target_attributions for att in attributions])
+            target_attributions = get_sequences_from_batched_steps(
+                [att.target_attributions for att in attributions], padding_dims=[1]
+            )
             for seq_id in range(num_sequences):
-                if has_bos_token:
-                    target_attributions[seq_id] = target_attributions[seq_id][1:, ...]
                 start_idx = max(pos_start) - pos_start[seq_id]
                 end_idx = start_idx + len(tokenized_target_sentences[seq_id])
                 target_attributions[seq_id] = target_attributions[seq_id][
                     start_idx:end_idx, : len(targets[seq_id]), ...  # noqa: E203
                 ]
                 if target_attributions[seq_id].shape[0] != len(tokenized_target_sentences[seq_id]):
-                    empty_final_row = torch.ones(1, *target_attributions[seq_id].shape[1:]) * float("nan")
-                    target_attributions[seq_id] = torch.cat([target_attributions[seq_id], empty_final_row], dim=0)
+                    target_attributions[seq_id] = pad_with_nan(target_attributions[seq_id], dim=0, pad_size=1)
                 seq_attributions[seq_id].target_attributions = target_attributions[seq_id]
         if attr.step_scores is not None:
             step_scores = [{} for _ in range(num_sequences)]
             for step_score_name in attr.step_scores.keys():
                 out_step_scores = get_sequences_from_batched_steps(
-                    [att.step_scores[step_score_name] for att in attributions]
+                    [att.step_scores[step_score_name] for att in attributions], stack_dim=1
                 )
                 for seq_id in range(num_sequences):
                     step_scores[seq_id][step_score_name] = out_step_scores[seq_id][: len(targets[seq_id])]
             for seq_id in range(num_sequences):
                 seq_attributions[seq_id].step_scores = step_scores[seq_id]
         if attr.sequence_scores is not None:
             seq_scores = [{} for _ in range(num_sequences)]
@@ -268,29 +266,29 @@
                 # that are not source-to-target (default for encoder-decoder) or target-to-target
                 # (default for decoder only).
                 remove_pad_fn = cls.get_remove_pad_fn(attr, seq_score_name)
                 if seq_score_name.startswith("encoder"):
                     out_seq_scores = [attr.sequence_scores[seq_score_name][i, ...] for i in range(num_sequences)]
                 else:
                     out_seq_scores = get_sequences_from_batched_steps(
-                        [att.sequence_scores[seq_score_name] for att in attributions]
+                        [att.sequence_scores[seq_score_name] for att in attributions], padding_dims=[1]
                     )
                 for seq_id in range(num_sequences):
                     seq_scores[seq_id][seq_score_name] = remove_pad_fn(out_seq_scores, sources, targets, seq_id)
             for seq_id in range(num_sequences):
                 seq_attributions[seq_id].sequence_scores = seq_scores[seq_id]
         return seq_attributions
 
     def show(
         self,
         min_val: Optional[int] = None,
         max_val: Optional[int] = None,
         display: bool = True,
         return_html: Optional[bool] = False,
-        aggregator: Union[AggregatorPipeline, Type[Aggregator]] = None,
+        aggregator: Union[AggregatorPipeline, type[Aggregator]] = None,
         do_aggregation: bool = True,
         **kwargs,
     ) -> Optional[str]:
         """Visualize the attributions.
 
         Args:
             min_val (:obj:`int`, *optional*, defaults to None):
@@ -361,18 +359,18 @@
             self.target_attributions = (step_scores * target_attr).T
         # Empty aggregator pipeline -> no aggregation
         self._aggregator = []
         return self
 
     def get_scores_dicts(
         self,
-        aggregator: Union[AggregatorPipeline, Type[Aggregator]] = None,
+        aggregator: Union[AggregatorPipeline, type[Aggregator]] = None,
         do_aggregation: bool = True,
         **kwargs,
-    ) -> Dict[str, Dict[str, Dict[str, float]]]:
+    ) -> dict[str, dict[str, dict[str, float]]]:
         # If no aggregator is specified, the default aggregator for the class is used
         aggr = self.aggregate(aggregator, **kwargs) if do_aggregation else self
         return_dict = {"source_attributions": {}, "target_attributions": {}, "step_scores": {}}
         for tgt_idx in range(aggr.attr_pos_start, aggr.attr_pos_end):
             tgt_tok = aggr.target[tgt_idx]
             if aggr.source_attributions is not None:
                 return_dict["source_attributions"][(tgt_idx, tgt_tok.token)] = {}
@@ -397,21 +395,21 @@
 
 
 @dataclass(eq=False, repr=False)
 class FeatureAttributionStepOutput(TensorWrapper):
     """Output of a single step of feature attribution, plus extra information related to what was attributed."""
 
     source_attributions: Optional[StepAttributionTensor] = None
-    step_scores: Optional[Dict[str, SingleScorePerStepTensor]] = None
+    step_scores: Optional[dict[str, SingleScorePerStepTensor]] = None
     target_attributions: Optional[StepAttributionTensor] = None
-    sequence_scores: Optional[Dict[str, MultipleScoresPerStepTensor]] = None
+    sequence_scores: Optional[dict[str, MultipleScoresPerStepTensor]] = None
     source: Optional[OneOrMoreTokenWithIdSequences] = None
     prefix: Optional[OneOrMoreTokenWithIdSequences] = None
     target: Optional[OneOrMoreTokenWithIdSequences] = None
-    _sequence_cls: Type["FeatureAttributionSequenceOutput"] = FeatureAttributionSequenceOutput
+    _sequence_cls: type["FeatureAttributionSequenceOutput"] = FeatureAttributionSequenceOutput
 
     def __post_init__(self):
         self.to(torch.float32)
         if self.step_scores is None:
             self.step_scores = {}
         if self.sequence_scores is None:
             self.sequence_scores = {}
@@ -419,39 +417,61 @@
     def get_sequence_cls(self, **kwargs):
         return self._sequence_cls(**kwargs)
 
     def remap_from_filtered(
         self,
         target_attention_mask: TargetIdsTensor,
         batch: Union[DecoderOnlyBatch, EncoderDecoderBatch],
+        is_final_step_method: bool = False,
     ) -> None:
         """Remaps the attributions to the original shape of the input sequence."""
+        batch_size = (
+            len(batch.sources.input_tokens) if self.source_attributions is not None else len(batch.target_tokens)
+        )
+        source_len = len(batch.sources.input_tokens[0])
+        target_len = len(batch.target_tokens[0])
+        # Normal per-step attribution outputs have shape (batch_size, seq_len, ...)
+        other_dims_start_idx = 2
+        # Final step attribution outputs have shape (batch_size, seq_len, seq_len, ...)
+        if is_final_step_method:
+            other_dims_start_idx += 1
+        other_dims = (
+            self.source_attributions.shape[other_dims_start_idx:]
+            if self.source_attributions is not None
+            else self.target_attributions.shape[other_dims_start_idx:]
+        )
         if self.source_attributions is not None:
             self.source_attributions = remap_from_filtered(
-                original_shape=(len(batch.sources.input_tokens), *self.source_attributions.shape[1:]),
+                original_shape=(batch_size, *self.source_attributions.shape[1:]),
                 mask=target_attention_mask,
                 filtered=self.source_attributions,
             )
         if self.target_attributions is not None:
             self.target_attributions = remap_from_filtered(
-                original_shape=(len(batch.target_tokens), *self.target_attributions.shape[1:]),
+                original_shape=(batch_size, *self.target_attributions.shape[1:]),
                 mask=target_attention_mask,
                 filtered=self.target_attributions,
             )
         if self.step_scores is not None:
             for score_name, score_tensor in self.step_scores.items():
                 self.step_scores[score_name] = remap_from_filtered(
-                    original_shape=(len(batch.target_tokens), 1),
+                    original_shape=(batch_size, 1),
                     mask=target_attention_mask,
                     filtered=score_tensor.unsqueeze(-1),
                 ).squeeze(-1)
         if self.sequence_scores is not None:
             for score_name, score_tensor in self.sequence_scores.items():
+                if score_name.startswith("decoder"):
+                    original_shape = (batch_size, target_len, target_len, *other_dims)
+                elif score_name.startswith("encoder"):
+                    original_shape = (batch_size, source_len, source_len, *other_dims)
+                else:  # default case: cross-attention
+                    original_shape = (batch_size, source_len, target_len, *other_dims)
                 self.sequence_scores[score_name] = remap_from_filtered(
-                    original_shape=(len(batch.target_tokens), *self.source_attributions.shape[1:]),
+                    original_shape=original_shape,
                     mask=target_attention_mask,
                     filtered=score_tensor,
                 )
 
 
 @dataclass
 class FeatureAttributionOutput:
@@ -477,17 +497,17 @@
         "model_class",
         "model_name",
         "step_scores",
         "tokenizer_class",
         "tokenizer_name",
     ]
 
-    sequence_attributions: List[FeatureAttributionSequenceOutput]
-    step_attributions: Optional[List[FeatureAttributionStepOutput]] = None
-    info: Dict[str, Any] = field(default_factory=dict)
+    sequence_attributions: list[FeatureAttributionSequenceOutput]
+    step_attributions: Optional[list[FeatureAttributionStepOutput]] = None
+    info: dict[str, Any] = field(default_factory=dict)
 
     def __str__(self):
         return f"{self.__class__.__name__}({pretty_dict(self.__dict__)})"
 
     def __repr__(self):
         return self.__str__()
 
@@ -598,15 +618,15 @@
         out.sequence_attributions = [seq.torch() for seq in out.sequence_attributions]
         if out.step_attributions is not None:
             out.step_attributions = [step.torch() for step in out.step_attributions]
         return out
 
     def aggregate(
         self,
-        aggregator: Union[AggregatorPipeline, Type[Aggregator]] = None,
+        aggregator: Union[AggregatorPipeline, type[Aggregator]] = None,
         **kwargs,
     ) -> "FeatureAttributionOutput":
         """Aggregate the sequence attributions using one or more aggregators.
 
         Args:
             aggregator (:obj:`AggregatorPipeline` or :obj:`Type[Aggregator]`, optional): Aggregator
                 or pipeline to use. If not provided, the default aggregator for every sequence attribution
@@ -622,15 +642,15 @@
 
     def show(
         self,
         min_val: Optional[int] = None,
         max_val: Optional[int] = None,
         display: bool = True,
         return_html: Optional[bool] = False,
-        aggregator: Union[AggregatorPipeline, Type[Aggregator]] = None,
+        aggregator: Union[AggregatorPipeline, type[Aggregator]] = None,
         do_aggregation: bool = True,
         **kwargs,
     ) -> Optional[str]:
         """Visualize the sequence attributions.
 
         Args:
             min_val (int, optional): Minimum value for color scale.
@@ -657,16 +677,16 @@
             return out_str
 
     def weight_attributions(self, step_score_id: str):
         for i, attr in enumerate(self.sequence_attributions):
             self.sequence_attributions[i] = attr.weight_attributions(step_score_id)
 
     def get_scores_dicts(
-        self, aggregator: Union[AggregatorPipeline, Type[Aggregator]] = None, do_aggregation: bool = True, **kwargs
-    ) -> List[Dict[str, Dict[str, Dict[str, float]]]]:
+        self, aggregator: Union[AggregatorPipeline, type[Aggregator]] = None, do_aggregation: bool = True, **kwargs
+    ) -> list[dict[str, dict[str, dict[str, float]]]]:
         """Get all computed scores (attributions and step scores) for all sequences as a list of dictionaries.
 
         Returns:
             :obj:`list(dict)`: List containing one dictionary per sequence. Every dictionary contains the keys
             "source_attributions", "target_attributions" and "step_scores". For each of these keys, the value is a
             dictionary with generated tokens as keys, and for values a final dictionary. For  "step_scores", the keys
             of the final dictionary are the step score ids, and the values are the scores.
@@ -702,15 +722,15 @@
             self._dict_aggregate_fn["step_scores"]["spans"]["deltas"] = "absmax"
 
 
 @dataclass(eq=False, repr=False)
 class GranularFeatureAttributionStepOutput(FeatureAttributionStepOutput):
     """Raw output of a single step of gradient feature attribution."""
 
-    _sequence_cls: Type["FeatureAttributionSequenceOutput"] = GranularFeatureAttributionSequenceOutput
+    _sequence_cls: type["FeatureAttributionSequenceOutput"] = GranularFeatureAttributionSequenceOutput
 
 
 @dataclass(eq=False, repr=False)
 class CoarseFeatureAttributionSequenceOutput(FeatureAttributionSequenceOutput):
     """Raw output of a single sequence of coarse-grained feature attribution.
 
     An example of coarse-grained feature attribution methods are occlusion methods in which a whole token is masked at
@@ -722,15 +742,15 @@
         self._aggregator = []
 
 
 @dataclass(eq=False, repr=False)
 class CoarseFeatureAttributionStepOutput(FeatureAttributionStepOutput):
     """Raw output of a single step of coarse-grained feature attribution."""
 
-    _sequence_cls: Type["FeatureAttributionSequenceOutput"] = CoarseFeatureAttributionSequenceOutput
+    _sequence_cls: type["FeatureAttributionSequenceOutput"] = CoarseFeatureAttributionSequenceOutput
 
 
 @dataclass(eq=False, repr=False)
 class MultiDimensionalFeatureAttributionSequenceOutput(FeatureAttributionSequenceOutput):
     """Raw output of a single sequence of multi-dimensional feature attribution.
 
     Multi-dimensional feature attribution methods are a generalization of granular feature attribution methods
@@ -746,11 +766,11 @@
 
 
 @dataclass(eq=False, repr=False)
 class MultiDimensionalFeatureAttributionStepOutput(FeatureAttributionStepOutput):
     """Raw output of a single step of multi-dimensional feature attribution."""
 
     _num_dimensions: int = 2
-    _sequence_cls: Type["FeatureAttributionSequenceOutput"] = MultiDimensionalFeatureAttributionSequenceOutput
+    _sequence_cls: type["FeatureAttributionSequenceOutput"] = MultiDimensionalFeatureAttributionSequenceOutput
 
     def get_sequence_cls(self, **kwargs):
         return MultiDimensionalFeatureAttributionSequenceOutput(_num_dimensions=self._num_dimensions, **kwargs)
```

### Comparing `inseq-0.5.0/inseq/data/batch.py` & `inseq-0.6.0/inseq/data/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Union
 
 from ..utils import get_aligned_idx
 from ..utils.typing import EmbeddingsTensor, ExpandedTargetIdsTensor, IdsTensor, OneOrMoreTokenSequences
 from .data_utils import TensorWrapper
 
 
 @dataclass(eq=False, repr=False)
@@ -91,15 +91,15 @@
         return self.embedding.baseline_embeds
 
     @input_ids.setter
     def input_ids(self, value: IdsTensor):
         self.encoding.input_ids = value
 
     @input_tokens.setter
-    def input_tokens(self, value: List[List[str]]):
+    def input_tokens(self, value: list[list[str]]):
         self.encoding.input_tokens = value
 
     @attention_mask.setter
     def attention_mask(self, value: IdsTensor):
         self.encoding.attention_mask = value
 
     @baseline_ids.setter
@@ -165,15 +165,15 @@
 
     @property
     def target_mask(self) -> IdsTensor:
         return self.targets.attention_mask
 
     def get_step_target(
         self, step: int, with_attention: bool = False
-    ) -> Union[ExpandedTargetIdsTensor, Tuple[ExpandedTargetIdsTensor, ExpandedTargetIdsTensor]]:
+    ) -> Union[ExpandedTargetIdsTensor, tuple[ExpandedTargetIdsTensor, ExpandedTargetIdsTensor]]:
         tgt = self.targets.input_ids[:, step]
         if with_attention:
             return tgt, self.targets.attention_mask[:, step]
         return tgt
 
 
 @dataclass(eq=False, repr=False)
@@ -214,29 +214,29 @@
 
     @property
     def target_mask(self) -> IdsTensor:
         return self.attention_mask
 
     def get_step_target(
         self, step: int, with_attention: bool = False
-    ) -> Union[ExpandedTargetIdsTensor, Tuple[ExpandedTargetIdsTensor, ExpandedTargetIdsTensor]]:
+    ) -> Union[ExpandedTargetIdsTensor, tuple[ExpandedTargetIdsTensor, ExpandedTargetIdsTensor]]:
         tgt = self.input_ids[:, step]
         if with_attention:
             return tgt, self.attention_mask[:, step]
         return tgt
 
     @classmethod
     def from_batch(self, batch: Batch) -> "DecoderOnlyBatch":
         return DecoderOnlyBatch(
             encoding=batch.encoding,
             embedding=batch.embedding,
         )
 
 
 def slice_batch_from_position(
-    batch: DecoderOnlyBatch, curr_idx: int, alignments: Optional[List[Tuple[int, int]]] = None
-) -> Tuple[DecoderOnlyBatch, IdsTensor]:
+    batch: DecoderOnlyBatch, curr_idx: int, alignments: Optional[list[tuple[int, int]]] = None
+) -> tuple[DecoderOnlyBatch, IdsTensor]:
     if len(alignments) > 0 and isinstance(alignments[0], list):
         alignments = alignments[0]
     truncate_idx = get_aligned_idx(curr_idx, alignments)
     tgt_ids = batch.target_ids[:, truncate_idx]
     return batch[:truncate_idx], tgt_ids
```

### Comparing `inseq-0.5.0/inseq/data/data_utils.py` & `inseq-0.6.0/inseq/data/data_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 from dataclasses import dataclass, fields
-from typing import Any, Dict, TypeVar
+from typing import Any, TypeVar
 
 import numpy as np
 import torch
 from jaxtyping import Int
 
 from ..utils import pretty_dict
 
@@ -108,15 +108,15 @@
         else:
             return attr
 
     @staticmethod
     def _eq(self_attr: TensorClass, other_attr: TensorClass) -> bool:
         try:
             if isinstance(self_attr, torch.Tensor):
-                return torch.allclose(self_attr, other_attr, equal_nan=True)
+                return torch.allclose(self_attr, other_attr, equal_nan=True, atol=1e-5)
             elif isinstance(self_attr, dict):
                 return all(TensorWrapper._eq(self_attr[k], other_attr[k]) for k in self_attr.keys())
             else:
                 return self_attr == other_attr
         except:  # noqa: E722
             return False
 
@@ -171,15 +171,19 @@
                 out_params[field.name] = attr.clone()
             elif attr is not None:
                 out_params[field.name] = deepcopy(attr)
             else:
                 out_params[field.name] = None
         return self.__class__(**out_params)
 
-    def to_dict(self: TensorClass) -> Dict[str, Any]:
+    def clone_empty(self: TensorClass) -> TensorClass:
+        out_params = {k: v for k, v in self.__dict__.items() if k.startswith("_") and v is not None}
+        return self.__class__(**out_params)
+
+    def to_dict(self: TensorClass) -> dict[str, Any]:
         return {k: v for k, v in self.__dict__.items() if not k.startswith("_")}
 
     def __str__(self):
         return f"{self.__class__.__name__}({pretty_dict(self.to_dict())})"
 
     def __repr__(self):
         return f"{self.__class__.__name__}({pretty_dict(self.__dict__)})"
```

### Comparing `inseq-0.5.0/inseq/data/viz.py` & `inseq-0.6.0/inseq/data/viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 # LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
 # IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 # WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
 # OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 import random
 import string
-from typing import Dict, List, Literal, Optional, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 from matplotlib.colors import Colormap
 from rich import box
-from rich import print as rprint
 from rich.color import Color
+from rich.console import Console
 from rich.live import Live
+from rich.markup import escape
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.progress import BarColumn, Progress, TextColumn, TimeRemainingColumn
 from rich.style import Style
 from rich.table import Column, Table
 from rich.text import Text
 from tqdm.std import tqdm
@@ -98,44 +99,47 @@
             curr_html += get_heatmap_type(attribution, curr_html_color, "Target", use_html=True)
         if display and isnotebook():
             from IPython.core.display import HTML, display
 
             display(HTML(curr_html))
         html_out += curr_html
         if not isnotebook():
+            console = Console()
             curr_color = None
             if attribution.source_attributions is not None:
                 curr_color = colors[idx]
                 if display:
                     print("\n\n")
-                    rprint(get_heatmap_type(attribution, curr_color, "Source", use_html=False))
+                    console.print(
+                        get_heatmap_type(attribution, curr_color, "Source", use_html=False), overflow="ignore"
+                    )
                 if attribution.target_attributions is not None:
                     curr_color = colors[idx + 1]
             display_scores = attribution.source_attributions is None and attribution.step_scores
             if (attribution.target_attributions is not None or display_scores) and display:
                 if curr_color is None and colors:
                     curr_color = colors[idx]
                 print("\n\n")
-                rprint(get_heatmap_type(attribution, curr_color, "Target", use_html=False))
+                console.print(get_heatmap_type(attribution, curr_color, "Target", use_html=False), overflow="ignore")
         if any(x is None for x in [attribution.source_attributions, attribution.target_attributions]):
             idx += 1
         else:
             idx += 2
     if return_html:
         return html_out
 
 
 def get_attribution_colors(
-    attributions: List[FeatureAttributionSequenceOutput],
+    attributions: list[FeatureAttributionSequenceOutput],
     min_val: Optional[int] = None,
     max_val: Optional[int] = None,
     cmap: Union[str, Colormap, None] = None,
     return_alpha: bool = True,
     return_strings: bool = True,
-) -> List[List[List[Union[str, Tuple[float, float, float]]]]]:
+) -> list[list[list[Union[str, tuple[float, float, float]]]]]:
     """A list (one element = one sentence) of lists (one element = attributions for one token)
     of lists (one element = one attribution) of colors. Colors are either strings or RGB(A) tuples.
     """
     if max_val is None:
         max_val = max(attribution.maximum for attribution in attributions)
     if min_val is None:
         min_val = -max_val
@@ -190,20 +194,20 @@
         )
     else:
         raise ValueError(f"Type {heatmap_type} is not supported.")
 
 
 def get_saliency_heatmap_html(
     scores: Union[np.ndarray, None],
-    column_labels: List[str],
-    row_labels: List[str],
-    input_colors: List[List[str]],
-    step_scores: Optional[Dict[str, np.ndarray]] = None,
+    column_labels: list[str],
+    row_labels: list[str],
+    input_colors: list[list[str]],
+    step_scores: Optional[dict[str, np.ndarray]] = None,
     label: str = "",
-    step_scores_threshold: Union[float, Dict[str, float]] = 0.5,
+    step_scores_threshold: Union[float, dict[str, float]] = 0.5,
 ):
     # unique ID added to HTML elements and function to avoid collision of differnent instances
     uuid = "".join(random.choices(string.ascii_lowercase, k=20))
     out = saliency_heatmap_table_header
     # add top row containing target tokens
     for column_label in column_labels:
         out += f"<th>{sanitize_html(column_label)}</th>"
@@ -239,69 +243,69 @@
         uuid=plot_uuid,
         saliency_plot_markup=saliency_heatmap_markup,
     )
 
 
 def get_saliency_heatmap_rich(
     scores: Union[np.ndarray, None],
-    column_labels: List[str],
-    row_labels: List[str],
-    input_colors: List[List[str]],
-    step_scores: Optional[Dict[str, np.ndarray]] = None,
+    column_labels: list[str],
+    row_labels: list[str],
+    input_colors: list[list[str]],
+    step_scores: Optional[dict[str, np.ndarray]] = None,
     label: str = "",
-    step_scores_threshold: Union[float, Dict[str, float]] = 0.5,
+    step_scores_threshold: Union[float, dict[str, float]] = 0.5,
 ):
-    columns = [Column(header="", justify="right")]
+    columns = [Column(header="", justify="right", overflow="fold")]
     for column_label in column_labels:
-        columns.append(Column(header=column_label, justify="center"))
+        columns.append(Column(header=escape(column_label), justify="center", overflow="fold"))
     table = Table(
         *columns,
         title=f"{label + ' ' if label else ''}Saliency Heatmap",
         caption="x: Generated tokens, y: Attributed tokens",
         padding=(0, 1, 0, 1),
         show_lines=False,
         box=box.HEAVY_HEAD,
     )
     if scores is not None:
         for row_index in range(scores.shape[0]):
-            row = [Text(row_labels[row_index], style="bold")]
+            row = [Text(escape(row_labels[row_index]), style="bold")]
             for col_index in range(scores.shape[1]):
                 color = Color.from_rgb(*input_colors[row_index][col_index])
                 score = ""
                 if not np.isnan(scores[row_index][col_index]):
                     score = round(float(scores[row_index][col_index]), 2)
                 row.append(Text(f"{score}", justify="center", style=Style(color=color)))
             table.add_row(*row, end_section=row_index == scores.shape[0] - 1)
     if step_scores is not None:
         for step_score_name, step_score_values in step_scores.items():
             if isinstance(step_scores_threshold, float):
                 threshold = step_scores_threshold
             else:
                 threshold = step_scores_threshold.get(step_score_name, 0.5)
             style = lambda val, limit: "bold" if abs(val) >= limit and isinstance(val, float) else ""
-            score_row = [Text(step_score_name, style="bold")]
+            score_row = [Text(escape(step_score_name), style="bold")]
             for score in step_score_values:
                 curr_score = round(score.item(), 2) if isinstance(score, float) else score.item()
                 score_row.append(Text(f"{score:.2f}", justify="center", style=style(curr_score, threshold)))
             table.add_row(*score_row, end_section=True)
     return table
 
 
 # Progress bar utilities
 
 
 def get_progress_bar(
     sequences: TextSequences,
-    target_lengths: List[int],
+    target_lengths: list[int],
     method_name: str,
     show: bool,
     pretty: bool,
     attr_pos_start: int,
     attr_pos_end: int,
-) -> Union[tqdm, Tuple[Progress, Live], None]:
+) -> Union[tqdm, tuple[Progress, Live], None]:
     if not show:
         return None
     elif show and not pretty:
         return tqdm(
             total=attr_pos_end,
             desc=f"Attributing with {method_name}...",
             initial=attr_pos_start,
@@ -310,29 +314,29 @@
         job_progress = Progress(
             TextColumn("{task.description}", table_column=Column(ratio=3, no_wrap=False)),
             BarColumn(table_column=Column(ratio=1)),
             TextColumn("[progress.percentage]{task.percentage:>3.0f}%"),
             TimeRemainingColumn(),
         )
         for idx, (tgt, tgt_len) in enumerate(zip(sequences.targets, target_lengths)):
-            clean_tgt = tgt.replace("\n", "\\n")
+            clean_tgt = escape(tgt.replace("\n", "\\n"))
             job_progress.add_task(f"{idx}. {clean_tgt}", total=tgt_len)
         progress_table = Table.grid()
         row_contents = [
             Panel.fit(
                 job_progress,
-                title=f"[b]Attributing with {method_name}",
+                title=f"[b]Attributing with {escape(method_name)}",
                 border_style="green",
                 padding=(1, 2),
             )
         ]
         if sequences.sources is not None:
             sources = []
             for idx, src in enumerate(sequences.sources):
-                clean_src = src.replace("\n", "\\n")
+                clean_src = escape(src.replace("\n", "\\n"))
                 sources.append(f"{idx}. {clean_src}")
             row_contents = [
                 Panel.fit(
                     "\n".join(sources),
                     title="Source sentences",
                     border_style="red",
                     padding=(1, 2),
@@ -341,20 +345,20 @@
         progress_table.add_row(*row_contents)
         live = Live(Padding(progress_table, (1, 0, 1, 0)), refresh_per_second=10)
         live.start(refresh=live._renderable is not None)
         return job_progress, live
 
 
 def update_progress_bar(
-    pbar: Union[tqdm, Tuple[Progress, Live], None],
-    skipped_prefixes: Optional[List[str]] = None,
-    attributed_sentences: Optional[List[str]] = None,
-    unattributed_suffixes: Optional[List[str]] = None,
-    skipped_suffixes: Optional[List[str]] = None,
-    whitespace_indexes: List[List[int]] = None,
+    pbar: Union[tqdm, tuple[Progress, Live], None],
+    skipped_prefixes: Optional[list[str]] = None,
+    attributed_sentences: Optional[list[str]] = None,
+    unattributed_suffixes: Optional[list[str]] = None,
+    skipped_suffixes: Optional[list[str]] = None,
+    whitespace_indexes: list[list[int]] = None,
     show: bool = False,
     pretty: bool = False,
 ) -> None:
     if not show:
         return
     elif show and not pretty:
         pbar.update(1)
@@ -363,23 +367,23 @@
         for job in pbar[0].tasks:
             if not job.finished:
                 pbar[0].advance(job.id)
                 formatted_desc = f"{job.id}. "
                 past_length = 0
                 for split, color in zip(split_targets, ["grey58", "green", "orange1", "grey58"]):
                     if split[job.id]:
-                        formatted_desc += f"[{color}]" + split[job.id].replace("\n", "\\n") + "[/]"
+                        formatted_desc += f"[{color}]" + escape(split[job.id].replace("\n", "\\n")) + "[/]"
                         past_length += len(split[job.id])
                         if past_length in whitespace_indexes[job.id]:
                             formatted_desc += " "
                             past_length += 1
                 pbar[0].update(job.id, description=formatted_desc, refresh=True)
 
 
-def close_progress_bar(pbar: Union[tqdm, Tuple[Progress, Live], None], show: bool, pretty: bool) -> None:
+def close_progress_bar(pbar: Union[tqdm, tuple[Progress, Live], None], show: bool, pretty: bool) -> None:
     if not show:
         return
     elif show and not pretty:
         pbar.close()
     else:
         _, live = pbar
         live.stop()
```

### Comparing `inseq-0.5.0/inseq/models/__init__.py` & `inseq-0.6.0/inseq/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import List, Optional, Union
+from typing import Optional, Union
 
 from rich.status import Status
 
 from ..utils import isnotebook, optional
 from ..utils.typing import ModelClass, ModelIdentifier
 from .attribution_model import AttributionModel, InputFormatter
 from .decoder_only import DecoderOnlyAttributionModel
@@ -43,15 +43,15 @@
     model_name = model if isinstance(model, str) else "model"
     method_desc = f"with {attribution_method} method..." if attribution_method else " without attribution methods..."
     load_msg = f"Loading {model_name} {method_desc}"
     with optional(not isnotebook(), Status(load_msg), logger.info, msg=load_msg):
         return FRAMEWORKS_MAP[framework].load(model, attribution_method, **kwargs)
 
 
-def list_supported_frameworks() -> List[str]:
+def list_supported_frameworks() -> list[str]:
     """Lists identifiers for all available frameworks. These can be used to load models with the `framework` argument
     in the :meth:`~inseq.load_model` function.
     """
     return list(FRAMEWORKS_MAP.keys())
 
 
 __all__ = [
```

### Comparing `inseq-0.5.0/inseq/models/attribution_model.py` & `inseq-0.6.0/inseq/models/attribution_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from abc import ABC, abstractmethod
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Protocol, Tuple, TypeVar, Union
+from typing import Any, Callable, Optional, Protocol, TypeVar, Union
 
 import torch
 
 from ..attr import STEP_SCORES_MAP, StepFunctionArgs
 from ..attr.feat import FeatureAttribution, extract_args, join_token_ids
 from ..data import (
     BatchEncoding,
@@ -52,15 +52,15 @@
 class ForwardMethod(Protocol):
     def __call__(
         self,
         batch: Union[DecoderOnlyBatch, EncoderDecoderBatch],
         target_ids: ExpandedTargetIdsTensor,
         attributed_fn: Callable[..., SingleScorePerStepTensor],
         use_embeddings: bool,
-        attributed_fn_argnames: Optional[List[str]],
+        attributed_fn_argnames: Optional[list[str]],
         *args,
     ) -> CustomForwardOutput:
         ...
 
 
 class InputFormatter:
     @staticmethod
@@ -75,31 +75,31 @@
     @staticmethod
     @abstractmethod
     def format_attribution_args(
         batch: Union[DecoderOnlyBatch, EncoderDecoderBatch],
         target_ids: TargetIdsTensor,
         attributed_fn: Callable[..., SingleScorePerStepTensor],
         attribute_target: bool = False,
-        attributed_fn_args: Dict[str, Any] = {},
+        attributed_fn_args: dict[str, Any] = {},
         attribute_batch_ids: bool = False,
         forward_batch_embeds: bool = True,
         use_baselines: bool = False,
-    ) -> Tuple[Dict[str, Any], Tuple[Union[IdsTensor, EmbeddingsTensor, None], ...]]:
+    ) -> tuple[dict[str, Any], tuple[Union[IdsTensor, EmbeddingsTensor, None], ...]]:
         raise NotImplementedError()
 
     @staticmethod
     @abstractmethod
     def enrich_step_output(
         attribution_model: "AttributionModel",
         step_output: FeatureAttributionStepOutput,
         batch: Union[DecoderOnlyBatch, EncoderDecoderBatch],
         target_tokens: OneOrMoreTokenSequences,
         target_ids: TargetIdsTensor,
         contrast_batch: Optional[DecoderOnlyBatch] = None,
-        contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+        contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     ) -> FeatureAttributionStepOutput:
         r"""Enriches the attribution output with token information, producing the finished
         :class:`~inseq.data.FeatureAttributionStepOutput` object.
 
         Args:
             step_output (:class:`~inseq.data.FeatureAttributionStepOutput`): The output produced
                 by the attribution step, with missing batch information.
@@ -142,28 +142,28 @@
     def get_text_sequences(
         attribution_model: "AttributionModel", batch: Union[DecoderOnlyBatch, EncoderDecoderBatch]
     ) -> TextSequences:
         raise NotImplementedError()
 
     @staticmethod
     @abstractmethod
-    def get_step_function_reserved_args() -> List[str]:
+    def get_step_function_reserved_args() -> list[str]:
         raise NotImplementedError()
 
     @staticmethod
     def format_contrast_targets_alignments(
-        contrast_targets_alignments: Union[List[Tuple[int, int]], List[List[Tuple[int, int]]], str],
-        target_sequences: List[str],
-        target_tokens: List[List[str]],
-        contrast_sequences: List[str],
-        contrast_tokens: List[List[str]],
-        special_tokens: List[str] = [],
+        contrast_targets_alignments: Union[list[tuple[int, int]], list[list[tuple[int, int]]], str],
+        target_sequences: list[str],
+        target_tokens: list[list[str]],
+        contrast_sequences: list[str],
+        contrast_tokens: list[list[str]],
+        special_tokens: list[str] = [],
         start_pos: int = 0,
         end_pos: Optional[int] = None,
-    ) -> Tuple[DecoderOnlyBatch, Optional[List[List[Tuple[int, int]]]]]:
+    ) -> tuple[DecoderOnlyBatch, Optional[list[list[tuple[int, int]]]]]:
         # Ensure that the contrast_targets_alignments are in the correct format (list of lists of idxs pairs)
         if contrast_targets_alignments:
             if isinstance(contrast_targets_alignments, list) and len(contrast_targets_alignments) > 0:
                 if isinstance(contrast_targets_alignments[0], tuple):
                     contrast_targets_alignments = [contrast_targets_alignments]
                 if not isinstance(contrast_targets_alignments[0], list):
                     raise ValueError("Invalid contrast_targets_alignments were provided.")
@@ -252,15 +252,15 @@
     @default_attributed_fn_id.setter
     def set_attributed_fn(self, fn: str):
         if fn not in STEP_SCORES_MAP:
             raise ValueError(f"Unknown function: {fn}. Register custom functions with inseq.register_step_function")
         self._default_attributed_fn_id = fn
 
     @property
-    def info(self) -> Dict[Optional[str], Optional[str]]:
+    def info(self) -> dict[Optional[str], Optional[str]]:
         return {
             "model_name": self.model_name,
             "model_class": self.model.__class__.__name__ if self.model is not None else None,
         }
 
     def get_attribution_method(
         self,
@@ -305,21 +305,21 @@
         override_default_attribution: Optional[bool] = False,
         attr_pos_start: Optional[int] = None,
         attr_pos_end: Optional[int] = None,
         show_progress: bool = True,
         pretty_progress: bool = True,
         output_step_attributions: bool = False,
         attribute_target: bool = False,
-        step_scores: List[str] = [],
+        step_scores: list[str] = [],
         include_eos_baseline: bool = False,
         attributed_fn: Union[str, Callable[..., SingleScorePerStepTensor], None] = None,
         device: Optional[str] = None,
         batch_size: Optional[int] = None,
         generate_from_target_prefix: bool = False,
-        generation_args: Dict[str, Any] = {},
+        generation_args: dict[str, Any] = {},
         **kwargs,
     ) -> FeatureAttributionOutput:
         """Perform sequential attribution of input texts for every token in generated texts using the specified method.
 
         Args:
             input_texts (:obj:`str` or :obj:`list(str)`): One or more input texts to be attributed.
             generated_texts (:obj:`str` or :obj:`list(str)`, `optional`): One or more generated texts to be used as
@@ -382,14 +382,32 @@
             logger.warning(
                 "generate_from_target_prefix parameter is set to True, but will be ignored (not an encoder-decoder)."
             )
             generate_from_target_prefix = False
         original_device = self.device
         if device is not None:
             self.device = device
+        attribution_method = self.get_attribution_method(method, override_default_attribution)
+        attributed_fn = self.get_attributed_fn(attributed_fn)
+        attribution_args, attributed_fn_args, step_scores_args = extract_args(
+            attribution_method,
+            attributed_fn,
+            step_scores,
+            default_args=self.formatter.get_step_function_reserved_args(),
+            **kwargs,
+        )
+        if isnotebook():
+            logger.debug("Pretty progress currently not supported in notebooks, falling back to tqdm.")
+            pretty_progress = False
+        if attribution_method.is_final_step_method:
+            if step_scores:
+                raise ValueError(
+                    "Step scores are not supported for final step methods since they do not iterate over the full"
+                    " sequence. Please remove the step scores and compute them separatly passing method='dummy'."
+                )
         input_texts, generated_texts = format_input_texts(input_texts, generated_texts)
         has_generated_texts = generated_texts is not None
         if not self.is_encoder_decoder:
             for i in range(len(input_texts)):
                 if not input_texts[i]:
                     input_texts[i] = self.bos_token
                     if has_generated_texts and not generated_texts[i].startswith(self.bos_token):
@@ -407,44 +425,38 @@
                 encoded_input, return_generation_output=False, batch_size=batch_size, **generation_args
             )
         elif generation_args:
             logger.warning(
                 f"Generation arguments {generation_args} are provided, but will be ignored (constrained decoding)."
             )
         logger.debug(f"reference_texts={generated_texts}")
-        attribution_method = self.get_attribution_method(method, override_default_attribution)
-        attributed_fn = self.get_attributed_fn(attributed_fn)
-        attribution_args, attributed_fn_args, step_scores_args = extract_args(
-            attribution_method,
-            attributed_fn,
-            step_scores,
-            default_args=self.formatter.get_step_function_reserved_args(),
-            **kwargs,
-        )
-        if isnotebook():
-            logger.debug("Pretty progress currently not supported in notebooks, falling back to tqdm.")
-            pretty_progress = False
         if not self.is_encoder_decoder:
             assert all(
                 generated_texts[idx].startswith(input_texts[idx]) for idx in range(len(input_texts))
             ), "Forced generations with decoder-only models must start with the input texts."
             if has_generated_texts and len(input_texts) > 1:
-                logger.info(
+                logger.warning(
                     "Batched constrained decoding is currently not supported for decoder-only models."
                     " Using batch size of 1."
                 )
                 batch_size = 1
             if len(input_texts) > 1 and (attr_pos_start is not None or attr_pos_end is not None):
-                logger.info(
+                logger.warning(
                     "Custom attribution positions are currently not supported when batching generations for"
                     " decoder-only models. Using batch size of 1."
                 )
                 batch_size = 1
+        elif attribution_method.is_final_step_method and len(input_texts) > 1:
+            logger.warning(
+                "Batched attribution with encoder-decoder models currently not supported for final-step methods."
+                " Using batch size of 1."
+            )
+            batch_size = 1
         if attribution_method.method_name == "lime":
-            logger.info("Batched attribution currently not supported for LIME. Using batch size of 1.")
+            logger.warning("Batched attribution currently not supported for LIME. Using batch size of 1.")
             batch_size = 1
         attribution_outputs = attribution_method.prepare_and_attribute(
             input_texts,
             generated_texts,
             batch_size=batch_size,
             attr_pos_start=attr_pos_start,
             attr_pos_end=attr_pos_end,
@@ -479,16 +491,16 @@
             inputs = batch.input_ids
         return self.embed_ids(inputs, as_targets=as_targets)
 
     def get_token_with_ids(
         self,
         batch: Union[EncoderDecoderBatch, DecoderOnlyBatch],
         contrast_target_tokens: Optional[OneOrMoreTokenSequences] = None,
-        contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
-    ) -> List[List[TokenWithId]]:
+        contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
+    ) -> list[list[TokenWithId]]:
         if contrast_target_tokens is not None:
             return join_token_ids(
                 batch.target_tokens,
                 batch.target_ids.tolist(),
                 contrast_target_tokens,
                 contrast_targets_alignments,
             )
@@ -499,15 +511,15 @@
     @unhooked
     @abstractmethod
     def generate(
         self,
         encodings: Union[TextInput, BatchEncoding],
         return_generation_output: Optional[bool] = False,
         **kwargs,
-    ) -> Union[List[str], Tuple[List[str], Any]]:
+    ) -> Union[list[str], tuple[list[str], Any]]:
         pass
 
     @staticmethod
     @abstractmethod
     def output2logits(forward_output) -> LogitsTensor:
         pass
 
@@ -518,15 +530,15 @@
         as_targets: bool = False,
         return_baseline: bool = False,
         include_eos_baseline: bool = False,
     ) -> BatchEncoding:
         pass
 
     @abstractmethod
-    def decode(self, ids: IdsTensor, skip_special_tokens: bool = True) -> List[str]:
+    def decode(self, ids: IdsTensor, skip_special_tokens: bool = True) -> list[str]:
         pass
 
     @abstractmethod
     def embed_ids(self, ids: IdsTensor, as_targets: bool = False) -> EmbeddingsTensor:
         pass
 
     @abstractmethod
@@ -534,15 +546,15 @@
         self, ids: torch.Tensor, skip_special_tokens: Optional[bool] = True
     ) -> OneOrMoreTokenSequences:
         pass
 
     @abstractmethod
     def convert_tokens_to_ids(
         self,
-        tokens: Union[List[str], List[List[str]]],
+        tokens: Union[list[str], list[list[str]]],
     ) -> OneOrMoreIdSequences:
         pass
 
     @abstractmethod
     def convert_tokens_to_string(
         self,
         tokens: OneOrMoreTokenSequences,
@@ -567,20 +579,20 @@
         skip_special_tokens: bool = False,
         as_targets: bool = False,
     ):
         pass
 
     @property
     @abstractmethod
-    def special_tokens(self) -> List[str]:
+    def special_tokens(self) -> list[str]:
         pass
 
     @property
     @abstractmethod
-    def special_tokens_ids(self) -> List[int]:
+    def special_tokens_ids(self) -> list[int]:
         pass
 
     @property
     @abstractmethod
     def vocabulary_embeddings(self) -> VocabularyEmbeddingsTensor:
         pass
 
@@ -622,31 +634,31 @@
 
     @abstractmethod
     def get_decoder(self) -> torch.nn.Module:
         pass
 
     @staticmethod
     @abstractmethod
-    def get_attentions_dict(output: ModelOutput) -> Dict[str, torch.Tensor]:
+    def get_attentions_dict(output: ModelOutput) -> dict[str, torch.Tensor]:
         pass
 
     @staticmethod
     @abstractmethod
-    def get_hidden_states_dict(output: ModelOutput) -> Dict[str, torch.Tensor]:
+    def get_hidden_states_dict(output: ModelOutput) -> dict[str, torch.Tensor]:
         pass
 
     # Model forward
 
     def _forward(
         self,
         batch: Union[DecoderOnlyBatch, EncoderDecoderBatch],
         target_ids: ExpandedTargetIdsTensor,
         attributed_fn: Callable[..., SingleScorePerStepTensor],
         use_embeddings: bool = True,
-        attributed_fn_argnames: Optional[List[str]] = None,
+        attributed_fn_argnames: Optional[list[str]] = None,
         *args,
         **kwargs,
     ) -> LogitsTensor:
         assert len(args) == len(attributed_fn_argnames), "Number of arguments and number of argnames must match"
         target_ids = target_ids.squeeze(-1)
         output = self.get_forward_output(batch, use_embeddings=use_embeddings, **kwargs)
         logger.debug(f"logits: {pretty_tensor(output.logits)}")
```

### Comparing `inseq-0.5.0/inseq/models/decoder_only.py` & `inseq-0.6.0/inseq/models/decoder_only.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Optional, TypeVar, Union
 
 import torch
 
 from ..attr.feat import join_token_ids
 from ..attr.step_functions import StepFunctionDecoderOnlyArgs
 from ..data import (
     BatchEmbedding,
@@ -50,19 +50,19 @@
 
     @staticmethod
     def format_attribution_args(
         batch: DecoderOnlyBatch,
         target_ids: TargetIdsTensor,
         attributed_fn: Callable[..., SingleScorePerStepTensor],
         attribute_target: bool = False,  # Needed for compatibility with EncoderDecoderAttributionModel
-        attributed_fn_args: Dict[str, Any] = {},
+        attributed_fn_args: dict[str, Any] = {},
         attribute_batch_ids: bool = False,
         forward_batch_embeds: bool = True,
         use_baselines: bool = False,
-    ) -> Tuple[Dict[str, Any], Tuple[Union[IdsTensor, EmbeddingsTensor, None], ...]]:
+    ) -> tuple[dict[str, Any], tuple[Union[IdsTensor, EmbeddingsTensor, None], ...]]:
         if attribute_batch_ids:
             inputs = (batch.input_ids,)
             baselines = (batch.baseline_ids,)
         else:
             inputs = (batch.input_embeds,)
             baselines = (batch.baseline_embeds,)
         attribute_fn_args = {
@@ -92,15 +92,15 @@
     def enrich_step_output(
         attribution_model: "DecoderOnlyAttributionModel",
         step_output: FeatureAttributionStepOutput,
         batch: DecoderOnlyBatch,
         target_tokens: OneOrMoreTokenSequences,
         target_ids: TargetIdsTensor,
         contrast_batch: Optional[DecoderOnlyBatch] = None,
-        contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+        contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     ) -> FeatureAttributionStepOutput:
         r"""Enriches the attribution output with token information, producing the finished
         :class:`~inseq.data.FeatureAttributionStepOutput` object.
 
         Args:
             step_output (:class:`~inseq.data.FeatureAttributionStepOutput`): The output produced
                 by the attribution step, with missing batch information.
@@ -115,15 +115,15 @@
             target_ids = target_ids.unsqueeze(0)
         step_output.source = None
         if contrast_batch is not None:
             contrast_aligned_idx = get_aligned_idx(len(batch.target_tokens[0]), contrast_targets_alignments[0])
             contrast_target_ids = contrast_batch.target_ids[:, contrast_aligned_idx]
             step_output.target = join_token_ids(
                 tokens=target_tokens,
-                ids=attribution_model.convert_ids_to_tokens(contrast_target_ids),
+                ids=attribution_model.convert_ids_to_tokens(contrast_target_ids, skip_special_tokens=False),
                 contrast_tokens=attribution_model.convert_ids_to_tokens(
                     contrast_target_ids[None, ...], skip_special_tokens=False
                 ),
             )
             step_output.prefix = join_token_ids(tokens=batch.target_tokens, ids=batch.target_ids.tolist())
         else:
             step_output.target = join_token_ids(target_tokens, [[idx] for idx in target_ids.tolist()])
@@ -171,15 +171,15 @@
             self: "DecoderOnlyAttributionModel",
             forward_tensor: AttributionForwardInputs,
             input_ids: IdsTensor,
             target_ids: ExpandedTargetIdsTensor,
             attributed_fn: Callable[..., SingleScorePerStepTensor],
             attention_mask: Optional[IdsTensor] = None,
             use_embeddings: bool = True,
-            attributed_fn_argnames: Optional[List[str]] = None,
+            attributed_fn_argnames: Optional[list[str]] = None,
             *args,
             **kwargs,
         ) -> CustomForwardOutput:
             batch = self.formatter.convert_args_to_batch(
                 decoder_input_ids=input_ids,
                 decoder_attention_mask=attention_mask,
                 decoder_input_embeds=forward_tensor if use_embeddings else None,
@@ -194,15 +194,15 @@
     def get_text_sequences(attribution_model: "DecoderOnlyAttributionModel", batch: DecoderOnlyBatch) -> TextSequences:
         return TextSequences(
             sources=None,
             targets=attribution_model.decode(batch.target_ids),
         )
 
     @staticmethod
-    def get_step_function_reserved_args() -> List[str]:
+    def get_step_function_reserved_args() -> list[str]:
         return [f.name for f in StepFunctionDecoderOnlyArgs.__dataclass_fields__.values()]
 
 
 class DecoderOnlyAttributionModel(AttributionModel):
     """AttributionModel class for attributing encoder-decoder models."""
 
     formatter = DecoderOnlyInputFormatter
```

### Comparing `inseq-0.5.0/inseq/models/encoder_decoder.py` & `inseq-0.6.0/inseq/models/encoder_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from functools import wraps
-from typing import Any, Callable, Dict, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Optional, TypeVar, Union
 
 from ..attr.feat import join_token_ids
 from ..attr.step_functions import StepFunctionEncoderDecoderArgs
 from ..data import (
     Batch,
     BatchEmbedding,
     BatchEncoding,
@@ -32,15 +32,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class EncoderDecoderInputFormatter(InputFormatter):
     def prepare_inputs_for_attribution(
         attribution_model: "EncoderDecoderAttributionModel",
-        inputs: Tuple[FeatureAttributionInput, FeatureAttributionInput],
+        inputs: tuple[FeatureAttributionInput, FeatureAttributionInput],
         include_eos_baseline: bool = False,
     ) -> EncoderDecoderBatch:
         r"""Prepares sources and target to produce an :class:`~inseq.data.EncoderDecoderBatch`.
         There are two stages of preparation:
 
             1. Raw text sources and target texts are encoded by the model.
             2. The encoded sources and targets are converted to tensors for the forward pass.
@@ -78,19 +78,19 @@
 
     @staticmethod
     def format_attribution_args(
         batch: EncoderDecoderBatch,
         target_ids: TargetIdsTensor,
         attributed_fn: Callable[..., SingleScorePerStepTensor],
         attribute_target: bool = False,
-        attributed_fn_args: Dict[str, Any] = {},
+        attributed_fn_args: dict[str, Any] = {},
         attribute_batch_ids: bool = False,
         forward_batch_embeds: bool = True,
         use_baselines: bool = False,
-    ) -> Tuple[Dict[str, Any], Tuple[Union[IdsTensor, EmbeddingsTensor, None], ...]]:
+    ) -> tuple[dict[str, Any], tuple[Union[IdsTensor, EmbeddingsTensor, None], ...]]:
         if attribute_batch_ids:
             inputs = (batch.sources.input_ids,)
             baselines = (batch.sources.baseline_ids,)
         else:
             inputs = (batch.sources.input_embeds,)
             baselines = (batch.sources.baseline_embeds,)
         if attribute_target:
@@ -133,15 +133,15 @@
     def enrich_step_output(
         attribution_model: "EncoderDecoderAttributionModel",
         step_output: FeatureAttributionStepOutput,
         batch: EncoderDecoderBatch,
         target_tokens: OneOrMoreTokenSequences,
         target_ids: TargetIdsTensor,
         contrast_batch: Optional[DecoderOnlyBatch] = None,
-        contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+        contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     ) -> FeatureAttributionStepOutput:
         r"""Enriches the attribution output with token information, producing the finished
         :class:`~inseq.data.FeatureAttributionStepOutput` object.
 
         Args:
             step_output (:class:`~inseq.data.FeatureAttributionStepOutput`): The output produced
                 by the attribution step, with missing batch information.
@@ -228,15 +228,15 @@
             encoder_input_ids: IdsTensor,
             decoder_input_ids: IdsTensor,
             target_ids: ExpandedTargetIdsTensor,
             attributed_fn: Callable[..., SingleScorePerStepTensor],
             encoder_attention_mask: Optional[IdsTensor] = None,
             decoder_attention_mask: Optional[IdsTensor] = None,
             use_embeddings: bool = True,
-            attributed_fn_argnames: Optional[List[str]] = None,
+            attributed_fn_argnames: Optional[list[str]] = None,
             *args,
             **kwargs,
         ) -> CustomForwardOutput:
             batch = self.formatter.convert_args_to_batch(
                 encoder_input_ids=encoder_input_ids,
                 decoder_input_ids=decoder_input_ids,
                 encoder_attention_mask=encoder_attention_mask,
@@ -256,15 +256,15 @@
     ) -> TextSequences:
         return TextSequences(
             sources=attribution_model.convert_tokens_to_string(batch.sources.input_tokens),
             targets=attribution_model.decode(batch.targets.input_ids),
         )
 
     @staticmethod
-    def get_step_function_reserved_args() -> List[str]:
+    def get_step_function_reserved_args() -> list[str]:
         return [f.name for f in StepFunctionEncoderDecoderArgs.__dataclass_fields__.values()]
 
 
 class EncoderDecoderAttributionModel(AttributionModel):
     """AttributionModel class for attributing encoder-decoder models."""
 
     formatter = EncoderDecoderInputFormatter
```

### Comparing `inseq-0.5.0/inseq/models/huggingface_model.py` & `inseq-0.6.0/inseq/models/huggingface_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """HuggingFace Seq2seq model."""
 import logging
 from abc import abstractmethod
-from typing import Dict, List, NoReturn, Optional, Tuple, Union
+from typing import Any, NoReturn, Optional, Union
 
 import torch
 from torch import long
 from transformers import (
     AutoConfig,
     AutoModelForCausalLM,
     AutoModelForSeq2SeqLM,
@@ -65,14 +65,16 @@
 
     def __init__(
         self,
         model: Union[str, PreTrainedModel],
         attribution_method: Optional[str] = None,
         tokenizer: Union[str, PreTrainedTokenizerBase, None] = None,
         device: Optional[str] = None,
+        model_kwargs: Optional[dict[str, Any]] = {},
+        tokenizer_kwargs: Optional[dict[str, Any]] = {},
         **kwargs,
     ) -> None:
         """AttributionModel subclass for Huggingface-compatible models.
 
         Args:
             model (:obj:`str` or :obj:`transformers.PreTrainedModel`): the name of the model in the
                 Huggingface Hub or path to folder containing local model files.
@@ -86,46 +88,41 @@
             **kwargs: additional arguments for the model and the tokenizer.
         """
         super().__init__(**kwargs)
         if self._autoclass is None or self._autoclass not in SUPPORTED_AUTOCLASSES:
             raise ValueError(
                 f"Invalid autoclass {self._autoclass}. Must be one of {[x.__name__ for x in SUPPORTED_AUTOCLASSES]}."
             )
-        model_args = kwargs.pop("model_args", {})
-        model_kwargs = kwargs.pop("model_kwargs", {})
         if isinstance(model, PreTrainedModel):
             self.model = model
         else:
             if "output_attentions" not in model_kwargs:
                 model_kwargs["output_attentions"] = True
 
-            self.model = self._autoclass.from_pretrained(model, *model_args, **model_kwargs)
+            self.model = self._autoclass.from_pretrained(model, **model_kwargs)
         self.model_name = self.model.config.name_or_path
         self.tokenizer_name = tokenizer if isinstance(tokenizer, str) else None
         if tokenizer is None:
             tokenizer = model if isinstance(model, str) else self.model_name
             if not tokenizer:
                 raise ValueError(
                     "Unspecified tokenizer for model loaded from scratch. Use explicit identifier as tokenizer=<ID>"
                     "during model loading."
                 )
-        tokenizer_inputs = kwargs.pop("tokenizer_inputs", {})
-        tokenizer_kwargs = kwargs.pop("tokenizer_kwargs", {})
-
         if isinstance(tokenizer, PreTrainedTokenizerBase):
             self.tokenizer = tokenizer
         else:
-            self.tokenizer = AutoTokenizer.from_pretrained(tokenizer, *tokenizer_inputs, **tokenizer_kwargs)
+            self.tokenizer = AutoTokenizer.from_pretrained(tokenizer, **tokenizer_kwargs)
         if self.model.config.pad_token_id is not None:
-            self.pad_token = self.tokenizer.convert_ids_to_tokens(self.model.config.pad_token_id)
+            self.pad_token = self._convert_ids_to_tokens(self.model.config.pad_token_id, skip_special_tokens=False)
             self.tokenizer.pad_token = self.pad_token
         self.bos_token_id = getattr(self.model.config, "decoder_start_token_id", None)
         if self.bos_token_id is None:
             self.bos_token_id = self.model.config.bos_token_id
-        self.bos_token = self.tokenizer.convert_ids_to_tokens(self.bos_token_id)
+        self.bos_token = self._convert_ids_to_tokens(self.bos_token_id, skip_special_tokens=False)
         self.eos_token_id = getattr(self.model.config, "eos_token_id", None)
         if self.eos_token_id is None:
             self.eos_token_id = self.tokenizer.pad_token_id
         if self.tokenizer.unk_token_id is None:
             self.tokenizer.unk_token_id = self.tokenizer.pad_token_id
         self.embed_scale = 1.0
         self.encoder_int_embeds = None
@@ -136,25 +133,31 @@
 
     @staticmethod
     def load(
         model: Union[str, PreTrainedModel],
         attribution_method: Optional[str] = None,
         tokenizer: Union[str, PreTrainedTokenizerBase, None] = None,
         device: str = None,
+        model_kwargs: Optional[dict[str, Any]] = {},
+        tokenizer_kwargs: Optional[dict[str, Any]] = {},
         **kwargs,
     ) -> "HuggingfaceModel":
         """Loads a HuggingFace model and tokenizer and wraps them in the appropriate AttributionModel."""
         if isinstance(model, str):
-            is_encoder_decoder = AutoConfig.from_pretrained(model).is_encoder_decoder
+            is_encoder_decoder = AutoConfig.from_pretrained(model, **model_kwargs).is_encoder_decoder
         else:
             is_encoder_decoder = model.config.is_encoder_decoder
         if is_encoder_decoder:
-            return HuggingfaceEncoderDecoderModel(model, attribution_method, tokenizer, device, **kwargs)
+            return HuggingfaceEncoderDecoderModel(
+                model, attribution_method, tokenizer, device, model_kwargs, tokenizer_kwargs, **kwargs
+            )
         else:
-            return HuggingfaceDecoderOnlyModel(model, attribution_method, tokenizer, device, **kwargs)
+            return HuggingfaceDecoderOnlyModel(
+                model, attribution_method, tokenizer, device, model_kwargs, tokenizer_kwargs, **kwargs
+            )
 
     @AttributionModel.device.setter
     def device(self, new_device: str) -> None:
         check_device(new_device)
         self._device = new_device
         is_loaded_in_8bit = getattr(self.model, "is_loaded_in_8bit", False)
         is_loaded_in_4bit = getattr(self.model, "is_loaded_in_4bit", False)
@@ -172,39 +175,43 @@
 
     @abstractmethod
     def configure_embeddings_scale(self) -> None:
         """Configure the scale factor for embeddings."""
         pass
 
     @property
-    def info(self) -> Dict[str, str]:
-        dic_info: Dict[str, str] = super().info
+    def info(self) -> dict[str, str]:
+        dic_info: dict[str, str] = super().info
         extra_info = {
             "tokenizer_name": self.tokenizer_name,
             "tokenizer_class": self.tokenizer.__class__.__name__,
         }
         dic_info.update(extra_info)
         return dic_info
 
     @unhooked
     @batched
     def generate(
         self,
         inputs: Union[TextInput, BatchEncoding],
         return_generation_output: bool = False,
         skip_special_tokens: bool = True,
+        output_generated_only: bool = False,
         **kwargs,
-    ) -> Union[List[str], Tuple[List[str], ModelOutput]]:
+    ) -> Union[list[str], tuple[list[str], ModelOutput]]:
         """Wrapper of model.generate to handle tokenization and decoding.
 
         Args:
             inputs (`Union[TextInput, BatchEncoding]`):
                 Inputs to be provided to the model for generation.
             return_generation_output (`bool`, *optional*, defaults to False):
                 If true, generation outputs are returned alongside the generated text.
+            output_generated_only (`bool`, *optional*, defaults to False):
+                If true, only the generated text is returned. Relevant for decoder-only models that would otherwise return
+                the full input + output.
 
         Returns:
             `Union[List[str], Tuple[List[str], ModelOutput]]`: Generated text or a tuple of generated text and
             generation outputs.
         """
         if isinstance(inputs, str) or (
             isinstance(inputs, list) and len(inputs) > 0 and all(isinstance(x, str) for x in inputs)
@@ -213,14 +220,16 @@
         inputs = inputs.to(self.device)
         generation_out = self.model.generate(
             inputs=inputs.input_ids,
             return_dict_in_generate=True,
             **kwargs,
         )
         sequences = generation_out.sequences
+        if output_generated_only and not self.is_encoder_decoder:
+            sequences = sequences[:, inputs.input_ids.shape[1] :]
         texts = self.decode(ids=sequences, skip_special_tokens=skip_special_tokens)
         if return_generation_output:
             return texts, generation_out
         return texts
 
     @staticmethod
     def output2logits(forward_output: Union[Seq2SeqLMOutput, CausalLMOutput]) -> LogitsTensor:
@@ -270,24 +279,24 @@
             batch["attention_mask"] = torch.cat((ones_mask, batch["attention_mask"]), dim=1)
             bos_ids = ones_mask * self.bos_token_id
             batch["input_ids"] = torch.cat((bos_ids, batch["input_ids"]), dim=1)
             if return_baseline:
                 baseline_ids = torch.cat((bos_ids, baseline_ids), dim=1)
         return BatchEncoding(
             input_ids=batch["input_ids"],
-            input_tokens=[self.tokenizer.convert_ids_to_tokens(x) for x in batch["input_ids"]],
+            input_tokens=[self._convert_ids_to_tokens(x, skip_special_tokens=False) for x in batch["input_ids"]],
             attention_mask=batch["attention_mask"],
             baseline_ids=baseline_ids,
         )
 
     def decode(
         self,
-        ids: Union[List[int], List[List[int]], IdsTensor],
+        ids: Union[list[int], list[list[int]], IdsTensor],
         skip_special_tokens: bool = True,
-    ) -> List[str]:
+    ) -> list[str]:
         return self.tokenizer.batch_decode(
             ids,
             skip_special_tokens=skip_special_tokens,
             clean_up_tokenization_spaces=False,
         )
 
     def embed_ids(self, ids: IdsTensor, as_targets: bool = False) -> EmbeddingsTensor:
@@ -297,37 +306,43 @@
             embeddings = self.encoder_int_embeds.indices_to_embeddings(ids)
         elif self.decoder_int_embeds is not None and as_targets:
             embeddings = self.decoder_int_embeds.indices_to_embeddings(ids)
         else:
             embeddings = self.get_embedding_layer()(ids)
         return embeddings * self.embed_scale
 
+    def _convert_ids_to_tokens(self, ids: IdsTensor, skip_special_tokens: bool = True) -> OneOrMoreTokenSequences:
+        tokens = self.tokenizer.convert_ids_to_tokens(ids, skip_special_tokens=skip_special_tokens)
+        if isinstance(tokens, bytes) and not isinstance(tokens, str):
+            return tokens.decode("utf-8")
+        elif isinstance(tokens, list):
+            return [t.decode("utf-8") if isinstance(t, bytes) else t for t in tokens]
+        return tokens
+
     def convert_ids_to_tokens(
         self, ids: IdsTensor, skip_special_tokens: Optional[bool] = True
     ) -> OneOrMoreTokenSequences:
         if ids.ndim < 2:
-            return self.tokenizer.convert_ids_to_tokens(ids, skip_special_tokens=skip_special_tokens)
-        return [
-            self.tokenizer.convert_ids_to_tokens(id_slice, skip_special_tokens=skip_special_tokens) for id_slice in ids
-        ]
+            return self._convert_ids_to_tokens(ids, skip_special_tokens)
+        return [self._convert_ids_to_tokens(id_slice, skip_special_tokens) for id_slice in ids]
 
     def convert_tokens_to_ids(self, tokens: TextInput) -> OneOrMoreIdSequences:
         if isinstance(tokens[0], str):
             return self.tokenizer.convert_tokens_to_ids(tokens)
         return [self.tokenizer.convert_tokens_to_ids(token_slice) for token_slice in tokens]
 
     def convert_tokens_to_string(
         self,
         tokens: OneOrMoreTokenSequences,
         skip_special_tokens: bool = True,
         as_targets: bool = False,
     ) -> TextInput:
         if isinstance(tokens, list) and len(tokens) == 0:
             return ""
-        elif isinstance(tokens[0], str):
+        elif isinstance(tokens[0], (bytes, str)):
             tmp_decode_state = self.tokenizer._decode_use_source_tokenizer
             self.tokenizer._decode_use_source_tokenizer = not as_targets
             out_strings = self.tokenizer.convert_tokens_to_string(
                 tokens if not skip_special_tokens else [t for t in tokens if t not in self.special_tokens]
             )
             self.tokenizer._decode_use_source_tokenizer = tmp_decode_state
             return out_strings
@@ -341,15 +356,15 @@
     ) -> OneOrMoreTokenSequences:
         if isinstance(text, str):
             ids = self.tokenizer(
                 text=text if not as_targets else None,
                 text_target=text if as_targets else None,
                 add_special_tokens=not skip_special_tokens,
             )["input_ids"]
-            return self.tokenizer.convert_ids_to_tokens(ids, skip_special_tokens)
+            return self._convert_ids_to_tokens(ids, skip_special_tokens)
         return [self.convert_string_to_tokens(t, skip_special_tokens, as_targets) for t in text]
 
     def clean_tokens(
         self,
         tokens: OneOrMoreTokenSequences,
         skip_special_tokens: bool = False,
         as_targets: bool = False,
@@ -365,33 +380,33 @@
                 If true, a target tokenizer is used to clean the tokens.
 
         Returns:
             `OneOrMoreTokenSequences`: A list containing one or more lists of cleaned tokens.
         """
         if isinstance(tokens, list) and len(tokens) == 0:
             return []
-        elif isinstance(tokens[0], str):
+        elif isinstance(tokens[0], (bytes, str)):
             clean_tokens = []
             for tok in tokens:
                 clean_tok = self.convert_tokens_to_string(
                     [tok], skip_special_tokens=skip_special_tokens, as_targets=as_targets
                 )
                 if clean_tok:
                     clean_tokens.append(clean_tok)
                 elif tok:
                     clean_tokens.append(" ")
             return clean_tokens
         return [self.clean_tokens(token_seq, skip_special_tokens, as_targets) for token_seq in tokens]
 
     @property
-    def special_tokens(self) -> List[str]:
+    def special_tokens(self) -> list[str]:
         return self.tokenizer.all_special_tokens
 
     @property
-    def special_tokens_ids(self) -> List[int]:
+    def special_tokens_ids(self) -> list[int]:
         return self.tokenizer.all_special_ids
 
     @property
     def vocabulary_embeddings(self) -> VocabularyEmbeddingsTensor:
         return self.get_embedding_layer().weight
 
     def get_embedding_layer(self) -> torch.nn.Module:
@@ -405,24 +420,14 @@
     Attributes:
         model (::obj:`transformers.AutoModelForSeq2SeqLM`):
             the model on which attribution is performed.
     """
 
     _autoclass = AutoModelForSeq2SeqLM
 
-    def __init__(
-        self,
-        model: Union[str, PreTrainedModel],
-        attribution_method: Optional[str] = None,
-        tokenizer: Union[str, PreTrainedTokenizerBase, None] = None,
-        device: str = None,
-        **kwargs,
-    ) -> NoReturn:
-        super().__init__(model, attribution_method, tokenizer, device, **kwargs)
-
     def configure_embeddings_scale(self):
         encoder = self.model.get_encoder()
         decoder = self.model.get_decoder()
         if hasattr(encoder, "embed_scale"):
             self.embed_scale = encoder.embed_scale
         if hasattr(decoder, "embed_scale") and decoder.embed_scale != self.embed_scale:
             raise ValueError("Different encoder and decoder embed scales are not supported")
@@ -432,25 +437,25 @@
 
     def get_decoder(self) -> torch.nn.Module:
         return self.model.get_decoder()
 
     @staticmethod
     def get_attentions_dict(
         output: Seq2SeqLMOutput,
-    ) -> Dict[str, MultiLayerMultiUnitScoreTensor]:
+    ) -> dict[str, MultiLayerMultiUnitScoreTensor]:
         if output.encoder_attentions is None or output.decoder_attentions is None:
             raise ValueError("Model does not support attribution relying on attention outputs.")
         return {
             "encoder_self_attentions": torch.stack(output.encoder_attentions, dim=1),
             "decoder_self_attentions": torch.stack(output.decoder_attentions, dim=1),
             "cross_attentions": torch.stack(output.cross_attentions, dim=1),
         }
 
     @staticmethod
-    def get_hidden_states_dict(output: Seq2SeqLMOutput) -> Dict[str, MultiLayerEmbeddingsTensor]:
+    def get_hidden_states_dict(output: Seq2SeqLMOutput) -> dict[str, MultiLayerEmbeddingsTensor]:
         return {
             "encoder_hidden_states": torch.stack(output.encoder_hidden_states, dim=1),
             "decoder_hidden_states": torch.stack(output.decoder_hidden_states, dim=1),
         }
 
 
 class HuggingfaceDecoderOnlyModel(HuggingfaceModel, DecoderOnlyAttributionModel):
@@ -466,33 +471,35 @@
 
     def __init__(
         self,
         model: Union[str, PreTrainedModel],
         attribution_method: Optional[str] = None,
         tokenizer: Union[str, PreTrainedTokenizerBase, None] = None,
         device: str = None,
+        model_kwargs: Optional[dict[str, Any]] = {},
+        tokenizer_kwargs: Optional[dict[str, Any]] = {},
         **kwargs,
     ) -> NoReturn:
-        super().__init__(model, attribution_method, tokenizer, device, **kwargs)
+        super().__init__(model, attribution_method, tokenizer, device, model_kwargs, tokenizer_kwargs, **kwargs)
         self.tokenizer.padding_side = "left"
         self.tokenizer.truncation_side = "left"
         if self.pad_token is None:
             self.pad_token = self.tokenizer.bos_token
             self.tokenizer.pad_token = self.tokenizer.bos_token
 
     def configure_embeddings_scale(self):
         if hasattr(self.model, "embed_scale"):
             self.embed_scale = self.model.embed_scale
 
     @staticmethod
-    def get_attentions_dict(output: CausalLMOutput) -> Dict[str, MultiLayerMultiUnitScoreTensor]:
+    def get_attentions_dict(output: CausalLMOutput) -> dict[str, MultiLayerMultiUnitScoreTensor]:
         if output.attentions is None:
             raise ValueError("Model does not support attribution relying on attention outputs.")
         return {
             "decoder_self_attentions": torch.stack(output.attentions, dim=1),
         }
 
     @staticmethod
-    def get_hidden_states_dict(output: CausalLMOutput) -> Dict[str, MultiLayerEmbeddingsTensor]:
+    def get_hidden_states_dict(output: CausalLMOutput) -> dict[str, MultiLayerEmbeddingsTensor]:
         return {
             "decoder_hidden_states": torch.stack(output.hidden_states, dim=1),
         }
```

### Comparing `inseq-0.5.0/inseq/models/model_config.py` & `inseq-0.6.0/inseq/models/model_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import logging
 from dataclasses import dataclass
 from pathlib import Path
+from typing import Optional
 
 import yaml
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ModelConfig:
     """Configuration used by the methods for which the attribute ``use_model_config=True``.
+
     Args:
-        attention_module (:obj:`str`):
-            The name of the module performing the attention computation (e.g.``attn`` for the GPT-2 model in
-            transformers). Can be identified by looking at the name of the attribute instantiating the attention module
+        self_attention_module (:obj:`str`):
+            The name of the module performing the self-attention computation (e.g.``attn`` for the GPT-2 model in
+            transformers). Can be identified by looking at the name of the self-attention module attribute
             in the model's transformer block class (e.g. :obj:`transformers.models.gpt2.GPT2Block` for GPT-2).
+        cross_attention_module (:obj:`str`):
+            The name of the module performing the cross-attention computation (e.g.``encoder_attn`` for MarianMT models
+            in transformers). Can be identified by looking at the name of the cross-attention module attribute
+            in the model's transformer block class (e.g. :obj:`transformers.models.marian.MarianDecoderLayer`).
+        value_vector (:obj:`str`):
+            The name of the variable in the forward pass of the attention module containing the value vector
+            (e.g. ``value`` for the GPT-2 model in transformers). Can be identified by looking at the forward pass of
+            the attention module (e.g. :obj:`transformers.models.gpt2.modeling_gpt2.GPT2Attention.forward` for GPT-2).
     """
 
-    attention_module: str
+    self_attention_module: str
+    value_vector: str
+    cross_attention_module: Optional[str] = None
 
 
 MODEL_CONFIGS = {
     model_type: ModelConfig(**cfg)
     for model_type, cfg in yaml.safe_load(open(Path(__file__).parent / "model_config.yaml", encoding="utf8")).items()
 }
```

### Comparing `inseq-0.5.0/inseq/utils/__init__.py` & `inseq-0.6.0/inseq/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from .alignment_utils import get_adjusted_alignments, get_aligned_idx
-from .argparse import InseqArgumentParser
+from .argparse import InseqArgumentParser, cli_arg
 from .cache import INSEQ_ARTIFACTS_CACHE, INSEQ_HOME_CACHE, cache_results
 from .errors import (
     InseqDeprecationWarning,
     LengthMismatchError,
     MissingAlignmentsError,
     MissingAttributionMethodError,
     UnknownAttributionMethodError,
 )
+from .hooks import StackFrame, get_post_variable_assignment_hook
 from .import_utils import (
     is_captum_available,
     is_datasets_available,
     is_ipywidgets_available,
     is_joblib_available,
+    is_nltk_available,
     is_scikitlearn_available,
     is_sentencepiece_available,
     is_transformers_available,
 )
 from .misc import (
     aggregate_token_pair,
     aggregate_token_sequence,
@@ -45,20 +47,24 @@
 from .registry import Registry, available_classes
 from .serialization import json_advanced_dump, json_advanced_dumps, json_advanced_load, json_advanced_loads
 from .torch_utils import (
     aggregate_contiguous,
     check_device,
     euclidean_distance,
     filter_logits,
+    find_block_stack,
     get_default_device,
     get_front_padding,
     get_sequences_from_batched_steps,
     normalize,
+    pad_with_nan,
+    recursive_get_submodule,
     remap_from_filtered,
     top_p_logits_mask,
+    validate_indices,
 )
 
 __all__ = [
     "LengthMismatchError",
     "MissingAttributionMethodError",
     "UnknownAttributionMethodError",
     "MissingAlignmentsError",
@@ -90,14 +96,15 @@
     "is_ipywidgets_available",
     "is_scikitlearn_available",
     "is_transformers_available",
     "is_sentencepiece_available",
     "is_datasets_available",
     "is_captum_available",
     "is_joblib_available",
+    "is_nltk_available",
     "check_device",
     "get_default_device",
     "ndarray_to_bin_str",
     "hashodict",
     "InseqDeprecationWarning",
     "get_module_name_from_object",
     "gzip_compress",
@@ -113,8 +120,14 @@
     "json_advanced_load",
     "get_nn_submodule",
     "find_block_stack",
     "get_adjusted_alignments",
     "get_aligned_idx",
     "top_p_logits_mask",
     "filter_logits",
+    "cli_arg",
+    "get_post_variable_assignment_hook",
+    "StackFrame",
+    "validate_indices",
+    "pad_with_nan",
+    "recursive_get_submodule",
 ]
```

### Comparing `inseq-0.5.0/inseq/utils/alignment_utils.py` & `inseq-0.6.0/inseq/utils/alignment_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
 import re
 from dataclasses import dataclass
 from enum import Enum
 from functools import lru_cache
 from itertools import chain
-from typing import List, Optional, Tuple, Union
+from typing import Optional, Union
 
 import torch
 from transformers import AutoModel, AutoTokenizer, PreTrainedModel, PreTrainedTokenizerBase
 
 from .misc import clean_tokens
 
 logger = logging.getLogger(__name__)
 
 ALIGN_MODEL_ID = "sentence-transformers/LaBSE"
 
 
 @dataclass
 class AlignedSequences:
-    source_tokens: List[str]
-    target_tokens: List[str]
-    alignments: List[Tuple[int, int]]
+    source_tokens: list[str]
+    target_tokens: list[str]
+    alignments: list[tuple[int, int]]
 
     @property
-    def aligned_tokens(self) -> List[Tuple[str, str]]:
+    def aligned_tokens(self) -> list[tuple[str, str]]:
         return [(self.source_tokens[a_idx], self.target_tokens[b_idx]) for a_idx, b_idx in self.alignments]
 
     def reverse(self) -> "AlignedSequences":
         return AlignedSequences(
             source_tokens=self.target_tokens,
             target_tokens=self.source_tokens,
             alignments=[(b_idx, a_idx) for a_idx, b_idx in self.alignments],
@@ -47,15 +47,15 @@
 
 
 @lru_cache
 def get_aligner_tokenizer() -> PreTrainedTokenizerBase:
     return AutoTokenizer.from_pretrained(ALIGN_MODEL_ID)
 
 
-def _preprocess_sequence_for_alignment(tokenized_seq: List[str]) -> Tuple[torch.Tensor, List[List[int]]]:
+def _preprocess_sequence_for_alignment(tokenized_seq: list[str]) -> tuple[torch.Tensor, list[list[int]]]:
     aligner_tokenizer = get_aligner_tokenizer()
     idxs = [aligner_tokenizer.convert_tokens_to_ids(x) for x in tokenized_seq]
     idxs = aligner_tokenizer.prepare_for_model(
         list(chain(*idxs)),
         return_tensors="pt",
         truncation=True,
         model_max_length=aligner_tokenizer.model_max_length,
@@ -63,16 +63,16 @@
     sub2word_map = []
     for i, word_list in enumerate(tokenized_seq):
         sub2word_map += [i for x in word_list]
     return idxs, sub2word_map
 
 
 def _get_aligner_subword_aligns(
-    src: List[str],
-    tgt: List[str],
+    src: list[str],
+    tgt: list[str],
     align_layer: int,
     score_threshold: float,
 ) -> torch.Tensor:
     aligner = get_aligner_model()
     tokenizer = get_aligner_tokenizer()
     tokenized_src = [tokenizer.tokenize(word) for word in src]
     tokenized_tgt = [tokenizer.tokenize(word) for word in tgt]
@@ -87,16 +87,16 @@
         softmax_tgtsrc = torch.nn.Softmax(dim=-2)(dot_prod)
         softmax_inter = (softmax_srctgt > score_threshold) * (softmax_tgtsrc > score_threshold)
     align_subwords = torch.nonzero(softmax_inter, as_tuple=False)
     return align_subwords, sub2word_map_src, sub2word_map_tgt
 
 
 def compute_word_aligns(
-    src: Union[str, List[str]],
-    tgt: Union[str, List[str]],
+    src: Union[str, list[str]],
+    tgt: Union[str, list[str]],
     split_pattern: str = r"\s+|\b",
     align_layer: int = 8,
     score_threshold: float = 1e-3,
 ) -> AlignedSequences:
     if isinstance(src, str):
         src = [word for word in re.split(split_pattern, src) if word]
     if isinstance(tgt, str):
@@ -112,16 +112,16 @@
         source_tokens=src.copy(),
         target_tokens=tgt.copy(),
         alignments=word_alignments.copy(),
     )
 
 
 def align_tokenizations(
-    tok_a: List[str],
-    tok_b: List[str],
+    tok_a: list[str],
+    tok_b: list[str],
 ) -> AlignedSequences:
     """Align tokens from a sentence tokenized by different tokenizers.
 
     Args:
         tok_a (:obj:`str` or :obj:`list` of :obj:`str`):
             Sequence of tokens produced by the first tokenizer.
         tok_b (:obj:`str` or :obj:`list` of :obj:`str`):
@@ -189,33 +189,33 @@
         source_tokens=aligns_a_b.source_tokens.copy(),
         target_tokens=aligns_b_c.target_tokens.copy(),
         alignments=aligns_a_c.copy(),
     )
 
 
 def add_alignment_extra_positions(
-    alignments: List[Tuple[int, int]], extra_positions: List[Tuple[int, int]]
-) -> List[Tuple[int, int]]:
+    alignments: list[tuple[int, int]], extra_positions: list[tuple[int, int]]
+) -> list[tuple[int, int]]:
     for x_idx_a, x_idx_b in extra_positions:
         for pos, (idx_a, idx_b) in enumerate(alignments):
             a_val, b_val = idx_a, idx_b
             if idx_a >= x_idx_a:
                 a_val += 1
             if idx_b >= x_idx_b:
                 b_val += 1
             alignments[pos] = (a_val, b_val)
     return alignments + extra_positions
 
 
 def auto_align_sequences(
     a_sequence: Optional[str] = None,
-    a_tokens: Optional[List[str]] = None,
+    a_tokens: Optional[list[str]] = None,
     b_sequence: Optional[str] = None,
-    b_tokens: Optional[List[str]] = None,
-    filter_special_tokens: List[str] = [],
+    b_tokens: Optional[list[str]] = None,
+    filter_special_tokens: list[str] = [],
     split_pattern: str = r"\s+|\b",
 ) -> AlignedSequences:
     if not a_sequence or not b_sequence or not a_tokens or not b_tokens:
         raise ValueError(
             "Missing required arguments to compute alignments. Please provide target and contrast sequence and tokens."
         )
     try:
@@ -227,15 +227,15 @@
         b_words = [word for word in re.split(split_pattern, b_sequence) if word]
         a_to_b_word_align = compute_word_aligns(a_words, b_words)
         # 2. Align word-level alignments to token-level alignments from the generative model tokenizer.
         # Requires cleaning up the model tokens from special tokens (special characters already removed)
         clean_a_tokens, removed_a_token_idxs = clean_tokens(a_tokens, filter_special_tokens)
         clean_b_tokens, removed_b_token_idxs = clean_tokens(b_tokens, filter_special_tokens)
         if len(removed_a_token_idxs) != len(removed_b_token_idxs):
-            logger.warning(
+            logger.debug(
                 "The number of special tokens in the target and contrast sequences do not match. "
                 "Trying to match special tokens based on their identity."
             )
             removed_a_tokens = [a_tokens[idx] for idx in removed_a_token_idxs]
             removed_b_tokens = [b_tokens[idx] for idx in removed_b_token_idxs]
             aligned_special_tokens = []
             for curr_idx, rm_a in enumerate(removed_a_tokens):
@@ -262,32 +262,32 @@
         )
         return AlignedSequences(
             source_tokens=a_tokens,
             target_tokens=b_tokens,
             alignments=a_to_b_aligns_with_special_tokens,
         )
     except Exception as e:
-        logger.warning(
+        logger.error(
             "Failed to compute alignments using the aligner. "
             f"Please check the following error and provide custom alignments if needed.\n{e}"
         )
         raise e
 
 
 def get_adjusted_alignments(
-    alignments: Union[List[Tuple[int, int]], str],
+    alignments: Union[list[tuple[int, int]], str],
     target_sequence: Optional[str] = None,
-    target_tokens: Optional[List[str]] = None,
+    target_tokens: Optional[list[str]] = None,
     contrast_sequence: Optional[str] = None,
-    contrast_tokens: Optional[List[str]] = None,
+    contrast_tokens: Optional[list[str]] = None,
     fill_missing: bool = False,
-    special_tokens: List[str] = [],
+    special_tokens: list[str] = [],
     start_pos: int = 0,
     end_pos: Optional[int] = None,
-) -> List[Tuple[int, int]]:
+) -> list[tuple[int, int]]:
     is_auto_aligned = False
     if fill_missing and not target_tokens:
         raise ValueError("Missing target tokens. Please provide target tokens to fill missing alignments.")
     if alignments is None:
         alignments = []
     if end_pos is None:
         end_pos = len(target_tokens)
@@ -298,69 +298,70 @@
                 a_tokens=target_tokens,
                 b_sequence=contrast_sequence,
                 b_tokens=contrast_tokens,
                 filter_special_tokens=special_tokens,
             ).alignments
             alignments = [(a_idx, b_idx) for a_idx, b_idx in alignments if start_pos <= a_idx < end_pos]
             is_auto_aligned = True
-            logger.warning(
+            logger.debug(
                 f"Using {ALIGN_MODEL_ID} for automatic alignments. Provide custom alignments for non-linguistic "
                 f"sequences, or for languages not covered by the aligner."
             )
         else:
             raise ValueError(
                 f"Unknown alignment method: {alignments}. "
                 f"Available methods: {','.join([m.value for m in AlignmentMethod])}"
             )
     # Sort alignments
     alignments = sorted(set(alignments), key=lambda x: (x[0], x[1]))
 
     # Filter alignments (restrict to one per token)
     filter_aligns = []
-    for pair_idx in range(start_pos, end_pos):
-        match_pairs = [(p0, p1) for p0, p1 in alignments if p0 == pair_idx and 0 <= p1 < len(contrast_tokens)]
-        if match_pairs:
-            # If found, use the first match that containing an unaligned target token, first match otherwise
-            match_pairs_unaligned = [p for p in match_pairs if p[1] not in [f[1] for f in filter_aligns]]
-            valid_match = match_pairs_unaligned[0] if match_pairs_unaligned else match_pairs[0]
-            filter_aligns.append(valid_match)
+    if len(alignments) > 0:
+        for pair_idx in range(start_pos, end_pos):
+            match_pairs = [(p0, p1) for p0, p1 in alignments if p0 == pair_idx and 0 <= p1 < len(contrast_tokens)]
+            if match_pairs:
+                # If found, use the first match that containing an unaligned target token, first match otherwise
+                match_pairs_unaligned = [p for p in match_pairs if p[1] not in [f[1] for f in filter_aligns]]
+                valid_match = match_pairs_unaligned[0] if match_pairs_unaligned else match_pairs[0]
+                filter_aligns.append(valid_match)
 
     # Filling alignments with missing tokens
     if fill_missing:
         filled_alignments = filter_aligns.copy()
         for step_idx, pair_idx in enumerate(reversed(range(start_pos, end_pos)), start=1):
             match_pairs = [(p0, p1) for p0, p1 in filter_aligns if p0 == pair_idx and 0 <= p1 < len(contrast_tokens)]
 
             # Default behavior: fill missing alignments with 1:1 position alignments starting from the bottom of the
             # two sequences
             if not match_pairs:
-                if (len(contrast_tokens) - step_idx) < start_pos:
-                    filled_alignments.append((pair_idx, len(contrast_tokens) - 1))
-                else:
+                if (len(contrast_tokens) - step_idx) > 0:
                     filled_alignments.append((pair_idx, len(contrast_tokens) - step_idx))
+                else:
+                    filled_alignments.append((pair_idx, len(contrast_tokens) - 1))
 
         if filter_aligns != filled_alignments:
             existing_aligns_message = (
                 f"Provided target alignments do not cover all {end_pos - start_pos} tokens from the original sequence."
             )
             no_aligns_message = (
                 "No target alignments were provided for the contrastive target. "
                 "Use e.g. 'contrast_targets_alignments=[(0,1), ...] to provide them in model.attribute"
             )
-            logger.warning(
+            logger.debug(
                 f"{existing_aligns_message if filter_aligns else no_aligns_message}\n"
                 "Filling missing position with right-aligned 1:1 position alignments."
             )
             filter_aligns = sorted(set(filled_alignments), key=lambda x: (x[0], x[1]))
     if is_auto_aligned or (fill_missing and filter_aligns != filled_alignments):
-        logger.warning(f"Generated alignments: {filter_aligns}")
+        logger.debug(f"Generated alignments: {filter_aligns}")
     return filter_aligns
 
 
-def get_aligned_idx(a_idx: int, alignments: List[Tuple[int, int]]) -> int:
+def get_aligned_idx(a_idx: int, alignments: list[tuple[int, int]]) -> int:
     if alignments:
         # Find all alignment pairs for the current original target
         aligned_idxs = [t_idx for s_idx, t_idx in alignments if s_idx == a_idx]
         if not aligned_idxs:
             # To be handled separately
             return -1
         # Select the minimum index to identify the next target token
```

### Comparing `inseq-0.5.0/inseq/utils/cache.py` & `inseq-0.6.0/inseq/utils/cache.py`

 * *Files identical despite different names*

### Comparing `inseq-0.5.0/inseq/utils/contrast_utils.py` & `inseq-0.6.0/inseq/utils/contrast_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import warnings
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Callable, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import torch
 
 from ..data import (
     DecoderOnlyBatch,
     EncoderDecoderBatch,
     FeatureAttributionInput,
@@ -57,15 +57,15 @@
     target_ids: Optional[TargetIdsTensor] = None
 
 
 def _get_contrast_inputs(
     args: "StepFunctionArgs",
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     return_contrastive_target_ids: bool = False,
     return_contrastive_batch: bool = False,
     **forward_kwargs,
 ) -> ContrastInputs:
     """Utility function to return the output of the model for given contrastive inputs.
 
     Args:
@@ -78,15 +78,15 @@
     if contrast_targets:
         c_batch = DecoderOnlyBatch.from_batch(
             get_batch_from_inputs(
                 attribution_model=args.attribution_model,
                 inputs=contrast_targets,
                 as_targets=is_enc_dec,
             )
-        )
+        ).to(args.decoder_input_ids.device)
         curr_prefix_len = args.decoder_input_ids.size(1)
         c_batch, c_tgt_ids = slice_batch_from_position(c_batch, curr_prefix_len, contrast_targets_alignments)
 
         if args.decoder_input_ids.size(0) != c_batch.target_ids.size(0):
             raise ValueError(
                 f"Contrastive batch size ({c_batch.target_ids.size(0)}) must match candidate batch size"
                 f" ({args.decoder_input_ids.size(0)}). Multi-sentence attribution and methods expanding inputs to"
@@ -103,15 +103,15 @@
         from ..attr.step_functions import StepFunctionEncoderDecoderArgs
 
         if not (is_enc_dec and isinstance(args, StepFunctionEncoderDecoderArgs)):
             raise ValueError(
                 "Contrastive source inputs can only be used with encoder-decoder models. "
                 "Use `contrast_targets` to set a contrastive target containing a prefix for decoder-only models."
             )
-        c_enc_in = args.attribution_model.encode(contrast_sources)
+        c_enc_in = args.attribution_model.encode(contrast_sources).to(args.encoder_input_ids.device)
         if (
             args.encoder_input_ids.shape != c_enc_in.input_ids.shape
             or torch.ne(args.encoder_input_ids, c_enc_in.input_ids).any()
         ):
             args.encoder_input_ids = c_enc_in.input_ids
             args.encoder_input_embeds = args.attribution_model.embed(args.encoder_input_ids, as_targets=False)
             args.encoder_attention_mask = c_enc_in.attention_mask
@@ -122,15 +122,15 @@
     )
 
 
 def _setup_contrast_args(
     args: "StepFunctionArgs",
     contrast_sources: Optional[FeatureAttributionInput] = None,
     contrast_targets: Optional[FeatureAttributionInput] = None,
-    contrast_targets_alignments: Optional[List[List[Tuple[int, int]]]] = None,
+    contrast_targets_alignments: Optional[list[list[tuple[int, int]]]] = None,
     contrast_force_inputs: bool = False,
 ):
     c_inputs = _get_contrast_inputs(
         args,
         contrast_sources=contrast_sources,
         contrast_targets=contrast_targets,
         contrast_targets_alignments=contrast_targets_alignments,
```

### Comparing `inseq-0.5.0/inseq/utils/errors.py` & `inseq-0.6.0/inseq/utils/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Tuple
+from typing import Any
 
 from .registry import available_classes
 
 
 class InseqDeprecationWarning(UserWarning):
     """Special deprecation warning because the built-in one is ignored by default."""
 
@@ -17,15 +17,15 @@
         "Unknown attribution method: {attribution_method}.\nAvailable methods: {available_methods}"
     )
 
     def __init__(
         self,
         method_name: str,
         msg: str = UNKNOWN_ATTRIBUTION_METHOD_MSG,
-        *args: Tuple[Any],
+        *args: tuple[Any],
     ) -> None:
         from inseq.attr import FeatureAttribution
 
         msg = msg.format(
             attribution_method=method_name,
             available_methods=", ".join(available_classes(FeatureAttribution)),
         )
@@ -37,15 +37,15 @@
 
     MISSING_ATTRIBUTION_METHOD_MSG = (
         "Attribution methods is not set. "
         "You can either define it permanently when instancing the AttributionModel, "
         "or pass it to the attribute method.\nAvailable methods: {available_methods}"
     )
 
-    def __init__(self, msg: str = MISSING_ATTRIBUTION_METHOD_MSG, *args: Tuple[Any]) -> None:
+    def __init__(self, msg: str = MISSING_ATTRIBUTION_METHOD_MSG, *args: tuple[Any]) -> None:
         from inseq.attr import FeatureAttribution
 
         msg = msg.format(available_methods=", ".join(available_classes(FeatureAttribution)))
         super().__init__(msg, *args)
 
 
 class LengthMismatchError(Exception):
```

### Comparing `inseq-0.5.0/inseq/utils/id_utils.py` & `inseq-0.6.0/inseq/utils/id_utils.py`

 * *Files identical despite different names*

### Comparing `inseq-0.5.0/inseq/utils/import_utils.py` & `inseq-0.6.0/inseq/utils/import_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 _ipywidgets_available = find_spec("ipywidgets") is not None
 _scikitlearn_available = find_spec("sklearn") is not None
 _transformers_available = find_spec("transformers") is not None
 _sentencepiece_available = find_spec("sentencepiece") is not None and find_spec("protobuf") is not None
 _datasets_available = find_spec("datasets") is not None
 _captum_available = find_spec("captum") is not None
 _joblib_available = find_spec("joblib") is not None
+_nltk_available = find_spec("nltk") is not None
 
 
 def is_ipywidgets_available():
     return _ipywidgets_available
 
 
 def is_scikitlearn_available():
@@ -31,7 +32,11 @@
 
 def is_captum_available():
     return _captum_available
 
 
 def is_joblib_available():
     return _joblib_available
+
+
+def is_nltk_available():
+    return _nltk_available
```

### Comparing `inseq-0.5.0/inseq/utils/misc.py` & `inseq-0.6.0/inseq/utils/misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import functools
 import gzip
 import io
 import logging
 import math
 from base64 import standard_b64decode, standard_b64encode
 from collections import OrderedDict
+from collections.abc import Sequence
 from contextlib import contextmanager
 from functools import wraps
 from importlib import import_module
 from inspect import signature
-from itertools import dropwhile
 from numbers import Number
 from os import PathLike, fsync
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Optional, Union
 
 from numpy import asarray, frombuffer
 from torch import Tensor
 
 from .errors import LengthMismatchError
 from .typing import TextInput, TokenWithId
 
@@ -67,54 +67,58 @@
         out_txt = f"list with {len(l)} sub-lists"
         if any(len(sl) > 20 for sl in l) or len(l) > 15:
             return out_txt
         if all(isinstance(ssl, list) for sl in l for ssl in sl):
             return out_txt
     if len(l) > 20:
         return out_txt
-    return f"{out_txt}:{_pretty_list(l, lpad)}"
+    return f"{out_txt}: {_pretty_list(l, lpad)}"
 
 
 def pretty_tensor(t: Optional[Tensor] = None, lpad: int = 8) -> str:
     if t is None:
         return "None"
     if t.ndim > 2 or any(x > 20 for x in t.shape):
         return f"{t.dtype} tensor of shape {list(t.shape)} on {t.device}"
     else:
         out_list = t.tolist()
         out_list = _pretty_list(out_list, lpad) if isinstance(out_list, list) else out_list
         return f"{t.dtype} tensor of shape {list(t.shape)} on {t.device}: {out_list}"
 
 
-def pretty_dict(d: Dict[str, Any], lpad: int = 4) -> str:
+def pretty_dict(d: dict[str, Any], lpad: int = 4) -> str:
     if not d:
         return "{}"
     out_txt = "{\n"
     for k, v in d.items():
         out_txt += f"{' ' * lpad}{k}: "
         if isinstance(v, (list, tuple)):
             out_txt += pretty_list(v, lpad + 4)
         elif isinstance(v, Tensor):
             out_txt += pretty_tensor(v, lpad + 4)
         elif isinstance(v, dict):
             out_txt += pretty_dict(v, lpad + 4)
         elif hasattr(v, "to_dict") and not isinstance(v, type):
             out_txt += f"{v.__class__.__name__}({pretty_dict(v.to_dict(), lpad + 4)})"
+        elif v is None:
+            out_txt += "None"
+        elif isinstance(v, str):
+            out_txt += f'"{v}"'
         else:
-            out_txt += "None" if v is None else str(v)
+            out_txt += str(v)
         out_txt += ",\n"
     return out_txt + f"{' ' * (lpad - 4)}}}"
 
 
 def extract_signature_args(
-    full_args: Dict[str, Any],
+    full_args: dict[str, Any],
     func: Callable[[Any], Any],
     exclude_args: Optional[Sequence[str]] = None,
     return_remaining: bool = False,
-) -> Union[Dict[str, Any], Tuple[Dict[str, Any], Dict[str, Any]]]:
+) -> Union[dict[str, Any], tuple[dict[str, Any], dict[str, Any]]]:
     extracted_args = {
         k: v
         for k, v in full_args.items()
         if k in signature(func).parameters and (exclude_args is None or k not in exclude_args)
     }
     if return_remaining:
         return extracted_args, {k: v for k, v in full_args.items() if k not in extracted_args}
@@ -162,18 +166,18 @@
 def pad(seq: Sequence[Sequence[Any]], pad_id: Any):
     """Pads a list of sequences to the same length."""
     max_len = max(len(x) for x in seq)
     seq = [x + [pad_id] * (max_len - len(x)) for x in seq]
     return seq
 
 
-def drop_padding(seq: Sequence[Any], pad_id: Any):
+def drop_padding(seq: Sequence[TokenWithId], pad_id: str):
     if pad_id is None:
         return seq
-    return list(reversed(list(dropwhile(lambda x: x == pad_id, reversed(seq)))))
+    return [x for x in seq if x.token != pad_id]
 
 
 def isnotebook():
     """Returns true if code is being executed in a notebook, false otherwise.
 
     Currently supported: Jupyter Notebooks, Google Colab
     To validate: Kaggle Notebooks, JupyterLab
@@ -194,15 +198,15 @@
     except ModuleNotFoundError:
         return False  # IPython not installed
 
 
 def format_input_texts(
     texts: TextInput,
     ref_texts: Optional[TextInput] = None,
-) -> Tuple[List[str], List[str]]:
+) -> tuple[list[str], list[str]]:
     texts = [texts] if isinstance(texts, str) else texts
     reference_texts = [ref_texts] if isinstance(ref_texts, str) else ref_texts
     if reference_texts and texts and len(texts) != len(reference_texts):
         raise LengthMismatchError(
             "Length mismatch for texts and reference_texts.Input length: {}, reference length: {} ".format(
                 len(texts), len(reference_texts)
             )
@@ -227,15 +231,15 @@
             curr_idx = end_idx
         else:
             out_sequence.append(token)
             curr_idx += 1
     return out_sequence
 
 
-def aggregate_token_pair(tokens: List[TokenWithId], other_tokens: List[TokenWithId]):
+def aggregate_token_pair(tokens: list[TokenWithId], other_tokens: list[TokenWithId]):
     if not other_tokens:
         return tokens
     out_tokens = []
     for tok, other in zip(tokens, other_tokens):
         if tok.token == other.token:
             out_tokens.append(TokenWithId(tok.token, tok.id))
         else:
@@ -416,17 +420,22 @@
         if imp_err:
             curr_class = cls_lookup_map.get(name, None)
             if curr_class is None:
                 raise ImportError(f"{imp_err}; add the class to `cls_lookup_map={{'{name}': Class}}` argument")
     return curr_class
 
 
-def clean_tokens(tokens: List[str], remove_tokens: List[str]) -> Tuple[List[str], List[int]]:
+def clean_tokens(tokens: list[str], remove_tokens: list[str]) -> tuple[list[str], list[int]]:
     """Removes tokens from a list of tokens and returns the cleaned list and the removed token indexes."""
     clean_tokens = []
     removed_token_idxs = []
     for idx, tok in enumerate(tokens):
         if tok not in remove_tokens:
             clean_tokens += [tok.strip()]
         else:
             removed_token_idxs += [idx]
     return clean_tokens, removed_token_idxs
+
+
+def get_left_padding(text: str):
+    """Returns the number of spaces at the beginning of a string."""
+    return len(text) - len(text.lstrip())
```

### Comparing `inseq-0.5.0/inseq/utils/registry.py` & `inseq-0.6.0/inseq/utils/registry.py`

 * *Files identical despite different names*

### Comparing `inseq-0.5.0/inseq/utils/serialization.py` & `inseq-0.6.0/inseq/utils/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE
 # USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import json
 from collections import OrderedDict
 from json import JSONEncoder
 from os import PathLike
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Union
+from typing import Any, Callable, Optional, TypeVar, Union
 
 from numpy import generic, ndarray
 
 from ..utils import (
     bin_str_to_ndarray,
     get_cls_from_instance_type,
     get_module_name_from_object,
@@ -92,15 +92,15 @@
 
 def ndarray_encode(
     obj: EncodableObject,
     use_primitives: bool = True,
     ndarray_compact: Optional[bool] = None,
     compression: bool = False,
     **kwargs,
-) -> Dict[str, Any]:
+) -> dict[str, Any]:
     """Encodes numpy ``ndarray`` as lists with meta data.
     Encodes numpy scalar types as Python equivalents. Special encoding is not possible,
     because float64 is a subclass of primitives, which never reach the encoder.
     """
     if isinstance(obj, ndarray):
         if use_primitives:
             return obj.tolist()
@@ -131,15 +131,15 @@
 
 ENCODE_HOOKS = [class_instance_encode, ndarray_encode]
 
 
 class AttributionSerializer(JSONEncoder):
     def __init__(
         self,
-        encoders: Optional[List[Callable]] = None,
+        encoders: Optional[list[Callable]] = None,
         use_primitives: bool = True,
         ndarray_compact: Optional[bool] = None,
         compression: bool = False,
         **json_kwargs,
     ):
         self.encoders = []
         if encoders:
@@ -170,15 +170,15 @@
             )
         return obj
 
 
 def json_advanced_dumps(
     obj: EncodableObject,
     sort_keys: bool = True,
-    encoders: List[Callable] = ENCODE_HOOKS,
+    encoders: list[Callable] = ENCODE_HOOKS,
     use_primitives: bool = True,
     allow_nan: bool = True,
     ndarray_compact: Optional[bool] = None,
     compression: bool = False,
     **jsonkwargs,
 ) -> str:
     """Dumps a complex object containing classes and arrays object to a string.
@@ -217,15 +217,15 @@
     return combined_encoder.encode(obj)
 
 
 @save_to_file
 def json_advanced_dump(
     obj: EncodableObject,
     sort_keys: bool = True,
-    encoders: List[Callable] = ENCODE_HOOKS,
+    encoders: list[Callable] = ENCODE_HOOKS,
     use_primitives: bool = False,
     allow_nan: bool = True,
     ndarray_compact: Optional[bool] = None,
     compression: bool = False,
     **jsonkwargs,
 ) -> str:
     """Dumps a complex object containing classes and arrays object to a file.
@@ -297,15 +297,15 @@
             return bin_str_to_ndarray(data_json, order, shape, nptype)
         else:
             return lists_of_numbers_to_ndarray(data_json, order, shape, nptype)
     else:
         return scalar_to_numpy(data_json, nptype)
 
 
-def class_instance_hook(dct: Any, cls_lookup_map: Optional[Dict[str, type]] = None, **kwargs) -> DecodableObject:
+def class_instance_hook(dct: Any, cls_lookup_map: Optional[dict[str, type]] = None, **kwargs) -> DecodableObject:
     """This hook tries to convert json encoded by class_instance_encoder back to it's original instance.
     It only works if the environment is the same, e.g. the class is similarly importable and hasn't changed.
 
     Args:
         dct:
             The object to be decoded. Will be processed by the hook if it is a dictionary containing the attribute
             ``__instance_type__`` provided by ``class_instance_encode``.
@@ -339,16 +339,16 @@
     """Hook that converts json maps to the appropriate python type (dict or OrderedDict)
     and then runs any number of hooks on the individual maps.
     """
 
     def __init__(
         self,
         ordered: bool = False,
-        hooks: Optional[List[Callable]] = None,
-        cls_lookup_map: Optional[Dict[str, type]] = None,
+        hooks: Optional[list[Callable]] = None,
+        cls_lookup_map: Optional[dict[str, type]] = None,
     ):
         self.map_type = OrderedDict if ordered else dict
         self.hooks = hooks if hooks else []
         self.cls_lookup_map = cls_lookup_map
 
     def __call__(self, pairs):
         """Applies all hooks to the map."""
@@ -361,16 +361,16 @@
 DECODE_HOOKS = [class_instance_hook, ndarray_hook]
 
 
 def json_advanced_loads(
     string: str,
     ordered: bool = False,
     decompression: bool = False,
-    hooks: List[Callable] = DECODE_HOOKS,
-    cls_lookup_map: Optional[Dict[str, type]] = None,
+    hooks: list[Callable] = DECODE_HOOKS,
+    cls_lookup_map: Optional[dict[str, type]] = None,
     **jsonkwargs,
 ) -> Any:
     """Load a complex object containing classes and arrays object from a string.
 
     Args:
         string (:obj:`str`):
             String to be loaded into an object.
@@ -401,16 +401,16 @@
     return json.loads(string, object_pairs_hook=hook, **jsonkwargs)
 
 
 def json_advanced_load(
     fp: Union[str, bytes, PathLike],
     ordered: bool = True,
     decompression: bool = False,
-    hooks: List[Callable] = DECODE_HOOKS,
-    cls_lookup_map: Optional[Dict[str, type]] = None,
+    hooks: list[Callable] = DECODE_HOOKS,
+    cls_lookup_map: Optional[dict[str, type]] = None,
     **jsonkwargs,
 ) -> Any:
     """Load a complex object containing classes and arrays from a JSON file.
 
     Args:
         fp (:obj:`str`, :obj:`bytes`, or :obj:`os.PathLike`):
             Path to the file to load.
```

### Comparing `inseq-0.5.0/inseq/utils/typing.py` & `inseq-0.6.0/inseq/utils/typing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import torch
+from captum.attr._utils.attribution import Attribution
 from jaxtyping import Float, Float32, Int64
 from transformers import PreTrainedModel
 
 TextInput = Union[str, Sequence[str]]
 
+if TYPE_CHECKING:
+    from inseq.models import AttributionModel
+
 
 @dataclass
 class TokenWithId:
     token: str
     id: int
 
     def __str__(self):
@@ -23,26 +28,56 @@
             return self.id == other
         elif isinstance(other, TokenWithId):
             return self.token == other.token and self.id == other.id
         else:
             return False
 
 
+class InseqAttribution(Attribution):
+    """A wrapper class for the Captum library's Attribution class to type hint the ``forward_func`` attribute
+    as an :class:`~inseq.models.AttributionModel`.
+    """
+
+    def __init__(self, forward_func: "AttributionModel") -> None:
+        r"""
+        Args:
+            forward_func (:class:`~inseq.models.AttributionModel`): The model hooker to the attribution method.
+        """
+        self.forward_func = forward_func
+
+    attribute: Callable
+
+    @property
+    def multiplies_by_inputs(self):
+        return False
+
+    def has_convergence_delta(self) -> bool:
+        return False
+
+    compute_convergence_delta: Callable
+
+    @classmethod
+    def get_name(cls: type["InseqAttribution"]) -> str:
+        return "".join([char if char.islower() or idx == 0 else " " + char for idx, char in enumerate(cls.__name__)])
+
+
 @dataclass
 class TextSequences:
     targets: TextInput
     sources: Optional[TextInput] = None
 
 
 OneOrMoreIdSequences = Sequence[Sequence[int]]
 OneOrMoreTokenSequences = Sequence[Sequence[str]]
 OneOrMoreTokenWithIdSequences = Sequence[Sequence[TokenWithId]]
 OneOrMoreAttributionSequences = Sequence[Sequence[float]]
 
-IndexSpan = Union[Tuple[int, int], Sequence[Tuple[int, int]]]
+IndexSpan = Union[tuple[int, int], Sequence[tuple[int, int]]]
+OneOrMoreIndices = Union[int, list[int], tuple[int, int]]
+OneOrMoreIndicesDict = dict[int, OneOrMoreIndices]
 
 IdsTensor = Int64[torch.Tensor, "batch_size seq_len"]
 TargetIdsTensor = Int64[torch.Tensor, "batch_size"]
 ExpandedTargetIdsTensor = Int64[torch.Tensor, "batch_size 1"]
 EmbeddingsTensor = Float[torch.Tensor, "batch_size seq_len embed_size"]
 MultiStepEmbeddingsTensor = Float[Float, "batch_size_x_n_steps seq_len embed_size"]
 VocabularyEmbeddingsTensor = Float[torch.Tensor, "vocab_size embed_size"]
@@ -88,11 +123,11 @@
 # For Fairseq it's a tuple of strings containing repo and model name
 # e.g. ("pytorch/fairseq", "transformer.wmt14.en-fr")
 ModelIdentifier = str  # Union[str, Tuple[str, str]]
 ModelClass = PreTrainedModel
 
 AttributionForwardInputs = Union[IdsTensor, EmbeddingsTensor]
 AttributionForwardInputsPair = Union[
-    Tuple[IdsTensor, IdsTensor],
-    Tuple[EmbeddingsTensor, EmbeddingsTensor],
+    tuple[IdsTensor, IdsTensor],
+    tuple[EmbeddingsTensor, EmbeddingsTensor],
 ]
 OneOrTwoAttributionForwardInputs = Union[AttributionForwardInputs, AttributionForwardInputsPair]
```

### Comparing `inseq-0.5.0/inseq/utils/viz_utils.py` & `inseq-0.6.0/inseq/utils/viz_utils.py`

 * *Files identical despite different names*

