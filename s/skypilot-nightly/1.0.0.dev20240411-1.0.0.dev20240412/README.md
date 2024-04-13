# Comparing `tmp/skypilot-nightly-1.0.0.dev20240411.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20240411.tar", last modified: Thu Apr 11 10:40:18 2024, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20240412.tar", last modified: Fri Apr 12 10:40:38 2024, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20240411.tar` & `skypilot-nightly-1.0.0.dev20240412.tar`

### file list

```diff
@@ -1,334 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.167288 skypilot-nightly-1.0.0.dev20240411/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-11 10:40:18.167288 skypilot-nightly-1.0.0.dev20240411/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 10:40:18.167288 skypilot-nightly-1.0.0.dev20240411/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-11 10:40:15.000000 skypilot-nightly-1.0.0.dev20240411/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.099288 skypilot-nightly-1.0.0.dev20240411/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-11 10:40:18.000000 skypilot-nightly-1.0.0.dev20240411/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.103288 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.103288 skypilot-nightly-1.0.0.dev20240411/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   221923 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.103288 skypilot-nightly-1.0.0.dev20240411/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.103288 skypilot-nightly-1.0.0.dev20240411/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   186851 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.107288 skypilot-nightly-1.0.0.dev20240411/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    30942 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    46892 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.111288 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.111288 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.115288 skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    39960 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.115288 skypilot-nightly-1.0.0.dev20240411/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31094 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    54049 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.115288 skypilot-nightly-1.0.0.dev20240411/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.119288 skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.119288 skypilot-nightly-1.0.0.dev20240411/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.119288 skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.119288 skypilot-nightly-1.0.0.dev20240411/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.119288 skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.123288 skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52429 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.123288 skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.123288 skypilot-nightly-1.0.0.dev20240411/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.123288 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.127288 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    60100 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.131288 skypilot-nightly-1.0.0.dev20240411/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.131288 skypilot-nightly-1.0.0.dev20240411/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-11 10:40:15.000000 skypilot-nightly-1.0.0.dev20240411/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.131288 skypilot-nightly-1.0.0.dev20240411/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.131288 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.135288 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.135288 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.135288 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.135288 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.135288 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.139288 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.139288 skypilot-nightly-1.0.0.dev20240411/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.139288 skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.139288 skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.139288 skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    46443 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.143288 skypilot-nightly-1.0.0.dev20240411/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/spot-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.143288 skypilot-nightly-1.0.0.dev20240411/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.147288 skypilot-nightly-1.0.0.dev20240411/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.147288 skypilot-nightly-1.0.0.dev20240411/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.151288 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/generate_kind_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.155288 skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-11 10:40:18.000000 skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-11 10:40:18.000000 skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 10:40:18.000000 skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 10:40:18.000000 skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-11 10:40:18.000000 skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-11 10:40:18.000000 skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 10:40:18.155288 skypilot-nightly-1.0.0.dev20240411/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   211200 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_spot_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-11 10:40:12.000000 skypilot-nightly-1.0.0.dev20240411/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.344960 skypilot-nightly-1.0.0.dev20240412/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-12 10:40:38.344960 skypilot-nightly-1.0.0.dev20240412/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 10:40:38.344960 skypilot-nightly-1.0.0.dev20240412/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-12 10:40:35.000000 skypilot-nightly-1.0.0.dev20240412/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.280960 skypilot-nightly-1.0.0.dev20240412/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-12 10:40:38.000000 skypilot-nightly-1.0.0.dev20240412/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.284960 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.284960 skypilot-nightly-1.0.0.dev20240412/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   221923 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.284960 skypilot-nightly-1.0.0.dev20240412/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.284960 skypilot-nightly-1.0.0.dev20240412/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   186846 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.288960 skypilot-nightly-1.0.0.dev20240412/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30942 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46892 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.292960 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.292960 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.292960 skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.296960 skypilot-nightly-1.0.0.dev20240412/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24916 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54049 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.296960 skypilot-nightly-1.0.0.dev20240412/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.296960 skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.296960 skypilot-nightly-1.0.0.dev20240412/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.296960 skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.300960 skypilot-nightly-1.0.0.dev20240412/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.300960 skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.300960 skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52429 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.300960 skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.304960 skypilot-nightly-1.0.0.dev20240412/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.304960 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.304960 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60100 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.308960 skypilot-nightly-1.0.0.dev20240412/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.308960 skypilot-nightly-1.0.0.dev20240412/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-12 10:40:35.000000 skypilot-nightly-1.0.0.dev20240412/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.312960 skypilot-nightly-1.0.0.dev20240412/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9204 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.312960 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.312960 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.312960 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.312960 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.312960 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.316960 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.316960 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.316960 skypilot-nightly-1.0.0.dev20240412/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.316960 skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.316960 skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.320960 skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46443 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.320960 skypilot-nightly-1.0.0.dev20240412/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/spot-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.324960 skypilot-nightly-1.0.0.dev20240412/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.328960 skypilot-nightly-1.0.0.dev20240412/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.328960 skypilot-nightly-1.0.0.dev20240412/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.328960 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/generate_kind_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.332960 skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-12 10:40:38.000000 skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-04-12 10:40:38.000000 skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:40:38.000000 skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 10:40:38.000000 skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-12 10:40:38.000000 skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 10:40:38.000000 skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:40:38.332960 skypilot-nightly-1.0.0.dev20240412/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211200 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_spot_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-12 10:40:33.000000 skypilot-nightly-1.0.0.dev20240412/tests/test_yaml_parser.py
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/LICENSE` & `skypilot-nightly-1.0.0.dev20240412/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20240412/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/PKG-INFO` & `skypilot-nightly-1.0.0.dev20240412/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240411
+Version: 1.0.0.dev20240412
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/README.md` & `skypilot-nightly-1.0.0.dev20240412/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/pyproject.toml` & `skypilot-nightly-1.0.0.dev20240412/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/setup.py` & `skypilot-nightly-1.0.0.dev20240412/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The SkyPilot package."""
 import os
 import subprocess
 from typing import Optional
 import urllib.request
 
 # Replaced with the current commit when building the wheels.
-_SKYPILOT_COMMIT_SHA = '226c1eb09410ce22979430f569cd1a7b333df9bf'
+_SKYPILOT_COMMIT_SHA = 'e60eb736422ecf541810a50cc9a37942b407dc41'
 
 
 def _get_git_commit():
     if 'SKYPILOT_COMMIT_SHA' not in _SKYPILOT_COMMIT_SHA:
         # This is a release build, so we don't need to get the commit hash from
         # git, as it's already been set.
         return _SKYPILOT_COMMIT_SHA
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240411'
+__version__ = '1.0.0.dev20240412'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
 
@@ -86,33 +86,36 @@
 from sky.core import autostop
 from sky.core import cancel
 from sky.core import cost_report
 from sky.core import down
 from sky.core import download_logs
 from sky.core import job_status
 from sky.core import queue
-from sky.core import spot_cancel
-from sky.core import spot_queue
 from sky.core import start
 from sky.core import status
 from sky.core import stop
 from sky.core import storage_delete
 from sky.core import storage_ls
 from sky.core import tail_logs
 from sky.dag import Dag
 from sky.data import Storage
 from sky.data import StorageMode
 from sky.data import StoreType
 from sky.execution import exec  # pylint: disable=redefined-builtin
 from sky.execution import launch
-from sky.execution import spot_launch
 from sky.optimizer import Optimizer
 from sky.optimizer import OptimizeTarget
 from sky.resources import Resources
 from sky.skylet.job_lib import JobStatus
+# TODO (zhwu): These imports are for backward compatibility, and spot APIs
+# should be called with `sky.spot.xxx` instead. Remove in release 0.7.0
+from sky.spot.core import spot_cancel
+from sky.spot.core import spot_launch
+from sky.spot.core import spot_queue
+from sky.spot.core import spot_tail_logs
 from sky.status_lib import ClusterStatus
 from sky.task import Task
 
 # Aliases.
 IBM = clouds.IBM
 AWS = clouds.AWS
 Azure = clouds.Azure
@@ -169,14 +172,15 @@
     'down',
     'autostop',
     'cost_report',
     # core APIs Job Management
     'queue',
     'cancel',
     'tail_logs',
+    'spot_tail_logs',
     'download_logs',
     'job_status',
     # core APIs Spot Job Management
     'spot_queue',
     'spot_cancel',
     # core APIs Storage Management
     'storage_ls',
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/common.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/kubernetes.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/adaptors/vsphere.py` & `skypilot-nightly-1.0.0.dev20240412/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20240412/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/backends/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20240412/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/backends/backend_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6378,15 +6378,15 @@
 00018e90: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
 00018ea0: 2020 2023 2054 6865 2061 6371 7569 7265     # The acquire
 00018eb0: 5f6c 6f63 6b5f 7469 6d65 6f75 7420 6973  _lock_timeout is
 00018ec0: 2073 6574 2074 6f20 3020 746f 2061 766f   set to 0 to avo
 00018ed0: 6964 2068 616e 6769 6e67 2074 6865 2063  id hanging the c
 00018ee0: 6f6d 6d61 6e64 2077 6865 6e0a 2020 2020  ommand when.    
 00018ef0: 2020 2020 2320 6d75 6c74 6970 6c65 2073      # multiple s
-00018f00: 706f 745f 6c61 756e 6368 2063 6f6d 6d61  pot_launch comma
+00018f00: 706f 742e 6c61 756e 6368 2063 6f6d 6d61  pot.launch comma
 00018f10: 6e64 7320 6172 6520 7275 6e6e 696e 6720  nds are running 
 00018f20: 6174 2074 6865 2073 616d 6520 7469 6d65  at the same time
 00018f30: 2e20 4f75 7220 6c61 7465 720a 2020 2020  . Our later.    
 00018f40: 2020 2020 2320 636f 6465 2077 696c 6c20      # code will 
 00018f50: 6368 6563 6b20 6966 2074 6865 2063 6f6e  check if the con
 00018f60: 7472 6f6c 6c65 7220 6973 2061 6363 6573  troller is acces
 00018f70: 7369 626c 6520 6279 2064 6972 6563 746c  sible by directl
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20240412/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20240412/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20240412/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20240412/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/check.py` & `skypilot-nightly-1.0.0.dev20240412/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/cli.py` & `skypilot-nightly-1.0.0.dev20240412/sky/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1246,16 +1246,16 @@
     """
     num_in_progress_jobs = None
     try:
         if not is_called_by_user:
             usage_lib.messages.usage.set_internal()
         with sky_logging.silent():
             # Make the call silent
-            spot_jobs = core.spot_queue(refresh=refresh,
-                                        skip_finished=skip_finished)
+            spot_jobs = spot_lib.queue(refresh=refresh,
+                                       skip_finished=skip_finished)
         num_in_progress_jobs = len(spot_jobs)
     except exceptions.ClusterNotUpError as e:
         controller_status = e.cluster_status
         msg = str(e)
         if controller_status is None:
             msg += (f' (See: {colorama.Style.BRIGHT}sky spot -h'
                     f'{colorama.Style.RESET_ALL})')
@@ -2504,15 +2504,15 @@
 def _hint_or_raise_for_down_spot_controller(controller_name: str):
     controller = controller_utils.Controllers.from_name(controller_name)
     assert controller is not None, controller_name
 
     with rich_utils.safe_status(
             '[bold cyan]Checking for in-progress spot jobs[/]'):
         try:
-            spot_jobs = core.spot_queue(refresh=False, skip_finished=True)
+            spot_jobs = spot_lib.queue(refresh=False, skip_finished=True)
         except exceptions.ClusterNotUpError as e:
             if controller.value.connection_error_hint in str(e):
                 with ux_utils.print_exception_no_traceback():
                     raise exceptions.NotSupportedError(
                         controller.value.
                         decline_down_when_failed_to_fetch_status_hint)
             if e.cluster_status is None:
@@ -3285,15 +3285,15 @@
     if not yes:
         prompt = f'Launching the spot job {dag.name!r}. Proceed?'
         if prompt is not None:
             click.confirm(prompt, default=True, abort=True, show_default=True)
 
     common_utils.check_cluster_name_is_valid(name)
 
-    sky.spot_launch(dag,
+    spot_lib.launch(dag,
                     name,
                     detach_run=detach_run,
                     retry_until_up=retry_until_up)
 
 
 @spot.command('queue', cls=_DocumentedCodeCommand)
 @click.option('--all',
@@ -3444,15 +3444,15 @@
         if all:
             job_identity_str = 'all managed spot jobs'
         click.confirm(f'Cancelling {job_identity_str}. Proceed?',
                       default=True,
                       abort=True,
                       show_default=True)
 
-    core.spot_cancel(job_ids=job_ids, name=name, all=all)
+    spot_lib.cancel(job_ids=job_ids, name=name, all=all)
 
 
 @spot.command('logs', cls=_DocumentedCodeCommand)
 @click.option('--name',
               '-n',
               required=False,
               type=str,
@@ -3476,15 +3476,15 @@
     """Tail the log of a managed spot job."""
     try:
         if controller:
             core.tail_logs(spot_lib.SPOT_CONTROLLER_NAME,
                            job_id=job_id,
                            follow=follow)
         else:
-            core.spot_tail_logs(name=name, job_id=job_id, follow=follow)
+            spot_lib.tail_logs(name=name, job_id=job_id, follow=follow)
     except exceptions.ClusterNotUpError as e:
         click.echo(e)
         sys.exit(1)
 
 
 @spot.command('dashboard', cls=_DocumentedCodeCommand)
 @click.option(
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20240412/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/cloud_registry.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/cudo.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/fluidstack.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/kubernetes.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/paperspace.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/runpod.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/gcp_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/oci_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/utils/scp_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/clouds/vsphere.py` & `skypilot-nightly-1.0.0.dev20240412/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/core.py` & `skypilot-nightly-1.0.0.dev20240412/sky/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,22 @@
 from sky import backends
 from sky import clouds
 from sky import dag
 from sky import data
 from sky import exceptions
 from sky import global_user_state
 from sky import sky_logging
-from sky import spot
 from sky import status_lib
 from sky import task
 from sky.backends import backend_utils
 from sky.skylet import constants
 from sky.skylet import job_lib
 from sky.usage import usage_lib
 from sky.utils import controller_utils
-from sky.utils import rich_utils
 from sky.utils import subprocess_utils
-from sky.utils import ux_utils
 
 if typing.TYPE_CHECKING:
     from sky import resources as resources_lib
 
 logger = sky_logging.init_logger(__name__)
 
 # ======================
@@ -226,15 +223,15 @@
 @usage_lib.entrypoint
 def start(
     cluster_name: str,
     idle_minutes_to_autostop: Optional[int] = None,
     retry_until_up: bool = False,
     down: bool = False,  # pylint: disable=redefined-outer-name
     force: bool = False,
-) -> None:
+) -> backends.CloudVmRayResourceHandle:
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Restart a cluster.
 
     If a cluster is previously stopped (status is STOPPED) or failed in
     provisioning/runtime installation (status is INIT), this function will
     attempt to start the cluster.  In the latter case, provisioning and runtime
     installation will be retried.
@@ -275,19 +272,19 @@
           operation.
         sky.exceptions.ClusterOwnerIdentitiesMismatchError: if the cluster to
             restart was launched by a different user.
     """
     if down and idle_minutes_to_autostop is None:
         raise ValueError(
             '`idle_minutes_to_autostop` must be set if `down` is True.')
-    _start(cluster_name,
-           idle_minutes_to_autostop,
-           retry_until_up,
-           down,
-           force=force)
+    return _start(cluster_name,
+                  idle_minutes_to_autostop,
+                  retry_until_up,
+                  down,
+                  force=force)
 
 
 def _stop_not_supported_message(resources: 'resources_lib.Resources') -> str:
     if resources.use_spot:
         message = ('Stopping spot instances is currently not supported on '
                    f'{resources.cloud}')
     else:
@@ -758,186 +755,14 @@
                       f'{colorama.Style.RESET_ALL}')
 
     usage_lib.record_cluster_name_for_current_operation(cluster_name)
     statuses = backend.get_job_status(handle, job_ids, stream_logs=stream_logs)
     return statuses
 
 
-# =======================
-# = Spot Job Management =
-# =======================
-
-
-@usage_lib.entrypoint
-def spot_queue(refresh: bool,
-               skip_finished: bool = False) -> List[Dict[str, Any]]:
-    # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
-    """Get statuses of managed spot jobs.
-
-    Please refer to the sky.cli.spot_queue for the documentation.
-
-    Returns:
-        [
-            {
-                'job_id': int,
-                'job_name': str,
-                'resources': str,
-                'submitted_at': (float) timestamp of submission,
-                'end_at': (float) timestamp of end,
-                'duration': (float) duration in seconds,
-                'recovery_count': (int) Number of retries,
-                'status': (sky.spot.SpotStatus) of the job,
-                'cluster_resources': (str) resources of the cluster,
-                'region': (str) region of the cluster,
-            }
-        ]
-    Raises:
-        sky.exceptions.ClusterNotUpError: the spot controller is not up or
-            does not exist.
-        RuntimeError: if failed to get the spot jobs with ssh.
-    """
-    stopped_message = ''
-    if not refresh:
-        stopped_message = ('No in-progress spot jobs.')
-    try:
-        handle = backend_utils.is_controller_accessible(
-            controller_type=controller_utils.Controllers.SPOT_CONTROLLER,
-            stopped_message=stopped_message)
-    except exceptions.ClusterNotUpError as e:
-        if not refresh:
-            raise
-        handle = None
-        controller_status = e.cluster_status
-
-    if refresh and handle is None:
-        sky_logging.print(f'{colorama.Fore.YELLOW}'
-                          'Restarting controller for latest status...'
-                          f'{colorama.Style.RESET_ALL}')
-
-        rich_utils.force_update_status('[cyan] Checking spot jobs - restarting '
-                                       'controller[/]')
-        handle = _start(spot.SPOT_CONTROLLER_NAME)
-        controller_status = status_lib.ClusterStatus.UP
-        rich_utils.force_update_status('[cyan] Checking spot jobs[/]')
-
-    assert handle is not None, (controller_status, refresh)
-
-    backend = backend_utils.get_backend_from_handle(handle)
-    assert isinstance(backend, backends.CloudVmRayBackend)
-
-    code = spot.SpotCodeGen.get_job_table()
-    returncode, job_table_payload, stderr = backend.run_on_head(
-        handle,
-        code,
-        require_outputs=True,
-        stream_logs=False,
-        separate_stderr=True)
-
-    try:
-        subprocess_utils.handle_returncode(returncode,
-                                           code,
-                                           'Failed to fetch managed spot jobs',
-                                           job_table_payload + stderr,
-                                           stream_logs=False)
-    except exceptions.CommandError as e:
-        raise RuntimeError(str(e)) from e
-
-    jobs = spot.load_spot_job_queue(job_table_payload)
-    if skip_finished:
-        # Filter out the finished jobs. If a multi-task job is partially
-        # finished, we will include all its tasks.
-        non_finished_tasks = list(
-            filter(lambda job: not job['status'].is_terminal(), jobs))
-        non_finished_job_ids = {job['job_id'] for job in non_finished_tasks}
-        jobs = list(
-            filter(lambda job: job['job_id'] in non_finished_job_ids, jobs))
-    return jobs
-
-
-@usage_lib.entrypoint
-# pylint: disable=redefined-builtin
-def spot_cancel(name: Optional[str] = None,
-                job_ids: Optional[List[int]] = None,
-                all: bool = False) -> None:
-    # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
-    """Cancel managed spot jobs.
-
-    Please refer to the sky.cli.spot_cancel for the document.
-
-    Raises:
-        sky.exceptions.ClusterNotUpError: the spot controller is not up.
-        RuntimeError: failed to cancel the job.
-    """
-    job_ids = [] if job_ids is None else job_ids
-    handle = backend_utils.is_controller_accessible(
-        controller_type=controller_utils.Controllers.SPOT_CONTROLLER,
-        stopped_message='All managed spot jobs should have finished.')
-
-    job_id_str = ','.join(map(str, job_ids))
-    if sum([len(job_ids) > 0, name is not None, all]) != 1:
-        argument_str = f'job_ids={job_id_str}' if len(job_ids) > 0 else ''
-        argument_str += f' name={name}' if name is not None else ''
-        argument_str += ' all' if all else ''
-        raise ValueError('Can only specify one of JOB_IDS or name or all. '
-                         f'Provided {argument_str!r}.')
-
-    backend = backend_utils.get_backend_from_handle(handle)
-    assert isinstance(backend, backends.CloudVmRayBackend)
-    if all:
-        code = spot.SpotCodeGen.cancel_jobs_by_id(None)
-    elif job_ids:
-        code = spot.SpotCodeGen.cancel_jobs_by_id(job_ids)
-    else:
-        assert name is not None, (job_ids, name, all)
-        code = spot.SpotCodeGen.cancel_job_by_name(name)
-    # The stderr is redirected to stdout
-    returncode, stdout, _ = backend.run_on_head(handle,
-                                                code,
-                                                require_outputs=True,
-                                                stream_logs=False)
-    try:
-        subprocess_utils.handle_returncode(returncode, code,
-                                           'Failed to cancel managed spot job',
-                                           stdout)
-    except exceptions.CommandError as e:
-        raise RuntimeError(e.error_msg) from e
-
-    sky_logging.print(stdout)
-    if 'Multiple jobs found with name' in stdout:
-        with ux_utils.print_exception_no_traceback():
-            raise RuntimeError(
-                'Please specify the job ID instead of the job name.')
-
-
-@usage_lib.entrypoint
-def spot_tail_logs(name: Optional[str], job_id: Optional[int],
-                   follow: bool) -> None:
-    # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
-    """Tail logs of managed spot jobs.
-
-    Please refer to the sky.cli.spot_logs for the document.
-
-    Raises:
-        ValueError: invalid arguments.
-        sky.exceptions.ClusterNotUpError: the spot controller is not up.
-    """
-    # TODO(zhwu): Automatically restart the spot controller
-    handle = backend_utils.is_controller_accessible(
-        controller_type=controller_utils.Controllers.SPOT_CONTROLLER,
-        stopped_message=('Please restart the spot controller with '
-                         f'`sky start {spot.SPOT_CONTROLLER_NAME}`.'))
-
-    if name is not None and job_id is not None:
-        raise ValueError('Cannot specify both name and job_id.')
-    backend = backend_utils.get_backend_from_handle(handle)
-    assert isinstance(backend, backends.CloudVmRayBackend), backend
-    # Stream the realtime logs
-    backend.tail_spot_logs(handle, job_id=job_id, job_name=name, follow=follow)
-
-
 # ======================
 # = Storage Management =
 # ======================
 @usage_lib.entrypoint
 def storage_ls() -> List[Dict[str, Any]]:
     # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
     """Get the storages.
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/dag.py` & `skypilot-nightly-1.0.0.dev20240412/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20240412/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20240412/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20240412/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/execution.py` & `skypilot-nightly-1.0.0.dev20240412/sky/execution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,35 @@
 """Execution layer.
 
 See `Stage` for a Task's life cycle.
 """
-import copy
 import enum
 import os
-import tempfile
-from typing import Any, List, Optional, Tuple, Union
-import uuid
+from typing import List, Optional, Tuple, Union
 
 import colorama
 
 import sky
 from sky import backends
 from sky import clouds
 from sky import global_user_state
 from sky import optimizer
 from sky import sky_logging
-from sky import spot
-from sky import task as task_lib
 from sky.backends import backend_utils
-from sky.clouds.service_catalog import common as service_catalog_common
-from sky.skylet import constants
 from sky.usage import usage_lib
-from sky.utils import common_utils
 from sky.utils import controller_utils
 from sky.utils import dag_utils
 from sky.utils import env_options
 from sky.utils import rich_utils
 from sky.utils import subprocess_utils
 from sky.utils import timeline
 from sky.utils import ux_utils
 
 logger = sky_logging.init_logger(__name__)
 
-# Message thrown when APIs sky.{exec,launch,spot_launch}() received a string
-# instead of a Dag.  CLI (cli.py) is implemented by us so should not trigger
-# this.
-_ENTRYPOINT_STRING_AS_DAG_MESSAGE = """\
-Expected a sky.Task or sky.Dag but received a string.
-
-If you meant to run a command, make it a Task's run command:
-
-    task = sky.Task(run=command)
-
-The command can then be run as:
-
-  sky.exec(task, cluster_name=..., ...)
-  # Or use {'V100': 1}, 'V100:0.5', etc.
-  task.set_resources(sky.Resources(accelerators='V100:1'))
-  sky.exec(task, cluster_name=..., ...)
-
-  sky.launch(task, ...)
-
-  sky.spot_launch(task, ...)
-""".strip()
-
-
-def _convert_to_dag(entrypoint: Any) -> 'sky.Dag':
-    """Convert the entrypoint to a sky.Dag.
-
-    Raises TypeError if 'entrypoint' is not a 'sky.Task' or 'sky.Dag'.
-    """
-    # Not suppressing stacktrace: when calling this via API user may want to
-    # see their own program in the stacktrace. Our CLI impl would not trigger
-    # these errors.
-    if isinstance(entrypoint, str):
-        raise TypeError(_ENTRYPOINT_STRING_AS_DAG_MESSAGE)
-    elif isinstance(entrypoint, sky.Dag):
-        return copy.deepcopy(entrypoint)
-    elif isinstance(entrypoint, task_lib.Task):
-        entrypoint = copy.deepcopy(entrypoint)
-        with sky.Dag() as dag:
-            dag.add(entrypoint)
-            dag.name = entrypoint.name
-        return dag
-    else:
-        raise TypeError(
-            'Expected a sky.Task or sky.Dag but received argument of type: '
-            f'{type(entrypoint)}')
-
 
 class Stage(enum.Enum):
     """Stages for a run of a sky.Task."""
     # TODO: rename actual methods to be consistent.
     CLONE_DISK = enum.auto()
     OPTIMIZE = enum.auto()
     PROVISION = enum.auto()
@@ -206,15 +152,15 @@
     Returns:
       job_id: Optional[int]; the job ID of the submitted job. None if the
         backend is not CloudVmRayBackend, or no job is submitted to
         the cluster.
       handle: Optional[backends.ResourceHandle]; the handle to the cluster. None
         if dryrun.
     """
-    dag = _convert_to_dag(entrypoint)
+    dag = dag_utils.convert_entrypoint_to_dag(entrypoint)
     assert len(dag) == 1, f'We support 1 task for now. {dag}'
     task = dag.tasks[0]
 
     if task.need_spot_recovery:
         with ux_utils.print_exception_no_traceback():
             raise ValueError(
                 'Spot recovery is specified in the task. To launch the '
@@ -288,15 +234,15 @@
             bold = colorama.Style.BRIGHT
             reset = colorama.Style.RESET_ALL
             logger.info(
                 f'{yellow}Launching an unmanaged spot task, which does not '
                 f'automatically recover from preemptions.{reset}\n{yellow}To '
                 'get automatic recovery, use managed spot instead: '
                 f'{reset}{bold}sky spot launch{reset} {yellow}or{reset} '
-                f'{bold}sky.spot_launch(){reset}.')
+                f'{bold}sky.spot.launch(){reset}.')
 
         if Stage.OPTIMIZE in stages:
             if task.best_resources is None:
                 # TODO: fix this for the situation where number of requested
                 # accelerators is not an integer.
                 if isinstance(backend, backends.CloudVmRayBackend):
                     # TODO: adding this check because docker backend on a
@@ -610,116 +556,7 @@
         stages=[
             Stage.SYNC_WORKDIR,
             Stage.EXEC,
         ],
         cluster_name=cluster_name,
         detach_run=detach_run,
     )
-
-
-@usage_lib.entrypoint
-def spot_launch(
-    task: Union['sky.Task', 'sky.Dag'],
-    name: Optional[str] = None,
-    stream_logs: bool = True,
-    detach_run: bool = False,
-    retry_until_up: bool = False,
-):
-    # NOTE(dev): Keep the docstring consistent between the Python API and CLI.
-    """Launch a managed spot job.
-
-    Please refer to the sky.cli.spot_launch for the document.
-
-    Args:
-        task: sky.Task, or sky.Dag (experimental; 1-task only) to launch as a
-          managed spot job.
-        name: Name of the spot job.
-        detach_run: Whether to detach the run.
-
-    Raises:
-        ValueError: cluster does not exist.
-        sky.exceptions.NotSupportedError: the feature is not supported.
-    """
-    entrypoint = task
-    dag_uuid = str(uuid.uuid4().hex[:4])
-
-    dag = _convert_to_dag(entrypoint)
-    assert dag.is_chain(), ('Only single-task or chain DAG is '
-                            'allowed for spot_launch.', dag)
-
-    dag_utils.maybe_infer_and_fill_dag_and_task_names(dag)
-
-    task_names = set()
-    for task_ in dag.tasks:
-        if task_.name in task_names:
-            raise ValueError(
-                f'Task name {task_.name!r} is duplicated in the DAG. Either '
-                'change task names to be unique, or specify the DAG name only '
-                'and comment out the task names (so that they will be auto-'
-                'generated) .')
-        task_names.add(task_.name)
-
-    dag_utils.fill_default_spot_config_in_dag_for_spot_launch(dag)
-
-    for task_ in dag.tasks:
-        controller_utils.maybe_translate_local_file_mounts_and_sync_up(
-            task_, path='spot')
-
-    with tempfile.NamedTemporaryFile(prefix=f'spot-dag-{dag.name}-',
-                                     mode='w') as f:
-        dag_utils.dump_chain_dag_to_yaml(dag, f.name)
-        controller_name = spot.SPOT_CONTROLLER_NAME
-        prefix = spot.SPOT_TASK_YAML_PREFIX
-        remote_user_yaml_path = f'{prefix}/{dag.name}-{dag_uuid}.yaml'
-        remote_user_config_path = f'{prefix}/{dag.name}-{dag_uuid}.config_yaml'
-        controller_resources = (controller_utils.get_controller_resources(
-            controller_type='spot',
-            controller_resources_config=spot.constants.CONTROLLER_RESOURCES))
-
-        vars_to_fill = {
-            'remote_user_yaml_path': remote_user_yaml_path,
-            'user_yaml_path': f.name,
-            'spot_controller': controller_name,
-            # Note: actual spot cluster name will be <task.name>-<spot job ID>
-            'dag_name': dag.name,
-            'retry_until_up': retry_until_up,
-            'remote_user_config_path': remote_user_config_path,
-            'sky_python_cmd': constants.SKY_PYTHON_CMD,
-            'modified_catalogs':
-                service_catalog_common.get_modified_catalog_file_mounts(),
-            **controller_utils.shared_controller_vars_to_fill(
-                'spot',
-                remote_user_config_path=remote_user_config_path,
-            ),
-        }
-
-        yaml_path = os.path.join(spot.SPOT_CONTROLLER_YAML_PREFIX,
-                                 f'{name}-{dag_uuid}.yaml')
-        common_utils.fill_template(spot.SPOT_CONTROLLER_TEMPLATE,
-                                   vars_to_fill,
-                                   output_path=yaml_path)
-        controller_task = task_lib.Task.from_yaml(yaml_path)
-        assert len(controller_task.resources) == 1, controller_task
-        # Backward compatibility: if the user changed the
-        # spot-controller.yaml.j2 to customize the controller resources,
-        # we should use it.
-        controller_task_resources = list(controller_task.resources)[0]
-        if not controller_task_resources.is_empty():
-            controller_resources = controller_task_resources
-        controller_task.set_resources(controller_resources)
-
-        controller_task.spot_dag = dag
-        assert len(controller_task.resources) == 1
-
-        print(f'{colorama.Fore.YELLOW}'
-              f'Launching managed spot job {dag.name!r} from spot controller...'
-              f'{colorama.Style.RESET_ALL}')
-        print('Launching spot controller...')
-        _execute(
-            entrypoint=controller_task,
-            stream_logs=stream_logs,
-            cluster_name=controller_name,
-            detach_run=detach_run,
-            idle_minutes_to_autostop=constants.
-            CONTROLLER_IDLE_MINUTES_TO_AUTOSTOP,
-            retry_until_up=True,
-        )
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20240412/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20240412/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/aws/utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/azure/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/common.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/cudo_machine_type.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/cudo_wrapper.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/cudo/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/docker_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/fluidstack/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/fluidstack/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/instance_setup.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/network.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/network_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/kubernetes/utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/logging.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/metadata_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/constants.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/paperspace/utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/provisioner.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/runpod/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/runpod/utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/cls_api_client.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/metadata_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/service_manager.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/ssl_helper.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/vapiconnect.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/common/vim_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/instance.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/provision/vsphere/vsphere_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/resources.py` & `skypilot-nightly-1.0.0.dev20240412/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/autoscalers.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/constants.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/controller.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/core.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/load_balancer.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/load_balancing_policies.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/replica_managers.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/serve_state.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/serve_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/service.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/serve/service_spec.py` & `skypilot-nightly-1.0.0.dev20240412/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20240412/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20240412/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20240412/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/log_lib.pyi` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/command_runner.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Modules for managed spot clusters."""
 import pathlib
 
 from sky.spot.constants import SPOT_CLUSTER_NAME_PREFIX_LENGTH
 from sky.spot.constants import SPOT_CONTROLLER_TEMPLATE
 from sky.spot.constants import SPOT_CONTROLLER_YAML_PREFIX
 from sky.spot.constants import SPOT_TASK_YAML_PREFIX
+from sky.spot.core import cancel
+from sky.spot.core import launch
+from sky.spot.core import queue
+from sky.spot.core import tail_logs
 from sky.spot.recovery_strategy import SPOT_DEFAULT_STRATEGY
 from sky.spot.recovery_strategy import SPOT_STRATEGIES
 from sky.spot.spot_state import SpotStatus
 from sky.spot.spot_utils import dump_job_table_cache
 from sky.spot.spot_utils import dump_spot_job_queue
 from sky.spot.spot_utils import format_job_table
 from sky.spot.spot_utils import load_job_table_cache
@@ -24,14 +28,19 @@
     'SPOT_CONTROLLER_NAME',
     # Constants
     'SPOT_CONTROLLER_TEMPLATE',
     'SPOT_CONTROLLER_YAML_PREFIX',
     'SPOT_TASK_YAML_PREFIX',
     # Enums
     'SpotStatus',
+    # Core
+    'cancel',
+    'launch',
+    'queue',
+    'tail_logs',
     # utils
     'SpotCodeGen',
     'dump_job_table_cache',
     'load_job_table_cache',
     'format_job_table',
     'dump_spot_job_queue',
     'load_spot_job_queue',
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20240412/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/task.py` & `skypilot-nightly-1.0.0.dev20240412/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/cudo-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/fluidstack-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-ingress.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/paperspace-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/runpod-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/sky-serve-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/templates/vsphere-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20240412/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20240412/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20240412/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/cluster_yaml_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/command_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
                 f'{self.ssh_user}@{self.ip}:{source!r}',
                 f'{os.path.expanduser(target)!r}',
             ])
         command = ' '.join(rsync_command)
 
         backoff = common_utils.Backoff(initial_backoff=5, max_backoff_factor=5)
         while max_retry >= 0:
-            returncode, _, stderr = log_lib.run_with_log(
+            returncode, stdout, stderr = log_lib.run_with_log(
                 command,
                 log_path=log_path,
                 stream_logs=stream_logs,
                 shell=True,
                 require_outputs=True)
             if returncode == 0:
                 break
@@ -450,15 +450,15 @@
 
         direction = 'up' if up else 'down'
         error_msg = (f'Failed to rsync {direction}: {source} -> {target}. '
                      'Ensure that the network is stable, then retry.')
         subprocess_utils.handle_returncode(returncode,
                                            command,
                                            error_msg,
-                                           stderr=stderr,
+                                           stderr=stdout + stderr,
                                            stream_logs=stream_logs)
 
     def check_connection(self) -> bool:
         """Check if the connection to the remote machine is successful."""
         returncode = self.run('true', connect_timeout=5, stream_logs=False)
         if returncode:
             return False
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/command_runner.pyi` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/common_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -626,7 +626,24 @@
     os.makedirs(os.path.dirname(output_path), exist_ok=True)
 
     # Write out yaml config.
     j2_template = jinja2.Template(template)
     content = j2_template.render(**variables)
     with open(output_path, 'w', encoding='utf-8') as fout:
         fout.write(content)
+
+
+def deprecated_function(func: Callable, name: str, deprecated_name: str,
+                        removing_version: str) -> Callable:
+    """Decorator for creating deprecated functions, for backward compatibility.
+
+    It will result in a warning being emitted when the function is used.
+    """
+
+    @functools.wraps(func)
+    def new_func(*args, **kwargs):
+        logger.warning(
+            f'Call to deprecated function {deprecated_name}, which will be '
+            f'removed in {removing_version}. Please use {name}() instead.')
+        return func(*args, **kwargs)
+
+    return new_func
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/controller_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/controller_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 if typing.TYPE_CHECKING:
     from sky import task as task_lib
     from sky.backends import cloud_vm_ray_backend
 
 logger = sky_logging.init_logger(__name__)
 
-# Message thrown when APIs sky.spot_launch(),sky.serve.up() received an invalid
+# Message thrown when APIs sky.spot.launch(),sky.serve.up() received an invalid
 # controller resources spec.
 CONTROLLER_RESOURCES_NOT_VALID_MESSAGE = (
     '{controller_type} controller resources is not valid, please check '
     '~/.sky/config.yaml file and make sure '
     '{controller_type}.controller.resources is a valid resources spec. '
     'Details:\n  {err}')
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/create_cluster.sh` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/delete_cluster.sh` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/generate_kind_config.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/gpu_labeler.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/kubernetes_enums.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/resources_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/rich_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20240412/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240411
+Version: 1.0.0.dev20240412
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 sky/skylet/ray_patches/log_monitor.py.patch
 sky/skylet/ray_patches/resource_demand_scheduler.py.patch
 sky/skylet/ray_patches/updater.py.patch
 sky/skylet/ray_patches/worker.py.patch
 sky/spot/__init__.py
 sky/spot/constants.py
 sky/spot/controller.py
+sky/spot/core.py
 sky/spot/recovery_strategy.py
 sky/spot/spot_state.py
 sky/spot/spot_utils.py
 sky/spot/dashboard/dashboard.py
 sky/spot/dashboard/static/favicon.ico
 sky/spot/dashboard/templates/index.html
 sky/templates/aws-ray.yml.j2
```

### Comparing `skypilot-nightly-1.0.0.dev20240411/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20240412/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_serve_autoscaler.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_spot_serve.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_spot_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20240411/tests/test_yaml_parser.py` & `skypilot-nightly-1.0.0.dev20240412/tests/test_yaml_parser.py`

 * *Files identical despite different names*

