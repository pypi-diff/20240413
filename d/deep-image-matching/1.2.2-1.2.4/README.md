# Comparing `tmp/deep_image_matching-1.2.2.tar.gz` & `tmp/deep_image_matching-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_image_matching-1.2.2.tar", last modified: Sat Apr 13 15:55:26 2024, max compression
+gzip compressed data, was "deep_image_matching-1.2.4.tar", last modified: Sat Apr 13 16:38:55 2024, max compression
```

## Comparing `deep_image_matching-1.2.2.tar` & `deep_image_matching-1.2.4.tar`

### file list

```diff
@@ -1,375 +1,375 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.231243 deep_image_matching-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-13 15:55:18.000000 deep_image_matching-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15971 2024-04-13 15:55:26.231243 deep_image_matching-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-13 15:55:18.000000 deep_image_matching-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:55:26.231243 deep_image_matching-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.167243 deep_image_matching-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.179243 deep_image_matching-1.2.2/src/deep_image_matching/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.183243 deep_image_matching-1.2.2/src/deep_image_matching/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/alike.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/aliked.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/cosplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/dedode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/extractor_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/keynetaffnethardnet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/kornia_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/netvlad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/no_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/openibl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/orb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/sift.py
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/extractors/superpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/image_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/image_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.183243 deep_image_matching-1.2.2/src/deep_image_matching/io/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22365 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/io/colmap_read_write_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/io/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/io/h5_to_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/io/h5_to_micmac.py
--rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/io/h5_to_openmvg.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/io/micmac_to_h5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/low_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.187243 deep_image_matching-1.2.2/src/deep_image_matching/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/adalam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/kornia_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/lightglue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/loftr.py
--rw-r--r--   0 runner    (1001) docker     (127)    45260 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/matcher_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/roma.py
--rw-r--r--   0 runner    (1001) docker     (127)    12963 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/se2loftr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/matchers/superglue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/openmvg_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/pairs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.187243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.187243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/count_flops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.187243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/custom_ops/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/custom_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/custom_ops/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/demo_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/demo_seq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.187243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/aliked.py
--rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/padder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/soft_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.187243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.191243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.191243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est_mnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/nll_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/num_inliers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.191243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/megadepth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.191243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/dedode_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/descriptor_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.191243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/dedode_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/keypoint_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.191243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/dual_softmax_matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.191243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/dedode_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.195243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/dinov2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.195243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/dino_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/layer_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/swiglu_ffn.py
--rw-r--r--   0 runner    (1001) docker     (127)    25761 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.195243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/data_prep/
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/data_prep/prep_keypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.195243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match_dedode_G.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_scoremap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.195243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-B.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-G.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.195243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-B.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-G.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.171243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.199243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25794 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/aliked.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/lightglue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/sift.py
--rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/superpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/viz2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.199243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.199243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.199243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/hpatches_sequences_homog_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_dense_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_pose_estimation_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/scannet_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.199243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.199243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/datasets/megadepth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/datasets/scannet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.199243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/losses/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/losses/robust_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.203243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    32038 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.203243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/roma_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.203243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/dinov2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.203243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/dino_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/layer_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/patch_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/swiglu_ffn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.203243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/train/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/train/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.207243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/local_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    20918 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.207243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11268 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18884 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.207243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.207243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/alike/
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/alike/alike.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/alike/alnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/alike/soft_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.211243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/colmap_from_nvm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extract_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.211243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/cosplace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/d2net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/dir.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/dog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/netvlad.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/openibl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/r2d2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/superpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/localize_inloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/localize_sfm.py
--rw-r--r--   0 runner    (1001) docker     (127)    21799 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/match_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/match_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.211243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/adalam.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/lightglue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/loftr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/nearest_neighbor.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/superglue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pairs_from_covisibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pairs_from_exhaustive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pairs_from_poses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pairs_from_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.211243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.215243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/localize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/prepare_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.215243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/create_gt_sfm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.215243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.215243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline_loftr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.215243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.215243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.215243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/colmap_from_nvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/triangulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.219243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22365 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/read_write_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/viz_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.219243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.175243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.175243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.219243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.219243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ds_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ot.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ot_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ds_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ot.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ot_dense.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.219243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval_new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.223243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.223243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ds_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ot.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ot_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_8rot.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_big.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ot.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ot_dense.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.223243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/demo/
--rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/demo/demo_loftr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.223243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.223243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/config/
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/config/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.223243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/datasets/megadepth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/datasets/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/datasets/scannet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.223243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/lightning/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/lightning/lightning_loftr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.223243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.227243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_e2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_fpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.227243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/fine_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/linear_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.227243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/coarse_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/cvpr_ds_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/fine_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/supervision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.227243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/losses/loftr_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.227243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.227243 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    67149 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/triangulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.231243 deep_image_matching-1.2.2/src/deep_image_matching/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/geometric_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/hloc_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/sensor_width_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/tiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/src/deep_image_matching/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.231243 deep_image_matching-1.2.2/src/deep_image_matching.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15971 2024-04-13 15:55:26.000000 deep_image_matching-1.2.2/src/deep_image_matching.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-04-13 15:55:26.000000 deep_image_matching-1.2.2/src/deep_image_matching.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:55:26.000000 deep_image_matching-1.2.2/src/deep_image_matching.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-13 15:55:26.000000 deep_image_matching-1.2.2/src/deep_image_matching.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 15:55:26.000000 deep_image_matching-1.2.2/src/deep_image_matching.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:55:26.231243 deep_image_matching-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/tests/test_geom_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-13 15:55:19.000000 deep_image_matching-1.2.2/tests/test_tiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.671280 deep_image_matching-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15993 2024-04-13 16:38:55.671280 deep_image_matching-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:38:55.671280 deep_image_matching-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.607280 deep_image_matching-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.619280 deep_image_matching-1.2.4/src/deep_image_matching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.623280 deep_image_matching-1.2.4/src/deep_image_matching/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/alike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/aliked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/cosplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/dedode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/extractor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/keynetaffnethardnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/kornia_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/netvlad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/no_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/openibl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/orb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/sift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/extractors/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/image_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/image_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.623280 deep_image_matching-1.2.4/src/deep_image_matching/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22365 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/io/colmap_read_write_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/io/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/io/h5_to_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/io/h5_to_micmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/io/h5_to_openmvg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/io/micmac_to_h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/low_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.623280 deep_image_matching-1.2.4/src/deep_image_matching/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/adalam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/kornia_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/lightglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/loftr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45260 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/matcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/roma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12963 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/se2loftr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/matchers/superglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/openmvg_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/pairs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.627280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.627280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/count_flops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.627280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/custom_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/custom_ops/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/demo_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/demo_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.627280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/aliked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/padder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/soft_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.627280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.627280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.631280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est_mnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/nll_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/num_inliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.631280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/megadepth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.631280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/dedode_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/descriptor_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.631280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/dedode_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/keypoint_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.631280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/dual_softmax_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.631280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/dedode_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.631280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/dinov2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.635280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/dino_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/layer_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/swiglu_ffn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25761 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.635280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/data_prep/
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/data_prep/prep_keypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.635280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match_dedode_G.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_scoremap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.635280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-G.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.635280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-G.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.607280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.635280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25794 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/aliked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/lightglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/sift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/viz2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.635280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.639280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.639280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/hpatches_sequences_homog_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_dense_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_pose_estimation_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/scannet_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.639280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.639280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/datasets/megadepth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/datasets/scannet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.639280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/losses/robust_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.639280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32038 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.639280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/roma_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.639280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/dinov2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.643280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/dino_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/layer_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/swiglu_ffn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.643280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/train/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.643280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/local_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20918 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.643280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11268 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18884 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.643280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-04-13 16:38:46.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.647280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/alike/
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/alike/alike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/alike/alnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/alike/soft_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.647280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/colmap_from_nvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extract_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.651280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/cosplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/d2net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/dog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/netvlad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/openibl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/r2d2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/localize_inloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/localize_sfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21799 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/match_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/match_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.651280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/adalam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/lightglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/loftr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/nearest_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/superglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pairs_from_covisibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pairs_from_exhaustive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pairs_from_poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pairs_from_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.651280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.651280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/localize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/prepare_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.651280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/create_gt_sfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.651280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.655280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline_loftr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.655280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.655280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.655280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/colmap_from_nvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.655280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22365 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/read_write_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/viz_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.655280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.611280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.611280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.659280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.659280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ds_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ot_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ds_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ot_dense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.659280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval_new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.659280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.659280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ds_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ot_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_8rot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_big.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ot_dense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.663280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/demo/demo_loftr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.663280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.663280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/config/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.663280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/datasets/megadepth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/datasets/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/datasets/scannet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.663280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/lightning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/lightning/lightning_loftr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.663280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.663280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_e2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.663280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/fine_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/linear_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.667280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/coarse_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/cvpr_ds_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/fine_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/supervision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.667280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/losses/loftr_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.667280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.667280 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67149 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.667280 deep_image_matching-1.2.4/src/deep_image_matching/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/geometric_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/hloc_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/sensor_width_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/tiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/src/deep_image_matching/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.671280 deep_image_matching-1.2.4/src/deep_image_matching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15993 2024-04-13 16:38:55.000000 deep_image_matching-1.2.4/src/deep_image_matching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-04-13 16:38:55.000000 deep_image_matching-1.2.4/src/deep_image_matching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:38:55.000000 deep_image_matching-1.2.4/src/deep_image_matching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-13 16:38:55.000000 deep_image_matching-1.2.4/src/deep_image_matching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 16:38:55.000000 deep_image_matching-1.2.4/src/deep_image_matching.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:38:55.671280 deep_image_matching-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/tests/test_geom_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-13 16:38:47.000000 deep_image_matching-1.2.4/tests/test_tiling.py
```

### Comparing `deep_image_matching-1.2.2/LICENSE` & `deep_image_matching-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/PKG-INFO` & `deep_image_matching-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_image_matching
-Version: 1.2.2
+Version: 1.2.4
 Summary: Multiview matching with deep-learning and hand-crafted local features for COLMAP and other SfM software.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>, Luca Morelli <lmorelli@fbk.eu>
 License: # LICENSE
         
         BSD 3-Clause License
         
         Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
@@ -62,14 +62,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: packaging
 Requires-Dist: einops
 Requires-Dist: pyvis>=0.3.2
 Requires-Dist: yacs>=0.1.8
 Requires-Dist: e2cnn
 Requires-Dist: pytorch_lightning
+Requires-Dist: pytest
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `deep_image_matching-1.2.2/README.md` & `deep_image_matching-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/pyproject.toml` & `deep_image_matching-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
   requires      = ["setuptools>=65", "wheel"]
   build-backend = "setuptools.build_meta"
 
 [project]
   name = "deep_image_matching"
-  version = "1.2.2"
+  version = "1.2.4"
   description = "Multiview matching with deep-learning and hand-crafted local features for COLMAP and other SfM software."
   readme = "README.md"
   authors = [
       { name = "Francesco Ioli", email = "francesco.ioli@polimi.it" },
       { name = "Luca Morelli", email = "lmorelli@fbk.eu"}
   ]
   license = { file = "LICENSE" }
@@ -37,14 +37,15 @@
     "pyyaml",
     "packaging",
     "einops",
     "pyvis>=0.3.2",
     "yacs>=0.1.8",
     "e2cnn",
     "pytorch_lightning",
+    "pytest"
 ]
 
   [project.optional-dependencies]
     dev = [
       "flake8", 
       "black", 
       "bumpver", 
@@ -64,15 +65,15 @@
 
 [tool.pytest.ini_options]
   addopts = [
       "--import-mode=importlib",
   ]
     
 [tool.bumpver]
-  current_version = "1.2.2"
+  current_version = "1.2.4"
   version_pattern = "MAJOR.MINOR.PATCH"
   commit_message = "bump version {old_version} -> {new_version}"
   commit = true
   tag = false
   push = false
 
   [tool.bumpver.file_patterns]
```

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/__init__.py` & `deep_image_matching-1.2.4/src/deep_image_matching/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.2.2"
+__version__ = "1.2.4"
 
 import logging
 from time import time
 from collections import OrderedDict
 
 time_dict = OrderedDict()
 time_dict["start"] = time()
```

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/config.py` & `deep_image_matching-1.2.4/src/deep_image_matching/config.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/constants.py` & `deep_image_matching-1.2.4/src/deep_image_matching/constants.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/alike.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/alike.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/aliked.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/aliked.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/cosplace.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/cosplace.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/dedode.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/dedode.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/disk.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/disk.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/extractor_base.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/extractor_base.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/keynetaffnethardnet.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/keynetaffnethardnet.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/netvlad.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/netvlad.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/no_extractor.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/no_extractor.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/openibl.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/openibl.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/orb.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/orb.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/sift.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/sift.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/extractors/superpoint.py` & `deep_image_matching-1.2.4/src/deep_image_matching/extractors/superpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/graph.py` & `deep_image_matching-1.2.4/src/deep_image_matching/graph.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/gui.py` & `deep_image_matching-1.2.4/src/deep_image_matching/gui.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/image_matching.py` & `deep_image_matching-1.2.4/src/deep_image_matching/image_matching.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/image_retrieval.py` & `deep_image_matching-1.2.4/src/deep_image_matching/image_retrieval.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/io/colmap_read_write_model.py` & `deep_image_matching-1.2.4/src/deep_image_matching/io/colmap_read_write_model.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/io/h5.py` & `deep_image_matching-1.2.4/src/deep_image_matching/io/h5.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/io/h5_to_db.py` & `deep_image_matching-1.2.4/src/deep_image_matching/io/h5_to_db.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/io/h5_to_micmac.py` & `deep_image_matching-1.2.4/src/deep_image_matching/io/h5_to_micmac.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/io/h5_to_openmvg.py` & `deep_image_matching-1.2.4/src/deep_image_matching/io/h5_to_openmvg.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/io/micmac_to_h5.py` & `deep_image_matching-1.2.4/src/deep_image_matching/io/micmac_to_h5.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/low_resolution.py` & `deep_image_matching-1.2.4/src/deep_image_matching/low_resolution.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/matchers/adalam.py` & `deep_image_matching-1.2.4/src/deep_image_matching/matchers/adalam.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/matchers/kornia_matcher.py` & `deep_image_matching-1.2.4/src/deep_image_matching/matchers/kornia_matcher.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/matchers/lightglue.py` & `deep_image_matching-1.2.4/src/deep_image_matching/matchers/lightglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/matchers/loftr.py` & `deep_image_matching-1.2.4/src/deep_image_matching/matchers/loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/matchers/matcher_base.py` & `deep_image_matching-1.2.4/src/deep_image_matching/matchers/matcher_base.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/matchers/roma.py` & `deep_image_matching-1.2.4/src/deep_image_matching/matchers/roma.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/matchers/se2loftr.py` & `deep_image_matching-1.2.4/src/deep_image_matching/matchers/se2loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/matchers/superglue.py` & `deep_image_matching-1.2.4/src/deep_image_matching/matchers/superglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/openmvg_reconstruction.py` & `deep_image_matching-1.2.4/src/deep_image_matching/openmvg_reconstruction.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/pairs_generator.py` & `deep_image_matching-1.2.4/src/deep_image_matching/pairs_generator.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/parser.py` & `deep_image_matching-1.2.4/src/deep_image_matching/parser.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/reconstruction.py` & `deep_image_matching-1.2.4/src/deep_image_matching/reconstruction.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/count_flops.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/count_flops.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/custom_ops/__init__.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/custom_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/demo_pair.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/demo_pair.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/demo_seq.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/demo_seq.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/aliked.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/aliked.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/blocks.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/blocks.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/padder.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/padder.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/ALIKED/nets/soft_detect.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/ALIKED/nets/soft_detect.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est_mnn.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est_mnn.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/nll_benchmark.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/nll_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/num_inliers.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/num_inliers.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/checkpoint.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/megadepth.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/megadepth.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/decoder.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/decoder.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/dedode_descriptor.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/dedode_descriptor.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/descriptor_loss.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/descriptor_loss.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/dedode_detector.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/dedode_detector.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/keypoint_loss.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/keypoint_loss.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/encoder.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/encoder.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/dual_softmax_matcher.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/dual_softmax_matcher.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/dedode_models.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/dedode_models.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/train.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/train.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/dinov2.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/dinov2.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/attention.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/attention.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/block.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/block.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/dino_head.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/dino_head.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/drop_path.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/layer_scale.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/layer_scale.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/mlp.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/patch_embed.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/swiglu_ffn.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/utils.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/data_prep/prep_keypoints.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/data_prep/prep_keypoints.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_kpts.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_kpts.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match_dedode_G.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match_dedode_G.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_scoremap.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_scoremap.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-B.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-B.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-G.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-G.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_detector.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_detector.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-B.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-B.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-G.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-G.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/aliked.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/disk.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/lightglue.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/sift.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/superpoint.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/utils.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/LightGlue/lightglue/viz2d.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/LightGlue/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/hpatches_sequences_homog_benchmark.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/hpatches_sequences_homog_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_dense_benchmark.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_dense_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_pose_estimation_benchmark.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_pose_estimation_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/scannet_benchmark.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/scannet_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/checkpoint.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/datasets/megadepth.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/datasets/megadepth.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/datasets/scannet.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/datasets/scannet.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/losses/robust_loss.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/losses/robust_loss.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/encoders.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/matcher.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/matcher.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/__init__.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/roma_models.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/roma_models.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/__init__.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/dinov2.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/dinov2.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/attention.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/attention.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/block.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/block.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/dino_head.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/dino_head.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/drop_path.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/layer_scale.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/layer_scale.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/mlp.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/patch_embed.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/swiglu_ffn.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/train/train.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/train/train.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/local_correlation.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/local_correlation.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/transforms.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/RoMa/roma/utils/utils.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/RoMa/roma/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/match_pairs.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/match_pairs.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/matching.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/matching.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superglue.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/utils.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/alike/alike.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/alike/alike.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/alike/alnet.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/alike/alnet.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/alike/soft_detect.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/alike/soft_detect.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/colmap_from_nvm.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/colmap_from_nvm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extract_features.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extract_features.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/cosplace.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/cosplace.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/d2net.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/d2net.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/dir.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/dir.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/disk.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/disk.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/dog.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/dog.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/netvlad.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/netvlad.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/openibl.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/openibl.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/r2d2.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/r2d2.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/extractors/superpoint.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/extractors/superpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/localize_inloc.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/localize_inloc.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/localize_sfm.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/localize_sfm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/match_dense.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/match_dense.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/match_features.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/match_features.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/adalam.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/adalam.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/lightglue.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/lightglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/loftr.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/nearest_neighbor.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/matchers/superglue.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/matchers/superglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pairs_from_covisibility.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pairs_from_covisibility.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pairs_from_exhaustive.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pairs_from_exhaustive.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pairs_from_poses.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pairs_from_poses.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pairs_from_retrieval.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pairs_from_retrieval.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/localize.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/localize.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/prepare_reference.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/prepare_reference.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/utils.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/create_gt_sfm.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/create_gt_sfm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/pipeline.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/utils.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/pipeline.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline_loftr.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline_loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/pipeline.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/pipeline.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/utils.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/colmap_from_nvm.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/colmap_from_nvm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/pipeline.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/reconstruction.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/reconstruction.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/triangulation.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/triangulation.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/base_model.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/database.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/database.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/geometry.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/io.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/io.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/parsers.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/read_write_model.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/read_write_model.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/viz.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/viz.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/utils/viz_3d.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/utils/viz_3d.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/hloc/visualization.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/hloc/visualization.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval_new.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval_new.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_8rot.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_8rot.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_big.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_big.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/demo/demo_loftr.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/demo/demo_loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/config/default.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/config/default.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/datasets/megadepth.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/datasets/megadepth.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/datasets/sampler.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/datasets/sampler.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/datasets/scannet.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/datasets/scannet.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/lightning/data.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/lightning/data.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/lightning/lightning_loftr.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/lightning/lightning_loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/__init__.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_e2.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_e2.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_fpn.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_fpn.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/fine_preprocess.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/fine_preprocess.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/linear_attention.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/linear_attention.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/transformer.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/transformer.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/coarse_matching.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/coarse_matching.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/cvpr_ds_config.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/cvpr_ds_config.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/fine_matching.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/fine_matching.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/geometry.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/position_encoding.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/position_encoding.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/supervision.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/supervision.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/losses/loftr_loss.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/losses/loftr_loss.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/__init__.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/augment.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/augment.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/comm.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/comm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataloader.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataset.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/metrics.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/misc.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/plotting.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/src/utils/profiler.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/src/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/test.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/test.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/se2loftr/train.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/se2loftr/train.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/thirdparty/transformations.py` & `deep_image_matching-1.2.4/src/deep_image_matching/thirdparty/transformations.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/triangulation.py` & `deep_image_matching-1.2.4/src/deep_image_matching/triangulation.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/__init__.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/database.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/database.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/geometric_verification.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/geometric_verification.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/hloc_base_model.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/hloc_base_model.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/image.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/image.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/logger.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/sensor_width_database.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/sensor_width_database.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/tiling.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/tiling.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/timer.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/utils/utils.py` & `deep_image_matching-1.2.4/src/deep_image_matching/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching/visualization.py` & `deep_image_matching-1.2.4/src/deep_image_matching/visualization.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching.egg-info/PKG-INFO` & `deep_image_matching-1.2.4/src/deep_image_matching.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_image_matching
-Version: 1.2.2
+Version: 1.2.4
 Summary: Multiview matching with deep-learning and hand-crafted local features for COLMAP and other SfM software.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>, Luca Morelli <lmorelli@fbk.eu>
 License: # LICENSE
         
         BSD 3-Clause License
         
         Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
@@ -62,14 +62,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: packaging
 Requires-Dist: einops
 Requires-Dist: pyvis>=0.3.2
 Requires-Dist: yacs>=0.1.8
 Requires-Dist: e2cnn
 Requires-Dist: pytorch_lightning
+Requires-Dist: pytest
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `deep_image_matching-1.2.2/src/deep_image_matching.egg-info/SOURCES.txt` & `deep_image_matching-1.2.4/src/deep_image_matching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/tests/test_config.py` & `deep_image_matching-1.2.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/tests/test_geom_verification.py` & `deep_image_matching-1.2.4/tests/test_geom_verification.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/tests/test_image.py` & `deep_image_matching-1.2.4/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/tests/test_pipelines.py` & `deep_image_matching-1.2.4/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.2.2/tests/test_tiling.py` & `deep_image_matching-1.2.4/tests/test_tiling.py`

 * *Files identical despite different names*

