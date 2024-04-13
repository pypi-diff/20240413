# Comparing `tmp/repod-0.3.0.post0.tar.gz` & `tmp/repod-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repod-0.3.0.post0.tar", last modified: Tue Jul 18 07:14:35 2023, max compression
+gzip compressed data, was "repod-0.3.1.tar", last modified: Sat Apr 13 12:31:29 2024, max compression
```

## Comparing `repod-0.3.0.post0.tar` & `repod-0.3.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-lrwxr-xr-x   0        0        0        0 2023-07-18 07:14:23.251012 repod-0.3.0.post0/AUTHORS.rst -> docs/authors.rst
--rw-r--r--   0        0        0    35149 2023-07-18 07:14:23.251012 repod-0.3.0.post0/LICENSE
--rw-r--r--   0        0        0    35149 2023-07-18 07:14:23.251012 repod-0.3.0.post0/LICENSE
--rw-r--r--   0        0        0     1741 2023-07-18 07:14:23.251012 repod-0.3.0.post0/Makefile
--rw-r--r--   0        0        0     1551 2023-07-18 07:14:23.251012 repod-0.3.0.post0/README.md
--rw-r--r--   0        0        0    22964 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/LICENSE
--rw-r--r--   0        0        0      634 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/Makefile
--rw-r--r--   0        0        0    20138 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/artwork/LICENSE
--rw-r--r--   0        0        0     4286 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/artwork/logo.ico
--rw-r--r--   0        0        0    15160 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/artwork/logo.png
--rw-r--r--   0        0        0     1509 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/artwork/repod.svg
--rw-r--r--   0        0        0      484 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/authors.rst
--rw-r--r--   0        0        0     2610 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/conf.py
--rw-r--r--   0        0        0     4011 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/contributing.rst
--rw-r--r--   0        0        0     1295 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/index.rst
--rw-r--r--   0        0        0     4107 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/packages/contents.rst
--rw-r--r--   0        0        0     1164 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/packages/signatures.rst
--rw-r--r--   0        0        0    12784 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/changelog.rst
--rw-r--r--   0        0        0     2000 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/installation.rst
--rw-r--r--   0        0        0       84 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/man/index.rst
--rw-r--r--   0        0        0    23153 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/man/repod_conf.rst
--rw-r--r--   0        0        0     2421 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/man/repod_file.rst
--rw-r--r--   0        0        0     5846 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repod/usage.rst
--rw-r--r--   0        0        0     2119 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/binary_repository.rst
--rw-r--r--   0        0        0     5101 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/management_repository.rst
--rw-r--r--   0        0        0     3177 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/source_repository.rst
--rw-r--r--   0        0        0     1077 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/source_tarball_repository.rst
--rw-r--r--   0        0        0     8834 2023-07-18 07:14:23.254346 repod-0.3.0.post0/docs/repositories/sync_database.rst
--rw-r--r--   0        0        0     5027 2023-07-18 07:14:35.304535 repod-0.3.0.post0/pyproject.toml
--rw-r--r--   0        0        0      502 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/__init__.py
--rw-r--r--   0        0        0    31984 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/action/check.py
--rw-r--r--   0        0        0    97335 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/action/task.py
--rw-r--r--   0        0        0    12824 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/action/workflow.py
--rw-r--r--   0        0        0     3154 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/archive/archive.py
--rw-r--r--   0        0        0       81 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/cli/__init__.py
--rw-r--r--   0        0        0    13334 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/cli/argparse.py
--rw-r--r--   0        0        0     8472 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/cli/cli.py
--rw-r--r--   0        0        0     2295 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/commands.py
--rw-r--r--   0        0        0    11902 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/common/enums.py
--rw-r--r--   0        0        0    18711 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/common/models.py
--rw-r--r--   0        0        0     1397 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/common/regex.py
--rw-r--r--   0        0        0      147 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/config/__init__.py
--rw-r--r--   0        0        0     2213 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/config/defaults.py
--rw-r--r--   0        0        0   105128 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/config/settings.py
--rw-r--r--   0        0        0      845 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/errors.py
--rw-r--r--   0        0        0     1269 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/__init__.py
--rw-r--r--   0        0        0    14590 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/buildinfo.py
--rw-r--r--   0        0        0     8789 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/common.py
--rw-r--r--   0        0        0    14183 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/mtree.py
--rw-r--r--   0        0        0     7319 2023-07-18 07:14:23.257679 repod-0.3.0.post0/repod/files/package.py
--rw-r--r--   0        0        0    15956 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/files/pkginfo.py
--rw-r--r--   0        0        0    20922 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/files/srcinfo.py
--rw-r--r--   0        0        0        0 2023-07-18 07:14:23.294346 repod-0.3.0.post0/repod/py.typed
--rw-r--r--   0        0        0     1003 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/__init__.py
--rw-r--r--   0        0        0      226 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/management/__init__.py
--rw-r--r--   0        0        0    35361 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/management/outputpackage.py
--rw-r--r--   0        0        0      943 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/package/__init__.py
--rw-r--r--   0        0        0    13103 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/package/repofile.py
--rw-r--r--   0        0        0    48850 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/repo/package/syncdb.py
--rw-r--r--   0        0        0     1271 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/templates/desc_v1.j2
--rw-r--r--   0        0        0     1232 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/templates/desc_v2.j2
--rw-r--r--   0        0        0       84 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/templates/files_v1.j2
--rw-r--r--   0        0        0      113 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/verification/__init__.py
--rw-r--r--   0        0        0     1688 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/verification/pgp.py
--rw-r--r--   0        0        0       47 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/version/__init__.py
--rw-r--r--   0        0        0     5461 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/version/alpm.py
--rw-r--r--   0        0        0      626 2023-07-18 07:14:23.261012 repod-0.3.0.post0/repod/version/util.py
--rw-r--r--   0        0        0       23 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/__init__.py
--rw-r--r--   0        0        0    12495 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/action/test_check.py
--rw-r--r--   0        0        0    85867 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/action/test_task.py
--rw-r--r--   0        0        0     8604 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/action/test_workflow.py
--rw-r--r--   0        0        0     3195 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/archive/test_archive.py
--rw-r--r--   0        0        0     4414 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/cli/test_argparse.py
--rw-r--r--   0        0        0    20655 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/cli/test_cli.py
--rw-r--r--   0        0        0     3489 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/common/test_enums.py
--rw-r--r--   0        0        0    11693 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/common/test_models.py
--rw-r--r--   0        0        0     5473 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/common/test_regex.py
--rw-r--r--   0        0        0   101383 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/config/test_settings.py
--rw-r--r--   0        0        0    59495 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/conftest.py
--rw-r--r--   0        0        0     8991 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_buildinfo.py
--rw-r--r--   0        0        0     7166 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_common.py
--rw-r--r--   0        0        0      220 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_files_init.py
--rw-r--r--   0        0        0    16214 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_mtree.py
--rw-r--r--   0        0        0     2480 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_package.py
--rw-r--r--   0        0        0     6711 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_pkginfo.py
--rw-r--r--   0        0        0     5094 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/files/test_srcinfo.py
--rw-r--r--   0        0        0    11279 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/repo/management/test_outputpackage.py
--rw-r--r--   0        0        0    13599 2023-07-18 07:14:23.261012 repod-0.3.0.post0/tests/repo/package/test_repofile.py
--rw-r--r--   0        0        0    33240 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/repo/package/test_syncdb.py
--rw-r--r--   0        0        0      216 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/repo/test_repo_init.py
--rw-r--r--   0        0        0     1248 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/test_commands.py
--rw-r--r--   0        0        0      197 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/test_repod_init.py
--rw-r--r--   0        0        0     2202 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/verification/test_pgp.py
--rw-r--r--   0        0        0     2414 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/version/test_alpm.py
--rw-r--r--   0        0        0      613 2023-07-18 07:14:23.264346 repod-0.3.0.post0/tests/version/test_util.py
--rw-r--r--   0        0        0     3630 1970-01-01 00:00:00.000000 repod-0.3.0.post0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2024-04-13 12:31:08.837226 repod-0.3.1/AUTHORS.rst -> docs/authors.rst
+-rw-r--r--   0        0        0    35149 2024-04-13 12:31:08.837226 repod-0.3.1/LICENSE
+-rw-r--r--   0        0        0    35149 2024-04-13 12:31:08.837226 repod-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1741 2024-04-13 12:31:08.837226 repod-0.3.1/Makefile
+-rw-r--r--   0        0        0     1551 2024-04-13 12:31:08.837226 repod-0.3.1/README.md
+-rw-r--r--   0        0        0    22964 2024-04-13 12:31:08.837226 repod-0.3.1/docs/LICENSE
+-rw-r--r--   0        0        0      634 2024-04-13 12:31:08.837226 repod-0.3.1/docs/Makefile
+-rw-r--r--   0        0        0    20138 2024-04-13 12:31:08.840559 repod-0.3.1/docs/artwork/LICENSE
+-rw-r--r--   0        0        0     4286 2024-04-13 12:31:08.840559 repod-0.3.1/docs/artwork/logo.ico
+-rw-r--r--   0        0        0    15160 2024-04-13 12:31:08.840559 repod-0.3.1/docs/artwork/logo.png
+-rw-r--r--   0        0        0     1509 2024-04-13 12:31:08.840559 repod-0.3.1/docs/artwork/repod.svg
+-rw-r--r--   0        0        0      484 2024-04-13 12:31:08.840559 repod-0.3.1/docs/authors.rst
+-rw-r--r--   0        0        0     2610 2024-04-13 12:31:08.840559 repod-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0     4011 2024-04-13 12:31:08.840559 repod-0.3.1/docs/contributing.rst
+-rw-r--r--   0        0        0     1295 2024-04-13 12:31:08.840559 repod-0.3.1/docs/index.rst
+-rw-r--r--   0        0        0     4285 2024-04-13 12:31:08.840559 repod-0.3.1/docs/packages/contents.rst
+-rw-r--r--   0        0        0     1164 2024-04-13 12:31:08.840559 repod-0.3.1/docs/packages/signatures.rst
+-rw-r--r--   0        0        0    13440 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repod/changelog.rst
+-rw-r--r--   0        0        0     2000 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repod/installation.rst
+-rw-r--r--   0        0        0       84 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repod/man/index.rst
+-rw-r--r--   0        0        0    23153 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repod/man/repod_conf.rst
+-rw-r--r--   0        0        0     2421 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repod/man/repod_file.rst
+-rw-r--r--   0        0        0     5846 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repod/usage.rst
+-rw-r--r--   0        0        0     2119 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repositories/binary_repository.rst
+-rw-r--r--   0        0        0     5486 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repositories/management_repository.rst
+-rw-r--r--   0        0        0     3177 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repositories/source_repository.rst
+-rw-r--r--   0        0        0     1077 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repositories/source_tarball_repository.rst
+-rw-r--r--   0        0        0     8938 2024-04-13 12:31:08.840559 repod-0.3.1/docs/repositories/sync_database.rst
+-rw-r--r--   0        0        0     5024 2024-04-13 12:31:29.944204 repod-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      503 2024-04-13 12:31:08.843893 repod-0.3.1/repod/__init__.py
+-rw-r--r--   0        0        0    31985 2024-04-13 12:31:08.843893 repod-0.3.1/repod/action/check.py
+-rw-r--r--   0        0        0    97366 2024-04-13 12:31:08.843893 repod-0.3.1/repod/action/task.py
+-rw-r--r--   0        0        0    12825 2024-04-13 12:31:08.843893 repod-0.3.1/repod/action/workflow.py
+-rw-r--r--   0        0        0     3155 2024-04-13 12:31:08.843893 repod-0.3.1/repod/archive/archive.py
+-rw-r--r--   0        0        0       82 2024-04-13 12:31:08.843893 repod-0.3.1/repod/cli/__init__.py
+-rw-r--r--   0        0        0    13335 2024-04-13 12:31:08.843893 repod-0.3.1/repod/cli/argparse.py
+-rw-r--r--   0        0        0     8473 2024-04-13 12:31:08.843893 repod-0.3.1/repod/cli/cli.py
+-rw-r--r--   0        0        0     2296 2024-04-13 12:31:08.843893 repod-0.3.1/repod/commands.py
+-rw-r--r--   0        0        0    11915 2024-04-13 12:31:08.847226 repod-0.3.1/repod/common/enums.py
+-rw-r--r--   0        0        0    18712 2024-04-13 12:31:08.847226 repod-0.3.1/repod/common/models.py
+-rw-r--r--   0        0        0     1398 2024-04-13 12:31:08.847226 repod-0.3.1/repod/common/regex.py
+-rw-r--r--   0        0        0      148 2024-04-13 12:31:08.847226 repod-0.3.1/repod/config/__init__.py
+-rw-r--r--   0        0        0     2214 2024-04-13 12:31:08.847226 repod-0.3.1/repod/config/defaults.py
+-rw-r--r--   0        0        0   105129 2024-04-13 12:31:08.847226 repod-0.3.1/repod/config/settings.py
+-rw-r--r--   0        0        0      845 2024-04-13 12:31:08.847226 repod-0.3.1/repod/errors.py
+-rw-r--r--   0        0        0     1270 2024-04-13 12:31:08.847226 repod-0.3.1/repod/files/__init__.py
+-rw-r--r--   0        0        0    14591 2024-04-13 12:31:08.847226 repod-0.3.1/repod/files/buildinfo.py
+-rw-r--r--   0        0        0     8790 2024-04-13 12:31:08.847226 repod-0.3.1/repod/files/common.py
+-rw-r--r--   0        0        0    14338 2024-04-13 12:31:08.847226 repod-0.3.1/repod/files/mtree.py
+-rw-r--r--   0        0        0     9523 2024-04-13 12:31:08.847226 repod-0.3.1/repod/files/package.py
+-rw-r--r--   0        0        0    15957 2024-04-13 12:31:08.847226 repod-0.3.1/repod/files/pkginfo.py
+-rw-r--r--   0        0        0    20923 2024-04-13 12:31:08.847226 repod-0.3.1/repod/files/srcinfo.py
+-rw-r--r--   0        0        0        0 2024-04-13 12:31:08.893894 repod-0.3.1/repod/py.typed
+-rw-r--r--   0        0        0     1004 2024-04-13 12:31:08.847226 repod-0.3.1/repod/repo/__init__.py
+-rw-r--r--   0        0        0      227 2024-04-13 12:31:08.847226 repod-0.3.1/repod/repo/management/__init__.py
+-rw-r--r--   0        0        0    42929 2024-04-13 12:31:08.847226 repod-0.3.1/repod/repo/management/outputpackage.py
+-rw-r--r--   0        0        0      944 2024-04-13 12:31:08.847226 repod-0.3.1/repod/repo/package/__init__.py
+-rw-r--r--   0        0        0    13104 2024-04-13 12:31:08.850560 repod-0.3.1/repod/repo/package/repofile.py
+-rw-r--r--   0        0        0    49141 2024-04-13 12:31:08.850560 repod-0.3.1/repod/repo/package/syncdb.py
+-rw-r--r--   0        0        0     1271 2024-04-13 12:31:08.850560 repod-0.3.1/repod/templates/desc_v1.j2
+-rw-r--r--   0        0        0     1248 2024-04-13 12:31:08.850560 repod-0.3.1/repod/templates/desc_v2.j2
+-rw-r--r--   0        0        0       84 2024-04-13 12:31:08.850560 repod-0.3.1/repod/templates/files_v1.j2
+-rw-r--r--   0        0        0      114 2024-04-13 12:31:08.850560 repod-0.3.1/repod/verification/__init__.py
+-rw-r--r--   0        0        0     1689 2024-04-13 12:31:08.850560 repod-0.3.1/repod/verification/pgp.py
+-rw-r--r--   0        0        0       47 2024-04-13 12:31:08.850560 repod-0.3.1/repod/version/__init__.py
+-rw-r--r--   0        0        0     5462 2024-04-13 12:31:08.850560 repod-0.3.1/repod/version/alpm.py
+-rw-r--r--   0        0        0      626 2024-04-13 12:31:08.850560 repod-0.3.1/repod/version/util.py
+-rw-r--r--   0        0        0       23 2024-04-13 12:31:08.850560 repod-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0    12942 2024-04-13 12:31:08.850560 repod-0.3.1/tests/action/test_check.py
+-rw-r--r--   0        0        0    85898 2024-04-13 12:31:08.850560 repod-0.3.1/tests/action/test_task.py
+-rw-r--r--   0        0        0     8605 2024-04-13 12:31:08.850560 repod-0.3.1/tests/action/test_workflow.py
+-rw-r--r--   0        0        0     3196 2024-04-13 12:31:08.850560 repod-0.3.1/tests/archive/test_archive.py
+-rw-r--r--   0        0        0     4415 2024-04-13 12:31:08.850560 repod-0.3.1/tests/cli/test_argparse.py
+-rw-r--r--   0        0        0    20656 2024-04-13 12:31:08.850560 repod-0.3.1/tests/cli/test_cli.py
+-rw-r--r--   0        0        0     3490 2024-04-13 12:31:08.850560 repod-0.3.1/tests/common/test_enums.py
+-rw-r--r--   0        0        0    11656 2024-04-13 12:31:08.850560 repod-0.3.1/tests/common/test_models.py
+-rw-r--r--   0        0        0     5474 2024-04-13 12:31:08.850560 repod-0.3.1/tests/common/test_regex.py
+-rw-r--r--   0        0        0   101698 2024-04-13 12:31:08.853893 repod-0.3.1/tests/config/test_settings.py
+-rw-r--r--   0        0        0    59947 2024-04-13 12:31:08.853893 repod-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     8992 2024-04-13 12:31:08.853893 repod-0.3.1/tests/files/test_buildinfo.py
+-rw-r--r--   0        0        0     7167 2024-04-13 12:31:08.853893 repod-0.3.1/tests/files/test_common.py
+-rw-r--r--   0        0        0      221 2024-04-13 12:31:08.853893 repod-0.3.1/tests/files/test_files_init.py
+-rw-r--r--   0        0        0    16215 2024-04-13 12:31:08.853893 repod-0.3.1/tests/files/test_mtree.py
+-rw-r--r--   0        0        0     3420 2024-04-13 12:31:08.853893 repod-0.3.1/tests/files/test_package.py
+-rw-r--r--   0        0        0     6712 2024-04-13 12:31:08.853893 repod-0.3.1/tests/files/test_pkginfo.py
+-rw-r--r--   0        0        0     5094 2024-04-13 12:31:08.853893 repod-0.3.1/tests/files/test_srcinfo.py
+-rw-r--r--   0        0        0    17238 2024-04-13 12:31:08.853893 repod-0.3.1/tests/repo/management/test_outputpackage.py
+-rw-r--r--   0        0        0    13599 2024-04-13 12:31:08.853893 repod-0.3.1/tests/repo/package/test_repofile.py
+-rw-r--r--   0        0        0    33258 2024-04-13 12:31:08.853893 repod-0.3.1/tests/repo/package/test_syncdb.py
+-rw-r--r--   0        0        0      217 2024-04-13 12:31:08.853893 repod-0.3.1/tests/repo/test_repo_init.py
+-rw-r--r--   0        0        0     1249 2024-04-13 12:31:08.853893 repod-0.3.1/tests/test_commands.py
+-rw-r--r--   0        0        0      198 2024-04-13 12:31:08.853893 repod-0.3.1/tests/test_repod_init.py
+-rw-r--r--   0        0        0     2203 2024-04-13 12:31:08.853893 repod-0.3.1/tests/verification/test_pgp.py
+-rw-r--r--   0        0        0     2387 2024-04-13 12:31:08.853893 repod-0.3.1/tests/version/test_alpm.py
+-rw-r--r--   0        0        0      614 2024-04-13 12:31:08.853893 repod-0.3.1/tests/version/test_util.py
+-rw-r--r--   0        0        0     3623 1970-01-01 00:00:00.000000 repod-0.3.1/PKG-INFO
```

### Comparing `repod-0.3.0.post0/LICENSE` & `repod-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/Makefile` & `repod-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/README.md` & `repod-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/LICENSE` & `repod-0.3.1/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/Makefile` & `repod-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/artwork/LICENSE` & `repod-0.3.1/docs/artwork/LICENSE`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/artwork/logo.ico` & `repod-0.3.1/docs/artwork/logo.ico`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/artwork/logo.png` & `repod-0.3.1/docs/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/artwork/repod.svg` & `repod-0.3.1/docs/artwork/repod.svg`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/conf.py` & `repod-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/contributing.rst` & `repod-0.3.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/index.rst` & `repod-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/packages/contents.rst` & `repod-0.3.1/docs/packages/contents.rst`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,24 @@
 
 PackageV1
 ^^^^^^^^^
 
 .. literalinclude:: ../schema/PackageV1.json
    :language: json
 
+.. _packagev2:
+
+PackageV2
+^^^^^^^^^
+
+This version removes the ``md5sum`` field as the hash algorithm is unsafe.
+
+.. literalinclude:: ../schema/PackageV2.json
+   :language: json
+
 .. _mtree:
 
 .MTREE
 ------
 
 The ``.MTREE`` files contained in a package are |mtree| files, which describe
 the contents of a package. Entities such as directories, files and symlinks are
```

### Comparing `repod-0.3.0.post0/docs/packages/signatures.rst` & `repod-0.3.1/docs/packages/signatures.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/repod/changelog.rst` & `repod-0.3.1/docs/repod/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,34 @@
 For more detailed information have a look at the |git log|.
 
 .. _version unreleased:
 
 [Unreleased]
 ------------
 
+[0.3.1] - 2024-04-13
+--------------------
+
+Changed
+^^^^^^^
+
+* The test dependency on ``pytest-lazy-fixture`` has been replaced with
+  ``pytest-lazy-fixtures``.
+
+Fixed
+^^^^^
+
+* The code has been adapted to changes in metadata files in pacman 6.1. Most
+  notably, the ``md5sum`` field in repository sync database ``desc`` files has
+  been removed, while the ``pgpsig`` field has been made optional. This change
+  made the introduction of ``PackageV2``, ``OutputPackageV2`` necessary, while
+  ``PackageDescV2`` has been adapted accordingly.
+* Various typing related issues have been addressed, that would lead to errors
+  in future versions of ``pydantic``.
+
 [0.3.0] - 2023-07-17
 --------------------
 
 Added
 ^^^^^
 
 * A section in the documentation now provides a high-level introduction to how
```

### Comparing `repod-0.3.0.post0/docs/repod/installation.rst` & `repod-0.3.1/docs/repod/installation.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/repod/man/repod_conf.rst` & `repod-0.3.1/docs/repod/man/repod_conf.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/repod/man/repod_file.rst` & `repod-0.3.1/docs/repod/man/repod_file.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/repod/usage.rst` & `repod-0.3.1/docs/repod/usage.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/repositories/binary_repository.rst` & `repod-0.3.1/docs/repositories/binary_repository.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/repositories/management_repository.rst` & `repod-0.3.1/docs/repositories/management_repository.rst`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,26 @@
 
 OutputPackageV1
 """""""""""""""
 
 .. literalinclude:: ../schema/OutputPackageV1.json
    :language: json
 
+.. _outputpackagev2_schema:
+
+OutputPackageV2
+"""""""""""""""
+
+This version removes the ``md5sum`` field as the hash algorithm is unsafe and
+renders the ``pgpsig`` field optional to lower the size of the created
+:ref:`sync database` files.
+
+.. literalinclude:: ../schema/OutputPackageV2.json
+   :language: json
+
 .. _packagedesc_schema:
 
 PackageDesc
 ^^^^^^^^^^^
 
 This is the schema of package information found in a :ref:`desc` file of a
 :ref:`sync database`.
@@ -175,15 +187,16 @@
    :language: json
 
 .. _packagedescv2_schema:
 
 PackageDescV2
 """""""""""""
 
-This version removes the ``pgpsig`` field to lower the size of the created
+This version removes the ``md5sum`` field as the hash algorithm is unsafe and
+renders the ``pgpsig`` field optional to lower the size of the created
 :ref:`sync database` files.
 
 .. note::
 
    This schema represents the definition of :ref:`desc_v2`.
 
 .. literalinclude:: ../schema/PackageDescV2.json
```

### Comparing `repod-0.3.0.post0/docs/repositories/source_repository.rst` & `repod-0.3.1/docs/repositories/source_repository.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/repositories/source_tarball_repository.rst` & `repod-0.3.1/docs/repositories/source_tarball_repository.rst`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/docs/repositories/sync_database.rst` & `repod-0.3.1/docs/repositories/sync_database.rst`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
   below the identifier)
 * ``%NAME%`` (**required**): The name of the package (one line below the
   identifier)
 * ``%OPTDEPENDS%``: A list of package names that can be used optionally to
   extend a package's functionality (one name per line below the identifier)
 * ``%PACKAGER%`` (**required**): The UID (name and e-mail address) of the
   packager who created a package (one line below the identifier)
-* ``%PGPSIG%``: The base64 encoded PGP signature of a package (one line below
+* ``%PGPSIG%`` (**required**): The base64 encoded PGP signature of a package (one line below
   the identifier)
 * ``%PROVIDES%``: A list of package names that a package provides (one name per
   line below the identifier)
 * ``%REPLACES%``: A list of package names that a package replaces (one name per
   line below the identifier)
 * ``%SHA256SUM%`` (**required**): The sha256 checksum of the package file (one
   line below the identifier)
@@ -125,16 +125,17 @@
   below the identifier)
 
 .. _desc_v2:
 
 Desc v2
 ^^^^^^^
 
-This version removes the ``%PGPSIG%`` field to lower the size of the created
-:ref:`sync database` files.
+This version removes the ``%MD5SUM%`` field as this hashing algorithm is unsafe.
+Furthermore the ``%PGPSIG%`` field has been made optional to lower the size of
+the created :ref:`sync database` files.
 
 * ``%ARCH%`` (**required**): The CPU architecture of the package (one line
   below the identifier)
 * ``%BACKUP%``: A list of package files to be backed up by the package manager
   (one file per line below the identifier)
 * ``%BASE%`` (**required**): The ``pkgbase`` (see |split package|) of a package
   (one line below the identifier)
@@ -157,22 +158,22 @@
 * ``%ISIZE%`` (**required**): The size - in Bytes - of the package when
   installed (one line below the identifier)
 * ``%LICENSE%`` (**required**): A list of license names that the files of a
   package are licensed under (one name per line below the identifier)
 * ``%MAKEDEPENDS%``: A list of package names required when running the
   ``prepare()`` and/ or ``build()`` |package function| (one name per line below
   the identifier)
-* ``%MD5SUM%`` (**required**): The md5 checksum of the package file (one line
-  below the identifier)
 * ``%NAME%`` (**required**): The name of the package (one line below the
   identifier)
 * ``%OPTDEPENDS%``: A list of package names that can be used optionally to
   extend a package's functionality (one name per line below the identifier)
 * ``%PACKAGER%`` (**required**): The UID (name and e-mail address) of the
   packager who created a package (one line below the identifier)
+* ``%PGPSIG%``: The base64 encoded PGP signature of a package (one line below
+  the identifier)
 * ``%PROVIDES%``: A list of package names that a package provides (one name per
   line below the identifier)
 * ``%REPLACES%``: A list of package names that a package replaces (one name per
   line below the identifier)
 * ``%SHA256SUM%`` (**required**): The sha256 checksum of the package file (one
   line below the identifier)
 * ``%URL%`` (**required**): The URL of the package (one line below the
```

### Comparing `repod-0.3.0.post0/pyproject.toml` & `repod-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 authors = [
     { name = "Arch Linux", email = "arch-projects@lists.archlinux.org" },
 ]
 dynamic = []
-requires-python = ">=3.10,<4.0"
+requires-python = ">=3.10"
 dependencies = [
-    "aiofiles>=23.1.0",
-    "email-validator>=2.0.0",
-    "jinja2>=3.1.2",
-    "orjson>=3.9.2",
-    "pydantic>=2.0",
-    "pydantic-settings>=2.0.2",
+    "aiofiles>=23.2.1",
+    "email-validator>=2.1.0",
+    "jinja2>=3.1.3",
+    "orjson>=3.9.15",
+    "pydantic>=2.6.4",
+    "pydantic-settings>=2.2.1",
     "python-magic>=0.4.27",
     "pyxdg>=0.28",
-    "pyzstd>=0.15.7",
+    "pyzstd>=0.15.10",
     "subprocess-tee>=0.4.1",
     "tomli>=2.0.1; python_version<'3.11'",
 ]
 name = "repod"
 description = "Tooling to maintain binary package repositories for Linux distributions using the pacman package manager"
 readme = "README.md"
 keywords = [
@@ -42,15 +42,15 @@
     "Topic :: Software Development",
     "Topic :: System :: Archiving :: Packaging",
     "Topic :: System :: Operating System",
     "Topic :: System :: Software Distribution",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-version = "0.3.0.post0"
+version = "0.3.1"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 "Bug Tracker" = "https://gitlab.archlinux.org/archlinux/repod/-/issues/"
 homepage = "https://gitlab.archlinux.org/archlinux/repod"
@@ -66,30 +66,30 @@
 ]
 
 [project.scripts]
 repod-file = "repod.cli:repod_file"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=23.7.0",
-    "coverage>=6.5.0",
+    "black>=24.3.0",
+    "coverage>=7.4.1",
     "coverage-conditional-plugin>=0.9.0",
-    "flake8>=6.0.0",
-    "isort>=5.12.0",
-    "mypy[install-types,reports]>=1.3",
-    "pytest>=7.4.0",
-    "pytest-asyncio>=0.21.0",
-    "pytest-lazy-fixture>=0.6.3",
-    "sphinx>=6.0.0",
-    "sphinx-rtd-theme>=1.2.2",
+    "flake8>=7.0.0",
+    "isort>=5.13.2",
+    "mypy[install-types,reports]>=1.9.0",
+    "pytest>=8.1.1",
+    "pytest-asyncio>=0.23.6",
+    "sphinx>=7.2.6",
+    "sphinx-rtd-theme>=1.3.0",
     "sphinx-argparse>=0.4.0",
     "sphinxcontrib-programoutput>=0.17",
-    "vulture>=2.7",
+    "vulture>=2.11",
     "pydocstyle>=6.3.0",
-    "bandit>=1.7.5",
+    "bandit>=1.7.7",
+    "pytest-lazy-fixtures>=1.0.7",
 ]
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 excludes = [
```

### Comparing `repod-0.3.0.post0/repod/action/check.py` & `repod-0.3.1/repod/action/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Checks for various circumstances."""
+
 from __future__ import annotations
 
 import asyncio
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from logging import debug, info
 from pathlib import Path
```

### Comparing `repod-0.3.0.post0/repod/action/task.py` & `repod-0.3.1/repod/action/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tasks for chaining workflows in repod."""
+
 from __future__ import annotations
 
 import asyncio
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from itertools import groupby
 from logging import debug, info
@@ -556,15 +557,15 @@
                 self.state = ActionStateEnum.FAILED_TASK
                 return self.state
 
         for key, group in groupby(packages, attrgetter("pkginfo.base")):
             debug(f"Create OutputPackageBase representing pkgbase {key}")
             try:
                 outputpackagebase = OutputPackageBase.from_package(packages=list(group))
-                outputpackagebase.source_url = self.pkgbase_urls.get(
+                outputpackagebase.source_url = self.pkgbase_urls.get(  # type: ignore[attr-defined]
                     outputpackagebase.base,  # type: ignore[attr-defined]
                 )
                 self.pkgbases.append(outputpackagebase)
             except (ValueError, RuntimeError) as e:
                 info(e)
                 self.state = ActionStateEnum.FAILED_TASK
                 return self.state
```

### Comparing `repod-0.3.0.post0/repod/action/workflow.py` & `repod-0.3.1/repod/action/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Workflows describing common repository actions."""
+
 from logging import debug
 from pathlib import Path
 from sys import exit, stderr
 
 from pydantic import AnyUrl
 
 from repod.action.task import (
```

### Comparing `repod-0.3.0.post0/repod/archive/archive.py` & `repod-0.3.1/repod/archive/archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functionality for package archiving."""
+
 from __future__ import annotations
 
 from pathlib import Path
 from shutil import copy2
 
 from pydantic import BaseModel, field_validator
```

### Comparing `repod-0.3.0.post0/repod/cli/argparse.py` & `repod-0.3.1/repod/cli/argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Argparser factory for repod's CLI."""
+
 from __future__ import annotations
 
 import os
 from argparse import ArgumentParser, ArgumentTypeError
 from pathlib import Path
 
 from pydantic import AnyUrl, TypeAdapter, ValidationError
```

### Comparing `repod-0.3.0.post0/repod/cli/cli.py` & `repod-0.3.1/repod/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functions for handling repod's CLI."""
+
 import asyncio
 from argparse import ArgumentParser, Namespace
 from logging import DEBUG, INFO, WARNING, StreamHandler, debug, getLogger
 from pathlib import Path
 from sys import exit, stderr, stdout
 from unittest.mock import patch
```

### Comparing `repod-0.3.0.post0/repod/commands.py` & `repod-0.3.1/repod/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility functions for running external commands."""
+
 from pathlib import Path
 from subprocess import PIPE, STDOUT, CalledProcessError  # nosec: B404
 
 from subprocess_tee import CompletedProcess, run  # nosec: B404
 
 
 def _print_env(env: dict[str, str] | None) -> None:
```

### Comparing `repod-0.3.0.post0/repod/common/enums.py` & `repod-0.3.1/repod/common/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Enums used through repod."""
+
 from __future__ import annotations
 
 from enum import Enum, IntEnum, IntFlag, auto
 
 
 class ArchitectureEnum(Enum):
     """An Enum to distinguish different CPU architectures.
@@ -213,16 +214,17 @@
     ----------
     DEFAULT: int
         The default OutputPackage version
     ONE: int
         The first OutputPackage version
     """
 
-    DEFAULT = 1
+    DEFAULT = 2
     ONE = 1
+    TWO = 2
 
 
 class PackageDescVersionEnum(IntEnum):
     """An IntEnum to distinguish different version of PackageDesc.
 
     Attributes
     ----------
@@ -230,15 +232,15 @@
         The default PackageDesc version
     ONE: int
         The first PackageDesc version
     TWO: int
         The second PackageDesc version
     """
 
-    DEFAULT = 1
+    DEFAULT = 2
     ONE = 1
     TWO = 2
 
 
 class PkgVerificationTypeEnum(Enum):
     """An Enum to distinguish different package signature verification implementations.
```

### Comparing `repod-0.3.0.post0/repod/common/models.py` & `repod-0.3.1/repod/common/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pydantic models shared throughout the codebase."""
+
 from __future__ import annotations
 
 from pathlib import Path
 
 from email_validator import EmailNotValidError, validate_email
 from pydantic import (
     BaseModel,
```

### Comparing `repod-0.3.0.post0/repod/common/regex.py` & `repod-0.3.1/repod/common/regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Regular expressions used for matching strings in packages and sync databases."""
+
 from repod.common.enums import (
     ArchitectureEnum,
     tar_compression_types_for_filename_regex,
 )
 
 RELATIVE_MTREE_PATH = r"[A-Za-z0-9.,:;/_()@\\&$?!+%~{}<>*\-\"\'\[\]\`^|]+"
 """
```

### Comparing `repod-0.3.0.post0/repod/config/defaults.py` & `repod-0.3.1/repod/config/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Module with configuration defaults for settings.
 
 The defaults for locations and directories are provided as dicts which use SettingsTypeEnum as keys to distinguish
 between different ways of running repod.
 """
+
 from pathlib import Path
 
 from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS
 from xdg.BaseDirectory import xdg_config_home, xdg_state_home
 
 from repod.common.enums import ArchitectureEnum, CompressionTypeEnum, SettingsTypeEnum
```

### Comparing `repod-0.3.0.post0/repod/config/settings.py` & `repod-0.3.1/repod/config/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Settings management for repod."""
+
 from __future__ import annotations
 
 import os
 from collections import defaultdict
 from logging import debug
 from pathlib import Path
 from typing import Any, Tuple, Type
```

### Comparing `repod-0.3.0.post0/repod/errors.py` & `repod-0.3.1/repod/errors.py`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/repod/files/__init__.py` & `repod-0.3.1/repod/files/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """File handling in repod."""
+
 from pathlib import Path
 
 from repod.files.buildinfo import BuildInfo  # noqa: F401
 from repod.files.buildinfo import export_schemas as buildinfo_export_schemas
 from repod.files.common import extract_file_from_tarfile, open_tarfile  # noqa: F401
 from repod.files.mtree import MTree, MTreeEntry  # noqa: F401
 from repod.files.mtree import export_schemas as mtree_export_schemas
```

### Comparing `repod-0.3.0.post0/repod/files/buildinfo.py` & `repod-0.3.1/repod/files/buildinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Handling of .BUILDINFO files."""
+
 from __future__ import annotations
 
 from io import StringIO
 from pathlib import Path
 from re import fullmatch
 from typing import Any
```

### Comparing `repod-0.3.0.post0/repod/files/common.py` & `repod-0.3.1/repod/files/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common function and tools to work with files."""
+
 from gzip import BadGzipFile
 from gzip import open as gzip_open
 from io import BytesIO, StringIO
 from logging import debug
 from pathlib import Path
 from tarfile import ReadError, TarFile
 from tarfile import open as tarfile_open
```

### Comparing `repod-0.3.0.post0/repod/files/mtree.py` & `repod-0.3.1/repod/files/mtree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Handling of .MTREE files."""
+
 from __future__ import annotations
 
 import io
 import re
 from logging import debug
 from pathlib import Path
 
 from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS, dumps
 from pydantic import (
     BaseModel,
+    Field,
     NonNegativeFloat,
     NonNegativeInt,
+    StringConstraints,
     ValidationError,
-    conint,
-    constr,
 )
+from typing_extensions import Annotated
 
 from repod.common.models import SchemaVersionV1
 from repod.common.regex import ABSOLUTE_MTREE_PATH, MD5, RELATIVE_MTREE_PATH, SHA256
 from repod.errors import RepoManagementValidationError
 
 
 class SystemGID(BaseModel):
@@ -26,80 +28,78 @@
 
     Attributes
     ----------
     gid: int
         A group ID >0, <1000
     """
 
-    gid: conint(ge=0, lt=1000)  # type: ignore[valid-type]
+    gid: Annotated[int, Field(strict=True, ge=0, lt=1000)]
 
 
 class LinkTarget(BaseModel):
     """The target location of a symlink.
 
     Attributes
     ----------
     link: str | None
         An optional string representing a relative or absolute file
     """
 
-    link: constr(  # type: ignore[valid-type]
-        pattern=rf"^({RELATIVE_MTREE_PATH}|{ABSOLUTE_MTREE_PATH})$"  # noqa: F722
-    ) | None = None
+    link: Annotated[str, StringConstraints(pattern=rf"^({RELATIVE_MTREE_PATH}|{ABSOLUTE_MTREE_PATH})$")] | None = None
 
 
 class Md5(BaseModel):
     """An MD5 checksum.
 
     Attributes
     ----------
     md5: str | None
         An optional string representing an MD5 checksum
     """
 
-    md5: constr(pattern=rf"^{MD5}$") | None = None  # type: ignore[valid-type]  # noqa: F722
+    md5: Annotated[str, StringConstraints(pattern=rf"^{MD5}$")] | None = None
 
 
 class FileMode(BaseModel):
     """A numeric unix file mode.
 
     Attributes
     ----------
     mode: str
         A three or four digit long string, consisting only of valid file modes
     """
 
-    mode: constr(pattern=r"^[01234567]{3,4}$")  # type: ignore[valid-type]  # noqa: F722
+    mode: Annotated[str, StringConstraints(pattern=r"^[01234567]{3,4}$")]
 
 
 class MTreeEntryName(BaseModel):
     """A file name in mtree representation.
 
     The mtree format allows for encoding characters using a block of backslash and three octal digits (see
     https://man.archlinux.org/man/mtree.5#General_Format).
 
     Attributes
     ----------
     name: str
         A string representing an absolute file location in mtree format
     """
 
-    name: constr(pattern=rf"^{ABSOLUTE_MTREE_PATH}$")  # type: ignore[valid-type]  # noqa: F722
+    name: Annotated[str, StringConstraints(pattern=rf"^{ABSOLUTE_MTREE_PATH}$")]
 
 
 class Sha256(BaseModel):
     """A SHA-256 checksum.
 
     Attributes
     ----------
     sha256:
         An optional string representing a SHA-256 checksum
     """
 
-    sha256: constr(pattern=rf"^{SHA256}$") | None = None  # type: ignore[valid-type]  # noqa: F722
+    sha256: Annotated[str, StringConstraints(pattern=rf"^{SHA256}$")] | None = None
 
 
 class FileSize(BaseModel):
     """A file size in bytes.
 
     Attributes
     ----------
@@ -127,27 +127,27 @@
 
     Attributes
     ----------
     type_: str
         A string representing a valid mtree type (one of block, char, dir, fifo, file, link or socket)
     """
 
-    type_: constr(pattern=r"^(block|char|dir|fifo|file|link|socket)$")  # type: ignore[valid-type]  # noqa: F722
+    type_: Annotated[str, StringConstraints(pattern=r"^(block|char|dir|fifo|file|link|socket)$")]
 
 
 class SystemUID(BaseModel):
     """The user ID of a system user.
 
     Attributes
     ----------
     uid: int
         A user ID >0, <1000
     """
 
-    uid: conint(ge=0, lt=1000)  # type: ignore[valid-type]
+    uid: Annotated[int, Field(strict=True, ge=0, lt=1000)]
 
 
 class MTreeEntry(BaseModel):
     """An entry in an MTree.
 
     This is a template class and should not be used directly. Instead instantiate one of the classes derived from it.
     """
@@ -367,24 +367,24 @@
                 # provide a list of all settings in an entry line (skip empty assigments due to multiple whitespace)
                 settings_list = [assignment.split("=") for assignment in line.split()[1:] if assignment]
                 sanitize_mtree_pairs(settings_list=settings_list, settings_dict=file_settings)
 
                 try:
                     entries.append(
                         MTreeEntryV1(
-                            gid=file_settings.get("gid") or base_settings.get("gid"),
-                            link=file_settings.get("link"),
-                            md5=file_settings.get("md5") or base_settings.get("md5"),
-                            mode=file_settings.get("mode") or base_settings.get("mode"),
-                            name=file_settings.get("name"),
-                            sha256=file_settings.get("sha256") or base_settings.get("sha256"),
+                            gid=file_settings.get("gid") or base_settings.get("gid"),  # type: ignore[arg-type]
+                            link=file_settings.get("link"),  # type: ignore[arg-type]
+                            md5=file_settings.get("md5") or base_settings.get("md5"),  # type: ignore[arg-type]
+                            mode=file_settings.get("mode") or base_settings.get("mode"),  # type: ignore[arg-type]
+                            name=file_settings.get("name"),  # type: ignore[arg-type]
+                            sha256=file_settings.get("sha256") or base_settings.get("sha256"),  # type: ignore[arg-type]
                             size=file_settings.get("size") or base_settings.get("size"),  # type: ignore[arg-type]
                             time=file_settings.get("time") or base_settings.get("time"),  # type: ignore[arg-type]
-                            type_=file_settings.get("type_") or base_settings.get("type_"),
-                            uid=file_settings.get("uid") or base_settings.get("uid"),
+                            type_=file_settings.get("type_") or base_settings.get("type_"),  # type: ignore[arg-type]
+                            uid=file_settings.get("uid") or base_settings.get("uid"),  # type: ignore[arg-type]
                         )
                     )
                 except ValidationError as e:
                     raise RepoManagementValidationError(
                         f"An error occured when validating mtree data!\n"
                         f"Basic settings: {base_settings}\n"
                         f"File settings: {file_settings}\n"
```

### Comparing `repod-0.3.0.post0/repod/files/package.py` & `repod-0.3.1/repod/files/package.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Handling of package files and their contents."""
+
 from __future__ import annotations
 
 from base64 import b64encode
 from hashlib import md5, sha256
 from logging import debug, info
 from pathlib import Path
 from typing import Any
@@ -17,14 +18,17 @@
 from repod.files.mtree import MTree
 from repod.files.pkginfo import PkgInfo
 
 PACKAGE_VERSIONS = {
     1: {
         "required": {".BUILDINFO", ".MTREE", ".PKGINFO"},
     },
+    2: {
+        "required": {".BUILDINFO", ".MTREE", ".PKGINFO"},
+    },
 }
 
 
 class Package(BaseModel):
     """Package representation.
 
     This is a template class and (apart from its class methods) should not be used directly. Instead instatiate one of
@@ -116,14 +120,43 @@
                                 tarfile=tarfile,
                                 file=".PKGINFO",
                                 as_stringio=True,
                             ),
                         ),
                         sha256sum=package_sha256sum,
                     )
+                case 2:
+                    return PackageV2(
+                        buildinfo=BuildInfo.from_file(
+                            data=await extract_file_from_tarfile(  # type: ignore[arg-type]
+                                tarfile=tarfile,
+                                file=".BUILDINFO",
+                                as_stringio=True,
+                            )
+                        ),
+                        csize=package.stat().st_size,
+                        filename=package.name,
+                        mtree=MTree.from_file(
+                            data=await extract_file_from_tarfile(  # type: ignore[arg-type]
+                                tarfile=tarfile,
+                                file=".MTREE",
+                                as_stringio=True,
+                                gzip_compressed=True,
+                            ),
+                        ),
+                        pgpsig=pgpsig,
+                        pkginfo=PkgInfo.from_file(
+                            data=await extract_file_from_tarfile(  # type: ignore[arg-type]
+                                tarfile=tarfile,
+                                file=".PKGINFO",
+                                as_stringio=True,
+                            ),
+                        ),
+                        sha256sum=package_sha256sum,
+                    )
                 case _:
                     raise RepoManagementFileError(
                         f"The provided file {package} does not match any known package versions!"
                     )
 
     def top_level_dict(self) -> dict[str, Any]:
         """Flatten the keys and values tracked by Package (one level deep) and return them in a dict.
@@ -169,36 +202,62 @@
     """
 
     buildinfo: SerializeAsAny[BuildInfo]
     mtree: SerializeAsAny[MTree]
     pkginfo: SerializeAsAny[PkgInfo]
 
 
+class PackageV2(CSize, FileName, Package, PgpSig, Sha256Sum):
+    """Package representation version 2.
+
+    Attributes
+    ----------
+    buildinfo: BuildInfo
+        A .BUILDINFO file representation
+    csize: CSize
+        The file size of the Package
+    filename: FileName
+        The filename of the Package
+    mtree: MTree
+        An .MTREE file representation
+    pgpsig: str | None
+        An optional PGP signature (in base64 representation) for the package
+    pkginfo: PkgInfo
+        A .PKGINFO file representation
+    sha256sum: str
+        A SHA256 checksum for the package
+    """
+
+    buildinfo: SerializeAsAny[BuildInfo]
+    mtree: SerializeAsAny[MTree]
+    pkginfo: SerializeAsAny[PkgInfo]
+
+
 def export_schemas(output: Path | str) -> None:
     """Export the JSON schema of selected pydantic models to an output directory.
 
     Parameters
     ----------
     output: Path
         A path to which to output the JSON schema files
 
     Raises
     ------
     RuntimeError
         If output is not an existing directory
     """
-    classes = [PackageV1]
+    classes = [PackageV1, PackageV2]
 
     if isinstance(output, str):
         output = Path(output)
 
     if not output.exists():
         raise RuntimeError(f"The output directory {output} must exist!")
 
     for class_ in classes:
         with open(output / f"{class_.__name__}.json", "wb") as f:
             f.write(
                 dumps(
-                    class_.model_json_schema(),
+                    class_.model_json_schema(),  # type: ignore[attr-defined]
                     option=OPT_INDENT_2 | OPT_APPEND_NEWLINE | OPT_SORT_KEYS,
                 )
             )
```

### Comparing `repod-0.3.0.post0/repod/files/pkginfo.py` & `repod-0.3.1/repod/files/pkginfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Handling of .PKGINFO files."""
+
 from __future__ import annotations
 
 from io import StringIO
 from logging import debug
 from pathlib import Path
 from typing import Any
```

### Comparing `repod-0.3.0.post0/repod/files/srcinfo.py` & `repod-0.3.1/repod/files/srcinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Handling of .SRCINFO files."""
+
 from __future__ import annotations
 
 from io import StringIO
 from logging import debug
 from pathlib import Path
 
 from orjson import OPT_APPEND_NEWLINE, OPT_INDENT_2, OPT_SORT_KEYS, dumps
```

### Comparing `repod-0.3.0.post0/repod/repo/__init__.py` & `repod-0.3.1/repod/repo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Handling of management and package repository files."""
+
 from pathlib import Path
 
 from repod.repo.management import (  # noqa: F401
     Files,
     OutputPackage,
     OutputPackageBase,
     PackageDesc,
```

### Comparing `repod-0.3.0.post0/repod/repo/management/outputpackage.py` & `repod-0.3.1/repod/repo/management/outputpackage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Reading and writing of OutputPackageBase and OutputPackage."""
+
 from __future__ import annotations
 
 from logging import debug
 from pathlib import Path
 from typing import Any
 
 from aiofiles import open as async_open
@@ -97,14 +98,40 @@
             "groups",
             "optdepends",
             "pgpsig",
             "provides",
             "replaces",
         },
     },
+    2: {
+        "required": {
+            "arch",
+            "builddate",
+            "csize",
+            "desc",
+            "filename",
+            "isize",
+            "license",
+            "name",
+            "sha256sum",
+            "url",
+        },
+        "optional": {
+            "backup",
+            "checkdepends",
+            "conflicts",
+            "depends",
+            "files",
+            "groups",
+            "optdepends",
+            "pgpsig",
+            "provides",
+            "replaces",
+        },
+    },
 }
 OUTPUT_PACKAGE_BASE_VERSIONS: dict[int, dict[str, int | set[str]]] = {
     1: {
         "required": {
             "base",
             "makedepends",
             "packager",
@@ -311,14 +338,44 @@
                     optdepends=package.pkginfo.optdepends,  # type: ignore[attr-defined]
                     pgpsig=package.pgpsig,  # type: ignore[attr-defined]
                     provides=package.pkginfo.provides,  # type: ignore[attr-defined]
                     replaces=package.pkginfo.replaces,  # type: ignore[attr-defined]
                     sha256sum=package.sha256sum,  # type: ignore[attr-defined]
                     url=package.pkginfo.url,  # type: ignore[attr-defined]
                 )
+            case 2:
+                return OutputPackageV2(
+                    arch=package.pkginfo.arch,  # type: ignore[attr-defined]
+                    backup=package.pkginfo.backup,  # type: ignore[attr-defined]
+                    builddate=package.pkginfo.builddate,  # type: ignore[attr-defined]
+                    checkdepends=package.pkginfo.checkdepends,  # type: ignore[attr-defined]
+                    conflicts=package.pkginfo.conflicts,  # type: ignore[attr-defined]
+                    csize=package.csize,  # type: ignore[attr-defined]
+                    depends=package.pkginfo.depends,  # type: ignore[attr-defined]
+                    desc=package.pkginfo.desc,  # type: ignore[attr-defined]
+                    filename=package.filename,  # type: ignore[attr-defined]
+                    files=Files.from_dict(
+                        {
+                            "files": [
+                                str(path)[1:]
+                                for path in package.mtree.get_paths(show_all=False)  # type: ignore[attr-defined]
+                            ],
+                        }
+                    ),
+                    groups=package.pkginfo.groups,  # type: ignore[attr-defined]
+                    isize=package.pkginfo.isize,  # type: ignore[attr-defined]
+                    license=package.pkginfo.license,  # type: ignore[attr-defined]
+                    name=package.pkginfo.name,  # type: ignore[attr-defined]
+                    optdepends=package.pkginfo.optdepends,  # type: ignore[attr-defined]
+                    pgpsig=package.pgpsig,  # type: ignore[attr-defined]
+                    provides=package.pkginfo.provides,  # type: ignore[attr-defined]
+                    replaces=package.pkginfo.replaces,  # type: ignore[attr-defined]
+                    sha256sum=package.sha256sum,  # type: ignore[attr-defined]
+                    url=package.pkginfo.url,  # type: ignore[attr-defined]
+                )
             case _:
                 raise RuntimeError(
                     "An error occurred trying to create an OutputPackage from a Package! "
                     f"Unable to find matching version for Package keys: {keys}"
                 )
 
 
@@ -394,15 +451,112 @@
         identifies a package's md5 checksum
     name: str
         The attribute can be used to describe the (required) data below a %NAME% identifier in a 'desc' file, which
         identifies a package's name
     optdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %OPTDEPENDS% identifier in a 'desc' file,
         which identifies what other package(s) a package optionally depends on
-    pgpsig: str
+    pgpsig: str | None
+        The attribute can be used to describe the (required) data below a %PGPSIG% identifier in a 'desc' file, which
+        identifies a package's PGP signature
+    provides: list[str] | None
+        The attribute can be used to describe the (optional) data below a %PROVIDES% identifier in a 'desc' file, which
+        identifies what other package(s) a package provides
+    replaces: list[str] | None
+        The attribute can be used to describe the (optional) data below a %REPLACES% identifier in a 'desc' file, which
+        identifies what other package(s) a package replaces
+    schema_version: PositiveInt
+        A positive integer - 1 - identifying the schema version of the object
+    sha256sum: str
+        The attribute can be used to describe the (required) data below an %SHA256SUM% identifier in a 'desc' file,
+        which identifies a package's sha256 checksum
+    url: str
+        The attribute can be used to describe the (required) data below a %URL% identifier in a 'desc' file, which
+        identifies a package's URL
+    """
+
+    files: SerializeAsAny[Files | None] = None
+
+
+class OutputPackageV2(
+    OutputPackage,
+    Arch,
+    Backup,
+    BuildDate,
+    CheckDepends,
+    Conflicts,
+    CSize,
+    Depends,
+    Desc,
+    FileName,
+    Groups,
+    ISize,
+    License,
+    Name,
+    OptDepends,
+    PgpSig,
+    Provides,
+    Replaces,
+    SchemaVersionV2,
+    Sha256Sum,
+    Url,
+):
+    """A model describing all required attributes that define a package in the context of an output file (version 2).
+
+    Attributes
+    ----------
+    arch: str
+        The attribute can be used to describe the (required) data below an %ARCH% identifier in a 'desc' file, which
+        identifies a package's architecture
+    backup: list[str] | None
+        The attribute can be used to describe the (optional) data below a %BACKUP% identifier in a 'desc' file, which
+        identifies which file(s) of a package pacman will create backups for
+    builddate: int
+        The attribute can be used to describe the (required) data below a %BUILDDATE% identifier in a 'desc' file,
+        which identifies a package's build date (represented in seconds since the epoch)
+    checkdepends: list[str] | None
+        The attribute can be used to describe the (optional) data below a %CHECKDEPENDS% identifier in a 'desc' file,
+        which identifies a package's checkdepends
+    conflicts: list[str] | None
+        The attribute can be used to describe the (optional) data below a %CONFLICTS% identifier in a 'desc' file, which
+        identifies what other package(s) a package conflicts with
+    csize: int
+        The attribute can be used to describe the (required) data below a %CSIZE% identifier in a 'desc' file, which
+        identifies a package's size
+    depends: list[str] | None
+        The attribute can be used to describe the (optional) data below a %DEPENDS% identifier in a 'desc' file, which
+        identifies what other package(s) a package depends on
+    desc: str
+        The attribute can be used to describe the (required) data below a %DESC% identifier in a 'desc' file, which
+        identifies a package's description
+    filename: str
+        The attribute can be used to describe the (required) data below a %FILENAME% identifier in a 'desc' file, which
+        identifies a package's file name
+    files: list[str] | None
+        The attribute can be used to describe the (optional) data below a %FILES% identifier in a 'files' file, which
+        identifies which file(s) belong to a package
+    groups: list[str] | None
+        The attribute can be used to describe the (optional) data below a %GROUPS% identifier in a 'desc' file, which
+        identifies a package's groups
+    isize: int
+        The attribute can be used to describe the (required) data below an %ISIZE% identifier in a 'desc' file, which
+        identifies a package's installed size
+    license: list[str]
+        The attribute can be used to describe the (required) data below a %LICENSE% identifier in a 'desc' file, which
+        identifies a package's license(s)
+    md5sum: str
+        The attribute can be used to describe the (required) data below an %MD5SUM% identifier in a 'desc' file, which
+        identifies a package's md5 checksum
+    name: str
+        The attribute can be used to describe the (required) data below a %NAME% identifier in a 'desc' file, which
+        identifies a package's name
+    optdepends: list[str] | None
+        The attribute can be used to describe the (optional) data below a %OPTDEPENDS% identifier in a 'desc' file,
+        which identifies what other package(s) a package optionally depends on
+    pgpsig: str | None
         The attribute can be used to describe the (required) data below a %PGPSIG% identifier in a 'desc' file, which
         identifies a package's PGP signature
     provides: list[str] | None
         The attribute can be used to describe the (optional) data below a %PROVIDES% identifier in a 'desc' file, which
         identifies what other package(s) a package provides
     replaces: list[str] | None
         The attribute can be used to describe the (optional) data below a %REPLACES% identifier in a 'desc' file, which
@@ -478,14 +632,23 @@
                     files = package.get("files")
                     if files:
                         if files.get("schema_version"):
                             del files["schema_version"]
                         package["files"] = FilesV1.model_validate(files)
 
                     return OutputPackageV1.model_validate(package)
+                case (2, 1):
+                    files = package.get("files")
+                    del package["schema_version"]
+                    if files:
+                        if files.get("schema_version"):
+                            del files["schema_version"]
+                        package["files"] = FilesV1.model_validate(files)
+
+                    return OutputPackageV2.model_validate(package)
                 # NOTE: the catch all can never be reached but is here to satisfy our tooling
                 case _:  # pragma: no cover
                     raise RuntimeError(
                         f"Invalid version provided for OutputPackage ({outputpackage_version} "
                         f"and/ or Files ({files_version})."
                     )
 
@@ -782,15 +945,14 @@
                             depends=package.depends,
                             desc=package.desc,
                             filename=package.filename,
                             groups=package.groups,
                             isize=package.isize,
                             license=package.license,
                             makedepends=self.makedepends,  # type: ignore[attr-defined]
-                            md5sum=package.md5sum,
                             name=package.name,
                             optdepends=package.optdepends,
                             packager=self.packager,  # type: ignore[attr-defined]
                             provides=package.provides,
                             replaces=package.replaces,
                             sha256sum=package.sha256sum,
                             url=package.url,
@@ -857,15 +1019,15 @@
         A path to which to output the JSON schema files
 
     Raises
     ------
     RuntimeError
         If output is not an existing directory
     """
-    classes = [OutputBuildInfoV1, OutputBuildInfoV2, OutputPackageV1, OutputPackageBaseV1]
+    classes = [OutputBuildInfoV1, OutputBuildInfoV2, OutputPackageV1, OutputPackageV2, OutputPackageBaseV1]
 
     if isinstance(output, str):
         output = Path(output)
 
     if not output.exists():
         raise RuntimeError(f"The output directory {output} must exist!")
```

### Comparing `repod-0.3.0.post0/repod/repo/package/__init__.py` & `repod-0.3.1/repod/repo/package/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Package repository handling for repod."""
+
 from repod.repo.package.repofile import RepoFile  # noqa: F401
 from repod.repo.package.syncdb import Files  # noqa: F401
 from repod.repo.package.syncdb import PackageDesc  # noqa: F401
 from repod.repo.package.syncdb import RepoDbMemberTypeEnum  # noqa: F401
 from repod.repo.package.syncdb import RepoDbTypeEnum  # noqa: F401
 from repod.repo.package.syncdb import SyncDatabase  # noqa: F401
 from repod.repo.package.syncdb import export_schemas  # noqa: F401
```

### Comparing `repod-0.3.0.post0/repod/repo/package/repofile.py` & `repod-0.3.1/repod/repo/package/repofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functions and helpers to work with files in repod managed repositories."""
+
 from itertools import zip_longest
 from logging import debug, info
 from pathlib import Path
 from re import Match, fullmatch
 from shutil import copy2
 from typing import Any
```

### Comparing `repod-0.3.0.post0/repod/repo/package/syncdb.py` & `repod-0.3.1/repod/repo/package/syncdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sync database handling."""
+
 from __future__ import annotations
 
 import io
 import re
 from enum import IntEnum
 from logging import debug, warning
 from pathlib import Path
@@ -39,14 +40,15 @@
     Name,
     OptDepends,
     Packager,
     PgpSig,
     Provides,
     Replaces,
     SchemaVersionV1,
+    SchemaVersionV2,
     Sha256Sum,
     Url,
     Version,
 )
 from repod.errors import (
     RepoManagementFileError,
     RepoManagementFileNotFoundError,
@@ -91,15 +93,15 @@
         "required": {
             "files",
         },
         "optional": set(),
     },
 }
 DEFAULT_FILES_VERSION = 1
-DEFAULT_PACKAGE_DESC_VERSION = 1
+DEFAULT_PACKAGE_DESC_VERSION = 2
 PACKAGE_DESC_VERSIONS: dict[int, dict[str, set[str] | int]] = {
     1: {
         "required": {
             "arch",
             "base",
             "builddate",
             "csize",
@@ -135,33 +137,33 @@
             "base",
             "builddate",
             "csize",
             "desc",
             "filename",
             "isize",
             "license",
-            "md5sum",
             "name",
             "packager",
             "sha256sum",
             "url",
             "version",
         },
         "optional": {
             "checkdepends",
             "conflicts",
             "depends",
             "backup",
             "groups",
             "makedepends",
             "optdepends",
+            "pgpsig",
             "provides",
             "replaces",
         },
-        "output_package_version": 1,
+        "output_package_version": 2,
         "output_package_base_version": 1,
     },
 }
 
 
 class RepoDbMemberTypeEnum(IntEnum):
     """An IntEnum to distinguish different types of files in a repository sync database.
@@ -720,25 +722,31 @@
             If no configuration is available for a given PackageDesc.schema_version
 
         Returns
         -------
         OutputPackage
             A pydantic model, that describes a package and its list of files
         """
+        # TODO: write detection version for
         schema_version = self.get_schema_version()
         schema_config = PACKAGE_DESC_VERSIONS.get(schema_version)
         desc_dict = self.model_dump(mode="json")
         if schema_config:
             output_package_version = schema_config.get("output_package_version")
             match output_package_version:
                 case 1:
                     if files:
                         desc_dict["files"] = files
 
                     return outputpackage.OutputPackageV1.model_validate(desc_dict)
+                case 2:
+                    if files:
+                        desc_dict["files"] = files
+
+                    return outputpackage.OutputPackageV2.model_validate(desc_dict)
                 case _:
                     raise RuntimeError(
                         f"The OutputPackage version '{output_package_version}' is not valid. This is a bug!"
                     )
         else:
             raise RepoManagementValidationError(
                 f"The schema version '{schema_version}' is not valid for creating a "
@@ -769,14 +777,15 @@
         -------
         OutputPackageBase
             A pydantic model, that describes a package base and one of it's split packages
         """
         schema_version = self.get_schema_version()
         schema_config = PACKAGE_DESC_VERSIONS.get(schema_version)
         desc_dict = self.model_dump(mode="json")
+        del desc_dict["schema_version"]
         if schema_config:
             output_package_version = schema_config.get("output_package_base_version")
             match output_package_version:
                 case 1:
                     desc_dict.update({"packages": [self.get_output_package(files=files)]})
                     return outputpackage.OutputPackageBaseV1.model_validate(desc_dict)
                 case _:
@@ -1145,16 +1154,16 @@
     optdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %OPTDEPENDS% identifier in a 'desc' file,
         which identifies what other package(s) a package optionally depends on
     packager: str
         The attribute can be used to describe the (required) data below a %PACKAGER% identifier in a 'desc' file, which
         identifies a package's packager
     pgpsig: str
-        The attribute can be used to describe the (optional) data below a %PGPSIG% identifier in a 'desc' file, which
-        identifies a package's PGP signature
+        The attribute can be used to describe the data below a %PGPSIG% identifier in a 'desc' file, which identifies a
+        package's PGP signature
     provides: list[str] | None
         The attribute can be used to describe the (optional) data below a %PROVIDES% identifier in a 'desc' file, which
         identifies what other package(s) a package provides
     replaces: list[str] | None
         The attribute can be used to describe the (optional) data below a %REPLACES% identifier in a 'desc' file, which
         identifies what other package(s) a package replaces
     schema_version: PositiveInt
@@ -1183,26 +1192,26 @@
     Depends,
     Desc,
     FileName,
     Groups,
     ISize,
     License,
     MakeDepends,
-    Md5Sum,
     Name,
     OptDepends,
     Packager,
+    PgpSig,
     Provides,
     Replaces,
-    SchemaVersionV1,
+    SchemaVersionV2,
     Sha256Sum,
     Url,
     Version,
 ):
-    """A model describing all identifiers in a 'desc' file (version 1).
+    """A model describing all identifiers in a 'desc' file (version 2).
 
     Attributes
     ----------
     arch: str
         The attribute can be used to describe the (required) data below an %ARCH% identifier in a 'desc' file, which
         identifies a package's architecture
     backup: list[str] | None
@@ -1240,26 +1249,26 @@
         identifies a package's installed size
     license: list[str]
         The attribute can be used to describe the (required) data below a %LICENSE% identifier in a 'desc' file, which
         identifies a package's license(s)
     makedepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %MAKEDEPENDS% identifier in a 'desc' file,
         which identifies a package's makedepends
-    md5sum: str
-        The attribute can be used to describe the (required) data below an %MD5SUM% identifier in a 'desc' file, which
-        identifies a package's md5 checksum
     name: str
         The attribute can be used to describe the (required) data below a %NAME% identifier in a 'desc' file, which
         identifies a package's name
     optdepends: list[str] | None
         The attribute can be used to describe the (optional) data below a %OPTDEPENDS% identifier in a 'desc' file,
         which identifies what other package(s) a package optionally depends on
     packager: str
         The attribute can be used to describe the (required) data below a %PACKAGER% identifier in a 'desc' file, which
         identifies a package's packager
+    pgpsig: str | None
+        The attribute can be used to describe the (optional) data below a %PGPSIG% identifier in a 'desc' file, which
+        identifies a package's PGP signature
     provides: list[str] | None
         The attribute can be used to describe the (optional) data below a %PROVIDES% identifier in a 'desc' file, which
         identifies what other package(s) a package provides
     replaces: list[str] | None
         The attribute can be used to describe the (optional) data below a %REPLACES% identifier in a 'desc' file, which
         identifies what other package(s) a package replaces
     schema_version: PositiveInt
```

### Comparing `repod-0.3.0.post0/repod/templates/desc_v1.j2` & `repod-0.3.1/repod/templates/desc_v1.j2`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/repod/templates/desc_v2.j2` & `repod-0.3.1/repod/templates/desc_v2.j2`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,21 @@
 {% endif %}
 %CSIZE%
 {{ csize }}
 
 %ISIZE%
 {{ isize }}
 
-%MD5SUM%
-{{ md5sum }}
-
 %SHA256SUM%
 {{ sha256sum }}
 
+{% if pgpsig %}
+%PGPSIG%
+{{ pgpsig }}
+
 {% endif %}
 %URL%
 {{ url }}
 
 {% if license %}
 %LICENSE%
 {% for license_ in license %}
```

### Comparing `repod-0.3.0.post0/repod/verification/pgp.py` & `repod-0.3.1/repod/verification/pgp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implementation of PGP based verification."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from logging import info
 from pathlib import Path
 
 from repod.commands import run_command
```

### Comparing `repod-0.3.0.post0/repod/version/alpm.py` & `repod-0.3.1/repod/version/alpm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """An implementation of libalpm functionality for version comparison."""
+
 from itertools import takewhile
 
 from .util import cmp
 
 PYALPM_VERCMP = False
 try:
     from pyalpm import vercmp as pyalpm_vercmp  # pragma: no-cover-nonlinux
```

### Comparing `repod-0.3.0.post0/repod/version/util.py` & `repod-0.3.1/repod/version/util.py`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/tests/action/test_check.py` & `repod-0.3.1/tests/action/test_check.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 def test_pacmankeypackagessignatureverificationcheck(
     with_signature: bool,
     verifies: bool,
     return_value: ActionStateEnum,
     default_package_file: tuple[Path, ...],
 ) -> None:
     check_ = check.PacmanKeyPackagesSignatureVerificationCheck(
-        packages=[[default_package_file[0], default_package_file[1]]]
-        if with_signature
-        else [[default_package_file[0]]],
+        packages=(
+            [[default_package_file[0], default_package_file[1]]] if with_signature else [[default_package_file[0]]]
+        ),
     )
     with patch("repod.action.check.PacmanKeyVerifier.verify", return_value=verifies):
         assert check_() == return_value  # nosec: B101
 
 
 @mark.parametrize(
     "debug, package_type, return_value",
@@ -124,15 +124,15 @@
     arch: str,
     return_value: ActionStateEnum,
     packagev1: Package,
     caplog: LogCaptureFixture,
 ) -> None:
     caplog.set_level(DEBUG)
 
-    packagev1.filename = filename
+    packagev1.filename = filename  # type: ignore[attr-defined]
     packagev1.pkginfo.name = name  # type: ignore[attr-defined]
     packagev1.pkginfo.version = version  # type: ignore[attr-defined]
     packagev1.pkginfo.arch = arch  # type: ignore[attr-defined]
     check_ = check.MatchingFilenameCheck(packages_and_paths=[(packagev1, Path(filename))])
     assert check_() == return_value  # nosec: B101
 
 
@@ -150,17 +150,17 @@
     caplog: LogCaptureFixture,
 ) -> None:
     caplog.set_level(DEBUG)
 
     new_outputpackagebase1 = deepcopy(outputpackagebasev1)
     new_outputpackagebase2 = deepcopy(outputpackagebasev1)
     if increase_version:
-        new_outputpackagebase1.version = "2:1.0.0-1"
-        new_outputpackagebase2.version = "2:1.0.0-1"
-        new_outputpackagebase2.base = "baz"
+        new_outputpackagebase1.version = "2:1.0.0-1"  # type: ignore[attr-defined]
+        new_outputpackagebase2.version = "2:1.0.0-1"  # type: ignore[attr-defined]
+        new_outputpackagebase2.base = "baz"  # type: ignore[attr-defined]
 
     check_ = check.PkgbasesVersionUpdateCheck(
         new_pkgbases=[new_outputpackagebase1, new_outputpackagebase2],
         current_pkgbases=[outputpackagebasev1],
     )
     assert check_() == return_value  # nosec: B101
 
@@ -186,18 +186,18 @@
     outputpackagebasev1_json_files_in_dir: Path,
     tmp_path: Path,
     caplog: LogCaptureFixture,
 ) -> None:
     caplog.set_level(DEBUG)
 
     if change_new_base:
-        outputpackagebasev1.base = "beh"
+        outputpackagebasev1.base = "beh"  # type: ignore[attr-defined]
 
     if increase_version:
-        outputpackagebasev1.version = "2:1.0.0-1"
+        outputpackagebasev1.version = "2:1.0.0-1"  # type: ignore[attr-defined]
 
     if not create_symlink:
         rmtree(outputpackagebasev1_json_files_in_dir / "pkgnames")
 
     check_ = check.PackagesNewOrUpdatedCheck(
         directory=outputpackagebasev1_json_files_in_dir,
         new_pkgbases=[outputpackagebasev1],
@@ -233,27 +233,33 @@
     caplog: LogCaptureFixture,
 ) -> None:
     caplog.set_level(DEBUG)
 
     new_pkgbase = outputpackagebasev1
     current_pkgbase = deepcopy(new_pkgbase)
     if new_pkgbase_provides_url:
-        new_pkgbase.source_url = TypeAdapter(AnyUrl).validate_python("https://foobar.com/foo/bar")
+        new_pkgbase.source_url = TypeAdapter(AnyUrl).validate_python(  # type: ignore[attr-defined]
+            "https://foobar.com/foo/bar"
+        )
     if current_pkgbase_provides_url:
-        current_pkgbase.source_url = TypeAdapter(AnyUrl).validate_python("https://foobar.com/foo/bar")
+        current_pkgbase.source_url = TypeAdapter(AnyUrl).validate_python(  # type: ignore[attr-defined]
+            "https://foobar.com/foo/bar"
+        )
 
     check_ = check.SourceUrlCheck(
         new_pkgbases=[new_pkgbase],
         current_pkgbases=[current_pkgbase],
-        url_validation_settings=UrlValidationSettings(
-            urls=["https://foobar.com/foo/"] if url_matches else ["https://beh.com/foo/"],  # type: ignore[list-item]
-            tls_required=True,
-        )
-        if require_validation
-        else None,
+        url_validation_settings=(
+            UrlValidationSettings(
+                urls=["https://foobar.com/foo/"] if url_matches else ["https://beh.com/foo/"],  # type: ignore
+                tls_required=True,
+            )
+            if require_validation
+            else None
+        ),
     )
 
     assert check_() == return_value  # nosec: B101
 
 
 @mark.parametrize(
     "pkgbase_version, pkgbase_above_version, pkgbase_below_version, return_value",
@@ -274,25 +280,25 @@
     outputpackagebasev1: OutputPackageBase,
 ) -> None:
     pkgbases = []
     pkgbases_above = []
     pkgbases_below = []
 
     pkgbase = outputpackagebasev1
-    pkgbase.version = pkgbase_version
+    pkgbase.version = pkgbase_version  # type: ignore[attr-defined]
     pkgbases.append(pkgbase)
 
     if pkgbase_above_version is not None:
         pkgbase_above = deepcopy(pkgbase)
-        pkgbase_above.version = pkgbase_above_version
+        pkgbase_above.version = pkgbase_above_version  # type: ignore[attr-defined]
         pkgbases_above.append(pkgbase_above)
 
     if pkgbase_below_version is not None:
         pkgbase_below = deepcopy(pkgbase)
-        pkgbase_below.version = pkgbase_below_version
+        pkgbase_below.version = pkgbase_below_version  # type: ignore[attr-defined]
         pkgbases_below.append(pkgbase_below)
 
     check_ = check.StabilityLayerCheck(
         pkgbases=pkgbases,
         pkgbases_above=pkgbases_above,
         pkgbases_below=pkgbases_below,
     )
@@ -312,17 +318,19 @@
     outputpackagebasev1: OutputPackageBase,
     caplog: LogCaptureFixture,
 ) -> None:
     caplog.set_level(DEBUG)
 
     check_ = check.ReproducibleBuildEnvironmentCheck(
         pkgbases=[outputpackagebasev1],
-        available_requirements=set(outputpackagebasev1.buildinfo.installed)  # type: ignore[arg-type,attr-defined]
-        if in_available_requirements
-        else {},
+        available_requirements=(
+            set(outputpackagebasev1.buildinfo.installed)  # type: ignore[arg-type,attr-defined]
+            if in_available_requirements
+            else {}
+        ),
     )
     assert check_() == return_value  # nosec: B101
 
 
 @mark.parametrize(
     "pkgbase_names, pkgbase_exists, package_names, package_exists, return_value",
     [
```

### Comparing `repod-0.3.0.post0/tests/action/test_task.py` & `repod-0.3.1/tests/action/test_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.action.task."""
+
 from contextlib import nullcontext as does_not_raise
 from copy import deepcopy
 from logging import DEBUG
 from pathlib import Path
 from typing import ContextManager
 from unittest.mock import Mock, patch
 
@@ -1478,15 +1479,15 @@
 ) -> None:
     """Tests for repod.action.task.ConsolidateOutputPackageBasesTask.do."""
     caplog.set_level(DEBUG)
 
     pkgbases = [outputpackagebasev1]
     if pkgbase_without_file:
         other_pkgbase = deepcopy(outputpackagebasev1)
-        other_pkgbase.base = "beh"
+        other_pkgbase.base = "beh"  # type: ignore[attr-defined]
         pkgbases.append(other_pkgbase)
 
     dependencies = [
         Mock(),
     ]
     if add_required_dep:
         dependencies.append(
```

### Comparing `repod-0.3.0.post0/tests/action/test_workflow.py` & `repod-0.3.1/tests/action/test_workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.action.workflow."""
+
 from logging import DEBUG
 from unittest.mock import Mock, patch
 
 from pytest import LogCaptureFixture, mark
 
 from repod.action import workflow
 from repod.common.enums import ActionStateEnum
```

### Comparing `repod-0.3.0.post0/tests/archive/test_archive.py` & `repod-0.3.1/tests/archive/test_archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.archive.archive."""
+
 from contextlib import nullcontext as does_not_raise
 from pathlib import Path
 from typing import ContextManager
 
 from pytest import mark, raises
 
 from repod.archive import archive
```

### Comparing `repod-0.3.0.post0/tests/cli/test_argparse.py` & `repod-0.3.1/tests/cli/test_argparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.cli.argparse."""
+
 from contextlib import nullcontext as does_not_raise
 from typing import ContextManager
 from unittest.mock import Mock, patch
 
 from pydantic import AnyUrl, TypeAdapter
 from pytest import mark, raises
```

### Comparing `repod-0.3.0.post0/tests/cli/test_cli.py` & `repod-0.3.1/tests/cli/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.cli.cli."""
+
 from argparse import ArgumentParser, ArgumentTypeError, Namespace
 from logging import DEBUG
 from pathlib import Path
 from random import sample
 from re import Match, fullmatch
 from tempfile import TemporaryDirectory
 from unittest.mock import Mock, patch
```

### Comparing `repod-0.3.0.post0/tests/common/test_enums.py` & `repod-0.3.1/tests/common/test_enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.common.enums."""
+
 from contextlib import nullcontext as does_not_raise
 from typing import ContextManager
 
 from pytest import mark, raises
 
 from repod.common import enums
```

### Comparing `repod-0.3.0.post0/tests/common/test_models.py` & `repod-0.3.1/tests/common/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Tests for repod.common.models."""
+
 from contextlib import nullcontext as does_not_raise
 from typing import ContextManager
 from unittest.mock import patch
 
 from pydantic import ValidationError
 from pytest import mark, raises
-from pytest_lazyfixture import lazy_fixture
+from pytest_lazy_fixtures import lf
 
 from repod.common import models
 from repod.version.alpm import vercmp
 from tests.conftest import (
     create_default_full_version,
     create_default_invalid_full_version,
 )
@@ -173,15 +174,15 @@
         ("1", "1.1", -1),
         ("1.1", "1", 1),
         ("1.1", "1.1", 0),
         ("1.2", "1.1", 1),
         ("1.1", "1.2", -1),
     ],
 )
-@mark.parametrize("pyalpm_vercmp", [lazy_fixture("pyalpm_vercmp_fun")])
+@mark.parametrize("pyalpm_vercmp", [lf("pyalpm_vercmp_fun")])
 def test_pkgrel_vercmp(subj: str, obj: str, expectation: int, pyalpm_vercmp: bool) -> None:
     """Tests for repod.common.models.PkgRel comparing using vercmp."""
     with patch("repod.version.alpm.PYALPM_VERCMP", pyalpm_vercmp):
         assert expectation == vercmp(  # nosec: B101
             a=models.PkgRel(pkgrel=subj).pkgrel, b=models.PkgRel(pkgrel=obj).pkgrel
         )
 
@@ -250,15 +251,15 @@
         ("1.0", "1+0", 0),
         ("1.1a1", "1.111", -1),
         ("01", "1", 0),
         ("001a", "1a", 0),
         ("1.a001a.1", "1.a1a.1", 0),
     ],
 )
-@mark.parametrize("pyalpm_vercmp", [lazy_fixture("pyalpm_vercmp_fun")])
+@mark.parametrize("pyalpm_vercmp", [lf("pyalpm_vercmp_fun")])
 def test_pkgver_vercmp(subj: str, obj: str, expectation: int, pyalpm_vercmp: bool) -> None:
     """Tests for repod.common.models.PkgVer comparing using vercmp."""
     with patch("repod.version.alpm.PYALPM_VERCMP", pyalpm_vercmp):
         assert expectation == vercmp(  # nosec: B101
             a=models.PkgVer(pkgver=subj).pkgver, b=models.PkgVer(pkgver=obj).pkgver
         )
 
@@ -335,15 +336,15 @@
         ("1:1.0.0-1", "1:1.0.1-1", -1),
         ("2:1.0.0-1", "1:1.0.0-1", 1),
         ("1:1.0.0-1", "2:1.0.1-1", -1),
         ("1:1.0.0-1", "1.0.0-1", 1),
         ("1.0.0-1", "1:1.0.0-1", -1),
     ],
 )
-@mark.parametrize("pyalpm_vercmp", [lazy_fixture("pyalpm_vercmp_fun")])
+@mark.parametrize("pyalpm_vercmp", [lf("pyalpm_vercmp_fun")])
 def test_version_vercmp(subj: str, obj: str, expectation: int, pyalpm_vercmp: bool) -> None:
     """Tests for repod.common.models.Version.vercmp."""
     with patch("repod.version.alpm.PYALPM_VERCMP", pyalpm_vercmp):
         assert models.Version(version=subj).vercmp(version=models.Version(version=obj)) == expectation  # nosec: B101
 
 
 @mark.parametrize(
```

### Comparing `repod-0.3.0.post0/tests/common/test_regex.py` & `repod-0.3.1/tests/common/test_regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.common.regex."""
+
 from re import Match, fullmatch
 
 from pytest import mark
 
 from repod.common import regex
```

### Comparing `repod-0.3.0.post0/tests/config/test_settings.py` & `repod-0.3.1/tests/config/test_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,27 +358,29 @@
                             conf = settings.SystemSettings(
                                 archiving=archiving,
                                 management_repo=(
                                     settings.ManagementRepo(directory=Path("/custom_management_repo"))
                                     if has_managementrepo
                                     else None
                                 ),
-                                repositories=[
-                                    settings.PackageRepo(
-                                        architecture="any",  # type: ignore[arg-type]
-                                        name="custom",  # type: ignore[arg-type]
-                                        management_repo=settings.ManagementRepo(
-                                            directory=Path("/custom_management_repo")
-                                        ),
-                                        package_pool=Path("/custom_package_pool"),
-                                        source_pool=Path("/custom_source_pool"),
-                                    )
-                                ]
-                                if has_repositories
-                                else [],
+                                repositories=(
+                                    [
+                                        settings.PackageRepo(
+                                            architecture="any",  # type: ignore[arg-type]
+                                            name="custom",  # type: ignore[arg-type]
+                                            management_repo=settings.ManagementRepo(
+                                                directory=Path("/custom_management_repo")
+                                            ),
+                                            package_pool=Path("/custom_package_pool"),
+                                            source_pool=Path("/custom_source_pool"),
+                                        )
+                                    ]
+                                    if has_repositories
+                                    else []
+                                ),
                             )
                             assert isinstance(conf, settings.SystemSettings)  # nosec: B101
                             assert len(conf.repositories) > 0  # nosec: B101
 
                             create_repository_directories_mock.assert_called_once()
                             ensure_non_overlapping_repositories_mock.assert_called_once()
                             check_repository_groups_dirs_mock.assert_called_once()
@@ -439,28 +441,30 @@
                                 archiving=archiving,
                                 build_requirements_exist=build_requirements_exist,
                                 management_repo=(
                                     settings.ManagementRepo(directory=Path("/custom_management_repo"))
                                     if has_managementrepo
                                     else None
                                 ),
-                                repositories=[
-                                    settings.PackageRepo(
-                                        architecture="any",  # type: ignore[arg-type]
-                                        build_requirements_exist=None,
-                                        name="custom",  # type: ignore[arg-type]
-                                        management_repo=settings.ManagementRepo(
-                                            directory=Path("/custom_management_repo")
-                                        ),
-                                        package_pool=Path("/custom_package_pool"),
-                                        source_pool=Path("/custom_source_pool"),
-                                    )
-                                ]
-                                if has_repositories
-                                else [],
+                                repositories=(
+                                    [
+                                        settings.PackageRepo(
+                                            architecture="any",  # type: ignore[arg-type]
+                                            build_requirements_exist=None,
+                                            name="custom",  # type: ignore[arg-type]
+                                            management_repo=settings.ManagementRepo(
+                                                directory=Path("/custom_management_repo")
+                                            ),
+                                            package_pool=Path("/custom_package_pool"),
+                                            source_pool=Path("/custom_source_pool"),
+                                        )
+                                    ]
+                                    if has_repositories
+                                    else []
+                                ),
                             )
                             assert isinstance(conf, settings.UserSettings)  # nosec: B101
                             assert len(conf.repositories) > 0  # nosec: B101
 
                             create_repository_directories_mock.assert_called_once()
                             ensure_non_overlapping_repositories_mock.assert_called_once()
                             check_repository_groups_dirs_mock.assert_called_once()
@@ -2022,16 +2026,16 @@
 
     if expanduser_raises:
         expanduser_mock.side_effect = RuntimeError
 
     with expectation:
         archiving = settings.ArchiveSettings(packages=packages, sources=sources)
 
-        assert packages_return_value == archiving.packages  # nosec: B101
-        assert sources_return_value == archiving.sources  # nosec: B101
+        assert packages_return_value == archiving.packages  # type: ignore[comparison-overlap] # nosec: B101
+        assert sources_return_value == archiving.sources  # type: ignore[comparison-overlap]  # nosec: B101
 
 
 @mark.parametrize(
     "settings_type, expectation",
     [
         (SettingsTypeEnum.USER, does_not_raise()),
         (SettingsTypeEnum.SYSTEM, does_not_raise()),
```

### Comparing `repod-0.3.0.post0/tests/conftest.py` & `repod-0.3.1/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pytest conftest."""
+
 import gzip
 import sys
 from copy import deepcopy
 from io import BytesIO, StringIO
 from logging import DEBUG, debug
 from os import chdir
 from pathlib import Path
@@ -35,15 +36,15 @@
     PackageRepo,
     UserSettings,
 )
 from repod.files import open_tarfile
 from repod.files.buildinfo import BuildInfo, BuildInfoV1, BuildInfoV2
 from repod.files.common import ZstdTarFile
 from repod.files.mtree import MTree, MTreeEntryV1
-from repod.files.package import PackageV1
+from repod.files.package import PackageV1, PackageV2
 from repod.files.pkginfo import PkgInfo, PkgInfoV1, PkgInfoV2, PkgType
 from repod.repo.management import OutputBuildInfo, OutputPackageBase
 from repod.repo.management.outputpackage import OutputPackageBaseV1, OutputPackageV1
 from repod.repo.package import Files, PackageDesc, RepoDbTypeEnum
 from repod.repo.package.repofile import relative_to_shared_base
 from repod.repo.package.syncdb import (
     FilesV1,
@@ -867,14 +868,33 @@
         mtree=valid_mtree,
         pkginfo=valid_pkginfov1,
         sha256sum=sha256sum,
     )
 
 
 @fixture(scope="function")
+def packagev2(
+    default_filename: str,
+    sha256sum: str,
+    valid_buildinfov1: BuildInfo,
+    valid_mtree: MTree,
+    valid_pkginfov1: PkgInfo,
+) -> PackageV2:
+    """Return a PackageV2 using BuildInfoV1 and PkgInfoV1."""
+    return PackageV2(
+        buildinfo=valid_buildinfov1,
+        csize=1,
+        filename=default_filename,
+        mtree=valid_mtree,
+        pkginfo=valid_pkginfov1,
+        sha256sum=sha256sum,
+    )
+
+
+@fixture(scope="function")
 def packagev1_pkginfov2(
     default_filename: str,
     md5sum: str,
     sha256sum: str,
     valid_buildinfov1: BuildInfo,
     valid_mtree: MTree,
     valid_pkginfov2: PkgInfo,
@@ -1434,15 +1454,14 @@
         base="foo",
         builddate=1,
         csize=1,
         desc=default_description,
         filename=default_filename,
         isize=1,
         license=[default_license],
-        md5sum=md5sum,
         name="foo",
         packager=default_packager,
         sha256sum=sha256sum,
         url=url,  # type: ignore[arg-type]
         version=default_full_version,
     )
```

### Comparing `repod-0.3.0.post0/tests/files/test_buildinfo.py` & `repod-0.3.1/tests/files/test_buildinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.files.buildinfo."""
+
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from pathlib import Path
 from random import sample
 from re import Match, fullmatch
 from tempfile import TemporaryDirectory
 from typing import ContextManager
```

### Comparing `repod-0.3.0.post0/tests/files/test_common.py` & `repod-0.3.1/tests/files/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.files.common."""
+
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from pathlib import Path
 from tarfile import TarFile
 from typing import ContextManager
 from unittest.mock import patch
```

### Comparing `repod-0.3.0.post0/tests/files/test_mtree.py` & `repod-0.3.1/tests/files/test_mtree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.files.mtree."""
+
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from logging import DEBUG
 from pathlib import Path
 from random import choice, randrange, sample
 from re import Match, fullmatch
 from string import ascii_lowercase, digits
```

### Comparing `repod-0.3.0.post0/tests/files/test_pkginfo.py` & `repod-0.3.1/tests/files/test_pkginfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.files.pkginfo."""
+
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from logging import DEBUG
 from pathlib import Path
 from random import sample
 from re import Match, fullmatch
 from typing import Any, ContextManager
```

### Comparing `repod-0.3.0.post0/tests/files/test_srcinfo.py` & `repod-0.3.1/tests/files/test_srcinfo.py`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/tests/repo/package/test_repofile.py` & `repod-0.3.1/tests/repo/package/test_repofile.py`

 * *Files identical despite different names*

### Comparing `repod-0.3.0.post0/tests/repo/package/test_syncdb.py` & `repod-0.3.1/tests/repo/package/test_syncdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.repo.package.syncdb."""
+
 from contextlib import nullcontext as does_not_raise
 from io import StringIO
 from logging import DEBUG
 from pathlib import Path
 from textwrap import dedent
 from typing import Any, ContextManager
 from unittest.mock import patch
@@ -388,15 +389,14 @@
                 "base": "foo",
                 "builddate": -1,
                 "csize": 1,
                 "desc": "foo",
                 "filename": create_default_filename(),
                 "isize": 1,
                 "license": ["foo"],
-                "md5sum": create_md5sum(),
                 "name": "foo",
                 "packager": create_default_packager(),
                 "sha256sum": create_sha256sum(),
                 "url": create_url(),
                 "version": create_default_full_version(),
             },
             False,
@@ -932,15 +932,15 @@
     expectation: ContextManager[str],
 ) -> None:
     """Tests for repod.repo.package.syncdb.PackageDesc.get_output_package."""
     output_package = outputpackagev1
     package_desc = packagedescv1
     files = filesv1
     if no_files:
-        output_package.files = None
+        output_package.files = None  # type: ignore[attr-defined]
         files = None
     if invalid_packagedesc_version:
         package_desc = PackageDescV9999()
 
     with expectation:
         assert output_package == package_desc.get_output_package(files)  # nosec: B101
 
@@ -972,15 +972,15 @@
     """Tests for repod.repo.package.syncdb.PackageDescV1.get_output_package_base."""
     output_package_base = outputpackagebasev1
     package_desc = packagedescv1
     files = filesv1
     # remove all but the first package
     output_package_base.packages = output_package_base.packages[0:1]  # type: ignore[attr-defined]
     # remove buildinfo data (when converting from sync databases we do not have the data available)
-    output_package_base.buildinfo = None
+    output_package_base.buildinfo = None  # type: ignore[attr-defined]
 
     if no_files:
         files = None
         output_package_base.packages[0].files = None  # type: ignore[attr-defined]
     if invalid_package_desc:
         package_desc = PackageDescV9999()
```

### Comparing `repod-0.3.0.post0/tests/test_commands.py` & `repod-0.3.1/tests/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.commands."""
+
 from contextlib import nullcontext as does_not_raise
 from pathlib import Path
 from subprocess import CalledProcessError  # nosec: B404
 from typing import ContextManager
 
 from pytest import mark, raises
```

### Comparing `repod-0.3.0.post0/tests/verification/test_pgp.py` & `repod-0.3.1/tests/verification/test_pgp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.verification.pgp."""
+
 from logging import DEBUG
 from pathlib import Path
 from random import sample
 from re import Match, fullmatch
 from unittest.mock import Mock, patch
 
 from pytest import LogCaptureFixture, mark
```

### Comparing `repod-0.3.0.post0/tests/version/test_alpm.py` & `repod-0.3.1/tests/version/test_alpm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Tests for repod.version.alpm."""
+
 from unittest.mock import patch
 
 from pytest import mark
-from pytest_lazyfixture import lazy_fixture
+from pytest_lazy_fixtures import lf
 
 from repod.version.alpm import pkg_vercmp, vercmp
 
 
 @mark.parametrize(
     "first, second, expectation",
     [
@@ -54,27 +55,27 @@
         ("001a", "1a", 0),
         ("1.a001a.1", "1.a1a.1", 0),
         ("", "", 0),
         ("", "1", -1),
         ("", "a", 1),
     ],
 )
-@mark.parametrize("pyalpm_vercmp", [lazy_fixture("pyalpm_vercmp_fun")])
+@mark.parametrize("pyalpm_vercmp", [lf("pyalpm_vercmp_fun")])
 def test_vercmp(first: str, second: str, expectation: int, pyalpm_vercmp: bool) -> None:
     """Tests for repod.version.alpm.vercmp."""
     with patch("repod.version.alpm.PYALPM_VERCMP", pyalpm_vercmp):
         assert vercmp(a=first, b=second) == expectation  # nosec: B101
 
 
 @mark.parametrize(
     "first, second, expectation",
     [
         ("1-2", "1-2", 0),
         ("1:2-3", "2-3", 1),
         ("1:2-3", "1:2-4", -1),
     ],
 )
-@mark.parametrize("pyalpm_vercmp", [lazy_fixture("pyalpm_vercmp_fun")])
+@mark.parametrize("pyalpm_vercmp", [lf("pyalpm_vercmp_fun")])
 def test_pkgver_vercmp(first: str, second: str, expectation: int, pyalpm_vercmp: bool) -> None:
     """Tests for repod.version.alpm.pkg_vercmp."""
     with patch("repod.version.alpm.PYALPM_VERCMP", pyalpm_vercmp):
         assert pkg_vercmp(a=first, b=second) == expectation  # nosec: B101
```

### Comparing `repod-0.3.0.post0/tests/version/test_util.py` & `repod-0.3.1/tests/version/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for repod.version.util."""
+
 from pytest import mark
 
 from repod.version.util import cmp
 
 
 @mark.parametrize(
     "first, second, expectation",
```

### Comparing `repod-0.3.0.post0/PKG-INFO` & `repod-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repod
-Version: 0.3.0.post0
+Version: 0.3.1
 Summary: Tooling to maintain binary package repositories for Linux distributions using the pacman package manager
 Keywords: arch linux repository pacman packages
 Home-page: https://gitlab.archlinux.org/archlinux/repod
 Author-Email: Arch Linux <arch-projects@lists.archlinux.org>
 License: GPL-3.0-or-later
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -24,24 +24,24 @@
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Project-URL: Bug tracker, https://gitlab.archlinux.org/archlinux/repod/-/issues/
 Project-URL: Homepage, https://gitlab.archlinux.org/archlinux/repod
 Project-URL: Repository, https://gitlab.archlinux.org/archlinux/repod
 Project-URL: Documentation, https://repod.archlinux.page
-Requires-Python: <4.0,>=3.10
-Requires-Dist: aiofiles>=23.1.0
-Requires-Dist: email-validator>=2.0.0
-Requires-Dist: jinja2>=3.1.2
-Requires-Dist: orjson>=3.9.2
-Requires-Dist: pydantic>=2.0
-Requires-Dist: pydantic-settings>=2.0.2
+Requires-Python: >=3.10
+Requires-Dist: aiofiles>=23.2.1
+Requires-Dist: email-validator>=2.1.0
+Requires-Dist: jinja2>=3.1.3
+Requires-Dist: orjson>=3.9.15
+Requires-Dist: pydantic>=2.6.4
+Requires-Dist: pydantic-settings>=2.2.1
 Requires-Dist: python-magic>=0.4.27
 Requires-Dist: pyxdg>=0.28
-Requires-Dist: pyzstd>=0.15.7
+Requires-Dist: pyzstd>=0.15.10
 Requires-Dist: subprocess-tee>=0.4.1
 Requires-Dist: tomli>=2.0.1; python_version < "3.11"
 Requires-Dist: pyalpm<1.0.0,>=0.10.6; extra == "alt-vercmp"
 Requires-Dist: file-magic<1.0.0,>=0.4.0; extra == "alt-file"
 Provides-Extra: alt_vercmp
 Provides-Extra: alt_file
 Description-Content-Type: text/markdown
```

