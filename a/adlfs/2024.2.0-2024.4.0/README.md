# Comparing `tmp/adlfs-2024.2.0.tar.gz` & `tmp/adlfs-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adlfs-2024.2.0.tar", last modified: Mon Feb  5 13:26:00 2024, max compression
+gzip compressed data, was "adlfs-2024.4.0.tar", last modified: Sat Apr 13 13:04:56 2024, max compression
```

## Comparing `adlfs-2024.2.0.tar` & `adlfs-2024.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:26:00.584037 adlfs-2024.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-05 13:25:49.000000 adlfs-2024.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:26:00.576037 adlfs-2024.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:26:00.576037 adlfs-2024.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-05 13:25:49.000000 adlfs-2024.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-05 13:25:49.000000 adlfs-2024.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-02-05 13:25:49.000000 adlfs-2024.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-05 13:25:49.000000 adlfs-2024.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 13:25:49.000000 adlfs-2024.2.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-05 13:25:49.000000 adlfs-2024.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-02-05 13:25:49.000000 adlfs-2024.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-05 13:25:49.000000 adlfs-2024.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-05 13:25:49.000000 adlfs-2024.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-05 13:25:49.000000 adlfs-2024.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-05 13:25:49.000000 adlfs-2024.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-02-05 13:26:00.584037 adlfs-2024.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-02-05 13:25:49.000000 adlfs-2024.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:26:00.580037 adlfs-2024.2.0/adlfs/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-05 13:26:00.000000 adlfs-2024.2.0/adlfs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/gen1.py
--rw-r--r--   0 runner    (1001) docker     (127)    78129 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:26:00.580037 adlfs-2024.2.0/adlfs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/tests/test_fetch_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/tests/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)    60736 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/tests/test_uri_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-05 13:25:49.000000 adlfs-2024.2.0/adlfs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:26:00.580037 adlfs-2024.2.0/adlfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-02-05 13:26:00.000000 adlfs-2024.2.0/adlfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-05 13:26:00.000000 adlfs-2024.2.0/adlfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 13:26:00.000000 adlfs-2024.2.0/adlfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-05 13:26:00.000000 adlfs-2024.2.0/adlfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-05 13:26:00.000000 adlfs-2024.2.0/adlfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 13:26:00.000000 adlfs-2024.2.0/adlfs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:26:00.580037 adlfs-2024.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-05 13:25:49.000000 adlfs-2024.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-05 13:25:49.000000 adlfs-2024.2.0/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-02-05 13:25:49.000000 adlfs-2024.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-02-05 13:25:49.000000 adlfs-2024.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-05 13:25:49.000000 adlfs-2024.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-05 13:25:49.000000 adlfs-2024.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-05 13:25:49.000000 adlfs-2024.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 13:26:00.580037 adlfs-2024.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-05 13:25:49.000000 adlfs-2024.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-05 13:25:49.000000 adlfs-2024.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-05 13:25:49.000000 adlfs-2024.2.0/requirements/earliest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-05 13:25:49.000000 adlfs-2024.2.0/requirements/latest.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-05 13:26:00.584037 adlfs-2024.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.515181 adlfs-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.507181 adlfs-2024.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.507181 adlfs-2024.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 13:04:43.000000 adlfs-2024.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-13 13:04:43.000000 adlfs-2024.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-13 13:04:43.000000 adlfs-2024.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 13:04:43.000000 adlfs-2024.4.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-13 13:04:43.000000 adlfs-2024.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-13 13:04:43.000000 adlfs-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-13 13:04:56.515181 adlfs-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-13 13:04:43.000000 adlfs-2024.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.507181 adlfs-2024.4.0/adlfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/gen1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78702 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.511181 adlfs-2024.4.0/adlfs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/test_fetch_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61876 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/tests/test_uri_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-13 13:04:43.000000 adlfs-2024.4.0/adlfs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.511181 adlfs-2024.4.0/adlfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 13:04:56.000000 adlfs-2024.4.0/adlfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.511181 adlfs-2024.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-13 13:04:43.000000 adlfs-2024.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-13 13:04:43.000000 adlfs-2024.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:04:56.511181 adlfs-2024.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-13 13:04:43.000000 adlfs-2024.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 13:04:43.000000 adlfs-2024.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-13 13:04:43.000000 adlfs-2024.4.0/requirements/earliest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-13 13:04:43.000000 adlfs-2024.4.0/requirements/latest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-13 13:04:56.515181 adlfs-2024.4.0/setup.cfg
```

### Comparing `adlfs-2024.2.0/.github/workflows/docs.yml` & `adlfs-2024.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/.github/workflows/release.yml` & `adlfs-2024.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/.github/workflows/tests.yml` & `adlfs-2024.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/.gitignore` & `adlfs-2024.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/CHANGELOG.md` & `adlfs-2024.4.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/CONTRIBUTING.md` & `adlfs-2024.4.0/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 To develop ``adlfs`` it best to work in an virtual environment.
 You can create a virtual environment using ``conda`` and install the development dependencies as follows:
 
 ```bash
 $ conda create -n adlfs-dev python=3.8
 $ conda activate adlfs-dev
-$ pip install -r requirements/latest.txt
+$ pip install -r requirements/latest.txt -r requirements.dev
 ```
 
 You can run tests from the main directory as follows:
 ```bash
 $ py.test adlfs/tests
 ```
```

### Comparing `adlfs-2024.2.0/LICENSE.txt` & `adlfs-2024.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/PKG-INFO` & `adlfs-2024.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlfs
-Version: 2024.2.0
+Version: 2024.4.0
 Summary: Access Azure Datalake Gen1 with fsspec and dask
 Maintainer-email: Greg Hayes <hayesgb@gmail.com>
 License: BSD
 Keywords: file-system,dask,azure
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -105,15 +105,18 @@
 ### Setting credentials
 The `storage_options` can be instantiated with a variety of keyword arguments depending on the filesystem. The most commonly used arguments are:
 - `connection_string`
 - `account_name`
 - `account_key`
 - `sas_token`
 - `tenant_id`, `client_id`, and `client_secret` are combined for an Azure ServicePrincipal e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`
-- `anon`: `True` or `False`. The default value for anon (i.e. anonymous) is True
+- `anon`: boo, optional.
+   The value to use for whether to attempt anonymous access if no other credential is passed. By default (`None`), the
+   `AZURE_STORAGE_ANON` environment variable is checked. False values (`false`, `0`, `f`) will resolve to `False` and
+   anonymous access will not be attempted. Otherwise the value for `anon` resolves to True.
 - `location_mode`: valid values are "primary" or "secondary" and apply to RA-GRS accounts
 
 For more argument details see all arguments for [`AzureBlobFileSystem` here](https://github.com/fsspec/adlfs/blob/f15c37a43afd87a04f01b61cd90294dd57181e1d/adlfs/spec.py#L328) and [`AzureDatalakeFileSystem` here](https://github.com/fsspec/adlfs/blob/f15c37a43afd87a04f01b61cd90294dd57181e1d/adlfs/spec.py#L69).
 
 The following environmental variables can also be set and picked up for authentication:
 - "AZURE_STORAGE_CONNECTION_STRING"
 - "AZURE_STORAGE_ACCOUNT_NAME"
@@ -122,13 +125,14 @@
 - "AZURE_STORAGE_TENANT_ID"
 - "AZURE_STORAGE_CLIENT_ID"
 - "AZURE_STORAGE_CLIENT_SECRET"
 
 The filesystem can be instantiated for different use cases based on a variety of `storage_options` combinations. The following list describes some common use cases utilizing `AzureBlobFileSystem`, i.e. protocols `abfs`or `az`. Note that all cases require the `account_name` argument to be provided:
 1. Anonymous connection to public container: `storage_options={'account_name': ACCOUNT_NAME, 'anon': True}` will assume the `ACCOUNT_NAME` points to a public container, and attempt to use an anonymous login. Note, the default value for `anon` is True.
 2. Auto credential solving using Azure's DefaultAzureCredential() library: `storage_options={'account_name': ACCOUNT_NAME, 'anon': False}` will use [`DefaultAzureCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python) to get valid credentials to the container `ACCOUNT_NAME`. `DefaultAzureCredential` attempts to authenticate via the [mechanisms and order visualized here](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme?view=azure-python#defaultazurecredential).
-3. Azure ServicePrincipal: `tenant_id`, `client_id`, and `client_secret` are all used as credentials for an Azure ServicePrincipal: e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`.
+3. Auto credential solving without requiring `storage_options`: Set `AZURE_STORAGE_ANON` to `false`, resulting in automatic credential resolution. Useful for compatibility with fsspec.
+4. Azure ServicePrincipal: `tenant_id`, `client_id`, and `client_secret` are all used as credentials for an Azure ServicePrincipal: e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`.
 
 ### Append Blob
 The `AzureBlobFileSystem` accepts [all of the Async BlobServiceClient arguments](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-quickstart-blobs-python).
 
 By default, write operations create BlockBlobs in Azure, which, once written can not be appended. It is possible to create an AppendBlob using `mode="ab"` when creating and operating on blobs. Currently, AppendBlobs are not available if hierarchical namespaces are enabled.
```

### Comparing `adlfs-2024.2.0/README.md` & `adlfs-2024.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -71,15 +71,18 @@
 ### Setting credentials
 The `storage_options` can be instantiated with a variety of keyword arguments depending on the filesystem. The most commonly used arguments are:
 - `connection_string`
 - `account_name`
 - `account_key`
 - `sas_token`
 - `tenant_id`, `client_id`, and `client_secret` are combined for an Azure ServicePrincipal e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`
-- `anon`: `True` or `False`. The default value for anon (i.e. anonymous) is True
+- `anon`: boo, optional.
+   The value to use for whether to attempt anonymous access if no other credential is passed. By default (`None`), the
+   `AZURE_STORAGE_ANON` environment variable is checked. False values (`false`, `0`, `f`) will resolve to `False` and
+   anonymous access will not be attempted. Otherwise the value for `anon` resolves to True.
 - `location_mode`: valid values are "primary" or "secondary" and apply to RA-GRS accounts
 
 For more argument details see all arguments for [`AzureBlobFileSystem` here](https://github.com/fsspec/adlfs/blob/f15c37a43afd87a04f01b61cd90294dd57181e1d/adlfs/spec.py#L328) and [`AzureDatalakeFileSystem` here](https://github.com/fsspec/adlfs/blob/f15c37a43afd87a04f01b61cd90294dd57181e1d/adlfs/spec.py#L69).
 
 The following environmental variables can also be set and picked up for authentication:
 - "AZURE_STORAGE_CONNECTION_STRING"
 - "AZURE_STORAGE_ACCOUNT_NAME"
@@ -88,13 +91,14 @@
 - "AZURE_STORAGE_TENANT_ID"
 - "AZURE_STORAGE_CLIENT_ID"
 - "AZURE_STORAGE_CLIENT_SECRET"
 
 The filesystem can be instantiated for different use cases based on a variety of `storage_options` combinations. The following list describes some common use cases utilizing `AzureBlobFileSystem`, i.e. protocols `abfs`or `az`. Note that all cases require the `account_name` argument to be provided:
 1. Anonymous connection to public container: `storage_options={'account_name': ACCOUNT_NAME, 'anon': True}` will assume the `ACCOUNT_NAME` points to a public container, and attempt to use an anonymous login. Note, the default value for `anon` is True.
 2. Auto credential solving using Azure's DefaultAzureCredential() library: `storage_options={'account_name': ACCOUNT_NAME, 'anon': False}` will use [`DefaultAzureCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python) to get valid credentials to the container `ACCOUNT_NAME`. `DefaultAzureCredential` attempts to authenticate via the [mechanisms and order visualized here](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme?view=azure-python#defaultazurecredential).
-3. Azure ServicePrincipal: `tenant_id`, `client_id`, and `client_secret` are all used as credentials for an Azure ServicePrincipal: e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`.
+3. Auto credential solving without requiring `storage_options`: Set `AZURE_STORAGE_ANON` to `false`, resulting in automatic credential resolution. Useful for compatibility with fsspec.
+4. Azure ServicePrincipal: `tenant_id`, `client_id`, and `client_secret` are all used as credentials for an Azure ServicePrincipal: e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`.
 
 ### Append Blob
 The `AzureBlobFileSystem` accepts [all of the Async BlobServiceClient arguments](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-quickstart-blobs-python).
 
 By default, write operations create BlockBlobs in Azure, which, once written can not be appended. It is possible to create an AppendBlob using `mode="ab"` when creating and operating on blobs. Currently, AppendBlobs are not available if hierarchical namespaces are enabled.
```

### Comparing `adlfs-2024.2.0/adlfs/gen1.py` & `adlfs-2024.4.0/adlfs/gen1.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/adlfs/spec.py` & `adlfs-2024.4.0/adlfs/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,37 +143,43 @@
     request_session: Session
         The session object to use for http requests.
     connection_string: str
         If specified, this will override all other parameters besides
         request session. See
         http://azure.microsoft.com/en-us/documentation/articles/storage-configure-connection-string/
         for the connection string format.
-    credential: TokenCredential or SAS token
+    credential: azure.core.credentials_async.AsyncTokenCredential or SAS token
         The credentials with which to authenticate.  Optional if the account URL already has a SAS token.
-        Can include an instance of TokenCredential class from azure.identity
+        Can include an instance of TokenCredential class from azure.identity.aio.
     blocksize: int
         The block size to use for download/upload operations. Defaults to hardcoded value of
         ``BlockBlobService.MAX_BLOCK_SIZE``
     client_id: str
         Client ID to use when authenticating using an AD Service Principal client/secret.
     client_secret: str
         Client secret to use when authenticating using an AD Service Principal client/secret.
     tenant_id: str
         Tenant ID to use when authenticating using an AD Service Principal client/secret.
+    anon: boolean, optional
+        The value to use for whether to attempt anonymous access if no other credential is
+        passed. By default (``None``), the ``AZURE_STORAGE_ANON`` environment variable is
+        checked. False values (``false``, ``0``, ``f``) will resolve to `False` and
+        anonymous access will not be attempted. Otherwise the value for ``anon`` resolves
+        to ``True``.
     default_fill_cache: bool = True
-        Whether to use cache filling with opoen by default
+        Whether to use cache filling with open by default
     default_cache_type: string ('bytes')
         If given, the default cache_type value used for "open()".  Set to none if no caching
         is desired.  Docs in fsspec
     version_aware : bool (False)
         Whether to support blob versioning.  If enable this will require the
         user to have the necessary permissions for dealing with versioned blobs.
     assume_container_exists: Optional[bool] (None)
-        Set this to true to not check for existance of containers at all, assuming they exist.
-        None (default) means to warn in case of a failure when checking for existance of a container
+        Set this to true to not check for existence of containers at all, assuming they exist.
+        None (default) means to warn in case of a failure when checking for existence of a container
         False throws if retrieving container properties fails, which might happen if your
         authentication is only valid at the storage container level, and not the
         storage account level.
     max_concurrency:
         The number of concurrent connections to use when uploading or downloading a blob.
         If None it will be inferred from fsspec.asyn._get_batch_size().
     timeout: int
@@ -235,15 +241,15 @@
         sas_token: str = None,
         request_session=None,
         socket_timeout=_SOCKET_TIMEOUT_DEFAULT,
         blocksize: int = _DEFAULT_BLOCK_SIZE,
         client_id: str = None,
         client_secret: str = None,
         tenant_id: str = None,
-        anon: bool = True,
+        anon: bool = None,
         location_mode: str = "primary",
         loop=None,
         asynchronous: bool = False,
         default_fill_cache: bool = True,
         default_cache_type: str = "bytes",
         version_aware: bool = False,
         assume_container_exists: Optional[bool] = None,
@@ -267,15 +273,19 @@
         self.connection_string = connection_string or os.getenv(
             "AZURE_STORAGE_CONNECTION_STRING"
         )
         self.sas_token = sas_token or os.getenv("AZURE_STORAGE_SAS_TOKEN")
         self.client_id = client_id or os.getenv("AZURE_STORAGE_CLIENT_ID")
         self.client_secret = client_secret or os.getenv("AZURE_STORAGE_CLIENT_SECRET")
         self.tenant_id = tenant_id or os.getenv("AZURE_STORAGE_TENANT_ID")
-        self.anon = anon
+        self.anon = anon or os.getenv("AZURE_STORAGE_ANON", "true").lower() not in [
+            "false",
+            "0",
+            "f",
+        ]
         self.location_mode = location_mode
         self.credential = credential
         self.request_session = request_session
         self.assume_container_exists = assume_container_exists
         if socket_timeout is not _SOCKET_TIMEOUT_DEFAULT:
             warnings.warn(
                 "socket_timeout is deprecated and has no effect.", FutureWarning
@@ -1216,15 +1226,15 @@
                 if ex is not None:
                     raise ex
 
             # Directory markers of non-empty directories must be deleted in reverse order to avoid deleting a directory
             # marker before the directory is empty. If these are deleted out of order we will get
             # `This operation is not permitted on a non-empty directory.` on hierarchical namespace storage accounts.
             for directory_marker in reversed(directory_markers):
-                cc.delete_blob(directory_marker)
+                await cc.delete_blob(directory_marker)
 
         for file in file_paths:
             self.invalidate_cache(self._parent(file))
 
     sync_wrapper(_rm_files)
 
     async def _separate_directory_markers_for_non_empty_directories(
```

### Comparing `adlfs-2024.2.0/adlfs/tests/conftest.py` & `adlfs-2024.4.0/adlfs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/adlfs/tests/test_fetch_range.py` & `adlfs-2024.4.0/adlfs/tests/test_fetch_range.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/adlfs/tests/test_loop.py` & `adlfs-2024.4.0/adlfs/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/adlfs/tests/test_spec.py` & `adlfs-2024.4.0/adlfs/tests/test_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
+import os
 import tempfile
 from unittest import mock
 
-import azure.storage.blob
 import azure.storage.blob.aio
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.testing import assert_frame_equal
 
@@ -26,14 +26,25 @@
     assert abs(x - y) <= threshold
 
 
 def test_connect(storage):
     AzureBlobFileSystem(account_name=storage.account_name, connection_string=CONN_STR)
 
 
+def test_anon_env(storage):
+    with mock.patch.dict(os.environ, {"AZURE_STORAGE_ANON": "false"}):
+        # Setting cachable to false to avoid re-testing the instance from the previous test
+        AzureBlobFileSystem.cachable = False
+        x = AzureBlobFileSystem(
+            account_name=storage.account_name, connection_string=CONN_STR
+        )
+        assert not x.anon
+        AzureBlobFileSystem.cachable = True  # Restoring cachable value
+
+
 def assert_blob_equals(blob, expected_blob):
     irregular_props = [
         "etag",
         "deleted",
     ]
 
     time_based_props = [
@@ -751,34 +762,60 @@
         fs.ls("data/root/c")
 
     assert mock_delete_blob.mock_calls[-1] == mock.call(
         mock.ANY, "root/c"
     ), "The directory deletion should be the last call"
 
 
-@mock.patch.object(
-    azure.storage.blob.aio.ContainerClient,
-    "delete_blob",
-    side_effect=azure.storage.blob.aio.ContainerClient.delete_blob,
-    autospec=True,
-)
-def test_rm_recursive2(mock_delete_blob, storage):
+@pytest.mark.filterwarnings("error")
+def test_rm_recursive2(storage):
     fs = AzureBlobFileSystem(
         account_name=storage.account_name, connection_string=CONN_STR
     )
 
     assert "data/root" in fs.ls("/data")
 
     fs.rm("data/root", recursive=True)
     assert "data/root" not in fs.ls("/data")
 
     with pytest.raises(FileNotFoundError):
         fs.ls("data/root")
 
-    last_deleted_paths = [call.args[1] for call in mock_delete_blob.mock_calls[-7:]]
+
+async def test_rm_recursive_call_order(storage, mocker):
+    from azure.storage.blob.aio import ContainerClient
+
+    delete_blob_mock = mocker.patch.object(
+        ContainerClient, "delete_blob", return_value=None
+    )
+    fs = AzureBlobFileSystem(
+        account_name=storage.account_name, connection_string=CONN_STR
+    )
+
+    container_name = "data"
+    file_paths = [
+        "root/a",
+        "root/a/file.txt",
+        "root/a1",
+        "root/a1/file1.txt",
+        "root/b",
+        "root/b/file.txt",
+        "root",
+        "root/c",
+        "root/c/file1.txt",
+        "root/c/file2.txt",
+        "root/d",
+        "root/d/file_with_metadata.txt",
+        "root/e+f",
+        "root/e+f/file1.txt",
+        "root/e+f/file2.txt",
+        "root/rfile.txt",
+    ]
+    await fs._rm_files(container_name=container_name, file_paths=file_paths)
+    last_deleted_paths = [call.args[0] for call in delete_blob_mock.call_args_list[-7:]]
     assert last_deleted_paths == [
         "root/e+f",
         "root/d",
         "root/c",
         "root/b",
         "root/a1",
         "root/a",
```

### Comparing `adlfs-2024.2.0/adlfs/tests/test_uri_format.py` & `adlfs-2024.4.0/adlfs/tests/test_uri_format.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/adlfs/utils.py` & `adlfs-2024.4.0/adlfs/utils.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/adlfs.egg-info/PKG-INFO` & `adlfs-2024.4.0/adlfs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adlfs
-Version: 2024.2.0
+Version: 2024.4.0
 Summary: Access Azure Datalake Gen1 with fsspec and dask
 Maintainer-email: Greg Hayes <hayesgb@gmail.com>
 License: BSD
 Keywords: file-system,dask,azure
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -105,15 +105,18 @@
 ### Setting credentials
 The `storage_options` can be instantiated with a variety of keyword arguments depending on the filesystem. The most commonly used arguments are:
 - `connection_string`
 - `account_name`
 - `account_key`
 - `sas_token`
 - `tenant_id`, `client_id`, and `client_secret` are combined for an Azure ServicePrincipal e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`
-- `anon`: `True` or `False`. The default value for anon (i.e. anonymous) is True
+- `anon`: boo, optional.
+   The value to use for whether to attempt anonymous access if no other credential is passed. By default (`None`), the
+   `AZURE_STORAGE_ANON` environment variable is checked. False values (`false`, `0`, `f`) will resolve to `False` and
+   anonymous access will not be attempted. Otherwise the value for `anon` resolves to True.
 - `location_mode`: valid values are "primary" or "secondary" and apply to RA-GRS accounts
 
 For more argument details see all arguments for [`AzureBlobFileSystem` here](https://github.com/fsspec/adlfs/blob/f15c37a43afd87a04f01b61cd90294dd57181e1d/adlfs/spec.py#L328) and [`AzureDatalakeFileSystem` here](https://github.com/fsspec/adlfs/blob/f15c37a43afd87a04f01b61cd90294dd57181e1d/adlfs/spec.py#L69).
 
 The following environmental variables can also be set and picked up for authentication:
 - "AZURE_STORAGE_CONNECTION_STRING"
 - "AZURE_STORAGE_ACCOUNT_NAME"
@@ -122,13 +125,14 @@
 - "AZURE_STORAGE_TENANT_ID"
 - "AZURE_STORAGE_CLIENT_ID"
 - "AZURE_STORAGE_CLIENT_SECRET"
 
 The filesystem can be instantiated for different use cases based on a variety of `storage_options` combinations. The following list describes some common use cases utilizing `AzureBlobFileSystem`, i.e. protocols `abfs`or `az`. Note that all cases require the `account_name` argument to be provided:
 1. Anonymous connection to public container: `storage_options={'account_name': ACCOUNT_NAME, 'anon': True}` will assume the `ACCOUNT_NAME` points to a public container, and attempt to use an anonymous login. Note, the default value for `anon` is True.
 2. Auto credential solving using Azure's DefaultAzureCredential() library: `storage_options={'account_name': ACCOUNT_NAME, 'anon': False}` will use [`DefaultAzureCredential`](https://learn.microsoft.com/en-us/python/api/azure-identity/azure.identity.defaultazurecredential?view=azure-python) to get valid credentials to the container `ACCOUNT_NAME`. `DefaultAzureCredential` attempts to authenticate via the [mechanisms and order visualized here](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme?view=azure-python#defaultazurecredential).
-3. Azure ServicePrincipal: `tenant_id`, `client_id`, and `client_secret` are all used as credentials for an Azure ServicePrincipal: e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`.
+3. Auto credential solving without requiring `storage_options`: Set `AZURE_STORAGE_ANON` to `false`, resulting in automatic credential resolution. Useful for compatibility with fsspec.
+4. Azure ServicePrincipal: `tenant_id`, `client_id`, and `client_secret` are all used as credentials for an Azure ServicePrincipal: e.g. `storage_options={'account_name': ACCOUNT_NAME, 'tenant_id': TENANT_ID, 'client_id': CLIENT_ID, 'client_secret': CLIENT_SECRET}`.
 
 ### Append Blob
 The `AzureBlobFileSystem` accepts [all of the Async BlobServiceClient arguments](https://docs.microsoft.com/en-us/azure/storage/blobs/storage-quickstart-blobs-python).
 
 By default, write operations create BlockBlobs in Azure, which, once written can not be appended. It is possible to create an AppendBlob using `mode="ab"` when creating and operating on blobs. Currently, AppendBlobs are not available if hierarchical namespaces are enabled.
```

### Comparing `adlfs-2024.2.0/adlfs.egg-info/SOURCES.txt` & `adlfs-2024.4.0/adlfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/docs/Makefile` & `adlfs-2024.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/docs/conf.py` & `adlfs-2024.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/docs/index.md` & `adlfs-2024.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/docs/make.bat` & `adlfs-2024.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `adlfs-2024.2.0/pyproject.toml` & `adlfs-2024.4.0/pyproject.toml`

 * *Files identical despite different names*

