# Comparing `tmp/keras-nightly-3.2.1.dev2024041103.tar.gz` & `tmp/keras-nightly-3.2.1.dev2024041203.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nightly-3.2.1.dev2024041103.tar", last modified: Thu Apr 11 03:22:43 2024, max compression
+gzip compressed data, was "keras-nightly-3.2.1.dev2024041203.tar", last modified: Fri Apr 12 03:20:01 2024, max compression
```

## Comparing `keras-nightly-3.2.1.dev2024041103.tar` & `keras-nightly-3.2.1.dev2024041203.tar`

### file list

```diff
@@ -1,691 +1,691 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.623718 keras-nightly-3.2.1.dev2024041103/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.623718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.623718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.627718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30090 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36171 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.627718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.631718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34607 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32141 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.635718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.635718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32837 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.643718 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.643718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.643718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.643718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    27410 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.647718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.647718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    62881 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.651718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.651718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.655718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.659718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.659718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.663718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.663718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.663718 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.667718 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.667718 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.667718 keras-nightly-3.2.1.dev2024041103/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.667718 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.671718 keras-nightly-3.2.1.dev2024041103/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    32151 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.671718 keras-nightly-3.2.1.dev2024041103/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   190163 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    36783 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.679718 keras-nightly-3.2.1.dev2024041103/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.679718 keras-nightly-3.2.1.dev2024041103/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.679718 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.679718 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17068 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45200 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16624 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26577 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.893330 keras-nightly-3.2.1.dev2024041203/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-12 03:20:01.893330 keras-nightly-3.2.1.dev2024041203/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.793330 keras-nightly-3.2.1.dev2024041203/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.793330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.793330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.793330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.797330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.801330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.805330 keras-nightly-3.2.1.dev2024041203/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.809330 keras-nightly-3.2.1.dev2024041203/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.813330 keras-nightly-3.2.1.dev2024041203/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.817330 keras-nightly-3.2.1.dev2024041203/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.821330 keras-nightly-3.2.1.dev2024041203/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.821330 keras-nightly-3.2.1.dev2024041203/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.825330 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.825330 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30090 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36171 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.829330 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.833330 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34607 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32269 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33061 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.833330 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10903 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.837330 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.841330 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.841330 keras-nightly-3.2.1.dev2024041203/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.841330 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.841330 keras-nightly-3.2.1.dev2024041203/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.841330 keras-nightly-3.2.1.dev2024041203/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.841330 keras-nightly-3.2.1.dev2024041203/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32837 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.845330 keras-nightly-3.2.1.dev2024041203/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.845330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.845330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.845330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27410 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.849330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.849330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62881 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.853330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.853330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.857330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.861330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.861330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.865330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.869330 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19158 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.869330 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.869330 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.869330 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.873330 keras-nightly-3.2.1.dev2024041203/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.873330 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.873330 keras-nightly-3.2.1.dev2024041203/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32265 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.877330 keras-nightly-3.2.1.dev2024041203/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34612 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190163 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.881330 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37466 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.881330 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.881330 keras-nightly-3.2.1.dev2024041203/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.881330 keras-nightly-3.2.1.dev2024041203/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.881330 keras-nightly-3.2.1.dev2024041203/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.885330 keras-nightly-3.2.1.dev2024041203/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.885330 keras-nightly-3.2.1.dev2024041203/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26581 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.885330 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.885330 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45200 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.893330 keras-nightly-3.2.1.dev2024041203/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16624 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26577 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/utils/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-12 03:19:55.000000 keras-nightly-3.2.1.dev2024041203/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.893330 keras-nightly-3.2.1.dev2024041203/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.893330 keras-nightly-3.2.1.dev2024041203/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.893330 keras-nightly-3.2.1.dev2024041203/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:20:01.893330 keras-nightly-3.2.1.dev2024041203/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-12 03:20:01.000000 keras-nightly-3.2.1.dev2024041203/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-12 03:20:01.000000 keras-nightly-3.2.1.dev2024041203/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:20:01.000000 keras-nightly-3.2.1.dev2024041203/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 03:20:01.000000 keras-nightly-3.2.1.dev2024041203/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 03:20:01.000000 keras-nightly-3.2.1.dev2024041203/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:20:01.893330 keras-nightly-3.2.1.dev2024041203/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-12 03:19:59.000000 keras-nightly-3.2.1.dev2024041203/setup.py
```

### Comparing `keras-nightly-3.2.1.dev2024041103/PKG-INFO` & `keras-nightly-3.2.1.dev2024041203/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.1.dev2024041103
+Version: 3.2.1.dev2024041203
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nightly-3.2.1.dev2024041103/README.md` & `keras-nightly-3.2.1.dev2024041203/README.md`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 from keras.src.optimizers.optimizer import Optimizer
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
 from keras.src.version import version
 
 
-__version__ = "3.2.1.dev2024041103"
+__version__ = "3.2.1.dev2024041203"
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/activations/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/backend/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/callbacks/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/config/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/constraints/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/distribution/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/initializers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/layers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/losses/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/metrics/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/random/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/regularizers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/saving/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/tree/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/activations/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/applications/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/applications/convnext/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet_v2/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/backend/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/callbacks/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/config/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/constraints/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/distribution/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/initializers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/layers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/losses/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/metrics/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/mixed_precision/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/ops/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/ops/linalg/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/ops/nn/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/ops/numpy/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/optimizers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/optimizers/legacy/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/optimizers/schedules/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/random/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/regularizers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/saving/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/activations/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/activations/activations.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/api_export.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/convnext.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/densenet.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/efficientnet.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/efficientnet_v2.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/imagenet_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/inception_resnet_v2.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/inception_v3.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet_v2.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet_v3.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/nasnet.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/resnet.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/resnet_v2.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/vgg16.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/vgg19.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/applications/xception.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/backend_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/dtypes.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/global_state.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/global_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import gc
 import threading
 
 from keras.src import backend
 from keras.src.api_export import keras_export
 
 GLOBAL_STATE_TRACKER = threading.local()
 GLOBAL_SETTINGS_TRACKER = threading.local()
@@ -17,25 +18,33 @@
         attr = default
         if set_to_default:
             set_global_attribute(name, attr)
     return attr
 
 
 @keras_export(["keras.utils.clear_session", "keras.backend.clear_session"])
-def clear_session():
+def clear_session(free_memory=True):
     """Resets all state generated by Keras.
 
     Keras manages a global state, which it uses to implement the Functional
     model-building API and to uniquify autogenerated layer names.
 
     If you are creating many models in a loop, this global state will consume
     an increasing amount of memory over time, and you may want to clear it.
     Calling `clear_session()` releases the global state: this helps avoid
     clutter from old models and layers, especially when memory is limited.
 
+    Args:
+        free_memory: Whether to call Python garbage collection.
+            It's usually a good practice to call it to make sure
+            memory used by deleted objects is immediately freed.
+            However, it may take a few seconds to execute, so
+            when using `clear_session()` in a short loop,
+            you may want to skip it.
+
     Example 1: calling `clear_session()` when creating models in a loop
 
     ```python
     for _ in range(100):
       # Without `clear_session()`, each iteration of this loop will
       # slightly increase the size of the global state managed by Keras
       model = keras.Sequential([
@@ -80,7 +89,11 @@
     elif backend.backend() == "torch":
         import torch._dynamo as dynamo
 
         # reset's torchdynamo's cache so that  cached guards, compiled fn, etc
         # do not persist between clear_session() calls
         dynamo.reset()
 
+    if free_memory:
+        # Manually trigger garbage collection.
+        gc.collect()
+
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/keras_tensor.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/name_scope.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/stateless_scope.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/variables.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/config.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/exports.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/core.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/distribution_lib.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/image.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,37 @@
     "nearest",
     "lanczos3",
     "lanczos5",
     "bicubic",
 )
 
 
+def rgb_to_grayscale(image, data_format="channels_last"):
+    if data_format == "channels_first":
+        if len(image.shape) == 4:
+            image = jnp.transpose(image, (0, 2, 3, 1))
+        elif len(image.shape) == 3:
+            image = jnp.transpose(image, (1, 2, 0))
+        else:
+            raise ValueError(
+                "Invalid input rank: expected rank 3 (single image) "
+                "or rank 4 (batch of images). Received input with shape: "
+                f"image.shape={image.shape}"
+            )
+    red, green, blue = image[..., 0], image[..., 1], image[..., 2]
+    grayscale_image = 0.2989 * red + 0.5870 * green + 0.1140 * blue
+    grayscale_image = jnp.expand_dims(grayscale_image, axis=-1)
+    if data_format == "channels_first":
+        if len(image.shape) == 4:
+            grayscale_image = jnp.transpose(grayscale_image, (0, 3, 1, 2))
+        elif len(image.shape) == 3:
+            grayscale_image = jnp.transpose(grayscale_image, (2, 0, 1))
+    return jnp.array(grayscale_image)
+
+
 def resize(
     image,
     size,
     interpolation="bilinear",
     antialias=False,
     data_format="channels_last",
 ):
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/linalg.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/math.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/nn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/numpy.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/optimizer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/random.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/rnn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/sparse.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/trainer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/core.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/image.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,37 @@
     "nearest",
     "lanczos3",
     "lanczos5",
     "bicubic",
 )
 
 
+def rgb_to_grayscale(image, data_format="channels_last"):
+    if data_format == "channels_first":
+        if len(image.shape) == 4:
+            image = np.transpose(image, (0, 2, 3, 1))
+        elif len(image.shape) == 3:
+            image = np.transpose(image, (1, 2, 0))
+        else:
+            raise ValueError(
+                "Invalid input rank: expected rank 3 (single image) "
+                "or rank 4 (batch of images). Received input with shape: "
+                f"image.shape={image.shape}"
+            )
+    red, green, blue = image[..., 0], image[..., 1], image[..., 2]
+    grayscale_image = 0.2989 * red + 0.5870 * green + 0.1140 * blue
+    grayscale_image = np.expand_dims(grayscale_image, axis=-1)
+    if data_format == "channels_first":
+        if len(image.shape) == 4:
+            grayscale_image = np.transpose(grayscale_image, (0, 3, 1, 2))
+        elif len(image.shape) == 3:
+            grayscale_image = np.transpose(grayscale_image, (2, 0, 1))
+    return np.array(grayscale_image)
+
+
 def resize(
     image,
     size,
     interpolation="bilinear",
     antialias=False,
     data_format="channels_last",
 ):
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/linalg.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/math.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/nn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/numpy.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/random.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/rnn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/trainer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/core.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import global_state
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.name_scope import name_scope as base_name_scope
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.common.stateless_scope import in_stateless_scope
+from keras.src.backend.tensorflow.sparse import sparse_to_dense
 from keras.src.utils import tree
 from keras.src.utils.naming import auto_name
 
 SUPPORTS_SPARSE_TENSORS = True
 
 
 class Variable(
@@ -96,17 +97,15 @@
 
     def _write_object_proto(self, proto, options):
         return self.value._write_object_proto(proto, options)
 
 
 def convert_to_tensor(x, dtype=None, sparse=None):
     if isinstance(x, tf.SparseTensor) and sparse is not None and not sparse:
-        x_shape = x.shape
-        x = tf.sparse.to_dense(x)
-        x.set_shape(x_shape)
+        x = sparse_to_dense(x)
     if dtype is not None:
         dtype = standardize_dtype(dtype)
     if not tf.is_tensor(x):
         if dtype == "bool":
             # TensorFlow boolean conversion is stricter than other backends.
             # It does not allow ints. We convert without dtype and cast instead.
             x = tf.convert_to_tensor(x)
@@ -120,17 +119,15 @@
             return x
         return tf.cast(x, dtype=dtype)
     return x
 
 
 def convert_to_numpy(x):
     if isinstance(x, tf.SparseTensor):
-        x_shape = x.shape
-        x = tf.sparse.to_dense(x)
-        x.set_shape(x_shape)
+        x = sparse_to_dense(x)
     elif isinstance(x, tf.IndexedSlices):
         x = tf.convert_to_tensor(x)
     elif isinstance(x, tf.RaggedTensor):
         x = x.to_tensor()
     return np.asarray(x)
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/distribution_lib.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/image.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,35 @@
     "nearest",
     "lanczos3",
     "lanczos5",
     "bicubic",
 )
 
 
+def rgb_to_grayscale(image, data_format="channels_last"):
+    if data_format == "channels_first":
+        if len(image.shape) == 4:
+            image = tf.transpose(image, (0, 2, 3, 1))
+        elif len(image.shape) == 3:
+            image = tf.transpose(image, (1, 2, 0))
+        else:
+            raise ValueError(
+                "Invalid input rank: expected rank 3 (single image) "
+                "or rank 4 (batch of images). Received input with shape: "
+                f"image.shape={image.shape}"
+            )
+    grayscale_image = tf.image.rgb_to_grayscale(image)
+    if data_format == "channels_first":
+        if len(image.shape) == 4:
+            grayscale_image = tf.transpose(grayscale_image, (0, 3, 1, 2))
+        elif len(image.shape) == 3:
+            grayscale_image = tf.transpose(grayscale_image, (2, 0, 1))
+    return tf.cast(grayscale_image, image.dtype)
+
+
 def resize(
     image,
     size,
     interpolation="bilinear",
     antialias=False,
     data_format="channels_last",
 ):
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/layer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/linalg.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/math.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/nn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/numpy.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/optimizer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/random.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/rnn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/sparse.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/sparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 ones_bool = functools.partial(tf.ones, dtype=tf.bool)
 ones_int8 = functools.partial(tf.ones, dtype=tf.int8)
 zeros_int8 = functools.partial(tf.zeros, dtype=tf.int8)
 ones_like_int8 = functools.partial(tf.ones_like, dtype=tf.int8)
 zeros_like_int8 = functools.partial(tf.zeros_like, dtype=tf.int8)
 
 
-def empty_tensor(shape, dtype):
-    return tf.reshape(tf.convert_to_tensor((), dtype=dtype), shape=shape)
-
-
 def sparse_to_dense(x, default_value=None):
     x_shape = x.shape
+    if x_shape.rank == 0:
+        # Workaround for bug on GPU when sparse tensor represents a scalar.
+        if x.values.shape[0] == 0:
+            return tf.constant(default_value, dtype=x.dtype)
+        else:
+            return tf.reshape(x.values, ())
     x = tf.sparse.to_dense(x, default_value=default_value)
     x.set_shape(x_shape)
     return x
 
 
 def sparse_with_values(x, values):
     x_shape = x.shape
@@ -180,17 +182,17 @@
     intersection_extra_dim = tf.sets.intersection(
         tf.sparse.expand_dims(ones1, axis=-1),
         tf.sparse.expand_dims(ones2, axis=-1),
     )
 
     def empty_intersection():
         return (
-            empty_tensor((0, x1.shape.rank), dtype=tf.int64),
-            empty_tensor((0,), dtype=x1.values.dtype),
-            empty_tensor((0,), dtype=x2.values.dtype),
+            tf.zeros((0, x1.shape.rank), dtype=tf.int64),
+            tf.zeros((0,), dtype=x1.values.dtype),
+            tf.zeros((0,), dtype=x2.values.dtype),
         )
 
     def non_empty_intersection():
         intersection = tf.sparse.reshape(intersection_extra_dim, x1.dense_shape)
 
         # Compute the masks to remove indices in x1 and x2 that are not
         # in the intersection, then trim x1 and x2.
@@ -245,16 +247,16 @@
         axis=-1,
     )
     intersection_indices_count = tf.shape(intersection_indices)[0]
 
     def empty_intersection():
         return (
             intersection_indices,
-            empty_tensor((0,) + x1.values.shape[1:], x1.dtype),
-            empty_tensor((0,) + x2.values.shape[1:], x2.dtype),
+            tf.zeros((0,) + x1.values.shape[1:], x1.dtype),
+            tf.zeros((0,) + x2.values.shape[1:], x2.dtype),
         )
 
     def non_empty_intersection():
         # Re-gather sub parts of the values that are part of the intersection.
         def values_for_intersection(indices_expanded, indices_count, values):
             indices_indices = tf.scatter_nd(
                 indices_expanded,
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/trackable.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/trainer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/tensorflow/trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import contextlib
 import warnings
 
 import numpy as np
 import tensorflow as tf
-from packaging.version import Version
 from tensorflow.python.eager import context as tf_context
 
 from keras.src import callbacks as callbacks_module
 from keras.src import metrics as metrics_module
 from keras.src import optimizers as optimizers_module
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import array_slicing
@@ -27,19 +26,14 @@
         # Model must be created under scope of DistStrat it will be trained
         # with.
         if tf.distribute.has_strategy():
             self._distribute_strategy = tf.distribute.get_strategy()
         else:
             self._distribute_strategy = None
 
-        self._distribute_reduction_method = None
-        self._supports_reduce_retracing = Version(tf.__version__) >= Version(
-            "2.9.0"
-        )
-
     @property
     def distribute_strategy(self):
         return self._distribute_strategy or tf.distribute.get_strategy()
 
     @property
     def distribute_reduction_method(self):
         return self._distribute_reduction_method or "auto"
@@ -106,30 +100,31 @@
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_data(data):
             """Runs a single training step on a batch of data."""
             return self.train_step(data)
 
         if not self.run_eagerly:
-            kwargs = {"jit_compile": self.jit_compile}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            one_step_on_data = tf.function(one_step_on_data, **kwargs)
+            one_step_on_data = tf.function(
+                one_step_on_data,
+                reduce_retracing=True,
+                jit_compile=self.jit_compile,
+            )
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_iterator(iterator):
             """Runs a single training step given a Dataset iterator."""
             data = next(iterator)
             outputs = self.distribute_strategy.run(
                 one_step_on_data, args=(data,)
             )
             outputs = reduce_per_replica(
                 outputs,
                 self.distribute_strategy,
-                reduction=self.distribute_reduction_method,
+                reduction="auto",
             )
             return outputs
 
         @tf.autograph.experimental.do_not_convert
         def multi_step_on_iterator(iterator):
             for _ in range(self.steps_per_execution):
                 outputs = one_step_on_iterator(iterator)
@@ -137,47 +132,43 @@
 
         if self.steps_per_execution > 1:
             train_function = multi_step_on_iterator
         else:
             train_function = one_step_on_iterator
 
         if not self.run_eagerly:
-            kwargs = {}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            train_function = tf.function(train_function, **kwargs)
+            train_function = tf.function(train_function, reduce_retracing=True)
 
         self.train_function = train_function
 
     def make_test_function(self, force=False):
         if self.test_function is not None and not force:
             return self.test_function
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_data(data):
             """Runs a single test step on a batch of data."""
             return self.test_step(data)
 
         if not self.run_eagerly and self.jit_compile:
-            kwargs = {"jit_compile": True}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            one_step_on_data = tf.function(one_step_on_data, **kwargs)
+            one_step_on_data = tf.function(
+                one_step_on_data, reduce_retracing=True, jit_compile=True
+            )
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_iterator(iterator):
             """Runs a single test step given a Dataset iterator."""
             data = next(iterator)
             outputs = self.distribute_strategy.run(
                 one_step_on_data, args=(data,)
             )
             outputs = reduce_per_replica(
                 outputs,
                 self.distribute_strategy,
-                reduction=self.distribute_reduction_method,
+                reduction="auto",
             )
             return outputs
 
         @tf.autograph.experimental.do_not_convert
         def multi_step_on_iterator(iterator):
             for _ in range(self.steps_per_execution):
                 outputs = one_step_on_iterator(iterator)
@@ -185,46 +176,42 @@
 
         if self.steps_per_execution > 1:
             test_function = multi_step_on_iterator
         else:
             test_function = one_step_on_iterator
 
         if not self.run_eagerly:
-            kwargs = {}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            test_function = tf.function(test_function, **kwargs)
+            test_function = tf.function(test_function, reduce_retracing=True)
 
         self.test_function = test_function
 
     def make_predict_function(self, force=False):
         if self.predict_function is not None and not force:
             return self.predict_function
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_data(data):
             """Runs a predict test step on a batch of data."""
             return self.predict_step(data)
 
         if not self.run_eagerly and self.jit_compile:
-            kwargs = {"jit_compile": True}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            one_step_on_data = tf.function(one_step_on_data, **kwargs)
+            one_step_on_data = tf.function(
+                one_step_on_data, reduce_retracing=True, jit_compile=True
+            )
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_data_distributed(data):
             data = data[0]
             outputs = self.distribute_strategy.run(
                 one_step_on_data, args=(data,)
             )
             outputs = reduce_per_replica(
                 outputs,
                 self.distribute_strategy,
-                reduction=self.distribute_reduction_method,
+                reduction="concat",
             )
             return outputs
 
         @tf.autograph.experimental.do_not_convert
         def multi_step_on_data(data):
             outputs = one_step_on_data_distributed(data[:1])
             for single_step_data in data[1:]:
@@ -236,19 +223,17 @@
 
         if self.steps_per_execution > 1:
             predict_function = multi_step_on_data
         else:
             predict_function = one_step_on_data_distributed
 
         if not self.run_eagerly:
-            kwargs = {}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-
-            predict_function = tf.function(predict_function, **kwargs)
+            predict_function = tf.function(
+                predict_function, reduce_retracing=True
+            )
 
         self.predict_function = predict_function
 
     @traceback_utils.filter_traceback
     def fit(
         self,
         x=None,
@@ -702,15 +687,15 @@
     which represents the values across all the replicas, `reduce_per_replica`
     attempts to "reduce" those values and returns the corresponding structure
     that represents only single values.
 
     Currently, `reduce_per_replica` is only used for reducing the metric results
     from `tf.distribute.Strategy.run()`. Depending on the underlying
     `Strategy` implementation, `values` may be a `PerReplica` object,
-     which can be thought of as a collection of values across the replicas,
+    which can be thought of as a collection of values across the replicas,
     or a `tf.Tensor`, if the strategy has already conducted the reduction
     for the downstream library.
 
     There are five possible outcomes of reduction:
 
     1) if the `values` is a structure of simple `tf.Tensor`s, meaning that
        reduction is not actually needed, `reduce_per_replica` returns the
@@ -729,53 +714,60 @@
        case, where each replica contain different values which are not
        synchronized.
     5) else, if `reduction="concat"`, then `reduce_per_replica`
        returns the concatenation of the values across the replicas, along the
        axis of dimension 0. This is used in the inference case (`predict()`).
 
     Args:
-      values: Structure of `PerReplica` objects or `tf.Tensor`s. `tf.Tensor`s
-        are returned as-is.
-      strategy: `tf.distribute.Strategy` object.
-      reduction: One of `"auto"`, `"first"`, `"concat"`, or `"sum"`.
-        `"auto"` will select `"first"` when used under a TPUStrategy, or
-        `"sum"` otherwise.
+        values: Structure of `PerReplica` objects or `tf.Tensor`s.
+            `tf.Tensor`s are returned as-is.
+        strategy: `tf.distribute.Strategy` object.
+        reduction: One of `"auto"`, `"first"`, `"concat"`, `"mean"`, or `"sum"`.
+            `"auto"` will select `"first"` when used under a TPUStrategy, or
+            `"mean"` otherwise.
 
     Returns:
-      Structure of `Tensor`s, representing the result of reduction.
-
-    Raises:
-      ValueError: if the reduction method is not supported.
+        Structure of `Tensor`s, representing the result of reduction.
     """
 
     if reduction == "auto":
-        reduction = "sum"  # Ignore TPU strategy which should default to "first"
+        if isinstance(strategy, tf.distribute.TPUStrategy):
+            reduction = "first"
+        else:
+            reduction = "mean"
 
     def _reduce(v):
         """Reduce a single `PerReplica` object."""
         if _collective_all_reduce_multi_worker(strategy):
             if reduction == "concat":
                 return _multi_worker_concat(v, strategy)
             elif reduction == "sum":
-                return strategy.reduce("SUM", v, axis=None)
+                return strategy.reduce("SUM", v)
+            elif reduction == "mean":
+                return strategy.reduce("MEAN", v, axis=0)
 
         if not _is_per_replica_instance(v):
             return v
         elif reduction == "first":
             return strategy.experimental_local_results(v)[0]
         elif reduction == "concat":
             if _is_tpu_multi_host(strategy):
                 return _tpu_multi_host_concat(v, strategy)
             else:
                 return concat(strategy.experimental_local_results(v))
         elif reduction == "sum":
             return tf.reduce_sum(strategy.experimental_local_results(v))
+        elif reduction == "mean":
+            return tf.reduce_mean(
+                strategy.experimental_local_results(v), axis=0
+            )
         else:
             raise ValueError(
-                '`reduction` must be "first", "concat", "sum", or "auto". '
+                "`reduction` must be one of "
+                '"first", "concat", "mean", "sum", or "auto". '
                 f"Received: reduction={reduction}."
             )
 
     return tree.map_structure(_reduce, values)
 
 
 def _multi_worker_concat(v, strategy):
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/core.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/image.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,46 @@
 
 UNSUPPORTED_INTERPOLATIONS = (
     "lanczos3",
     "lanczos5",
 )
 
 
+def rgb_to_grayscale(image, data_format="channel_last"):
+    try:
+        import torchvision
+    except:
+        raise ImportError(
+            "The torchvision package is necessary to use "
+            "`rgb_to_grayscale` with the torch backend. "
+            "Please install torchvision. "
+        )
+    image = convert_to_tensor(image)
+    if data_format == "channels_last":
+        if image.ndim == 4:
+            image = image.permute((0, 3, 1, 2))
+        elif image.ndim == 3:
+            image = image.permute((2, 0, 1))
+        else:
+            raise ValueError(
+                "Invalid input rank: expected rank 3 (single image) "
+                "or rank 4 (batch of images). Received input with shape: "
+                f"image.shape={image.shape}"
+            )
+    grayscale_image = torchvision.transforms.functional.rgb_to_grayscale(
+        img=image,
+    )
+    if data_format == "channels_last":
+        if len(image.shape) == 4:
+            grayscale_image = grayscale_image.permute((0, 2, 3, 1))
+        elif len(image.shape) == 3:
+            grayscale_image = grayscale_image.permute((1, 2, 0))
+    return grayscale_image
+
+
 def resize(
     image,
     size,
     interpolation="bilinear",
     antialias=False,
     data_format="channels_last",
 ):
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/layer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/linalg.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/math.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/nn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/numpy.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adam.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_lion.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/random.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/rnn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/trainer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/backup_and_restore.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/callback.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/callback_list.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/csv_logger.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/early_stopping.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/history.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/lambda_callback.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/learning_rate_scheduler.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/model_checkpoint.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/progbar_logger.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/remote_monitor.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/swap_ema_weights.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/tensorboard.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/terminate_on_nan.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/constraints/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/constraints/constraints.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/boston_housing.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/california_housing.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar10.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar100.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/fashion_mnist.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/imdb.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/mnist.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/reuters.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/distribution/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/distribution/distribution_lib.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/dtype_policy.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/export/export_lib.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/initializers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/initializers/constant_initializers.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/initializers/initializer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/initializers/random_initializers.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/activation.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/elu.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/leaky_relu.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/prelu.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/relu.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/softmax.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/additive_attention.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/attention.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/grouped_query_attention.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/multi_head_attention.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_conv.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_conv_transpose.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_separable_conv.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv1d_transpose.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv2d_transpose.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv3d_transpose.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/separable_conv1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/separable_conv2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/dense.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/einsum_dense.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/embedding.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,17 @@
             This is useful when using recurrent layers which
             may take variable length input. If this is `True`,
             then all subsequent layers in the model need
             to support masking or an exception will be raised.
             If `mask_zero` is set to `True`, as a consequence,
             index 0 cannot be used in the vocabulary (`input_dim` should
             equal size of vocabulary + 1).
+        weights: Optional floating-point matrix of size
+            `(input_dim, output_dim)`. The initial embeddings values
+            to use.
         lora_rank: Optional integer. If set, the layer's forward pass
             will implement LoRA (Low-Rank Adaptation)
             with the provided rank. LoRA sets the layer's embeddings
             matrix to non-trainable and replaces it with a delta over the
             original matrix, obtained via multiplying two lower-rank
             trainable matrices. This can be useful to reduce the
             computation cost of fine-tuning large embedding layers.
@@ -74,14 +77,15 @@
         self,
         input_dim,
         output_dim,
         embeddings_initializer="uniform",
         embeddings_regularizer=None,
         embeddings_constraint=None,
         mask_zero=False,
+        weights=None,
         lora_rank=None,
         **kwargs,
     ):
         input_length = kwargs.pop("input_length", None)
         if input_length is not None:
             warnings.warn(
                 "Argument `input_length` is deprecated. Just remove it."
@@ -94,15 +98,23 @@
         self.embeddings_constraint = constraints.get(embeddings_constraint)
         self.mask_zero = mask_zero
         self.supports_masking = mask_zero
         self.autocast = False
         self.lora_rank = lora_rank
         self.lora_enabled = False
 
+        self.build()
+        if weights is not None:
+            if not (isinstance(weights, list) and len(weights) == 1):
+                weights = [weights]
+            self.set_weights(weights)
+
     def build(self, input_shape=None):
+        if self.built:
+            return
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             self.quantized_build(
                 input_shape, mode=self.dtype_policy.quantization_mode
             )
         else:
             self._embeddings = self.add_weight(
                 shape=(self.input_dim, self.output_dim),
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/identity.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/input_layer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/lambda_layer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/masking.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/wrapper.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/input_spec.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/layer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/add.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/average.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/base_merge.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/concatenate.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/dot.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/maximum.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/minimum.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/multiply.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/subtract.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/batch_normalization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/group_normalization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/layer_normalization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/spectral_normalization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/unit_normalization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/base_global_pooling.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/base_pooling.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/category_encoding.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/center_crop.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/discretization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/feature_space.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/hashed_crossing.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/hashing.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/index_lookup.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/integer_lookup.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/normalization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_brightness.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_contrast.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_crop.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_flip.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_rotation.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_translation.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_zoom.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/rescaling.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/resizing.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/string_lookup.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/text_vectorization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/tf_data_layer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/activity_regularization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/alpha_dropout.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/dropout.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/gaussian_dropout.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/gaussian_noise.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/spatial_dropout.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/flatten.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/permute.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/repeat_vector.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/reshape.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/bidirectional.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm1d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm2d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm3d.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/gru.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/lstm.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/rnn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,26 +232,34 @@
             self.state_size = [state_size]
             self.single_state = True
         else:
             self.state_size = list(state_size)
             self.single_state = False
 
     def compute_output_shape(self, sequences_shape, initial_state_shape=None):
-        state_shape = [(sequences_shape[0], d) for d in self.state_size]
+        batch_size = sequences_shape[0]
+        length = sequences_shape[1]
+        states_shape = []
+        for state_size in self.state_size:
+            if isinstance(state_size, int):
+                states_shape.append((batch_size, state_size))
+            elif isinstance(state_size, (list, tuple)):
+                states_shape.append([(batch_size, s) for s in state_size])
+
         output_size = getattr(self.cell, "output_size", None)
         if output_size is None:
             output_size = self.state_size[0]
         if not isinstance(output_size, int):
             raise ValueError("output_size must be an integer.")
         if self.return_sequences:
-            output_shape = (sequences_shape[0], sequences_shape[1], output_size)
+            output_shape = (batch_size, length, output_size)
         else:
-            output_shape = (sequences_shape[0], output_size)
+            output_shape = (batch_size, output_size)
         if self.return_state:
-            return output_shape, *state_shape
+            return output_shape, *states_shape
         return output_shape
 
     def compute_mask(self, _, mask):
         # Time step masks must be the same for each input.
         # This is because the mask for an RNN is of size [batch, time_steps, 1],
         # and specifies which time steps should be skipped, and a time step
         # must be skipped for all inputs.
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/simple_rnn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/time_distributed.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/backend.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/layers.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/losses.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/image.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/sequence.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/text.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/json_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/legacy_h5_format.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/saving_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/serialization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/losses/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/losses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import inspect
+
 from keras.src.api_export import keras_export
 from keras.src.losses.loss import Loss
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
@@ -179,11 +181,13 @@
         obj = deserialize(identifier)
     elif isinstance(identifier, str):
         obj = ALL_OBJECTS_DICT.get(identifier, None)
     else:
         obj = identifier
 
     if callable(obj):
+        if inspect.isclass(obj):
+            obj = obj()
         return obj
     else:
         raise ValueError(f"Could not interpret loss identifier: {identifier}")
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/losses/loss.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/losses/losses.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/accuracy_metrics.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/confusion_metrics.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/f_score_metrics.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/hinge_metrics.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/iou_metrics.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/metric.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/metrics_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/probabilistic_metrics.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/reduction_metrics.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/regression_metrics.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/models/cloning.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/models/functional.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/models/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -556,15 +556,18 @@
         layer_output_tensors = layer._inbound_nodes[node_index].output_tensors
         return layer_output_tensors[tensor_index]
 
     def map_tensors(tensors):
         if isinstance(tensors, dict):
             return {k: get_tensor(*v) for k, v in tensors.items()}
         else:
-            return [get_tensor(*v) for v in tensors]
+            tensor_list = [get_tensor(*v) for v in tensors]
+            if len(tensor_list) == 1:
+                return tensor_list[0]
+            return tensor_list
 
     input_tensors = map_tensors(config["input_layers"])
     output_tensors = map_tensors(config["output_layers"])
     return cls(
         inputs=input_tensors,
         outputs=output_tensors,
         name=name,
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/models/model.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/models/sequential.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/models/variable_mapping.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/core.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/function.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/image.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,111 @@
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.backend import any_symbolic_tensors
 from keras.src.ops.operation import Operation
 from keras.src.ops.operation_utils import compute_conv_output_shape
 
 
+class RGBToGrayscale(Operation):
+    def __init__(
+        self,
+        data_format="channels_last",
+    ):
+        super().__init__()
+        self.data_format = data_format
+
+    def call(self, image):
+        return backend.image.rgb_to_grayscale(
+            image,
+            data_format=self.data_format,
+        )
+
+    def compute_output_spec(self, image):
+        if len(image.shape) not in (3, 4):
+            raise ValueError(
+                "Invalid image rank: expected rank 3 (single image) "
+                "or rank 4 (batch of images). Received input with shape: "
+                f"image.shape={image.shape}"
+            )
+
+        if len(image.shape) == 3:
+            if self.data_format == "channels_last":
+                return KerasTensor(image.shape[:-1] + (1,), dtype=image.dtype)
+            else:
+                return KerasTensor((1,) + image.shape[1:], dtype=image.dtype)
+        elif len(image.shape) == 4:
+            if self.data_format == "channels_last":
+                return KerasTensor(
+                    (image.shape[0],) + image.shape[1:-1] + (1,),
+                    dtype=image.dtype,
+                )
+            else:
+                return KerasTensor(
+                    (
+                        image.shape[0],
+                        1,
+                    )
+                    + image.shape[2:],
+                    dtype=image.dtype,
+                )
+
+
+@keras_export("keras.ops.image.rgb_to_grayscale")
+def rgb_to_grayscale(
+    image,
+    data_format="channels_last",
+):
+    """Convert RGB images to grayscale.
+
+    This function converts RGB images to grayscale images. It supports both
+    3D and 4D tensors, where the last dimension represents channels.
+
+    Args:
+        image: Input RGB image or batch of RGB images. Must be a 3D tensor
+            with shape `(height, width, channels)` or a 4D tensor with shape
+            `(batch, height, width, channels)`.
+        data_format: A string specifying the data format of the input tensor.
+            It can be either `"channels_last"` or `"channels_first"`.
+            `"channels_last"` corresponds to inputs with shape
+            `(batch, height, width, channels)`, while `"channels_first"`
+            corresponds to inputs with shape `(batch, channels, height, width)`.
+            Defaults to `"channels_last"`.
+
+    Returns:
+        Grayscale image or batch of grayscale images.
+
+    Examples:
+
+    >>> import numpy as np
+    >>> from keras import ops
+    >>> x = np.random.random((2, 4, 4, 3))
+    >>> y = ops.image.rgb_to_grayscale(x)
+    >>> y.shape
+    (2, 4, 4, 1)
+
+    >>> x = np.random.random((4, 4, 3)) # Single RGB image
+    >>> y = ops.image.rgb_to_grayscale(x)
+    >>> y.shape
+    (4, 4, 1)
+
+    >>> x = np.random.random((2, 3, 4, 4))
+    >>> y = ops.image.rgb_to_grayscale(x, data_format="channels_first")
+    >>> y.shape
+    (2, 1, 4, 4)
+    """
+    if any_symbolic_tensors((image,)):
+        return RGBToGrayscale(
+            data_format=data_format,
+        ).symbolic_call(image)
+    return backend.image.rgb_to_grayscale(
+        image,
+        data_format=data_format,
+    )
+
+
 class Resize(Operation):
     def __init__(
         self,
         size,
         interpolation="bilinear",
         antialias=False,
         data_format="channels_last",
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/linalg.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/math.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/nn.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/node.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/numpy.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/operation.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/operation_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/ops/symbolic_arguments.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adadelta.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adafactor.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adagrad.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adam.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adamax.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adamw.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/base_optimizer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/base_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,19 @@
         """Add an all-zeros variable with the shape and dtype of a reference
         variable.
         """
         name = name or "var"
         if hasattr(reference_variable, "path"):
             name = reference_variable.path.replace("/", "_") + "_" + name
         else:
-            name = str(reference_variable.name).replace(":", "_") + "_" + name
+            name = (
+                str(reference_variable.name).replace("/", "_").replace(":", "_")
+                + "_"
+                + name
+            )
         return self.add_variable(
             shape=reference_variable.shape,
             initializer=initializer,
             dtype=reference_variable.dtype,
             name=name,
         )
 
@@ -497,14 +501,18 @@
 
     @property
     def learning_rate(self):
         return self._get_current_learning_rate()
 
     @learning_rate.setter
     def learning_rate(self, learning_rate):
+        if isinstance(self._learning_rate, backend.Variable):
+            prev_lr_var = self._learning_rate
+        else:
+            prev_lr_var = None
         if isinstance(
             learning_rate, learning_rate_schedule.LearningRateSchedule
         ):
             self._learning_rate = learning_rate
         elif callable(learning_rate):
             self._learning_rate = learning_rate
         else:
@@ -515,14 +523,19 @@
                     "This optimizer was created with a `LearningRateSchedule`"
                     " object as its `learning_rate` constructor argument, "
                     "hence its learning rate is not settable. If you need the"
                     " learning rate to be settable, you should instantiate "
                     "the optimizer with a float `learning_rate` argument."
                 )
             self._learning_rate.assign(learning_rate)
+        if prev_lr_var is not None and not isinstance(
+            self._learning_rate, backend.Variable
+        ):
+            # Untrack learning rate variable
+            self._untrack_variable(prev_lr_var)
 
     def set_weights(self, weights):
         """Set the weights of the optimizer."""
         if not self.built:
             raise ValueError(
                 "You are calling `set_weights()` on an optimizer that has not "
                 "yet been built. Please call "
@@ -828,14 +841,21 @@
         l2norm = ops.where(pred, ops.sqrt(l2sum_safe), l2sum)
         intermediate = ops.multiply(values, self.clipnorm)
         values_clip = ops.convert_to_tensor(intermediate) / ops.maximum(
             l2norm, self.clipnorm
         )
         return values_clip
 
+    def _untrack_variable(self, variable):
+        previous_lock_state = self._tracker.locked
+        self._tracker.unlock()
+        self._tracker.untrack(variable)
+        if previous_lock_state is True:
+            self._tracker.lock()
+
 
 base_optimizer_keyword_args = """name: String. The name to use
             for momentum accumulator weights created by
             the optimizer.
         weight_decay: Float. If set, weight decay is applied.
         clipnorm: Float. If set, the gradient of each weight is individually
             clipped so that its norm is no higher than this value.
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/ftrl.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/lion.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/loss_scale_optimizer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/nadam.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/optimizer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/rmsprop.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/sgd.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/quantizers.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/random/random.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/random/seed_generator.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/regularizers.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/saving/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/saving/object_registration.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/saving/saving_api.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/saving/saving_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,17 @@
         return saving_lib.load_model(
             filepath,
             custom_objects=custom_objects,
             compile=compile,
             safe_mode=safe_mode,
         )
     if str(filepath).endswith((".h5", ".hdf5")):
-        return legacy_h5_format.load_model_from_hdf5(filepath)
+        return legacy_h5_format.load_model_from_hdf5(
+            filepath, custom_objects=custom_objects, compile=compile
+        )
     elif str(filepath).endswith(".keras"):
         raise ValueError(
             f"File not found: filepath={filepath}. "
             "Please ensure the file is an accessible `.keras` "
             "zip file."
         )
     else:
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/saving/saving_lib.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/saving/serialization_lib.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/testing/test_case.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/testing/test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def setUp(self):
         # clear global state so that test cases are independent
         # required for the jit enabled torch tests since dynamo has
         # a global cache for guards, compiled fn, etc
-        clear_session()
+        clear_session(free_memory=False)
         if traceback_utils.is_traceback_filtering_enabled():
             traceback_utils.disable_traceback_filtering()
 
     def get_temp_dir(self):
         temp_dir = tempfile.mkdtemp()
         self.addCleanup(lambda: shutil.rmtree(temp_dir))
         return temp_dir
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/testing/test_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/compile_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/array_slicing.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,17 +171,17 @@
 
     @classmethod
     def convert_to_jax_compatible(cls, x):
         return data_adapter_utils.tf_sparse_to_jax_sparse(x)
 
     @classmethod
     def convert_to_torch_compatible(cls, x):
-        from keras.src.utils.module_utils import tensorflow as tf
+        from keras.src.backend.tensorflow import sparse as tf_sparse
 
-        return tf.sparse.to_dense(x)
+        return tf_sparse.sparse_to_dense(x)
 
 
 class JaxSliceable(Sliceable):
     def __getitem__(self, indices):
         return self.array[indices, ...]
 
     @classmethod
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/data_adapter.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/epoch_iterator.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/trainer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/argument_validation.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/audio_dataset_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/backend_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/code_stats.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/dataset_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/dtype_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/file_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/image_dataset_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/image_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/io_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/jax_layer.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/model_visualization.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/module_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/naming.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/numerical_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/progbar.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/python_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/rng_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/sequence_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/summary_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/text_dataset_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/tf_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/timeseries_dataset_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/torch_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/traceback_utils.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/tracking.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/src/utils/tree.py` & `keras-nightly-3.2.1.dev2024041203/keras/src/utils/tree.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/tree/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras/utils/__init__.py` & `keras-nightly-3.2.1.dev2024041203/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/PKG-INFO` & `keras-nightly-3.2.1.dev2024041203/keras_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.1.dev2024041103
+Version: 3.2.1.dev2024041203
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/SOURCES.txt` & `keras-nightly-3.2.1.dev2024041203/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.1.dev2024041103/setup.py` & `keras-nightly-3.2.1.dev2024041203/setup.py`

 * *Files identical despite different names*

