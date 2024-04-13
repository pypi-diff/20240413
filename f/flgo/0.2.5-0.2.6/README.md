# Comparing `tmp/flgo-0.2.5.tar.gz` & `tmp/flgo-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flgo-0.2.5.tar", last modified: Mon Apr  1 08:37:05 2024, max compression
+gzip compressed data, was "flgo-0.2.6.tar", last modified: Sat Apr 13 06:26:45 2024, max compression
```

## Comparing `flgo-0.2.5.tar` & `flgo-0.2.6.tar`

### file list

```diff
@@ -1,546 +1,547 @@
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1091 2023-03-21 13:46:37.000000 flgo-0.2.5/LICENSE
--rw-r--r--   0 wz        (1001) wz        (1001)      716 2024-04-01 08:37:05.654097 flgo-0.2.5/PKG-INFO
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-21 13:46:37.000000 flgo-0.2.5/README.md
--rw-rw-r--   0 wz        (1001) wz        (1001)      764 2024-04-01 08:36:58.000000 flgo-0.2.5/pyproject.toml
--rw-rw-r--   0 wz        (1001) wz        (1001)       38 2024-04-01 08:37:05.654097 flgo-0.2.5/setup.cfg
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.618097 flgo-0.2.5/src/
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.626097 flgo-0.2.5/src/flgo/
--rw-rw-r--   0 wz        (1001) wz        (1001)      915 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/algorithm/
--rw-rw-r--   0 wz        (1001) wz        (1001)     3753 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/TiFL.py
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3358 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/afl.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6959 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/clustered_sampling.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11333 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/decentralized.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2056 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/ditto.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2391 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedasync.py
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedavg.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      711 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedavgm.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    40012 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedbase.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2776 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedbuff.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2856 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/feddyn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2258 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedfa.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3381 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedfv.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7205 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedmf.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2920 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fedmgda.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2110 2024-04-01 08:35:42.000000 flgo-0.2.5/src/flgo/algorithm/fednova.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1444 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/fedprox.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8853 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/hierarchical.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1800 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/mifa.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1501 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/powerofchoice.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/qfedavg.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    32417 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/realbase.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3421 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/scaffold.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9202 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/sesorec.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3013 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/standalone.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    17504 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/algorithm/vflbase.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2390 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/adult_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      239 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/adult_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      700 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/adult_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/adult_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/adult_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      466 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/adult_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/agnews_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/agnews_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2003 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/agnews_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3955 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/agnews_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/agnews_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/agnews_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/bankmarketing_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/bankmarketing_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      725 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/bankmarketing_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/bankmarketing_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/bankmarketing_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      430 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/bankmarketing_classification/model/lr.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    24978 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/base.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/ciao_recommendation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/ciao_recommendation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      821 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/ciao_recommendation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/ciao_recommendation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      848 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/ciao_recommendation/model/mf.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1734 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1288 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      510 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.630097 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      991 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5388 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/model/resnet18.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2262 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar100_classification/model/resnet18_gn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1888 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1223 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      520 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      824 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1502 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/cnn_data_aug.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      741 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/mlp.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2261 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/resnet18_gn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1733 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/citeseer_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/citeseer_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      771 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/citeseer_node_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      807 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/citeseer_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/citeseer_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/citeseer_node_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/coco_detection/
--rw-rw-r--   0 wz        (1001) wz        (1001)      265 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/coco_detection/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6847 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/coco_detection/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/coco_detection/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     9240 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/coco_detection/model/FasterRCNN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/coco_detection/model/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/coco_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/coco_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8013 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/coco_segmentation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/coco_segmentation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/coco_segmentation/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      521 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/coco_segmentation/model/unet.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1717 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      853 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/model/GCN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      805 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      807 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      727 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/model/GCN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      730 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4070 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/model/GraphSage.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/cora_node_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/crop_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      241 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/crop_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      842 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/crop_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/crop_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1243 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/crop_classification/model/cnn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/distributed_quadratic_programming/
--rw-rw-r--   0 wz        (1001) wz        (1001)       93 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/distributed_quadratic_programming/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2298 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/distributed_quadratic_programming/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/distributed_quadratic_programming/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      569 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/distributed_quadratic_programming/model/vec.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/electricdevices_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      252 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/electricdevices_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      864 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/electricdevices_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/electricdevices_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1243 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/electricdevices_classification/model/cnn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/electricity_forecasting/
--rw-rw-r--   0 wz        (1001) wz        (1001)      245 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/electricity_forecasting/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      697 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/electricity_forecasting/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/electricity_forecasting/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      916 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/electricity_forecasting/model/GRU.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/emnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      357 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/emnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1199 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/emnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/emnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      875 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/emnist_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      709 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/emnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/enzymes_graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/enzymes_graph_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1873 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/enzymes_graph_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/enzymes_graph_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.634097 flgo-0.2.5/src/flgo/benchmark/enzymes_graph_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/enzymes_graph_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      833 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      848 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      938 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/model/mf.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/exchange_rate_forecasting/
--rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/exchange_rate_forecasting/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2884 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/exchange_rate_forecasting/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/exchange_rate_forecasting/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      914 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/exchange_rate_forecasting/model/GRU.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/fashion_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/fashion_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/fashion_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      487 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/fashion_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/fashion_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      578 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/fashion_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/fcube_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       78 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/fcube_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1912 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/fcube_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/fcube_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/fcube_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      553 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/fcube_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/femnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      358 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/femnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/femnist_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5327 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/femnist_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/femnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/femnist_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      875 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/femnist_classification/model/cnn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/heart_disease_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/heart_disease_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      723 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/heart_disease_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/heart_disease_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/heart_disease_classification/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      465 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/heart_disease_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/imdb_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/imdb_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1993 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/imdb_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3907 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/imdb_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/imdb_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/imdb_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/leaf_reddit/
--rw-rw-r--   0 wz        (1001) wz        (1001)       87 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/leaf_reddit/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    10132 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/leaf_reddit/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/leaf_reddit/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      980 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/leaf_sent140/
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/leaf_sent140/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11379 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/leaf_sent140/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/leaf_sent140/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/local_movielens_recommendation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      211 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/local_movielens_recommendation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      839 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/local_movielens_recommendation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/local_movielens_recommendation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1748 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/local_movielens_recommendation/model/mf.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/mnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1850 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/mnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      463 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/mnist_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      660 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/mnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/mnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      899 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/mnist_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      703 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/mnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/movielens_recommendation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/movielens_recommendation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      835 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/movielens_recommendation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/movielens_recommendation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/movielens_recommendation/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      787 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/movielens_recommendation/model/mf.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/multi30k_translation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/multi30k_translation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6631 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/multi30k_translation/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6514 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/multi30k_translation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/multi30k_translation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/multi30k_translation/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/mutag_graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/mutag_graph_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1564 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/mutag_graph_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/mutag_graph_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.638097 flgo-0.2.5/src/flgo/benchmark/mutag_graph_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/mutag_graph_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/nifECG_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      243 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/nifECG_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      886 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/nifECG_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/nifECG_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1246 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/nifECG_classification/model/cnn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/oxfordiiitpet_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/oxfordiiitpet_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1006 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/oxfordiiitpet_segmentation/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      797 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/oxfordiiitpet_segmentation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/oxfordiiitpet_segmentation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/oxfordiiitpet_segmentation/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    34092 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/benchmark/partition.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/penntreebank_modeling/
--rw-rw-r--   0 wz        (1001) wz        (1001)      275 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/penntreebank_modeling/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3387 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/penntreebank_modeling/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/penntreebank_modeling/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/penntreebank_modeling/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/penntreebank_modeling/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1726 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/pubmed_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/pubmed_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      820 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/pubmed_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/pubmed_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      726 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/pubmed_node_classification/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)      277 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6604 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/model/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      521 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/model/unet.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/shakespeare_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      262 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/shakespeare_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    15413 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/shakespeare_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/shakespeare_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2169 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/social_splitted_ciao/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_ciao/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9479 2024-04-01 08:35:44.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_ciao/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/social_splitted_ciao/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_ciao/model/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/social_splitted_ciaodvd/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_ciaodvd/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9210 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_ciaodvd/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/social_splitted_douban/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_douban/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8344 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_douban/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/social_splitted_epinions/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_epinions/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9394 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_epinions/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/social_splitted_epinions/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_epinions/model/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/social_splitted_filmtrust/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_filmtrust/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9247 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/social_splitted_filmtrust/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/sst2_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/sst2_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1987 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/sst2_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3955 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/sst2_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/sst2_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/sst2_classification/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/stl10_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      500 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1302 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      517 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      857 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1536 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/cnn_data_aug.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2261 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/resnet18_gn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3391 2024-04-01 08:35:46.000000 flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/resnet34_gn.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.642097 flgo-0.2.5/src/flgo/benchmark/svhn_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      355 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/svhn_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/svhn_classification/core.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      444 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/svhn_classification/dataset.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/svhn_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      895 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/svhn_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      897 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/svhn_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/synthetic_regression/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1079 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/synthetic_regression/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3901 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/synthetic_regression/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/synthetic_regression/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      555 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/synthetic_regression/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1687 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)    21425 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/dec_temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      341 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/dec_temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/dec_temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1035 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/dec_temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/dec_temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/dec_temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/hier_temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      260 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/hier_temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/hier_temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      847 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/hier_temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/hier_temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/hier_temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/
--rw-rw-r--   0 wz        (1001) wz        (1001)     8935 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6637 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9179 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2636 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/presets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      794 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/temp/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    23912 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/transforms.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    16307 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)    21601 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/pointnet2_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/pointnet_utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      811 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)    25417 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet2_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet_utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      813 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)    24155 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet2_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet_utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      347 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4059 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.646097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/
--rw-rw-r--   0 wz        (1001) wz        (1001)    16044 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3939 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1314 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/presets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      797 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2797 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    10798 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     9023 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)    12697 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      524 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5455 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      682 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)    17008 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5558 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     7121 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      338 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3907 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      275 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2774 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6514 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/temp/model/default_model.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    25125 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/partition.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/rec/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/rec/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     8776 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/rec/datasets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/rec/rating_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)    11647 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      425 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/rec/utils.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/series/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     9882 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1600 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/datasets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4639 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.650097 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/
--rw-rw-r--   0 wz        (1001) wz        (1001)    13427 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4531 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/datasets.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/temp/
--rw-rw-r--   0 wz        (1001) wz        (1001)      185 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/temp/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/temp/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7994 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/temp/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/temp/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:49.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/temp/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/toolkits/tabular/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/tabular/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/toolkits/tabular/classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     9992 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/tabular/classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11416 2024-04-01 08:35:48.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/tabular/classification/datasets.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7488 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/toolkits/visualization.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/vertical_mnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      260 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/vertical_mnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7230 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/vertical_mnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/vertical_mnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1162 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/voc_detection/
--rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/voc_detection/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2159 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/voc_detection/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      794 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/voc_detection/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/voc_detection/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/voc_detection/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/wikitext2_modeling/
--rw-rw-r--   0 wz        (1001) wz        (1001)      273 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/wikitext2_modeling/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3375 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/wikitext2_modeling/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/benchmark/wikitext2_modeling/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/benchmark/wikitext2_modeling/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-01 08:35:47.000000 flgo-0.2.5/src/flgo/benchmark/wikitext2_modeling/model/default_model.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/experiment/
--rw-rw-r--   0 wz        (1001) wz        (1001)       62 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/experiment/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    27628 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/experiment/analyzer.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6651 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/experiment/device_scheduler.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/experiment/logger/
--rw-rw-r--   0 wz        (1001) wz        (1001)    90223 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    36834 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1857 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/dec_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2262 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/full_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      343 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/gval_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    59619 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/handlers.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      469 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/hier_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      323 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/parallel_hlogger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1522 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/pfl_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      415 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/pool.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1598 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/simple_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      386 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/test_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      951 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/tune_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1040 2024-04-01 08:35:45.000000 flgo-0.2.5/src/flgo/experiment/logger/vertical_logger.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/simulator/
--rw-rw-r--   0 wz        (1001) wz        (1001)     5181 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/simulator/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    25114 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/simulator/base.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    17046 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/simulator/default_simulator.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1030 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/simulator/my_simulator.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    17600 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/simulator/phone_simulator.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo/utils/
--rw-rw-r--   0 wz        (1001) wz        (1001)     3173 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/utils/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    73860 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/utils/fflow.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    28264 2024-04-01 08:35:43.000000 flgo-0.2.5/src/flgo/utils/fmodule.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/src/flgo.egg-info/
--rw-r--r--   0 wz        (1001) wz        (1001)      716 2024-04-01 08:37:05.000000 flgo-0.2.5/src/flgo.egg-info/PKG-INFO
--rw-rw-r--   0 wz        (1001) wz        (1001)    20282 2024-04-01 08:37:05.000000 flgo-0.2.5/src/flgo.egg-info/SOURCES.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)        1 2024-04-01 08:37:05.000000 flgo-0.2.5/src/flgo.egg-info/dependency_links.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)       81 2024-04-01 08:37:05.000000 flgo-0.2.5/src/flgo.egg-info/requires.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)        5 2024-04-01 08:37:05.000000 flgo-0.2.5/src/flgo.egg-info/top_level.txt
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-01 08:37:05.654097 flgo-0.2.5/tests/
--rw-rw-r--   0 wz        (1001) wz        (1001)      947 2023-03-21 13:46:37.000000 flgo-0.2.5/tests/test.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.620278 flgo-0.2.6/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1091 2023-03-21 13:46:37.000000 flgo-0.2.6/LICENSE
+-rw-r--r--   0 wz        (1001) wz        (1001)      716 2024-04-13 06:26:45.620278 flgo-0.2.6/PKG-INFO
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-21 13:46:37.000000 flgo-0.2.6/README.md
+-rw-rw-r--   0 wz        (1001) wz        (1001)      764 2024-04-13 06:26:37.000000 flgo-0.2.6/pyproject.toml
+-rw-rw-r--   0 wz        (1001) wz        (1001)       38 2024-04-13 06:26:45.620278 flgo-0.2.6/setup.cfg
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.580278 flgo-0.2.6/src/
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.592278 flgo-0.2.6/src/flgo/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      915 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.592278 flgo-0.2.6/src/flgo/algorithm/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3753 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/TiFL.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3358 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/afl.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3766 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/asyncbase.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6959 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/clustered_sampling.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11333 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/decentralized.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2056 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/ditto.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1264 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedasync.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedavg.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      711 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedavgm.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    40012 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedbase.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1702 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedbuff.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2856 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/feddyn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2258 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedfa.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3381 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedfv.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7205 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedmf.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2920 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedmgda.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2110 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fednova.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1444 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/fedprox.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8853 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/hierarchical.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1800 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/mifa.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1501 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/powerofchoice.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/qfedavg.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    32417 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/realbase.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3421 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/scaffold.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9202 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/sesorec.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3013 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/standalone.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17504 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/algorithm/vflbase.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.592278 flgo-0.2.6/src/flgo/benchmark/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2390 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/benchmark/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.592278 flgo-0.2.6/src/flgo/benchmark/adult_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      239 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/adult_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      700 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/adult_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.592278 flgo-0.2.6/src/flgo/benchmark/adult_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/adult_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      466 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/adult_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/agnews_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/agnews_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2003 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/agnews_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3955 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/agnews_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/agnews_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/agnews_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/bankmarketing_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/bankmarketing_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      725 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/bankmarketing_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/bankmarketing_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/bankmarketing_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      430 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/bankmarketing_classification/model/lr.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    24978 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/benchmark/base.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/ciao_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/ciao_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      821 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/ciao_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/ciao_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      848 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/ciao_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1734 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1288 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      510 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      991 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5388 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/model/resnet18.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2262 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar100_classification/model/resnet18_gn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1888 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1223 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      520 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      824 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1502 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/cnn_data_aug.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      741 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/mlp.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2261 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/resnet18_gn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1733 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/citeseer_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/citeseer_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      771 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/citeseer_node_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      807 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/citeseer_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/citeseer_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/citeseer_node_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/coco_detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      265 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/coco_detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6847 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/coco_detection/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/coco_detection/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9240 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/coco_detection/model/FasterRCNN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/coco_detection/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/coco_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/coco_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8013 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/coco_segmentation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/coco_segmentation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/coco_segmentation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      521 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/coco_segmentation/model/unet.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1717 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      853 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/model/GCN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      805 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      807 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.596278 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      727 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/model/GCN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      730 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4070 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/model/GraphSage.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/cora_node_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/crop_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      241 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/crop_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      842 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/crop_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/crop_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1243 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/crop_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/distributed_quadratic_programming/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       93 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/distributed_quadratic_programming/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2298 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/distributed_quadratic_programming/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/distributed_quadratic_programming/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      569 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/distributed_quadratic_programming/model/vec.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/electricdevices_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      252 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/electricdevices_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      864 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/electricdevices_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/electricdevices_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1243 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/electricdevices_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/electricity_forecasting/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      245 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/electricity_forecasting/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      697 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/electricity_forecasting/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/electricity_forecasting/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      916 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/electricity_forecasting/model/GRU.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/emnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      357 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/emnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1199 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/emnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/emnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      875 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/emnist_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      709 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/emnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/enzymes_graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/enzymes_graph_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1873 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/enzymes_graph_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/enzymes_graph_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/enzymes_graph_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/enzymes_graph_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      833 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      848 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      938 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/exchange_rate_forecasting/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/exchange_rate_forecasting/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2884 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/exchange_rate_forecasting/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/exchange_rate_forecasting/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      914 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/exchange_rate_forecasting/model/GRU.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/fashion_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/fashion_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/fashion_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      487 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/fashion_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/fashion_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      578 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/fashion_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/fcube_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       78 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/fcube_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1912 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/fcube_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/fcube_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/fcube_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      553 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/fcube_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/femnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      358 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/femnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/femnist_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5327 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/femnist_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/femnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/femnist_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      875 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/femnist_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/heart_disease_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      247 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/heart_disease_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      723 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/heart_disease_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/heart_disease_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/heart_disease_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      465 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/heart_disease_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/imdb_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/imdb_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1993 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/imdb_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3907 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/imdb_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/imdb_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/imdb_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/leaf_reddit/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       87 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/leaf_reddit/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10132 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/leaf_reddit/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/leaf_reddit/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      980 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.600278 flgo-0.2.6/src/flgo/benchmark/leaf_sent140/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/leaf_sent140/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11379 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/leaf_sent140/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/leaf_sent140/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/local_movielens_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      211 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/local_movielens_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      839 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/local_movielens_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/local_movielens_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1748 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/local_movielens_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/mnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1850 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/mnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      463 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/mnist_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      660 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/mnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/mnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      899 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/mnist_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      703 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/mnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/movielens_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/movielens_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      835 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/movielens_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/movielens_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/movielens_recommendation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      787 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/movielens_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/multi30k_translation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/multi30k_translation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6631 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/multi30k_translation/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6514 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/multi30k_translation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/multi30k_translation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/multi30k_translation/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/mutag_graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/mutag_graph_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1564 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/mutag_graph_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/mutag_graph_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/mutag_graph_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/mutag_graph_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/nifECG_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      243 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/nifECG_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      886 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/nifECG_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/nifECG_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1246 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/nifECG_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/oxfordiiitpet_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/oxfordiiitpet_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1006 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/oxfordiiitpet_segmentation/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      797 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/oxfordiiitpet_segmentation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/oxfordiiitpet_segmentation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/oxfordiiitpet_segmentation/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    34092 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/benchmark/partition.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/penntreebank_modeling/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      275 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/penntreebank_modeling/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3387 2024-04-13 06:25:53.000000 flgo-0.2.6/src/flgo/benchmark/penntreebank_modeling/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/penntreebank_modeling/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/penntreebank_modeling/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/penntreebank_modeling/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1726 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      803 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      576 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/pubmed_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/pubmed_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      820 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/pubmed_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/pubmed_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      726 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/pubmed_node_classification/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      277 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6604 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      521 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/model/unet.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/shakespeare_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      262 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/shakespeare_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    15413 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/shakespeare_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/shakespeare_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2169 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/social_splitted_ciao/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_ciao/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9479 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_ciao/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/social_splitted_ciao/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_ciao/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/social_splitted_ciaodvd/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_ciaodvd/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9210 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_ciaodvd/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/social_splitted_douban/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_douban/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8344 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_douban/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.604278 flgo-0.2.6/src/flgo/benchmark/social_splitted_epinions/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_epinions/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9394 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_epinions/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/social_splitted_epinions/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_epinions/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/social_splitted_filmtrust/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_filmtrust/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9247 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/social_splitted_filmtrust/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/sst2_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/sst2_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1987 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/sst2_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3955 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/sst2_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/sst2_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/sst2_classification/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/stl10_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      500 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1302 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      517 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      857 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1536 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/cnn_data_aug.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2261 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/resnet18_gn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3391 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/resnet34_gn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/svhn_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      355 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/svhn_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      631 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/svhn_classification/core.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      444 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/svhn_classification/dataset.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/svhn_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      895 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/svhn_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      897 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/svhn_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/synthetic_regression/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1079 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/synthetic_regression/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3901 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/synthetic_regression/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/synthetic_regression/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      555 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/synthetic_regression/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1687 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    21425 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/dec_temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      341 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/dec_temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/dec_temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1035 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/dec_temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/dec_temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/dec_temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/hier_temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      260 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/hier_temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/hier_temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      847 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/hier_temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/hier_temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/hier_temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      799 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8935 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6637 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9179 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2636 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/presets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      794 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/temp/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    23912 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/transforms.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    16307 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.608278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    21601 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/pointnet2_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/pointnet_utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      811 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    25417 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet2_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet_utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      813 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    24155 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11482 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet2_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4534 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet_utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      347 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4059 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    16044 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3939 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1314 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/presets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      797 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2797 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10798 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9023 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      808 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    12697 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      524 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5455 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      682 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17008 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5558 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7121 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      338 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3907 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      275 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.612278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2774 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      370 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6514 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/temp/model/default_model.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    25125 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/partition.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/rec/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/rec/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8776 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/rec/datasets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/rec/rating_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11647 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      425 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/rec/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/series/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9882 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1600 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/datasets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      345 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4639 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    13427 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4531 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/datasets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/temp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      185 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/temp/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      308 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/temp/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7994 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/temp/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/temp/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/temp/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/tabular/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/tabular/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/toolkits/tabular/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9992 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/tabular/classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11416 2024-04-13 06:25:56.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/tabular/classification/datasets.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7488 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/toolkits/visualization.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/vertical_mnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      260 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/vertical_mnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7230 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/vertical_mnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/vertical_mnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1162 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/voc_detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/voc_detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2159 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/voc_detection/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      794 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/voc_detection/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/voc_detection/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      551 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/voc_detection/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/wikitext2_modeling/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      273 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/wikitext2_modeling/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3375 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/wikitext2_modeling/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6330 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/benchmark/wikitext2_modeling/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/benchmark/wikitext2_modeling/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      445 2024-04-13 06:25:55.000000 flgo-0.2.6/src/flgo/benchmark/wikitext2_modeling/model/default_model.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/experiment/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       62 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/experiment/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    27628 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/experiment/analyzer.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6651 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/experiment/device_scheduler.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.616278 flgo-0.2.6/src/flgo/experiment/logger/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    90223 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    36834 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1857 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/dec_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2262 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/full_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      343 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/gval_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    59619 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/handlers.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      469 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/hier_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      323 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/parallel_hlogger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1522 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/pfl_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      415 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/pool.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1598 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/simple_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      386 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/test_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      951 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/tune_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1040 2024-04-13 06:25:54.000000 flgo-0.2.6/src/flgo/experiment/logger/vertical_logger.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.620278 flgo-0.2.6/src/flgo/simulator/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5181 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/simulator/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    25114 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/simulator/base.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17046 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/simulator/default_simulator.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1030 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/simulator/my_simulator.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17600 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/simulator/phone_simulator.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.620278 flgo-0.2.6/src/flgo/utils/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3173 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/utils/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    73860 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/utils/fflow.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    28264 2024-04-13 06:25:52.000000 flgo-0.2.6/src/flgo/utils/fmodule.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.620278 flgo-0.2.6/src/flgo.egg-info/
+-rw-r--r--   0 wz        (1001) wz        (1001)      716 2024-04-13 06:26:45.000000 flgo-0.2.6/src/flgo.egg-info/PKG-INFO
+-rw-rw-r--   0 wz        (1001) wz        (1001)    20314 2024-04-13 06:26:45.000000 flgo-0.2.6/src/flgo.egg-info/SOURCES.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)        1 2024-04-13 06:26:45.000000 flgo-0.2.6/src/flgo.egg-info/dependency_links.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)       81 2024-04-13 06:26:45.000000 flgo-0.2.6/src/flgo.egg-info/requires.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)        5 2024-04-13 06:26:45.000000 flgo-0.2.6/src/flgo.egg-info/top_level.txt
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2024-04-13 06:26:45.620278 flgo-0.2.6/tests/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      947 2023-03-21 13:46:37.000000 flgo-0.2.6/tests/test.py
```

### Comparing `flgo-0.2.5/LICENSE` & `flgo-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/PKG-INFO` & `flgo-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flgo
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Research-oriented FL Platform. 
 Author-email: Zheng Wang <zwang@stu.xmu.edu.cn>
 Project-URL: Homepage, https://flgo-xmu.github.io
 Project-URL: Bug Tracker, https://github.com/WwZzz/easyFL/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flgo-0.2.5/pyproject.toml` & `flgo-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "setuptools" 
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "flgo"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Zheng Wang", email="zwang@stu.xmu.edu.cn" },
 ]
 dependencies = [
     "tqdm",
     "torch",
     "torchvision",
```

### Comparing `flgo-0.2.5/src/flgo/__init__.py` & `flgo-0.2.6/src/flgo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .utils.fflow import init, gen_task, gen_task_by_, gen_benchmark_from_file, zip_task, pull_task_from_, gen_real_task, gen_decentralized_benchmark, gen_hierarchical_benchmark, gen_empty_task, convert_model,tune, run_in_parallel, module2fmodule, multi_init_and_run, set_data_root,download_resource, list_resource, option_helper
 from .benchmark import data_root
 communicator = None
 _data_root = data_root
 _name = None
-__version__ = "v0.2.5"
+__version__ = "v0.2.6"
 class VirtualCommunicator:
     """
     Communicator that simulates the communication phase between any two objects
     """
     def __init__(self, objects):
         self.objects_map = {obj.id:obj for obj in objects}
         self.objects = objects
```

### Comparing `flgo-0.2.5/src/flgo/algorithm/TiFL.py` & `flgo-0.2.6/src/flgo/algorithm/TiFL.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/afl.py` & `flgo-0.2.6/src/flgo/algorithm/afl.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/clustered_sampling.py` & `flgo-0.2.6/src/flgo/algorithm/clustered_sampling.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/decentralized.py` & `flgo-0.2.6/src/flgo/algorithm/decentralized.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/ditto.py` & `flgo-0.2.6/src/flgo/algorithm/ditto.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedasync.py` & `flgo-0.2.6/src/flgo/algorithm/mifa.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-"""This is a non-official implementation of 'Asynchronous Federated Optimization' (http://arxiv.org/abs/1903.03934). """
-from .fedbase import BasicServer
-from .fedprox import Client
-
+"""
+This is a non-official implementation of 'Fast Federated Learning in the
+Presence of Arbitrary Device Unavailability' (http://arxiv.org/abs/2106.04159)
+"""
+from flgo.algorithm.fedbase import BasicServer, BasicClient
+from flgo.algorithm.fedavg import Client
+from flgo.utils import fmodule
 
 class Server(BasicServer):
-    def initialize(self):
-        self.init_algo_para(
-            {'period': 20, 'alpha': 0.6, 'mu': 0.005, 'flag': 'constant', 'hinge_a': 10, 'hinge_b': 6, 'poly_a': 0.5})
-        self.tolerance_for_latency = 1000
-        self.client_taus = [0 for _ in self.clients]
+    def initialize(self, *args, **kwargs):
+        self.init_algo_para({'c':1.0})
+        self.update_table = [None for _ in range(self.num_clients)]
+        self.initflag = False
+        # choose all the clients that are active
+        self.clients_per_round = self.num_clients
+
+    def check_if_init(self):
+        """Check whether the update_table is initialized"""
+        s = len([u for u in self.update_table if u])
+        # c==0 infers that updating starts immediately
+        if s < self.c*self.num_clients: return False
+        self.gv.logger.info("G_i Initialized For {}/{} The Clients.".format(s,self.num_clients))
+        self.initflag = True
+        return True
 
     def iterate(self):
-        # Scheduler periodically triggers the idle clients to locally train the model
-        if (self.gv.clock.current_time % self.period) == 0 or self.gv.clock.current_time == 1:
-            self.selected_clients = self.sample()
-        else:
-            self.selected_clients = []
-        if len(self.selected_clients) > 0:
-            self.gv.logger.info(
-                'Select clients {} at time {}'.format(self.selected_clients, self.gv.clock.current_time))
-        # Record the timestamp of the selected clients
-        for cid in self.selected_clients: self.client_taus[cid] = self.current_round
-        # Check the currently received models
-        res = self.communicate(self.selected_clients, asynchronous=True)
-        received_models = res['model']
-        received_client_ids = res['__cid']
-        if len(received_models) > 0:
-            self.gv.logger.info(
-                'Receive new models from clients {} at time {}'.format(received_client_ids, self.gv.clock.current_time))
-            # averaging the simultaneously received models at the current moment
-            taus = [self.client_taus[cid] for cid in received_client_ids]
-            alpha_ts = [self.alpha * self.s(self.current_round - tau) for tau in taus]
-            currently_updated_models = [(1 - alpha_t) * self.model + alpha_t * model_k for alpha_t, model_k in
-                                        zip(alpha_ts, received_models)]
-            self.model = self.aggregate(currently_updated_models)
-        return len(received_models) > 0
+        # sample all the active clients
+        self.selected_clients = self.sample()
+        # training
+        models = self.communicate(self.selected_clients)['model']
+        # update G
+        for k in range(len(self.received_clients)):
+            self.update_table[self.received_clients[k]] = 1.0 / self.lr * (self.model - models[k])
+        # check if the update_table being initialized
+        if not self.initflag:
+            if not self.check_if_init():
+                return
+        # aggregate: w = w - eta_t * 1/N * sum(G_i)
+        self.model = self.aggregate()
+        return
 
-    def s(self, delta_tau):
-        if self.flag == 'constant':
-            return 1
-        elif self.flag == 'hinge':
-            return 1 if delta_tau <= self.hinge_b else 1.0 / (self.hinge_a * (delta_tau - self.hinge_b))
-        elif self.flag == 'poly':
-            return (delta_tau + 1) ** (-self.poly_a)
+    def aggregate(self):
+        return self.model - self.lr * fmodule._model_average([update_i for update_i in self.update_table if update_i])
```

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedavgm.py` & `flgo-0.2.6/src/flgo/algorithm/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedbase.py` & `flgo-0.2.6/src/flgo/algorithm/fedbase.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedbuff.py` & `flgo-0.2.6/src/flgo/algorithm/fedbuff.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,59 +2,37 @@
 from flgo.algorithm.fedasync import Server as AsyncServer
 from flgo.algorithm.fedbase import BasicClient
 import flgo.utils.fmodule as fmodule
 import copy
 
 class Server(AsyncServer):
     def initialize(self):
-        self.init_algo_para({'buffer_ratio': 0.2, 'eta': 1.0, 'period': 1,})
-        self.tolerance_for_latency = 1000
-        self.updated = True
+        self.init_algo_para({'buffer_ratio': 0.1, 'eta': 1.0})
         self.buffer = []
 
-    def pack(self, client_id, mtype=0, *args, **kwargs):
-        return {
-            'model': copy.deepcopy(self.model),
-            'round': self.current_round,
-        }
-
-    def iterate(self):
-        # Scheduler periodically triggers the idle clients to locally train the model
-        self.selected_clients = self.sample() if (self.gv.clock.current_time % self.period) == 0 or self.gv.clock.current_time == 1 else []
-        if len(self.selected_clients) > 0:
-            self.gv.logger.info('Select clients {} at time {}'.format(self.selected_clients, self.gv.clock.current_time))
-        res = self.communicate(self.selected_clients, asynchronous=True)
-        received_updates = res['update']
-        received_client_taus = res['round']
-        received_client_ids = res['__cid']
-        # if reveive client update
-        if len(received_updates) > 0:
-            self.gv.logger.info('Receive new models from clients {} at time {}'.format(received_client_ids, self.gv.clock.current_time))
-            for cdelta, ctau in zip(received_updates, received_client_taus):
-                self.buffer.append((cdelta, ctau))
-            if len(self.buffer)>=int(self.buffer_ratio*self.num_clients):
-                # aggregate and clear updates in buffer
-                taus_bf = [b[1] for b in self.buffer]
-                updates_bf = [b[0] for b in self.buffer]
-                weights_bf = [(1+self.current_round-ctau)**(-0.5) for ctau in taus_bf]
-                model_delta = fmodule._model_average(updates_bf, weights_bf)/len(self.buffer)
-                self.model = self.model + self.eta * model_delta
-                # clear buffer
-                self.buffer = []
-                return True
+    def package_handler(self, received_packages:dict):
+        if self.is_package_empty(received_packages): return False
+        received_updates = received_packages['model']
+        received_client_taus = [u._round for u in received_updates]
+        for cdelta, ctau in zip(received_updates, received_client_taus):
+            self.buffer.append((cdelta, ctau))
+        if len(self.buffer) >= int(self.buffer_ratio * self.num_clients):
+            # aggregate and clear updates in buffer
+            taus_bf = [b[1] for b in self.buffer]
+            updates_bf = [b[0] for b in self.buffer]
+            weights_bf = [(1 + self.current_round - ctau) ** (-0.5) for ctau in taus_bf]
+            model_delta = fmodule._model_average(updates_bf, weights_bf) / len(self.buffer)
+            self.model = self.model + self.eta * model_delta
+            # clear buffer
+            self.buffer = []
+            return True
         return False
 
 class Client(BasicClient):
-    def unpack(self, received_pkg):
-        round = received_pkg['round']
-        model = received_pkg['model']
-        return model, round
-
-    def pack(self, model, round):
-        return {'update':model, 'round':round}
-
     def reply(self, svr_pkg):
-        model,round  = self.unpack(svr_pkg)
+        model = self.unpack(svr_pkg)
         global_model = copy.deepcopy(model)
         self.train(model)
-        cpkg = self.pack(model-global_model, round)
+        update = model-global_model
+        update._round = model._round
+        cpkg = self.pack(update)
         return cpkg
```

### Comparing `flgo-0.2.5/src/flgo/algorithm/feddyn.py` & `flgo-0.2.6/src/flgo/algorithm/feddyn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedfa.py` & `flgo-0.2.6/src/flgo/algorithm/fedfa.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedfv.py` & `flgo-0.2.6/src/flgo/algorithm/fedfv.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedmf.py` & `flgo-0.2.6/src/flgo/algorithm/fedmf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedmgda.py` & `flgo-0.2.6/src/flgo/algorithm/fedmgda.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fednova.py` & `flgo-0.2.6/src/flgo/algorithm/fednova.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/fedprox.py` & `flgo-0.2.6/src/flgo/algorithm/fedprox.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/hierarchical.py` & `flgo-0.2.6/src/flgo/algorithm/hierarchical.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/mifa.py` & `flgo-0.2.6/src/flgo/algorithm/qfedavg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,31 @@
-"""
-This is a non-official implementation of 'Fast Federated Learning in the
-Presence of Arbitrary Device Unavailability' (http://arxiv.org/abs/2106.04159)
-"""
-from flgo.algorithm.fedbase import BasicServer, BasicClient
-from flgo.algorithm.fedavg import Client
-from flgo.utils import fmodule
+"""This is a non-official implementation of 'Fair Resource Allocation in
+Federated Learning' (http://arxiv.org/abs/1905.10497).  And this implementation
+refers to the official github repository https://github.com/litian96/fair_flearn """
+import flgo.algorithm.fedbase as fedbase
+import flgo.utils.fmodule as fmodule
+import copy
 
-class Server(BasicServer):
+class Server(fedbase.BasicServer):
     def initialize(self, *args, **kwargs):
-        self.init_algo_para({'c':1.0})
-        self.update_table = [None for _ in range(self.num_clients)]
-        self.initflag = False
-        # choose all the clients that are active
-        self.clients_per_round = self.num_clients
-
-    def check_if_init(self):
-        """Check whether the update_table is initialized"""
-        s = len([u for u in self.update_table if u])
-        # c==0 infers that updating starts immediately
-        if s < self.c*self.num_clients: return False
-        self.gv.logger.info("G_i Initialized For {}/{} The Clients.".format(s,self.num_clients))
-        self.initflag = True
-        return True
+        self.init_algo_para({'q': 1.0})
 
     def iterate(self):
-        # sample all the active clients
         self.selected_clients = self.sample()
-        # training
-        models = self.communicate(self.selected_clients)['model']
-        # update G
-        for k in range(len(self.received_clients)):
-            self.update_table[self.received_clients[k]] = 1.0 / self.lr * (self.model - models[k])
-        # check if the update_table being initialized
-        if not self.initflag:
-            if not self.check_if_init():
-                return
-        # aggregate: w = w - eta_t * 1/N * sum(G_i)
-        self.model = self.aggregate()
-        return
+        res = self.communicate(self.selected_clients)
+        self.model = self.model - fmodule._model_sum(res['dk']) / sum(res['hk'])
+        return len(self.received_clients) > 0
+
+class Client(fedbase.BasicClient):
+    def unpack(self, package):
+        model = package['model']
+        self.global_model = copy.deepcopy(model)
+        return model
 
-    def aggregate(self):
-        return self.model - self.lr * fmodule._model_average([update_i for update_i in self.update_table if update_i])
+    def pack(self, model):
+        Fk = self.test(self.global_model, 'train')['loss'] + 1e-8
+        L = 1.0 / self.learning_rate
+        delta_wk = L * (self.global_model - model)
+        dk = (Fk ** self.q) * delta_wk
+        hk = self.q * (Fk ** (self.q - 1)) * (delta_wk.norm() ** 2) + L * (Fk ** self.q)
+        self.global_model = None
+        return {'dk': dk, 'hk': hk}
```

### Comparing `flgo-0.2.5/src/flgo/algorithm/powerofchoice.py` & `flgo-0.2.6/src/flgo/algorithm/powerofchoice.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/realbase.py` & `flgo-0.2.6/src/flgo/algorithm/realbase.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/scaffold.py` & `flgo-0.2.6/src/flgo/algorithm/scaffold.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/sesorec.py` & `flgo-0.2.6/src/flgo/algorithm/sesorec.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/standalone.py` & `flgo-0.2.6/src/flgo/algorithm/standalone.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/algorithm/vflbase.py` & `flgo-0.2.6/src/flgo/algorithm/vflbase.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/adult_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/adult_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/agnews_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/agnews_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/agnews_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/agnews_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/bankmarketing_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/bankmarketing_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/base.py` & `flgo-0.2.6/src/flgo/benchmark/base.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/ciao_recommendation/core.py` & `flgo-0.2.6/src/flgo/benchmark/ciao_recommendation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/ciao_recommendation/model/mf.py` & `flgo-0.2.6/src/flgo/benchmark/ciao_recommendation/model/mf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar100_classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/cifar100_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar100_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/cifar100_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar100_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/cifar100_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar100_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/cifar100_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar100_classification/model/resnet18.py` & `flgo-0.2.6/src/flgo/benchmark/cifar100_classification/model/resnet18.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar100_classification/model/resnet18_gn.py` & `flgo-0.2.6/src/flgo/benchmark/cifar100_classification/model/resnet18_gn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar10_classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/cifar10_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar10_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/cifar10_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar10_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/cifar10_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar10_classification/dataset.py` & `flgo-0.2.6/src/flgo/benchmark/cifar10_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/cnn_data_aug.py` & `flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/cnn_data_aug.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/mlp.py` & `flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cifar10_classification/model/resnet18_gn.py` & `flgo-0.2.6/src/flgo/benchmark/cifar10_classification/model/resnet18_gn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/config.py` & `flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/core.py` & `flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/citeseer_link_prediction/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/citeseer_link_prediction/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/citeseer_node_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/citeseer_node_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/citeseer_node_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/citeseer_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/coco_detection/core.py` & `flgo-0.2.6/src/flgo/benchmark/coco_detection/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/coco_detection/model/FasterRCNN.py` & `flgo-0.2.6/src/flgo/benchmark/coco_detection/model/FasterRCNN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/coco_segmentation/core.py` & `flgo-0.2.6/src/flgo/benchmark/coco_segmentation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py` & `flgo-0.2.6/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/coco_segmentation/model/unet.py` & `flgo-0.2.6/src/flgo/benchmark/coco_segmentation/model/unet.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/config.py` & `flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/core.py` & `flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/model/GCN.py` & `flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_link_prediction/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/cora_link_prediction/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_node_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/cora_node_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_node_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/cora_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_node_classification/model/GCN.py` & `flgo-0.2.6/src/flgo/benchmark/cora_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py` & `flgo-0.2.6/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/cora_node_classification/model/GraphSage.py` & `flgo-0.2.6/src/flgo/benchmark/cora_node_classification/model/GraphSage.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/crop_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/crop_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/crop_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/crop_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/distributed_quadratic_programming/core.py` & `flgo-0.2.6/src/flgo/benchmark/distributed_quadratic_programming/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/distributed_quadratic_programming/model/vec.py` & `flgo-0.2.6/src/flgo/benchmark/distributed_quadratic_programming/model/vec.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/electricdevices_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/electricdevices_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/electricdevices_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/electricdevices_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/electricity_forecasting/core.py` & `flgo-0.2.6/src/flgo/benchmark/electricity_forecasting/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/electricity_forecasting/model/GRU.py` & `flgo-0.2.6/src/flgo/benchmark/electricity_forecasting/model/GRU.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/emnist_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/emnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/emnist_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/emnist_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/emnist_classification/model/mlp.py` & `flgo-0.2.6/src/flgo/benchmark/emnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/enzymes_graph_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/enzymes_graph_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/enzymes_graph_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/enzymes_graph_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/core.py` & `flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/model/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/model/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/epinions_recommendation/model/mf.py` & `flgo-0.2.6/src/flgo/benchmark/epinions_recommendation/model/mf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/exchange_rate_forecasting/core.py` & `flgo-0.2.6/src/flgo/benchmark/exchange_rate_forecasting/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/exchange_rate_forecasting/model/GRU.py` & `flgo-0.2.6/src/flgo/benchmark/exchange_rate_forecasting/model/GRU.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/fashion_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/fashion_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/fashion_classification/model/lr.py` & `flgo-0.2.6/src/flgo/benchmark/fashion_classification/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/fcube_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/fcube_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/fcube_classification/model/lr.py` & `flgo-0.2.6/src/flgo/benchmark/fcube_classification/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/femnist_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/femnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/femnist_classification/dataset.py` & `flgo-0.2.6/src/flgo/benchmark/femnist_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/femnist_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/femnist_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/heart_disease_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/heart_disease_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/imdb_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/imdb_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/imdb_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/imdb_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/leaf_reddit/core.py` & `flgo-0.2.6/src/flgo/benchmark/leaf_reddit/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py` & `flgo-0.2.6/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/leaf_sent140/core.py` & `flgo-0.2.6/src/flgo/benchmark/leaf_sent140/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py` & `flgo-0.2.6/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/local_movielens_recommendation/core.py` & `flgo-0.2.6/src/flgo/benchmark/local_movielens_recommendation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/local_movielens_recommendation/model/mf.py` & `flgo-0.2.6/src/flgo/benchmark/local_movielens_recommendation/model/mf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/mnist_classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/mnist_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/mnist_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/mnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/mnist_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/mnist_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/mnist_classification/model/mlp.py` & `flgo-0.2.6/src/flgo/benchmark/mnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/movielens_recommendation/core.py` & `flgo-0.2.6/src/flgo/benchmark/movielens_recommendation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/movielens_recommendation/model/mf.py` & `flgo-0.2.6/src/flgo/benchmark/movielens_recommendation/model/mf.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/multi30k_translation/config.py` & `flgo-0.2.6/src/flgo/benchmark/multi30k_translation/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/multi30k_translation/core.py` & `flgo-0.2.6/src/flgo/benchmark/multi30k_translation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/mutag_graph_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/mutag_graph_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/mutag_graph_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/mutag_graph_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/nifECG_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/nifECG_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/nifECG_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/nifECG_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/oxfordiiitpet_segmentation/config.py` & `flgo-0.2.6/src/flgo/benchmark/oxfordiiitpet_segmentation/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/oxfordiiitpet_segmentation/core.py` & `flgo-0.2.6/src/flgo/benchmark/oxfordiiitpet_segmentation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/partition.py` & `flgo-0.2.6/src/flgo/benchmark/partition.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/penntreebank_modeling/config.py` & `flgo-0.2.6/src/flgo/benchmark/penntreebank_modeling/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/penntreebank_modeling/core.py` & `flgo-0.2.6/src/flgo/benchmark/penntreebank_modeling/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/config.py` & `flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/core.py` & `flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/pubmed_link_prediction/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/pubmed_link_prediction/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/pubmed_node_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/pubmed_node_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/pubmed_node_classification/model/GCN.py` & `flgo-0.2.6/src/flgo/benchmark/pubmed_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/core.py` & `flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py` & `flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/sbdataset_segmentation/model/unet.py` & `flgo-0.2.6/src/flgo/benchmark/sbdataset_segmentation/model/unet.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/shakespeare_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/shakespeare_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py` & `flgo-0.2.6/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/social_splitted_ciao/core.py` & `flgo-0.2.6/src/flgo/benchmark/social_splitted_ciao/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/social_splitted_ciaodvd/core.py` & `flgo-0.2.6/src/flgo/benchmark/social_splitted_ciaodvd/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/social_splitted_douban/core.py` & `flgo-0.2.6/src/flgo/benchmark/social_splitted_douban/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/social_splitted_epinions/core.py` & `flgo-0.2.6/src/flgo/benchmark/social_splitted_epinions/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/social_splitted_filmtrust/core.py` & `flgo-0.2.6/src/flgo/benchmark/social_splitted_filmtrust/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/sst2_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/sst2_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/sst2_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/sst2_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/stl10_classification/config.py` & `flgo-0.2.6/src/flgo/benchmark/stl10_classification/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/stl10_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/stl10_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/stl10_classification/dataset.py` & `flgo-0.2.6/src/flgo/benchmark/stl10_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/cnn_data_aug.py` & `flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/cnn_data_aug.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/resnet18_gn.py` & `flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/resnet18_gn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/stl10_classification/model/resnet34_gn.py` & `flgo-0.2.6/src/flgo/benchmark/stl10_classification/model/resnet34_gn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/svhn_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/svhn_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/svhn_classification/model/cnn.py` & `flgo-0.2.6/src/flgo/benchmark/svhn_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/svhn_classification/model/mlp.py` & `flgo-0.2.6/src/flgo/benchmark/svhn_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/synthetic_regression/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/synthetic_regression/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/synthetic_regression/core.py` & `flgo-0.2.6/src/flgo/benchmark/synthetic_regression/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/synthetic_regression/model/lr.py` & `flgo-0.2.6/src/flgo/benchmark/synthetic_regression/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/dec_temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/dec_temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/hier_temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/hier_temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/classification/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/presets.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/presets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/transforms.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/transforms.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/detection/utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/detection/utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/pointnet2_utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/pointnet2_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/pointnet_utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/pointnet_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet2_utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet2_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet_utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/pointnet_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_part_segmentation/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet2_utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet2_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet_utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/pointnet_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/points_semantic_segmentation/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/presets.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/presets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/cv/segmentation/utils.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/cv/segmentation/utils.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/graph_classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/link_prediction/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/graph/node_classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/classification/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/language_modeling/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/nlp/translation/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/nlp/translation/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/partition.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/partition.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/rec/datasets.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/rec/datasets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/datasets.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/datasets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/series/classification/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/series/classification/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/datasets.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/datasets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/temp/core.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/temp/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/series/forecasting/temp/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/series/forecasting/temp/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/tabular/classification/__init__.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/tabular/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/tabular/classification/datasets.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/tabular/classification/datasets.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/toolkits/visualization.py` & `flgo-0.2.6/src/flgo/benchmark/toolkits/visualization.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/vertical_mnist_classification/core.py` & `flgo-0.2.6/src/flgo/benchmark/vertical_mnist_classification/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py` & `flgo-0.2.6/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/voc_detection/config.py` & `flgo-0.2.6/src/flgo/benchmark/voc_detection/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/voc_detection/core.py` & `flgo-0.2.6/src/flgo/benchmark/voc_detection/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/voc_detection/model/default_model.py` & `flgo-0.2.6/src/flgo/benchmark/voc_detection/model/default_model.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/wikitext2_modeling/config.py` & `flgo-0.2.6/src/flgo/benchmark/wikitext2_modeling/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/benchmark/wikitext2_modeling/core.py` & `flgo-0.2.6/src/flgo/benchmark/wikitext2_modeling/core.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/analyzer.py` & `flgo-0.2.6/src/flgo/experiment/analyzer.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/device_scheduler.py` & `flgo-0.2.6/src/flgo/experiment/device_scheduler.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/__init__.py` & `flgo-0.2.6/src/flgo/experiment/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/config.py` & `flgo-0.2.6/src/flgo/experiment/logger/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/dec_logger.py` & `flgo-0.2.6/src/flgo/experiment/logger/dec_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/full_logger.py` & `flgo-0.2.6/src/flgo/experiment/logger/full_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/handlers.py` & `flgo-0.2.6/src/flgo/experiment/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/pfl_logger.py` & `flgo-0.2.6/src/flgo/experiment/logger/pfl_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/simple_logger.py` & `flgo-0.2.6/src/flgo/experiment/logger/simple_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/tune_logger.py` & `flgo-0.2.6/src/flgo/experiment/logger/tune_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/experiment/logger/vertical_logger.py` & `flgo-0.2.6/src/flgo/experiment/logger/vertical_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/simulator/__init__.py` & `flgo-0.2.6/src/flgo/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/simulator/base.py` & `flgo-0.2.6/src/flgo/simulator/base.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/simulator/default_simulator.py` & `flgo-0.2.6/src/flgo/simulator/default_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/simulator/my_simulator.py` & `flgo-0.2.6/src/flgo/simulator/my_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/simulator/phone_simulator.py` & `flgo-0.2.6/src/flgo/simulator/phone_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/utils/__init__.py` & `flgo-0.2.6/src/flgo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/utils/fflow.py` & `flgo-0.2.6/src/flgo/utils/fflow.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo/utils/fmodule.py` & `flgo-0.2.6/src/flgo/utils/fmodule.py`

 * *Files identical despite different names*

### Comparing `flgo-0.2.5/src/flgo.egg-info/PKG-INFO` & `flgo-0.2.6/src/flgo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flgo
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Research-oriented FL Platform. 
 Author-email: Zheng Wang <zwang@stu.xmu.edu.cn>
 Project-URL: Homepage, https://flgo-xmu.github.io
 Project-URL: Bug Tracker, https://github.com/WwZzz/easyFL/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flgo-0.2.5/src/flgo.egg-info/SOURCES.txt` & `flgo-0.2.6/src/flgo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/flgo.egg-info/SOURCES.txt
 src/flgo.egg-info/dependency_links.txt
 src/flgo.egg-info/requires.txt
 src/flgo.egg-info/top_level.txt
 src/flgo/algorithm/TiFL.py
 src/flgo/algorithm/__init__.py
 src/flgo/algorithm/afl.py
+src/flgo/algorithm/asyncbase.py
 src/flgo/algorithm/clustered_sampling.py
 src/flgo/algorithm/decentralized.py
 src/flgo/algorithm/ditto.py
 src/flgo/algorithm/fedasync.py
 src/flgo/algorithm/fedavg.py
 src/flgo/algorithm/fedavgm.py
 src/flgo/algorithm/fedbase.py
```

### Comparing `flgo-0.2.5/tests/test.py` & `flgo-0.2.6/tests/test.py`

 * *Files identical despite different names*

