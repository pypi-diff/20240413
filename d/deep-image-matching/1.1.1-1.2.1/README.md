# Comparing `tmp/deep_image_matching-1.1.1.tar.gz` & `tmp/deep_image_matching-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_image_matching-1.1.1.tar", last modified: Mon Apr  8 15:02:15 2024, max compression
+gzip compressed data, was "deep_image_matching-1.2.1.tar", last modified: Sat Apr 13 13:30:03 2024, max compression
```

## Comparing `deep_image_matching-1.1.1.tar` & `deep_image_matching-1.2.1.tar`

### file list

```diff
@@ -1,375 +1,375 @@
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.268258 deep_image_matching-1.1.1/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1569 2024-03-29 15:01:50.000000 deep_image_matching-1.1.1/LICENSE
--rw-r--r--   0 francesco  (1000) francesco  (1000)    15575 2024-04-08 15:02:15.268258 deep_image_matching-1.1.1/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11953 2024-03-29 16:05:31.000000 deep_image_matching-1.1.1/README.md
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2480 2024-04-08 15:02:06.000000 deep_image_matching-1.1.1/pyproject.toml
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       38 2024-04-08 15:02:15.268258 deep_image_matching-1.1.1/setup.cfg
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.244258 deep_image_matching-1.1.1/src/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.248258 deep_image_matching-1.1.1/src/deep_image_matching/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      858 2024-04-08 15:02:06.000000 deep_image_matching-1.1.1/src/deep_image_matching/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    24284 2024-03-29 16:41:40.000000 deep_image_matching-1.1.1/src/deep_image_matching/config.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1147 2024-03-30 15:15:46.000000 deep_image_matching-1.1.1/src/deep_image_matching/constants.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.248258 deep_image_matching-1.1.1/src/deep_image_matching/extractors/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      299 2024-03-29 16:07:36.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1420 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/alike.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2552 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/aliked.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1428 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/cosplace.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4215 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/dedode.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1882 2024-03-30 16:02:49.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/disk.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16625 2024-03-29 17:01:08.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/extractor_base.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1725 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/keynetaffnethardnet.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/kornia_features.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5783 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/netvlad.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3253 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/no_extractor.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      734 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/openibl.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2891 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/orb.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2612 2024-03-29 17:07:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/sift.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5514 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/extractors/superpoint.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3990 2024-03-30 15:58:49.000000 deep_image_matching-1.1.1/src/deep_image_matching/graph.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6172 2024-03-29 15:33:36.000000 deep_image_matching-1.1.1/src/deep_image_matching/gui.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    19263 2024-03-30 15:17:00.000000 deep_image_matching-1.1.1/src/deep_image_matching/image_matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1979 2024-03-30 16:01:22.000000 deep_image_matching-1.1.1/src/deep_image_matching/image_retrieval.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.248258 deep_image_matching-1.1.1/src/deep_image_matching/io/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      145 2024-03-29 15:40:29.000000 deep_image_matching-1.1.1/src/deep_image_matching/io/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    22365 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/io/colmap_read_write_model.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3709 2024-03-30 12:26:40.000000 deep_image_matching-1.1.1/src/deep_image_matching/io/h5.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13485 2024-03-29 15:41:40.000000 deep_image_matching-1.1.1/src/deep_image_matching/io/h5_to_db.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    14627 2024-03-30 15:19:47.000000 deep_image_matching-1.1.1/src/deep_image_matching/io/h5_to_micmac.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    15600 2024-03-29 15:41:13.000000 deep_image_matching-1.1.1/src/deep_image_matching/io/h5_to_openmvg.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      534 2024-03-19 12:56:26.000000 deep_image_matching-1.1.1/src/deep_image_matching/io/micmac_to_h5.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8516 2024-03-30 16:03:03.000000 deep_image_matching-1.1.1/src/deep_image_matching/low_resolution.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/matchers/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      335 2024-03-29 16:07:56.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2456 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/adalam.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2346 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/kornia_matcher.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2887 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/lightglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11877 2024-03-29 17:11:24.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/loftr.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    44086 2024-03-30 16:02:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/matcher_base.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    16564 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/roma.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12963 2024-03-29 15:38:55.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/se2loftr.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3131 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/matchers/superglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2182 2024-03-29 15:31:04.000000 deep_image_matching-1.1.1/src/deep_image_matching/openmvg_reconstruction.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12477 2024-03-30 16:03:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/pairs_generator.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5115 2024-03-19 12:56:26.000000 deep_image_matching-1.1.1/src/deep_image_matching/parser.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3314 2024-03-29 15:27:16.000000 deep_image_matching-1.1.1/src/deep_image_matching/reconstruction.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3094 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/count_flops.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/custom_ops/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2173 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/custom_ops/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      280 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/custom_ops/setup.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5265 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/demo_pair.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7678 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/demo_seq.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7008 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/aliked.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9798 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/blocks.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      933 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/padder.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8541 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/soft_detect.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      143 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      211 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5734 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6387 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est_mnn.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2661 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/nll_benchmark.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4774 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/num_inliers.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1965 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/checkpoint.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11631 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/megadepth.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2951 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/decoder.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2529 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/dedode_descriptor.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3523 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/descriptor_loss.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3516 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/dedode_detector.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    10790 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/keypoint_loss.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4027 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/encoder.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2114 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/dual_softmax_matcher.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      127 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7473 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/dedode_models.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2166 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/train.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      213 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13193 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/dinov2.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      414 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2384 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/attention.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9695 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/block.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2099 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/dino_head.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1174 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/drop_path.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      823 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/layer_scale.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1272 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/mlp.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2974 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/patch_embed.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1859 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/swiglu_ffn.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    25761 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/data_prep/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2982 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/data_prep/prep_keypoints.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      768 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_kpts.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2202 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2201 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match_dedode_G.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      899 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_scoremap.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5049 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-B.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5467 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-G.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4466 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_detector.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1360 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-B.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1360 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-G.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      274 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/setup.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.244258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      219 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    25794 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/aliked.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1752 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/disk.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    25452 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/lightglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7985 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/sift.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8369 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/superpoint.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5491 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5885 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/viz2d.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.252258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      183 2024-03-26 11:43:22.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      264 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4114 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/hpatches_sequences_homog_benchmark.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4648 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_dense_benchmark.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5269 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_pose_estimation_benchmark.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5501 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/scannet_benchmark.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       35 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2001 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/checkpoint.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       75 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9290 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/megadepth.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6637 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/scannet.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/losses/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       37 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/losses/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7376 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/losses/robust_loss.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       63 2024-03-26 11:43:17.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4663 2024-03-26 11:43:41.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/encoders.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    32038 2024-03-26 16:39:24.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/matcher.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2753 2024-03-26 16:56:51.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5705 2024-03-26 13:29:26.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/roma_models.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2385 2024-03-26 11:47:39.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12644 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/dinov2.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      414 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2334 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/attention.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9332 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/block.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2010 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/dino_head.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1160 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/drop_path.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      823 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/layer_scale.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1272 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/mlp.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2832 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/patch_embed.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1859 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/swiglu_ffn.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/train/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       34 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/train/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3750 2024-03-26 11:17:57.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/train/train.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      354 2024-03-26 11:43:43.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      266 2024-03-26 11:43:36.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/kde.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2177 2024-03-26 11:42:47.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/local_correlation.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4582 2024-03-26 11:42:46.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/transforms.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20918 2024-03-26 11:42:45.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      199 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/setup.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    11268 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
--rwxrwxr-x   0 francesco  (1000) francesco  (1000)    18884 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3419 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11870 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8657 2024-03-19 12:56:26.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    20646 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-03-19 12:56:26.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/alike/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6314 2024-03-29 15:55:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/alike/alike.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6444 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/alike/alnet.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9185 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/alike/soft_detect.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      160 2024-03-29 15:47:56.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6435 2024-03-29 15:28:35.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/colmap_from_nvm.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    10373 2024-03-30 09:24:12.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extract_features.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.256258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1423 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/cosplace.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1763 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/d2net.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2588 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/dir.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      975 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/disk.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4434 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/dog.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5831 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/netvlad.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      729 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/openibl.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1789 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/r2d2.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1349 2024-03-30 16:07:45.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/superpoint.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5574 2024-03-29 15:28:25.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/localize_inloc.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8467 2024-03-29 15:28:38.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/localize_sfm.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    21799 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/match_dense.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8396 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/match_features.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      120 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2095 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/adalam.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      889 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/lightglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1630 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/loftr.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2208 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/nearest_neighbor.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      685 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/superglue.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2093 2024-03-29 15:28:30.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pairs_from_covisibility.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2154 2024-03-29 15:28:30.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pairs_from_exhaustive.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2236 2024-03-29 15:28:42.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pairs_from_poses.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4600 2024-03-29 15:49:42.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pairs_from_retrieval.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3210 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/localize.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1830 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/prepare_reference.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8210 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5207 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/create_gt_sfm.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4335 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/pipeline.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1119 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2914 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/pipeline.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2697 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2562 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline_loftr.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4251 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/pipeline.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4223 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/pipeline.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4921 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/utils.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5665 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/colmap_from_nvm.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3845 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/pipeline.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5950 2024-03-29 15:28:48.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/reconstruction.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9798 2024-03-30 09:33:10.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/triangulation.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1549 2024-03-29 17:09:20.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/base_model.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    13017 2024-03-29 15:29:01.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/database.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1074 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/geometry.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2254 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/io.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1761 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/parsers.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    22365 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/read_write_model.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4418 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/viz.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5429 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/viz_3d.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5986 2024-01-26 11:18:14.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/visualization.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.248258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.248258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      197 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ds.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      241 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ds_dense.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      193 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ot.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      237 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ot_dense.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      159 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ds.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      203 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ds_dense.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      155 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ot.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      199 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ot_dense.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      723 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      807 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval_new.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      456 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ds.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      499 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ds_dense.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      452 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ot.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      495 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ot_dense.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      418 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      461 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_dense.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      497 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      573 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      577 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_8rot.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      588 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_big.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      414 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ot.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      457 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ot_dense.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/demo/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9954 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/demo/demo_loftr.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        0 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/config/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7360 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/config/default.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5922 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/megadepth.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4293 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/sampler.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4672 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/scannet.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.260258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    15205 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/data.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    12115 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/lightning_loftr.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       71 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      805 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6177 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_e2.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7040 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_fpn.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3771 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       93 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2822 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/fine_preprocess.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2826 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/linear_attention.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3701 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/transformer.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    10541 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/coarse_matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1548 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/cvpr_ds_config.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2901 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/fine_matching.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2250 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/geometry.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1984 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/position_encoding.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5893 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/supervision.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/losses/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9489 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/losses/loftr_loss.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1625 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/__init__.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1762 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/augment.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7820 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/comm.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      873 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataloader.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5695 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataset.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6506 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/metrics.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3510 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/misc.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5710 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/plotting.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1200 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/profiler.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2779 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/test.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     5153 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/train.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    67149 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/transformations.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     8813 2024-03-30 15:36:18.000000 deep_image_matching-1.1.1/src/deep_image_matching/triangulation.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching/utils/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      517 2024-03-30 16:10:27.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/__init__.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    11827 2024-03-30 10:43:37.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/database.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6772 2024-03-30 16:10:17.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/geometric_verification.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1549 2024-03-29 17:09:19.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/hloc_base_model.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    15643 2024-03-30 15:16:36.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/image.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     7411 2024-03-29 15:02:38.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/logger.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2112 2024-03-29 15:24:48.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/sensor_width_database.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     9067 2024-03-19 12:56:26.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/tiling.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4411 2024-03-29 15:35:36.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/timer.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     3434 2024-03-30 15:42:29.000000 deep_image_matching-1.1.1/src/deep_image_matching/utils/utils.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4054 2024-01-26 11:18:15.000000 deep_image_matching-1.1.1/src/deep_image_matching/visualization.py
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/src/deep_image_matching.egg-info/
--rw-r--r--   0 francesco  (1000) francesco  (1000)    15575 2024-04-08 15:02:15.000000 deep_image_matching-1.1.1/src/deep_image_matching.egg-info/PKG-INFO
--rw-rw-r--   0 francesco  (1000) francesco  (1000)    18904 2024-04-08 15:02:15.000000 deep_image_matching-1.1.1/src/deep_image_matching.egg-info/SOURCES.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)        1 2024-04-08 15:02:15.000000 deep_image_matching-1.1.1/src/deep_image_matching.egg-info/dependency_links.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)      330 2024-04-08 15:02:15.000000 deep_image_matching-1.1.1/src/deep_image_matching.egg-info/requires.txt
--rw-rw-r--   0 francesco  (1000) francesco  (1000)       20 2024-04-08 15:02:15.000000 deep_image_matching-1.1.1/src/deep_image_matching.egg-info/top_level.txt
-drwxrwxr-x   0 francesco  (1000) francesco  (1000)        0 2024-04-08 15:02:15.264258 deep_image_matching-1.1.1/tests/
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2908 2024-03-30 16:04:55.000000 deep_image_matching-1.1.1/tests/test_config.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     1392 2024-03-30 16:10:34.000000 deep_image_matching-1.1.1/tests/test_geom_verification.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     2840 2024-03-30 16:05:15.000000 deep_image_matching-1.1.1/tests/test_image.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     6165 2024-03-30 16:05:19.000000 deep_image_matching-1.1.1/tests/test_pipelines.py
--rw-rw-r--   0 francesco  (1000) francesco  (1000)     4849 2024-03-30 16:05:37.000000 deep_image_matching-1.1.1/tests/test_tiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.910811 deep_image_matching-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-13 13:29:58.000000 deep_image_matching-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-13 13:30:03.910811 deep_image_matching-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-04-13 13:29:58.000000 deep_image_matching-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:30:03.910811 deep_image_matching-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.854810 deep_image_matching-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.862810 deep_image_matching-1.2.1/src/deep_image_matching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.866810 deep_image_matching-1.2.1/src/deep_image_matching/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/alike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/aliked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/cosplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/dedode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/extractor_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/keynetaffnethardnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/kornia_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/netvlad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/no_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/openibl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/orb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/sift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/extractors/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19320 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/image_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/image_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.866810 deep_image_matching-1.2.1/src/deep_image_matching/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22365 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/io/colmap_read_write_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/io/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13835 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/io/h5_to_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14627 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/io/h5_to_micmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16504 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/io/h5_to_openmvg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/io/micmac_to_h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/low_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.866810 deep_image_matching-1.2.1/src/deep_image_matching/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/adalam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/kornia_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/lightglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/loftr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45260 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/matcher_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/roma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12963 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/se2loftr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/matchers/superglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/openmvg_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/pairs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.870810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.870810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/count_flops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.870810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/custom_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/custom_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/custom_ops/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/demo_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/demo_seq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.870810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/aliked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/padder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/soft_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.870810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.870810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.870810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est_mnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/nll_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/num_inliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.870810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/megadepth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.874811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/dedode_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/descriptor_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.874811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/dedode_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/keypoint_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.874811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/dual_softmax_matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.874811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/dedode_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.874811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/dinov2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.874811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/dino_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/layer_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/swiglu_ffn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25761 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.874811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/data_prep/
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/data_prep/prep_keypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.874811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match_dedode_G.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_scoremap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.878811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-G.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.878811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-B.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-G.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.854810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.878811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25794 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/aliked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/lightglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/sift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8369 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/viz2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.878811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.878811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.878811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/hpatches_sequences_homog_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_dense_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_pose_estimation_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/scannet_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.878811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.882811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/megadepth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/scannet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.882811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/losses/robust_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.882811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32038 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.882811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/roma_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.882811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/dinov2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.882811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/dino_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/layer_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/patch_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/swiglu_ffn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.882811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/train/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.886811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/local_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20918 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.886811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11268 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18884 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/match_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.886811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11870 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.886811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/alike/
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/alike/alike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/alike/alnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/alike/soft_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.890811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/colmap_from_nvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extract_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.890811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/cosplace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/d2net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/dog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/netvlad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/openibl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/r2d2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/superpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/localize_inloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/localize_sfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21799 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/match_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/match_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.890811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/adalam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/lightglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/loftr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/nearest_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/superglue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pairs_from_covisibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pairs_from_exhaustive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pairs_from_poses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pairs_from_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.890811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.890811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/localize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/prepare_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.894811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/create_gt_sfm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.894811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.894811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline_loftr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.894811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.894811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.894811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/colmap_from_nvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.898811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22365 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/read_write_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/viz_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-13 13:29:59.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.898811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.858810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.858810 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.898811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.898811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ds_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/buggy_pos_enc/loftr_ot_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ds_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/loftr_ot_dense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.898811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval_new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.898811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ds_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/buggy_pos_enc/loftr_ot_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_8rot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_big.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ot_dense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/demo/
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/demo/demo_loftr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/config/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/megadepth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/scannet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12115 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/lightning_loftr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_e2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.902811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/fine_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/linear_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.906811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/coarse_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/cvpr_ds_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/fine_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/supervision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.906811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/losses/loftr_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.906811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.906811 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67149 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.906811 deep_image_matching-1.2.1/src/deep_image_matching/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/geometric_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/hloc_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/sensor_width_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/tiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/src/deep_image_matching/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.910811 deep_image_matching-1.2.1/src/deep_image_matching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-13 13:30:03.000000 deep_image_matching-1.2.1/src/deep_image_matching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-04-13 13:30:03.000000 deep_image_matching-1.2.1/src/deep_image_matching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:30:03.000000 deep_image_matching-1.2.1/src/deep_image_matching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-13 13:30:03.000000 deep_image_matching-1.2.1/src/deep_image_matching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-13 13:30:03.000000 deep_image_matching-1.2.1/src/deep_image_matching.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:30:03.910811 deep_image_matching-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/tests/test_geom_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-13 13:30:00.000000 deep_image_matching-1.2.1/tests/test_tiling.py
```

### Comparing `deep_image_matching-1.1.1/LICENSE` & `deep_image_matching-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/PKG-INFO` & `deep_image_matching-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_image_matching
-Version: 1.1.1
+Version: 1.2.1
 Summary: Multiview matching with deep-learning and hand-crafted local features for COLMAP and other SfM software.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>, Luca Morelli <lmorelli@fbk.eu>
 License: # LICENSE
         
         BSD 3-Clause License
         
         Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
@@ -44,15 +44,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
-Requires-Dist: torch<=2.2.1
+Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 Requires-Dist: opencv-contrib-python
 Requires-Dist: pydegensac
 Requires-Dist: kornia>=0.7.2
 Requires-Dist: h5py
@@ -62,15 +62,14 @@
 Requires-Dist: pyyaml
 Requires-Dist: packaging
 Requires-Dist: einops
 Requires-Dist: pyvis>=0.3.2
 Requires-Dist: yacs>=0.1.8
 Requires-Dist: e2cnn
 Requires-Dist: pytorch_lightning
-Requires-Dist: xformers
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
@@ -159,15 +158,15 @@
 
 ```
 git clone https://github.com/3DOM-FBK/deep-image-matching.git
 cd deep-image-matching
 pip install -e .
 ```
 
-Install pycolmap (optional):
+Install pycolmap (optional, but recommended):
 
 ```
 pip install pycolmap==0.6.1
 ```
 Pycolmap is optional to run reconstruction directly in DIM. If pycolmap is not available, matches will be written both in a h5 and colmap database for later processing with COLMAP GUI or API, or other processing.
 
 For more information, check the [documentation](https://3dom-fbk.github.io/deep-image-matching/installation/).
```

### Comparing `deep_image_matching-1.1.1/README.md` & `deep_image_matching-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 ```
 git clone https://github.com/3DOM-FBK/deep-image-matching.git
 cd deep-image-matching
 pip install -e .
 ```
 
-Install pycolmap (optional):
+Install pycolmap (optional, but recommended):
 
 ```
 pip install pycolmap==0.6.1
 ```
 Pycolmap is optional to run reconstruction directly in DIM. If pycolmap is not available, matches will be written both in a h5 and colmap database for later processing with COLMAP GUI or API, or other processing.
 
 For more information, check the [documentation](https://3dom-fbk.github.io/deep-image-matching/installation/).
```

#### html2text {}

```diff
@@ -53,23 +53,23 @@
 Line Interface (refer to the `Usage Instructions`). For an illustrative
 example, please see `notebooks/sfm_pipeline.ipynb`. ## Local Installation For
 installing deep-image-matching, first create a conda environment: ``` conda
 create -n deep-image-matching python=3.9 conda activate deep-image-matching pip
 install --upgrade pip ``` Clone the repository and install deep-image-matching
 in editable mode: ``` git clone https://github.com/3DOM-FBK/deep-image-
 matching.git cd deep-image-matching pip install -e . ``` Install pycolmap
-(optional): ``` pip install pycolmap==0.6.1 ``` Pycolmap is optional to run
-reconstruction directly in DIM. If pycolmap is not available, matches will be
-written both in a h5 and colmap database for later processing with COLMAP GUI
-or API, or other processing. For more information, check the [documentation]
-(https://3dom-fbk.github.io/deep-image-matching/installation/). ## Docker
-Installation If you prefer using Docker, first, build the image: ``` docker
-build --tag deep-image-matching . ``` Note that the first time you run the
-command, it will take a while to download the base image and install all the
-dependencies. Once the image is built, you can run it with the following
+(optional, but recommended): ``` pip install pycolmap==0.6.1 ``` Pycolmap is
+optional to run reconstruction directly in DIM. If pycolmap is not available,
+matches will be written both in a h5 and colmap database for later processing
+with COLMAP GUI or API, or other processing. For more information, check the
+[documentation](https://3dom-fbk.github.io/deep-image-matching/installation/).
+## Docker Installation If you prefer using Docker, first, build the image: ```
+docker build --tag deep-image-matching . ``` Note that the first time you run
+the command, it will take a while to download the base image and install all
+the dependencies. Once the image is built, you can run it with the following
 commands. On Linux: ``` docker run --name run-deep-image-matching --mount
 type=bind,source=/home/username/data,target=/workspace/data --gpus all -it
 deep-image-matching ``` On Windows (please use Powershell): ``` docker run --
 name run-deep-image-matching --mount type=bind,source=D:\data,target=/
 workspace/data --gpus all -it deep-image-matching ``` **replace** `/home/
 username/data` (on Linux) or `D:\data` (on Winows) with the desired path for
 mounting a shared volume between the local OS and the docker container. Make
```

### Comparing `deep_image_matching-1.1.1/pyproject.toml` & `deep_image_matching-1.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
   requires      = ["setuptools>=65", "wheel"]
   build-backend = "setuptools.build_meta"
 
 [project]
   name = "deep_image_matching"
-  version = "1.1.1"
+  version = "1.2.1"
   description = "Multiview matching with deep-learning and hand-crafted local features for COLMAP and other SfM software."
   readme = "README.md"
   authors = [
       { name = "Francesco Ioli", email = "francesco.ioli@polimi.it" },
       { name = "Luca Morelli", email = "lmorelli@fbk.eu"}
   ]
   license = { file = "LICENSE" }
@@ -19,15 +19,15 @@
   requires-python = ">=3.8"
   keywords = ["image-matching", "deep-learning", "local-features", "multiview-matching", "sfm"]
   
   dependencies = [
     "numpy",
     "scipy",
     "matplotlib",
-    "torch<=2.2.1",
+    "torch",
     "torchvision",
     "pillow",
     "opencv-python",
     "opencv-contrib-python",
     "pydegensac",
     "kornia>=0.7.2",
     "h5py",
@@ -37,16 +37,15 @@
     "pyyaml",
     "packaging",
     "einops",
     "pyvis>=0.3.2",
     "yacs>=0.1.8",
     "e2cnn",
     "pytorch_lightning",
-    "xformers",
-  ]
+]
 
   [project.optional-dependencies]
     dev = [
       "flake8", 
       "black", 
       "bumpver", 
       "isort", 
@@ -65,15 +64,15 @@
 
 [tool.pytest.ini_options]
   addopts = [
       "--import-mode=importlib",
   ]
     
 [tool.bumpver]
-  current_version = "1.1.1"
+  current_version = "1.2.1"
   version_pattern = "MAJOR.MINOR.PATCH"
   commit_message = "bump version {old_version} -> {new_version}"
   commit = true
   tag = false
   push = false
 
   [tool.bumpver.file_patterns]
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/config.py` & `deep_image_matching-1.2.1/src/deep_image_matching/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,22 +39,24 @@
     "tile_preselection_size": 1000,
     # Minimum number of matches per tile
     "min_matches_per_tile": 10,
     # Geometric verification method and parameters:
     #   GeometricVerification.NONE (no geometric verification),
     #   GeometricVerification.PYDEGENSAC (use pydegensac),
     #   GeometricVerification.MAGSAC (use opencv MAGSAC),
+    #   Other methods: RANSAC, LMEDS, RHO, USAC_DEFAULT, USAC_PARALLEL, USAC_FM_8PTS, USAC_FAST, USAC_ACCURATE, USAC_PROSAC, USAC_MAGSAC
     "geom_verification": GeometricVerification.PYDEGENSAC,
     "gv_threshold": 4,
     "gv_confidence": 0.99999,
     # Minimum number of inliers matches and minumum inlier ratio per pair
     "min_inliers_per_pair": 15,
     "min_inlier_ratio_per_pair": 0.25,
     # Even if the features are extracted by tiles, you can try to match the features of the entire image first (if the number of features is not too high and they can fit into memory). Default is False.
     "try_match_full_images": False,
+    "preselection_pipeline": "superpoint+lightglue",
 }
 
 
 # The configuration for DeepImageMatcher is defined as a dictionary with the following keys:
 # - 'extractor': extractor configuration
 # - 'matcher': matcher configuration
 # The 'extractor' and 'matcher' values must contain a 'name' key with the name of the extractor/matcher to be used. Additionally, the other parameters of the extractor/matcher can be specified.
@@ -253,14 +255,16 @@
         "global_feature": None,
         "db_path": None,
         "upright": False,
         "skip_reconstruction": False,
         "force": True,
         "verbose": False,
         "graph": True,
+        "openmvg": None,
+        "camera_options": None,
     }
     _cfg = {
         "general": {},
         "extractor": {},
         "matcher": {},
     }
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/alike.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/alike.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/aliked.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/aliked.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/cosplace.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/cosplace.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/dedode.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/dedode.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/disk.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/disk.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/extractor_base.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/extractor_base.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/keynetaffnethardnet.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/keynetaffnethardnet.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/netvlad.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/netvlad.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/no_extractor.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/no_extractor.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/openibl.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/openibl.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/orb.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/orb.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/sift.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/sift.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/extractors/superpoint.py` & `deep_image_matching-1.2.1/src/deep_image_matching/extractors/superpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/graph.py` & `deep_image_matching-1.2.1/src/deep_image_matching/graph.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/gui.py` & `deep_image_matching-1.2.1/src/deep_image_matching/gui.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/image_matching.py` & `deep_image_matching-1.2.1/src/deep_image_matching/image_matching.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         "tile_size": [2048, 1365],
         "tile_overlap": 0,
         "force_cpu": False,
         "do_viz": False,
         "fast_viz": True,
         "hide_matching_track": True,
         "do_viz_tiles": False,
+        "preselection_pipeline": "superpoint+lightglue",
     }
 
     def __init__(
         self,
         config: Config,
         # imgs_dir: Path,
         # output_dir: Path,
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/image_retrieval.py` & `deep_image_matching-1.2.1/src/deep_image_matching/image_retrieval.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import os
 import shutil
 
 from .thirdparty.hloc import extract_features, pairs_from_retrieval
 
 
 def ImageRetrieval(imgs_dir, outs_dir, retrieval_option, sfm_pairs):
+    max_track_length = 10  # Increase this number to increase the number of pairs
     if outs_dir.exists():
         shutil.rmtree(outs_dir)
         os.mkdir(outs_dir)
     else:
         os.mkdir(outs_dir)
 
     number_imgs = len(os.listdir(imgs_dir))
     retrieval_conf = extract_features.confs[retrieval_option]
     retrieval_path = extract_features.main(retrieval_conf, imgs_dir, outs_dir)
 
     try:
-        pairs_from_retrieval.main(retrieval_path, sfm_pairs, num_matched=number_imgs)
+        pairs_from_retrieval.main(
+            retrieval_path, sfm_pairs, num_matched=max_track_length
+        )
     except Exception as e:
         print("retrieval_path", retrieval_path)
         print("sfm_pairs", sfm_pairs)
         print("number_imgs", number_imgs)
         print(f"Error: {e}")
         quit()
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/io/colmap_read_write_model.py` & `deep_image_matching-1.2.1/src/deep_image_matching/io/colmap_read_write_model.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/io/h5.py` & `deep_image_matching-1.2.1/src/deep_image_matching/io/h5.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/io/h5_to_db.py` & `deep_image_matching-1.2.1/src/deep_image_matching/io/h5_to_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,45 +20,46 @@
 import logging
 import os
 import warnings
 from pathlib import Path
 
 import h5py
 import numpy as np
+import yaml
 from PIL import ExifTags, Image
 from tqdm import tqdm
 
 from ..utils.database import COLMAPDatabase, image_ids_to_pair_id
 
 logger = logging.getLogger("dim")
 
-default_camera_options = {
+DEFAULT_CAM_OPTIONS = {
     "general": {
         "single_camera": False,
         "camera_model": "simple-radial",
     },
 }
 
 
 def export_to_colmap(
     img_dir: Path,
     feature_path: Path,
     match_path: Path,
     database_path: str = "database.db",
-    camera_options: dict = default_camera_options,
+    camera_config_path: Path = None,
 ):
     """
     Exports image features and matches to a COLMAP database.
 
     Args:
         img_dir (str): Path to the directory containing the source images.
         feature_path (Path): Path to the feature file (in HDF5 format) containing the extracted keypoints.
         match_path (Path): Path to the match file (in HDF5 format) containing the matches between keypoints.
         database_path (str, optional): Path to the COLMAP database file. Defaults to "colmap.db".
-        camera_options (dict, optional): Flag indicating whether to use camera options. Defaults to default_camera_options.
+        camera_config_path (Path, optional): Path to the camera options yaml file. If none is passesed, the default camera configuration is used.
 
     Returns:
         None
 
     Raises:
         IOError: If the image path is invalid.
 
@@ -75,14 +76,22 @@
         )
     """
     database_path = Path(database_path)
     if database_path.exists():
         logger.warning(f"Database path {database_path} already exists - deleting it")
         database_path.unlink()
 
+    # If a config file is provided, read camera options, otherwise use defaults
+    if camera_config_path is not None:
+        with open(camera_config_path, "r") as file:
+            camera_options = yaml.safe_load(file)
+    else:
+        camera_options = DEFAULT_CAM_OPTIONS
+
+    # Create the database and add keypoints and matches
     db = COLMAPDatabase.connect(database_path)
     db.create_tables()
     fname_to_id = add_keypoints(db, feature_path, img_dir, camera_options)
     raw_match_path = match_path.parent / "raw_matches.h5"
     if raw_match_path.exists():
         add_raw_matches(
             db,
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/io/h5_to_micmac.py` & `deep_image_matching-1.2.1/src/deep_image_matching/io/h5_to_micmac.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/io/h5_to_openmvg.py` & `deep_image_matching-1.2.1/src/deep_image_matching/io/h5_to_openmvg.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,34 @@
 import threading
 import urllib.request
 import warnings
 from pathlib import Path
 
 import h5py
 import numpy as np
+import yaml
 from PIL import Image
 from tqdm import tqdm
 
 from deep_image_matching.io.h5_to_db import get_focal
 
 logger = logging.getLogger("dim")
 
 __OPENMVG_DIST_NAME_MAP = {
     "pinhole_radial_k3": "disto_k3",
     "pinhole_brown_t2": "disto_t2",
 }
 
+DEFAULT_CAM_OPTIONS = {
+    "general": {
+        "single_camera": False,
+        "openmvg_camera_model": "pinhole_radial_k3",
+    },
+}
+
 
 def loadJSON(sfm_data):
     with open(sfm_data) as file:
         sfm_data = json.load(file)
     view_ids = {view["value"]["ptr_wrapper"]["data"]["filename"]: view["key"] for view in sfm_data["views"]}
     image_paths = [
         os.path.join(sfm_data["root_path"], view["value"]["ptr_wrapper"]["data"]["filename"])
@@ -327,41 +335,57 @@
 
 
 def export_to_openmvg(
     img_dir,
     feature_path: Path,
     match_path: Path,
     openmvg_out_path: Path,
-    camera_options: dict,
+    camera_config_path: Path,
     openmvg_sfm_bin: Path = None,
     openmvg_database: Path = None,
 ) -> None:
     """
     Exports image features, matches, and camera data to an OpenMVG project.
 
     This function prepares the necessary files and directories for running OpenMVG's SfM pipeline.
 
     Args:
         img_dir (Path): Path to the directory containing source images.
         feature_path (Path): Path to the feature file (HDF5 format).
         match_path (Path): Path to the match file (HDF5 format).
         openmvg_out_path (Path): Path to the desired output directory for the OpenMVG project.
-        camera_options (dict): Camera configuration options.
+        camera_config_path (Path): Path to the camera options yaml file.
         openmvg_sfm_bin (Path, optional): Path to the OpenMVG SfM executable. If not provided,
                                           attempts to find it automatically (Linux only).
         openmvg_database (Path, optional): Path to the OpenMVG sensor width database.
                                            If not provided, downloads it to the output directory.
 
     """
     openmvg_out_path = Path(openmvg_out_path)
     if openmvg_out_path.exists():
         logger.warning(f"OpenMVG output folder {openmvg_out_path} already exists - deleting it")
         os.rmdir(openmvg_out_path)
     openmvg_out_path.mkdir(parents=True)
 
+    if not img_dir.exists():
+        raise FileNotFoundError(f"Image directory {img_dir} does not exist.")
+    if not feature_path.exists():
+        raise FileNotFoundError(f"Feature file {feature_path} does not exist.")
+    if not match_path.exists():
+        raise FileNotFoundError(f"Match file {match_path} does not exist.")
+    if not camera_config_path.exists():
+        raise FileNotFoundError(f"Camera options file {camera_config_path} does not exist.")
+
+    # If a config file is provided, read camera options, otherwise use defaults
+    if camera_config_path is not None:
+        with open(camera_config_path, "r") as file:
+            camera_options = yaml.safe_load(file)
+    else:
+        camera_options = DEFAULT_CAM_OPTIONS
+
     # NOTE: this part meybe is not needed here...
     if openmvg_sfm_bin is None:
         # Try to find openMVG binaries (only on linux)
         if sys.platform == "linux":
             openmvg_sfm_bin = shutil.which("openMVG_main_SfM")
         else:
             raise FileNotFoundError(
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/io/micmac_to_h5.py` & `deep_image_matching-1.2.1/src/deep_image_matching/io/micmac_to_h5.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/low_resolution.py` & `deep_image_matching-1.2.1/src/deep_image_matching/low_resolution.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/matchers/adalam.py` & `deep_image_matching-1.2.1/src/deep_image_matching/matchers/adalam.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/matchers/kornia_matcher.py` & `deep_image_matching-1.2.1/src/deep_image_matching/matchers/kornia_matcher.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/matchers/lightglue.py` & `deep_image_matching-1.2.1/src/deep_image_matching/matchers/lightglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/matchers/loftr.py` & `deep_image_matching-1.2.1/src/deep_image_matching/matchers/loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/matchers/matcher_base.py` & `deep_image_matching-1.2.1/src/deep_image_matching/matchers/matcher_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,21 +368,23 @@
 
         # Select tile pairs to match
         tile_pairs = tile_selection(
             img0,
             img1,
             method=method,
             quality=self.config["general"]["quality"],
-            preselction_extractor=self._preselction_extractor,
-            preselction_matcher=self._preselction_matcher,
             tile_size=self.config["general"]["tile_size"],
             tile_overlap=self.config["general"]["tile_overlap"],
+            preselction_extractor=self._preselction_extractor,
+            preselction_matcher=self._preselction_matcher,
+            pipeline=self.config["general"]["preselection_pipeline"],
             tile_preselection_size=self.tile_preselection_size,
             min_matches_per_tile=self.min_matches_per_tile,
             device=self._device,
+            debug_dir=self.config["general"]["output_dir"] / "debug" if self.config["general"]["do_viz"] else None,
         )
         timer.update("tile selection")
 
         # If no tile pairs are selected, return an empty array
         if len(tile_pairs) == 0:
             logger.debug("No tile pairs selected.")
             return matches_full
@@ -920,35 +922,39 @@
 
 
 def tile_selection(
     img0: Path,
     img1: Path,
     method: TileSelection,
     quality: Quality,
-    preselction_extractor: ExtractorBase,
-    preselction_matcher: MatcherBase,
     tile_size: Tuple[int, int],
     tile_overlap: int,
+    preselction_extractor: ExtractorBase = None,
+    preselction_matcher: MatcherBase = None,
+    pipeline: str = "superpoint+lightglue",
     tile_preselection_size: int = 1024,
     min_matches_per_tile: int = 5,
-    do_geometric_verification: bool = True,
-    device: str = "cpu",
+    do_geometric_verification: bool = False,
+    device: str = "cuda",
+    debug_dir: Path = None,
 ):
     """
     Selects tile pairs for matching based on the specified method.
 
     Args:
         img0 (Path): Path to the first image.
         img1 (Path): Path to the second image.
         method (TileSelection, optional): Tile selection method. Defaults to TileSelection.PRESELECTION.
 
     Returns:
         List[Tuple[int, int]]: The selected tile pairs.
     """
 
+    timer = Timer(log_level="debug")
+
     # Compute tiles limits and origin
     tiler = Tiler(tiling_mode="size")
     i0 = cv2.imread(str(img0), cv2.IMREAD_GRAYSCALE).astype(np.float32)
     i1 = cv2.imread(str(img1), cv2.IMREAD_GRAYSCALE).astype(np.float32)
 
     # Resize images to the specified quality to reproduce the same tiling as in feature extraction
     if quality != Quality.HIGH:
@@ -974,64 +980,78 @@
         # Match tiles by regular grid
         logger.debug("Matching tiles by regular grid")
         tile_pairs = sorted(zip(tiles0.keys(), tiles1.keys()))
     elif method == TileSelection.PRESELECTION:
         # Match tiles by preselection running matching on downsampled images
         logger.debug("Matching tiles by downsampling preselection")
 
-        # match downsampled images with roma
-        from ..thirdparty.RoMa.roma import roma_outdoor
+        if pipeline == "superpoint+lightglue":
+            if not preselction_extractor or not preselction_matcher:
+                raise ValueError(
+                    "Preselection extractor and matcher must be provided for superpoint+lightglue pipeline"
+                )
 
-        n_matches = 5000
-        matcher = roma_outdoor(device, coarse_res=448)
-        H_A, W_A = i0_new_size
-        H_B, W_B = i1_new_size
-        warp, certainty = matcher.match(str(img0), str(img1), device=device)
-        matches, certainty = matcher.sample(warp, certainty, num=n_matches)
-        kp0, kp1 = matcher.to_pixel_coordinates(matches, H_A, W_A, H_B, W_B)
-        kp0, kp1 = kp0.cpu().numpy(), kp1.cpu().numpy()
-
-        # # Downsampled images
-        # size0 = i0.shape[:2][::-1]
-        # size1 = i1.shape[:2][::-1]
-        # scale0 = tile_preselection_size / max(size0)
-        # scale1 = tile_preselection_size / max(size1)
-        # size0_new = tuple(int(round(x * scale0)) for x in size0)
-        # size1_new = tuple(int(round(x * scale1)) for x in size1)
-        # i0 = cv2.resize(i0, size0_new, interpolation=cv2.INTER_AREA)
-        # i1 = cv2.resize(i1, size1_new, interpolation=cv2.INTER_AREA)
-
-        # # Run SuperPoint on downsampled images
-        # with torch.inference_mode():
-        #     feats0 = preselction_extractor({"image": frame2tensor(i0, device)})
-        #     feats1 = preselction_extractor({"image": frame2tensor(i1, device)})
-
-        #     # Match features with LightGlue
-        #     feats0 = sp2lg(feats0)
-        #     feats1 = sp2lg(feats1)
-        #     res = preselction_matcher({"image0": feats0, "image1": feats1})
-        #     res = rbd2np(res)
-
-        # # Get keypoints in original image
-        # kp0 = feats0["keypoints"].cpu().numpy()[0]
-        # kp0 = kp0[res["matches"][:, 0], :]
-        # kp1 = feats1["keypoints"].cpu().numpy()[0]
-        # kp1 = kp1[res["matches"][:, 1], :]
-
-        # # Scale up keypoints
-        # kp0 = kp0 / scale0
-        # kp1 = kp1 / scale1
+            # Downsampled images
+            size0 = i0.shape[:2][::-1]
+            size1 = i1.shape[:2][::-1]
+            scale0 = tile_preselection_size / max(size0)
+            scale1 = tile_preselection_size / max(size1)
+            size0_new = tuple(int(round(x * scale0)) for x in size0)
+            size1_new = tuple(int(round(x * scale1)) for x in size1)
+            i0 = cv2.resize(i0, size0_new, interpolation=cv2.INTER_AREA)
+            i1 = cv2.resize(i1, size1_new, interpolation=cv2.INTER_AREA)
+
+            # Run SuperPoint on downsampled images
+            with torch.inference_mode():
+                feats0 = preselction_extractor({"image": frame2tensor(i0, device)})
+                feats1 = preselction_extractor({"image": frame2tensor(i1, device)})
+
+                # Match features with LightGlue
+                feats0 = sp2lg(feats0)
+                feats1 = sp2lg(feats1)
+                res = preselction_matcher({"image0": feats0, "image1": feats1})
+                res = rbd2np(res)
+
+            # Get keypoints in original image
+            kp0 = feats0["keypoints"].cpu().numpy()[0]
+            kp0 = kp0[res["matches"][:, 0], :]
+            kp1 = feats1["keypoints"].cpu().numpy()[0]
+            kp1 = kp1[res["matches"][:, 1], :]
+
+            # Scale up keypoints
+            kp0 = kp0 / scale0
+            kp1 = kp1 / scale1
+
+        elif pipeline == "roma":
+            # match downsampled images with roma
+            from ..thirdparty.RoMa.roma import roma_outdoor
+
+            n_matches = 5000
+            coarse_res = 420
+            upsample_res = 560
+            matcher = roma_outdoor(device, coarse_res=coarse_res, upsample_res=upsample_res)
+            H_A, W_A = i0_new_size
+            H_B, W_B = i1_new_size
+            warp, certainty = matcher.match(str(img0), str(img1), device=device)
+            matches, certainty = matcher.sample(warp, certainty, num=n_matches)
+            kp0, kp1 = matcher.to_pixel_coordinates(matches, H_A, W_A, H_B, W_B)
+            kp0, kp1 = kp0.cpu().numpy(), kp1.cpu().numpy()
+
+        else:
+            raise ValueError(
+                f"Invalid tile selection method: {method}. Only superpoint+lightglue and roma are supported so far"
+            )
 
         # geometric verification
         if do_geometric_verification:
             _, inlMask = geometric_verification(
                 kpts0=kp0,
                 kpts1=kp1,
-                threshold=5,
-                confidence=0.9999,
+                threshold=10,
+                confidence=0.99999,
                 quiet=True,
             )
             kp0 = kp0[inlMask]
             kp1 = kp1[inlMask]
 
         # Select tile pairs where there are enough matches
         tile_pairs = set()
@@ -1040,42 +1060,46 @@
             ret0 = points_in_rect(kp0, get_tile_bounding_box(t_orig0[tidx0], tile_size))
             ret1 = points_in_rect(kp1, get_tile_bounding_box(t_orig1[tidx1], tile_size))
             n_matches = sum(ret0 & ret1)
             if n_matches > min_matches_per_tile:
                 tile_pairs.add((tidx0, tidx1))
         tile_pairs = sorted(tile_pairs)
 
+        timer.update("preselection")
+
         # For Debugging...
-        # if False:
-        from matplotlib import pyplot as plt
+        if debug_dir:
+            from matplotlib import pyplot as plt
+
+            out_dir = Path(debug_dir) / "preselection"
+            out_dir.mkdir(parents=True, exist_ok=True)
+            image0 = cv2.imread(str(img0), cv2.IMREAD_GRAYSCALE)
+            image1 = cv2.imread(str(img1), cv2.IMREAD_GRAYSCALE)
+            image0 = resize_image(image0, (i0_new_size[1], i0_new_size[0]))
+            image1 = resize_image(image1, (i1_new_size[1], i1_new_size[0]))
+            c = "r"
+            s = 2
+            fig, axes = plt.subplots(1, 2)
+            for ax, img, kp in zip(axes, [image0, image1], [kp0, kp1]):
+                ax.imshow(cv2.cvtColor(img, cv2.COLOR_BAYER_BG2BGR))
+                ax.scatter(kp[:, 0], kp[:, 1], s=s, c=c)
+                ax.axis("off")
+                ax.set_aspect("equal")
+            for lim0, lim1 in zip(t_orig0.values(), t_orig0.values()):
+                axes[0].axvline(lim0[0])
+                axes[0].axhline(lim0[1])
+                axes[1].axvline(lim1[0])
+                axes[1].axhline(lim1[1])
+            axes[1].get_yaxis().set_visible(False)
+            fig.tight_layout()
+            fig.savefig(out_dir / f"{img0.name}-{img1.name}.jpg")
+            plt.close()
 
-        out_dir = Path("sandbox/preselection")
-        out_dir.mkdir(parents=True, exist_ok=True)
-        image0 = cv2.imread(str(img0), cv2.IMREAD_GRAYSCALE)
-        image1 = cv2.imread(str(img1), cv2.IMREAD_GRAYSCALE)
-        image0 = resize_image(image0, (i0_new_size[1], i0_new_size[0]))
-        image1 = resize_image(image1, (i1_new_size[1], i1_new_size[0]))
-        c = "r"
-        s = 5
-        fig, axes = plt.subplots(1, 2)
-        for ax, img, kp in zip(axes, [image0, image1], [kp0, kp1]):
-            ax.imshow(cv2.cvtColor(img, cv2.COLOR_BAYER_BG2BGR))
-            ax.scatter(kp[:, 0], kp[:, 1], s=s, c=c)
-            ax.axis("off")
-            ax.set_aspect("equal")
-        for lim0, lim1 in zip(t_orig0.values(), t_orig0.values()):
-            axes[0].axvline(lim0[0])
-            axes[0].axhline(lim0[1])
-            axes[1].axvline(lim1[0])
-            axes[1].axhline(lim1[1])
-        axes[1].get_yaxis().set_visible(False)
-        fig.tight_layout()
-        # plt.show()
-        fig.savefig(out_dir / f"{img0.name}-{img1.name}.jpg")
-        plt.close()
+    timer.update("Tile selection")
+    timer.print("Tile selection")
 
     return tile_pairs
 
 
 def load_image_np(img_path: Path, as_float: bool = True, grayscale: bool = False):
     image = cv2.imread(str(img_path))
     if as_float:
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/matchers/roma.py` & `deep_image_matching-1.2.1/src/deep_image_matching/matchers/roma.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,46 +38,45 @@
         "coarse_res": 560,  # (h,w) or only one value for square images
         "upsample_res": 864,  # (h,w) or only one value for square images
         "num_sampled_points": 10000,  # number of points to sample for each image (or for each tile if tile_preselection_size is set)
     }
 
     grayscale = False
     as_float = True
-    max_tile_pairs = 150  # Maximum number of tile pairs to match, raise an error if more than this number to avoid slow and likely inaccurate matching
-    # max_matches_per_pair = 10000
+    max_tile_pairs = 250  # Maximum number of tile pairs to match, raise an error if more than this number to avoid slow and likely inaccurate matching
     min_matches_per_tile = 3
-    max_matches_per_tile = 5000
+    max_matches_per_tile = 10000
     keep_tiles = True  # False
 
     def __init__(self, config={}) -> None:
         super().__init__(config)
 
         # Set up RoMa matcher
         if self.config["general"]["tile_selection"] == TileSelection.NONE:
             logger.info(
-                f"RoMa always use a coarse resolution of {self.config['matcher']['coarse_res']} pixels, regardless of the quality parameter resolution."
+                f"RoMa always use a coarse resolution of {self.config['matcher']['upsample_res']} pixels, regardless of the quality parameter resolution."
             )
         else:
             logger.info("Running RoMa by tile..")
             logger.info(
-                f"RoMa uses a fixed tile size of {self.config['matcher']['coarse_res']} pixels. This can result in a large number of tiles for high-resolution images. If the number of tiles is too high, consider reducing the image resolution via the 'Quality' parameter."
+                f"RoMa uses a fixed tile size of {self.config['matcher']['upsample_res']} pixels. This can result in a large number of tiles for high-resolution images. If the number of tiles is too high, consider reducing the image resolution via the 'Quality' parameter."
             )
 
-        if isinstance(self.config["matcher"]["coarse_res"], tuple):
+        if isinstance(self.config["matcher"]["upsample_res"], tuple):
             tile_size = (
-                self.config["matcher"]["coarse_res"][1],
-                self.config["matcher"]["coarse_res"][0],
+                self.config["matcher"]["upsample_res"][1],
+                self.config["matcher"]["upsample_res"][0],
             )
-        elif isinstance(self.config["matcher"]["coarse_res"], int):
+        elif isinstance(self.config["matcher"]["upsample_res"], int):
             tile_size = (
-                self.config["matcher"]["coarse_res"],
-                self.config["matcher"]["coarse_res"],
+                self.config["matcher"]["upsample_res"],
+                self.config["matcher"]["upsample_res"],
             )
         else:
-            raise ValueError("Invalid type for 'coarse_res'. It should be an integer or a tuple of two integers.")
+            raise ValueError("Invalid type for 'upsample_res'. It should be an integer or a tuple of two integers.")
         # Force the tile size to be the same as the RoMa coarse_res
         self.config["general"]["tile_size"] = tile_size
 
         self.matcher = roma_outdoor(
             device=self._device,
             coarse_res=self.config["matcher"]["coarse_res"],
             upsample_res=self.config["matcher"]["upsample_res"],
@@ -254,25 +253,28 @@
 
         # Select tile pairs to match
         tile_pairs = tile_selection(
             img0,
             img1,
             method=method,
             quality=self._quality,
-            preselction_extractor=self._preselction_extractor,
-            preselction_matcher=self._preselction_matcher,
             tile_size=tile_size,
             tile_overlap=overlap,
+            preselction_extractor=self._preselction_extractor,
+            preselction_matcher=self._preselction_matcher,
+            pipeline=self.config["general"]["preselection_pipeline"],
             tile_preselection_size=self.tile_preselection_size,
             min_matches_per_tile=self.min_matches_per_tile,
             device=self._device,
+            debug_dir=self.config["general"]["output_dir"] / "debug" if self.config["general"]["verbose"] else None,
         )
+
         if len(tile_pairs) > self.max_tile_pairs:
             raise RuntimeError(
-                f"Too many tile pairs ({len(tile_pairs)}) to match, the matching process will be too slow and it may be inaccurate. Try to reduce the image resolution using a lower 'Quality' value (or change the 'max_tile_pairs' class attribute, if you know what you are doing)."
+                f"Too many tile pairs ({len(tile_pairs)}) to match, the matching process will be too slow and it may be inaccurate. Try to reduce the image resolution using a lower 'Quality' parameter."
             )
         else:
             logger.info(f"Matching {len(tile_pairs)} tile pairs")
         timer.update("tile selection")
 
         # Read images and resize them if needed
         image0 = cv2.imread(str(img0))
@@ -294,15 +296,15 @@
         logger.debug(f"Tiles saved to {tiles_dir}")
 
         # Match each tile pair
         mkpts0_full = np.array([], dtype=np.float32).reshape(0, 2)
         mkpts1_full = np.array([], dtype=np.float32).reshape(0, 2)
         conf_full = np.array([], dtype=np.float32)
 
-        for tidx0, tidx1 in tqdm(tile_pairs, leave=False, desc="Matching tiles"):
+        for tidx0, tidx1 in tqdm(tile_pairs, leave=True, desc="Matching tiles"):
             logger.debug(f"  - Matching tile pair ({tidx0}, {tidx1})")
 
             tile_path0 = tiles_dir / img0.name / f"tile_{tidx0}.png"
             tile_path1 = tiles_dir / img1.name / f"tile_{tidx1}.png"
 
             W_A, H_A = tiles0[tidx0].shape[1], tiles0[tidx0].shape[0]
             W_B, H_B = tiles1[tidx1].shape[1], tiles1[tidx1].shape[0]
@@ -360,25 +362,29 @@
                 return (
                     (kp[:, 0] >= border_thr)
                     & (kp[:, 0] < img_size[1] - border_thr)
                     & (kp[:, 1] >= border_thr)
                     & (kp[:, 1] < img_size[0] - border_thr)
                 )
 
-            maskA = kps_in_image(kptsA, image0.shape[:2])
-            maskB = kps_in_image(kptsB, image1.shape[:2])
+            border_thr = 50
+            maskA = kps_in_image(kptsA, image0.shape[:2], border_thr)
+            maskB = kps_in_image(kptsB, image1.shape[:2], border_thr)
             msk = maskA & maskB
             kptsA = kptsA[msk]
             kptsB = kptsB[msk]
 
             # Append to full arrays
             mkpts0_full = np.vstack((mkpts0_full, kptsA))
             mkpts1_full = np.vstack((mkpts1_full, kptsB))
             conf_full = np.concatenate((conf_full, conf))
 
+        logger.info("Tiles completed")
+        logger.info(f"Total matches before geometric verification: {len(mkpts0_full)}")
+
         # Rescale keypoints to original image size
         mkpts0_full = self._resize_keypoints(self._quality, mkpts0_full)
         mkpts1_full = self._resize_keypoints(self._quality, mkpts1_full)
 
         # Select uniue features on image 0, on rounded coordinates
         if select_unique is True:
             decimals = 1
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/matchers/se2loftr.py` & `deep_image_matching-1.2.1/src/deep_image_matching/matchers/se2loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/matchers/superglue.py` & `deep_image_matching-1.2.1/src/deep_image_matching/matchers/superglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/openmvg_reconstruction.py` & `deep_image_matching-1.2.1/src/deep_image_matching/openmvg_reconstruction.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/pairs_generator.py` & `deep_image_matching-1.2.1/src/deep_image_matching/pairs_generator.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/parser.py` & `deep_image_matching-1.2.1/src/deep_image_matching/parser.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/reconstruction.py` & `deep_image_matching-1.2.1/src/deep_image_matching/reconstruction.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/count_flops.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/count_flops.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/custom_ops/__init__.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/custom_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/demo_pair.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/demo_pair.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/demo_seq.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/demo_seq.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/aliked.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/aliked.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/blocks.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/blocks.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/padder.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/padder.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/ALIKED/nets/soft_detect.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/ALIKED/nets/soft_detect.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est_mnn.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/mega_pose_est_mnn.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/nll_benchmark.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/nll_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/num_inliers.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/benchmarks/num_inliers.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/checkpoint.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/megadepth.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/datasets/megadepth.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/decoder.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/decoder.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/dedode_descriptor.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/dedode_descriptor.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/descriptor_loss.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/descriptors/descriptor_loss.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/dedode_detector.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/dedode_detector.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/keypoint_loss.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/detectors/keypoint_loss.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/encoder.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/encoder.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/dual_softmax_matcher.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/matchers/dual_softmax_matcher.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/dedode_models.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/model_zoo/dedode_models.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/train.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/train.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/dinov2.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/dinov2.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/attention.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/attention.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/block.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/block.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/dino_head.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/dino_head.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/drop_path.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/layer_scale.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/layer_scale.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/mlp.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/patch_embed.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/swiglu_ffn.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/transformer/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/utils.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/DeDoDe/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/data_prep/prep_keypoints.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/data_prep/prep_keypoints.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_kpts.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_kpts.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match_dedode_G.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_match_dedode_G.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_scoremap.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/demo/demo_scoremap.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-B.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-B.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-G.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_descriptor-G.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_detector.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/dedode_detector.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-B.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-B.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-G.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/DeDoDe/experiments/eval/eval_dedode_descriptor-G.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/aliked.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/aliked.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/disk.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/disk.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/lightglue.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/lightglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/sift.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/sift.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/superpoint.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/superpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/utils.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/viz2d.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/LightGlue/lightglue/viz2d.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/hpatches_sequences_homog_benchmark.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/hpatches_sequences_homog_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_dense_benchmark.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_dense_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_pose_estimation_benchmark.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/megadepth_pose_estimation_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/scannet_benchmark.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/benchmarks/scannet_benchmark.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/checkpoint.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/checkpointing/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/megadepth.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/megadepth.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/scannet.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/datasets/scannet.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/losses/robust_loss.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/losses/robust_loss.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/encoders.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/encoders.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/matcher.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/matcher.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/__init__.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/roma_models.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/model_zoo/roma_models.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/__init__.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/dinov2.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/dinov2.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/attention.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/attention.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/block.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/block.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/dino_head.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/dino_head.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/drop_path.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/layer_scale.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/layer_scale.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/mlp.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/patch_embed.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/patch_embed.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/swiglu_ffn.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/models/transformer/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/train/train.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/train/train.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/local_correlation.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/local_correlation.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/transforms.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/utils.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/RoMa/roma/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/demo_superglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/match_pairs.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/match_pairs.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/matching.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/matching.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superglue.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/utils.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/SuperGluePretrainedNetwork/models/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/alike/alike.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/alike/alike.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/alike/alnet.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/alike/alnet.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/alike/soft_detect.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/alike/soft_detect.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/colmap_from_nvm.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/colmap_from_nvm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extract_features.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extract_features.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/cosplace.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/cosplace.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/d2net.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/d2net.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/dir.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/dir.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/disk.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/disk.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/dog.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/dog.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/netvlad.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/netvlad.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/openibl.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/openibl.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/r2d2.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/r2d2.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/extractors/superpoint.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/extractors/superpoint.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/localize_inloc.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/localize_inloc.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/localize_sfm.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/localize_sfm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/match_dense.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/match_dense.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/match_features.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/match_features.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/adalam.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/adalam.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/lightglue.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/lightglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/loftr.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/nearest_neighbor.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/matchers/superglue.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/matchers/superglue.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pairs_from_covisibility.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pairs_from_covisibility.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pairs_from_exhaustive.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pairs_from_exhaustive.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pairs_from_poses.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pairs_from_poses.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pairs_from_retrieval.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pairs_from_retrieval.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/localize.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/localize.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/prepare_reference.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/prepare_reference.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/utils.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/4Seasons/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/create_gt_sfm.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/create_gt_sfm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/pipeline.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/utils.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/7Scenes/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/pipeline.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline_loftr.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Aachen_v1_1/pipeline_loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/pipeline.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/CMU/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/pipeline.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/utils.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/Cambridge/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/colmap_from_nvm.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/colmap_from_nvm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/pipeline.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/pipelines/RobotCar/pipeline.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/reconstruction.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/reconstruction.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/triangulation.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/triangulation.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/base_model.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/database.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/database.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/geometry.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/io.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/io.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/parsers.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/read_write_model.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/read_write_model.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/viz.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/viz.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/utils/viz_3d.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/utils/viz_3d.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/hloc/visualization.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/hloc/visualization.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval_new.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/indoor/scannet/loftr_ds_eval_new.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_8rot.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_8rot.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_big.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/configs/loftr/outdoor/loftr_ds_e2_dense_big.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/demo/demo_loftr.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/demo/demo_loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/config/default.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/config/default.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/megadepth.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/megadepth.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/sampler.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/sampler.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/scannet.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/datasets/scannet.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/data.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/data.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/lightning_loftr.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/lightning/lightning_loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/__init__.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_e2.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_e2.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_fpn.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/backbone/resnet_fpn.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/fine_preprocess.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/fine_preprocess.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/linear_attention.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/linear_attention.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/transformer.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/loftr_module/transformer.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/coarse_matching.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/coarse_matching.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/cvpr_ds_config.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/cvpr_ds_config.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/fine_matching.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/fine_matching.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/geometry.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/position_encoding.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/position_encoding.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/supervision.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/loftr/utils/supervision.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/losses/loftr_loss.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/losses/loftr_loss.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/__init__.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/augment.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/augment.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/comm.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/comm.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataloader.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataloader.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataset.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/metrics.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/misc.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/misc.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/plotting.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/profiler.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/src/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/test.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/test.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/se2loftr/train.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/se2loftr/train.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/thirdparty/transformations.py` & `deep_image_matching-1.2.1/src/deep_image_matching/thirdparty/transformations.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/triangulation.py` & `deep_image_matching-1.2.1/src/deep_image_matching/triangulation.py`

 * *Files 16% similar despite different names*

```diff
@@ -238,7 +238,60 @@
         np.median(inlier_ratios) * 100,
         np.min(inlier_ratios) * 100,
         np.max(inlier_ratios) * 100,
     )
 
     db.commit()
     db.close()
+
+
+def db_from_existing_poses(
+    new_db: Path,
+    features_h5: Path,
+    matches_h5: Path,
+    sfm_rec_path: Path,
+    pair_file: Path,
+    do_geometric_verification: bool = False,
+    max_error: float = 4.0,
+):
+    """
+    db_from_existing_poses _summary_
+
+    Args:
+        new_db (Path): _description_
+        features_h5 (Path): _description_
+        matches_h5 (Path): _description_
+        sfm_rec_path (Path): _description_
+        pair_file (Path): _description_
+        do_geometric_verification (bool, optional): _description_. Defaults to False.
+        max_error (float, optional): _description_. Defaults to 4.0.
+    """
+
+    # Import the sparse reconstruction
+    sfm_rec = pycolmap.Reconstruction(sfm_rec_path)
+
+    # Create an empty database from the sparse reconstruction
+    image_ids = create_db_from_model(sfm_rec, new_db)
+
+    # Add keypoints to the database
+    import_keypoints(features_h5, image_ids, new_db)
+
+    # Add matches to the database, but do not add two-view geometry
+    import_matches(
+        matches_h5,
+        image_ids,
+        new_db,
+        pair_file,
+        add_two_view_geometry=not do_geometric_verification,
+    )
+
+    if do_geometric_verification:
+        # Run the geometric verification with the knwon camera poses and add the inliers matches to the database in the two-view geometry table
+        import_verifed_matches(
+            image_ids,
+            sfm_rec,
+            new_db,
+            features_h5,
+            matches_h5,
+            pair_file,
+            max_error=max_error,
+        )
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/__init__.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/database.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,15 @@
                 width,
                 height,
                 array_to_blob(params),
                 prior_focal_length,
                 camera_id,
             ),
         )
+        self.commit()
         return cursor.lastrowid
 
     def add_image(
         self,
         name: str,
         camera_id: int,
         prior_q: np.ndarray = np.zeros(4),
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/geometric_verification.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/geometric_verification.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pydegesac_default_params = {
     "laf_consistensy_coef": -1.0,
     "error_type": "sampson",
     "symmetric_error_check": True,
     "enable_degeneracy_check": True,
 }
 opencv_methods_mapping = {
+    "NONE": None,
     "LMEDS": cv2.LMEDS,
     "RANSAC": cv2.RANSAC,
     "RHO": cv2.RHO,
     "USAC_DEFAULT": cv2.USAC_DEFAULT,
     "USAC_PARALLEL": cv2.USAC_PARALLEL,
     "USAC_FM_8PTS": cv2.USAC_FM_8PTS,
     "USAC_FAST": cv2.USAC_FAST,
@@ -79,14 +80,17 @@
         except ValueError:
             raise ValueError(f"Invalid Geometry Verification method. It must be one of {gv_names}")
     if not isinstance(method, GeometricVerification):
         raise ValueError(
             f"Invalid Geometry Verification method. It must be a GeometricVerification enum, a string with the method name among {gv_names} or an integer corresponding to the method index."
         )
 
+    if method == GeometricVerification.NONE:
+        return None, np.ones(len(kpts0), dtype=bool)
+
     fallback = False
     F = None
     inlMask = np.ones(len(kpts0), dtype=bool)
 
     if len(kpts0) < 8:
         if not quiet:
             logger.warning("Not enough matches to perform geometric verification.")
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/hloc_base_model.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/hloc_base_model.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/image.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/image.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/logger.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/logger.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/sensor_width_database.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/sensor_width_database.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/tiling.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/tiling.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/timer.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/utils/utils.py` & `deep_image_matching-1.2.1/src/deep_image_matching/utils/utils.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching/visualization.py` & `deep_image_matching-1.2.1/src/deep_image_matching/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,17 @@
                 out,
                 (x0, y0),
                 (x1 + margin + W0, y1),
                 color=line_col,
                 thickness=line_thickness,
                 lineType=cv2.LINE_AA,
             )
-        # display line end-points as circles
+
+    # display line end-points as circles
+    for (x0, y0), (x1, y1) in zip(mkpts0, mkpts1):
         cv2.circle(out, (x0, y0), point_size, pts_col, -1, lineType=cv2.LINE_AA)
         cv2.circle(
             out,
             (x1 + margin + W0, y1),
             point_size,
             pts_col,
             -1,
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching.egg-info/PKG-INFO` & `deep_image_matching-1.2.1/src/deep_image_matching.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_image_matching
-Version: 1.1.1
+Version: 1.2.1
 Summary: Multiview matching with deep-learning and hand-crafted local features for COLMAP and other SfM software.
 Author-email: Francesco Ioli <francesco.ioli@polimi.it>, Luca Morelli <lmorelli@fbk.eu>
 License: # LICENSE
         
         BSD 3-Clause License
         
         Copyright (c) 2018, the respective contributors, as shown by the AUTHORS file.
@@ -44,15 +44,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
-Requires-Dist: torch<=2.2.1
+Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: pillow
 Requires-Dist: opencv-python
 Requires-Dist: opencv-contrib-python
 Requires-Dist: pydegensac
 Requires-Dist: kornia>=0.7.2
 Requires-Dist: h5py
@@ -62,15 +62,14 @@
 Requires-Dist: pyyaml
 Requires-Dist: packaging
 Requires-Dist: einops
 Requires-Dist: pyvis>=0.3.2
 Requires-Dist: yacs>=0.1.8
 Requires-Dist: e2cnn
 Requires-Dist: pytorch_lightning
-Requires-Dist: xformers
 Provides-Extra: dev
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
@@ -159,15 +158,15 @@
 
 ```
 git clone https://github.com/3DOM-FBK/deep-image-matching.git
 cd deep-image-matching
 pip install -e .
 ```
 
-Install pycolmap (optional):
+Install pycolmap (optional, but recommended):
 
 ```
 pip install pycolmap==0.6.1
 ```
 Pycolmap is optional to run reconstruction directly in DIM. If pycolmap is not available, matches will be written both in a h5 and colmap database for later processing with COLMAP GUI or API, or other processing.
 
 For more information, check the [documentation](https://3dom-fbk.github.io/deep-image-matching/installation/).
```

### Comparing `deep_image_matching-1.1.1/src/deep_image_matching.egg-info/SOURCES.txt` & `deep_image_matching-1.2.1/src/deep_image_matching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/tests/test_config.py` & `deep_image_matching-1.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/tests/test_geom_verification.py` & `deep_image_matching-1.2.1/tests/test_geom_verification.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/tests/test_image.py` & `deep_image_matching-1.2.1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `deep_image_matching-1.1.1/tests/test_tiling.py` & `deep_image_matching-1.2.1/tests/test_tiling.py`

 * *Files identical despite different names*

