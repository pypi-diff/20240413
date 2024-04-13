# Comparing `tmp/pylops-mpi-0.0.1.tar.gz` & `tmp/pylops-mpi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylops-mpi-0.0.1.tar", last modified: Mon Aug 28 04:52:49 2023, max compression
+gzip compressed data, was "pylops-mpi-0.1.0.tar", last modified: Sat Apr 13 13:13:33 2024, max compression
```

## Comparing `pylops-mpi-0.0.1.tar` & `pylops-mpi-0.1.0.tar`

### file list

```diff
@@ -1,100 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.766149 pylops-mpi-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.746149 pylops-mpi-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.754149 pylops-mpi-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     1424 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (999)      956 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (999)      857 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (999)      689 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/.github/workflows/flake.yml
--rw-r--r--   0 runner    (1001) docker     (999)      226 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)       48 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (999)     7652 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     1466 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (999)     5300 2023-08-28 04:52:49.766149 pylops-mpi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4625 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.754149 pylops-mpi-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (999)      638 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (999)       67 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (999)      495 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/pylops_mpi.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.754149 pylops-mpi-0.0.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.754149 pylops-mpi-0.0.1/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.754149 pylops-mpi-0.0.1/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (999)       67 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (999)    15406 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (999)    11533 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_static/pylopsmpi.png
--rw-r--r--   0 runner    (1001) docker     (999)    12273 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_static/pylopsmpi_b.png
--rw-r--r--   0 runner    (1001) docker     (999)     1908 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.754149 pylops-mpi-0.0.1/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.758149 pylops-mpi-0.0.1/docs/source/_templates/autosummary/
--rwxr-xr-x   0 runner    (1001) docker     (999)      160 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_templates/autosummary/base.rst
--rwxr-xr-x   0 runner    (1001) docker     (999)      760 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_templates/autosummary/class.rst
--rwxr-xr-x   0 runner    (1001) docker     (999)      157 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_templates/autosummary/exception.rst
--rwxr-xr-x   0 runner    (1001) docker     (999)      208 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_templates/autosummary/function.rst
--rwxr-xr-x   0 runner    (1001) docker     (999)      781 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_templates/autosummary/module.rst
--rwxr-xr-x   0 runner    (1001) docker     (999)      969 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (999)     8914 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/adding.rst
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.758149 pylops-mpi-0.0.1/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (999)     1132 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)      132 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (999)     4363 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (999)     3945 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (999)      278 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/credits.rst
--rw-r--r--   0 runner    (1001) docker     (999)     4582 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (999)     4561 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (999)      366 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (999)      165 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.758149 pylops-mpi-0.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (999)      533 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)     2156 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/examples/plot_cgls.py
--rw-r--r--   0 runner    (1001) docker     (999)     4677 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/examples/plot_derivative.py
--rw-r--r--   0 runner    (1001) docker     (999)     4510 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/examples/plot_distributed_array.py
--rw-r--r--   0 runner    (1001) docker     (999)     4095 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/examples/plot_mpilinop.py
--rw-r--r--   0 runner    (1001) docker     (999)     7190 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/examples/plot_stacking.py
--rw-r--r--   0 runner    (1001) docker     (999)      409 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/mpi_examples.sh
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.758149 pylops-mpi-0.0.1/pylops_mpi/
--rw-r--r--   0 runner    (1001) docker     (999)    21790 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/DistributedArray.py
--rw-r--r--   0 runner    (1001) docker     (999)    13440 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/LinearOperator.py
--rw-r--r--   0 runner    (1001) docker     (999)      605 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.762149 pylops-mpi-0.0.1/pylops_mpi/basicoperators/
--rw-r--r--   0 runner    (1001) docker     (999)     5306 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/basicoperators/BlockDiag.py
--rw-r--r--   0 runner    (1001) docker     (999)    12373 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/basicoperators/FirstDerivative.py
--rw-r--r--   0 runner    (1001) docker     (999)     3804 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/basicoperators/HStack.py
--rw-r--r--   0 runner    (1001) docker     (999)     5573 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/basicoperators/Laplacian.py
--rw-r--r--   0 runner    (1001) docker     (999)    10069 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/basicoperators/SecondDerivative.py
--rw-r--r--   0 runner    (1001) docker     (999)     5054 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/basicoperators/VStack.py
--rw-r--r--   0 runner    (1001) docker     (999)      823 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/basicoperators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.762149 pylops-mpi-0.0.1/pylops_mpi/optimization/
--rw-r--r--   0 runner    (1001) docker     (999)      321 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4835 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/optimization/basic.py
--rw-r--r--   0 runner    (1001) docker     (999)    17790 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/optimization/cls_basic.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.762149 pylops-mpi-0.0.1/pylops_mpi/plotting/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2749 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/plotting/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.762149 pylops-mpi-0.0.1/pylops_mpi/utils/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2926 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/pylops_mpi/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (999)      160 2023-08-28 04:52:49.000000 pylops-mpi-0.0.1/pylops_mpi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.758149 pylops-mpi-0.0.1/pylops_mpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     5300 2023-08-28 04:52:49.000000 pylops-mpi-0.0.1/pylops_mpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2190 2023-08-28 04:52:49.000000 pylops-mpi-0.0.1/pylops_mpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 04:52:49.000000 pylops-mpi-0.0.1/pylops_mpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       57 2023-08-28 04:52:49.000000 pylops-mpi-0.0.1/pylops_mpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-28 04:52:49.000000 pylops-mpi-0.0.1/pylops_mpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 04:52:49.000000 pylops-mpi-0.0.1/pylops_mpi.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      148 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)      213 2023-08-28 04:52:49.766149 pylops-mpi-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1392 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.750149 pylops-mpi-0.0.1/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.762149 pylops-mpi-0.0.1/testdata/avo/
--rw-r--r--   0 runner    (1001) docker     (999)  3531328 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/testdata/avo/poststack_model.npz
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.766149 pylops-mpi-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     1678 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tests/test_blockdiag.py
--rw-r--r--   0 runner    (1001) docker     (999)    13505 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tests/test_derivative.py
--rw-r--r--   0 runner    (1001) docker     (999)     9024 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tests/test_distributedarray.py
--rw-r--r--   0 runner    (1001) docker     (999)    13208 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tests/test_linearop.py
--rw-r--r--   0 runner    (1001) docker     (999)     8705 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (999)     3782 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tests/test_stack.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 04:52:49.766149 pylops-mpi-0.0.1/tutorials/
--rw-r--r--   0 runner    (1001) docker     (999)      431 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tutorials/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)     7165 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tutorials/plot_lsm.py
--rw-r--r--   0 runner    (1001) docker     (999)    10981 2023-08-28 04:52:36.000000 pylops-mpi-0.0.1/tutorials/plot_post_stack_inversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.835600 pylops-mpi-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.811600 pylops-mpi-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.819600 pylops-mpi-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/.github/workflows/flake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-04-13 13:13:33.835600 pylops-mpi-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.819600 pylops-mpi-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/pylops_mpi.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.819600 pylops-mpi-0.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.819600 pylops-mpi-0.1.0/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.819600 pylops-mpi-0.1.0/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    11533 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_static/pylopsmpi.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12273 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_static/pylopsmpi_b.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.823600 pylops-mpi-0.1.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.823600 pylops-mpi-0.1.0/docs/source/_templates/autosummary/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_templates/autosummary/base.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      760 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_templates/autosummary/class.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_templates/autosummary/exception.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      208 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_templates/autosummary/function.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      781 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_templates/autosummary/module.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      969 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/adding.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.823600 pylops-mpi-0.1.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.823600 pylops-mpi-0.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/examples/plot_cgls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/examples/plot_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/examples/plot_distributed_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/examples/plot_mpilinop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/examples/plot_stacked_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/examples/plot_stacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/mpi_examples.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.823600 pylops-mpi-0.1.0/pylops_mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)    27976 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/DistributedArray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/LinearOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15705 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/StackedLinearOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.827600 pylops-mpi-0.1.0/pylops_mpi/basicoperators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/basicoperators/BlockDiag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/basicoperators/FirstDerivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/basicoperators/Gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/basicoperators/HStack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/basicoperators/Laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/basicoperators/SecondDerivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/basicoperators/VStack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/basicoperators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.827600 pylops-mpi-0.1.0/pylops_mpi/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/optimization/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18464 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/optimization/cls_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.827600 pylops-mpi-0.1.0/pylops_mpi/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/plotting/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.827600 pylops-mpi-0.1.0/pylops_mpi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pylops_mpi/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 13:13:33.000000 pylops-mpi-0.1.0/pylops_mpi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.835600 pylops-mpi-0.1.0/pylops_mpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-04-13 13:13:33.000000 pylops-mpi-0.1.0/pylops_mpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-13 13:13:33.000000 pylops-mpi-0.1.0/pylops_mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:13:33.000000 pylops-mpi-0.1.0/pylops_mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 13:13:33.000000 pylops-mpi-0.1.0/pylops_mpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-13 13:13:33.000000 pylops-mpi-0.1.0/pylops_mpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-13 13:13:33.835600 pylops-mpi-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.815600 pylops-mpi-0.1.0/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.827600 pylops-mpi-0.1.0/testdata/avo/
+-rw-r--r--   0 runner    (1001) docker     (127)  3531328 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/testdata/avo/poststack_model.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.835600 pylops-mpi-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tests/test_blockdiag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15620 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tests/test_derivative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tests/test_distributedarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tests/test_linearop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tests/test_stackedarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15268 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tests/test_stackedlinearop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:13:33.835600 pylops-mpi-0.1.0/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tutorials/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tutorials/lsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12095 2024-04-13 13:13:28.000000 pylops-mpi-0.1.0/tutorials/poststack.py
```

### Comparing `pylops-mpi-0.0.1/.github/workflows/build.yml` & `pylops-mpi-0.1.0/.github/workflows/build.yml`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   workflow_dispatch:
   
 jobs:
   build:
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest]
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
         mpi: ['mpich', 'openmpi', 'intelmpi']
         exclude:
           - os: macos-latest
             mpi: 'intelmpi'
         # MPICH v4 fails on Ubuntu for Python <3.10
         # ”libfabric EFA provider is operating in a
         # condition that could result in memory
@@ -29,23 +29,27 @@
           - os: ubuntu-latest
             python-version: '3.9'
             mpi: 'mpich'
     runs-on: ${{ matrix.os }}
     steps:
       - name: Checkout
         uses: actions/checkout@v3
+      - name: Get history and tags for SCM versioning to work
+        run: |
+          git fetch --prune --unshallow
+          git fetch --depth=1 origin +refs/tags/*:refs/tags/*
       - name: Setup MPI
         uses: mpi4py/setup-mpi@v1
         with:
           mpi: ${{ matrix.mpi }}
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Installing Dependencies
         run: |
-          python -m pip install --upgrade pip
+          python -m pip install --upgrade pip setuptools
           if [ -f requirements.txt ]; then pip install -r requirements-dev.txt; fi
       - name: Install pylops-mpi
         run: pip install .
       - name: Testing using pytest-mpi
         run: mpiexec -n 2 pytest --with-mpi
```

### Comparing `pylops-mpi-0.0.1/.github/workflows/deploy-docs.yml` & `pylops-mpi-0.1.0/.github/workflows/deploy-docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -17,23 +17,23 @@
         uses: mpi4py/setup-mpi@v1
         with:
           mpi: 'openmpi'
 
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.x
+          python-version: 3.9
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           if [ -f requirements.txt ]; then pip install -r requirements-dev.txt; fi
           pip install .
       - name: Build docs
         run: |
           sphinx-build -b html ./docs/source ./docs/build
       - name: Deploy to GitHub Pages
         uses: peaceiris/actions-gh-pages@v3
         with:
           publish_branch: gh-pages
           personal_token: ${{ secrets.GITHUB_TOKEN }}
-          publish_dir: ./docs/build/
+          publish_dir: ./docs/build/
```

### Comparing `pylops-mpi-0.0.1/.github/workflows/deploy.yml` & `pylops-mpi-0.1.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/.github/workflows/flake.yml` & `pylops-mpi-0.1.0/.github/workflows/flake.yml`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/LICENSE` & `pylops-mpi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/Makefile` & `pylops-mpi-0.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/PKG-INFO` & `pylops-mpi-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pylops-mpi
-Version: 0.0.1
-Summary: Python library implementing linear operators with MPI
-Keywords: algebra,inverse problems,large-scale optimization
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![PyLops-MPI](https://github.com/PyLops/pylops-mpi/blob/main/docs/source/_static/pylopsmpi_b.png)
 
 [![Build status](https://github.com/PyLops/pylops-mpi/actions/workflows/build.yml/badge.svg)](https://github.com/PyLops/pylops-mpi/actions/workflows/build.yml)
 [![Documentation status](https://github.com/PyLops/pylops-mpi/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/PyLops/pylops-mpi/actions/workflows/pages/pages-build-deployment)
 ![OS-support](https://img.shields.io/badge/OS-linux,osx-850A8B.svg)
 [![Slack Status](https://img.shields.io/badge/chat-slack-green.svg)](https://pylops.slack.com)
 
@@ -35,17 +19,17 @@
 2. **Verify MPI Installation**: After installing MPI, verify its installation by opening a terminal or command prompt 
 and running the following command:
     ```
     mpiexec --version
    ```
  3. **Install pylops-mpi**: Once MPI is installed and verified, you can proceed to install `pylops-mpi`. 
    
-      You can install with `make` and `pip`:
+      You can install with `pip`:
       ```
-      make install
+      pip install pylops-mpi
       ```
    
       You can install with `make` and `conda`:
       ```
       make install_conda
       ```
```

### Comparing `pylops-mpi-0.0.1/docs/Makefile` & `pylops-mpi-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/_static/favicon.ico` & `pylops-mpi-0.1.0/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/_static/pylopsmpi.png` & `pylops-mpi-0.1.0/docs/source/_static/pylopsmpi.png`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/_static/pylopsmpi_b.png` & `pylops-mpi-0.1.0/docs/source/_static/pylopsmpi_b.png`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/_static/style.css` & `pylops-mpi-0.1.0/docs/source/_static/style.css`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/_templates/autosummary/class.rst` & `pylops-mpi-0.1.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/_templates/autosummary/module.rst` & `pylops-mpi-0.1.0/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/_templates/layout.html` & `pylops-mpi-0.1.0/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/adding.rst` & `pylops-mpi-0.1.0/docs/source/adding.rst`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/api/index.rst` & `pylops-mpi-0.1.0/docs/source/api/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,52 +13,57 @@
 .. currentmodule:: pylops_mpi
 
 .. autosummary::
    :toctree: generated/
 
     Partition
     DistributedArray
+    StackedDistributedArray
 
 Linear operators
 ----------------
 
 Templates
 ~~~~~~~~~
 
 .. currentmodule:: pylops_mpi
 
 .. autosummary::
    :toctree: generated/
 
     MPILinearOperator
     asmpilinearoperator
+    MPIStackedLinearOperator
 
 Basic Operators
 ~~~~~~~~~~~~~~~
 
 .. currentmodule:: pylops_mpi.basicoperators
 
 .. autosummary::
    :toctree: generated/
 
     MPIBlockDiag
+    MPIStackedBlockDiag
     MPIVStack
+    MPIStackedVStack
     MPIHStack
 
 Derivatives
 ~~~~~~~~~~~
 
 .. currentmodule:: pylops_mpi.basicoperators
 
 .. autosummary::
    :toctree: generated/
 
     MPIFirstDerivative
     MPISecondDerivative
     MPILaplacian
+    MPIGradient
 
 Solvers
 -------
 
 Basic
 ~~~~~
```

### Comparing `pylops-mpi-0.0.1/docs/source/conf.py` & `pylops-mpi-0.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/contributing.rst` & `pylops-mpi-0.1.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/index.rst` & `pylops-mpi-0.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/docs/source/installation.rst` & `pylops-mpi-0.1.0/docs/source/installation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -56,19 +56,20 @@
 
    >> make install_conda
 
 This will create and activate an environment called ``pylops_mpi``, with all required dependencies.
 
 Pip
 ===
-If you prefer a ``pip`` installation, we provide the following command
+If you prefer a ``pip`` installation, simply type the following command in your terminal to install the
+PyPI distribution:
 
 .. code-block:: bash
 
-   >> make install
+   >> pip install pylops-mpi
 
 When installing via pip, only required dependencies are installed.
 Note that, differently from the  ``conda`` command, the above **will not** create a virtual environment.
 Make sure you create and activate your environment previously.
 
 .. _DevInstall:
```

### Comparing `pylops-mpi-0.0.1/examples/README.rst` & `pylops-mpi-0.1.0/examples/README.rst`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/examples/plot_cgls.py` & `pylops-mpi-0.1.0/examples/plot_cgls.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 ###############################################################################
 # We now utilize the cgls solver to obtain the inverse of the ``MPIBlockDiag``.
 # In the case of MPIBlockDiag, each operator is responsible for performing
 # an inversion operation iteratively at a specific rank. The resulting inversions
 # are then obtained in a :py:class:`pylops_mpi.DistributedArray`. To obtain the
 # overall inversion of the entire MPIBlockDiag, you can utilize the ``asarray()``
 # function of the DistributedArray as shown below.
-xinv, istop, niter, r1norm, r2norm, cost = pylops_mpi.cgls(BDiag, y, niter=15, tol=1e-10, show=True)
+
+# Set initial guess `x0` to zeroes
+x0 = pylops_mpi.DistributedArray(BDiag.shape[1], dtype=np.float128)
+x0[:] = 0
+xinv, istop, niter, r1norm, r2norm, cost = pylops_mpi.cgls(BDiag, y, x0=x0, niter=15, tol=1e-10, show=True)
 xinv_array = xinv.asarray()
 
 if rank == 0:
     print(f"CGLS Solution xinv={xinv_array}")
     # Visualize
     plt.figure(figsize=(18, 5))
     plt.plot(cost, lw=2, label="CGLS")
```

### Comparing `pylops-mpi-0.0.1/examples/plot_derivative.py` & `pylops-mpi-0.1.0/examples/plot_derivative.py`

 * *Files 16% similar despite different names*

```diff
@@ -120,7 +120,41 @@
     plt.colorbar(im, ax=axs[1])
     im = axs[2].imshow(yasym, interpolation="nearest", cmap="rainbow")
     axs[2].axis("tight")
     axs[2].set_title("y asym")
     plt.colorbar(im, ax=axs[2])
     plt.tight_layout()
     plt.subplots_adjust(top=0.8)
+
+###############################################################################
+# We now consider the :py:class:`pylops_mpi.basicoperators.MPIGradient` operator.
+# Given a 2-dimensional array, this operator applies first-order derivatives on both
+# dimensions and concatenates them.
+Gop = pylops_mpi.MPIGradient(dims=(nx, ny), dtype=np.float64)
+
+y_grad_dist = Gop @ x_dist
+# Reshaping to (ndims, nx, ny) for plotting
+y_grad = y_grad_dist.asarray().reshape((2, nx, ny))
+y_grad_adj_dist = Gop.H @ y_grad_dist
+# Reshaping to (nx, ny) for plotting
+y_grad_adj = y_grad_adj_dist.asarray().reshape((nx, ny))
+
+if rank == 0:
+    fig, axs = plt.subplots(2, 2, figsize=(10, 6), sharex=True, sharey=True)
+    fig.suptitle("Gradient", fontsize=12, fontweight="bold", y=0.95)
+    im = axs[0, 0].imshow(x, interpolation="nearest", cmap="rainbow")
+    axs[0, 0].axis("tight")
+    axs[0, 0].set_title("x")
+    plt.colorbar(im, ax=axs[0, 0])
+    im = axs[0, 1].imshow(y_grad[0, ...], interpolation="nearest", cmap="rainbow")
+    axs[0, 1].axis("tight")
+    axs[0, 1].set_title("y - 1st direction")
+    plt.colorbar(im, ax=axs[0, 1])
+    im = axs[1, 1].imshow(y_grad[1, ...], interpolation="nearest", cmap="rainbow")
+    axs[1, 1].axis("tight")
+    axs[1, 1].set_title("y - 2nd direction")
+    plt.colorbar(im, ax=axs[1, 1])
+    im = axs[1, 0].imshow(y_grad_adj, interpolation="nearest", cmap="rainbow")
+    axs[1, 0].axis("tight")
+    axs[1, 0].set_title("xadj")
+    plt.colorbar(im, ax=axs[1, 0])
+    plt.tight_layout()
```

### Comparing `pylops-mpi-0.0.1/examples/plot_distributed_array.py` & `pylops-mpi-0.1.0/examples/plot_distributed_array.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,20 +68,33 @@
 array = array / 2.0
 arr2 = pylops_mpi.DistributedArray.to_dist(x=array.reshape(global_shape), axis=1)
 # plot local arrays
 pylops_mpi.plot_local_arrays(arr1, "Distributed Array - 1", vmin=0, vmax=1)
 pylops_mpi.plot_local_arrays(arr2, "Distributed Array - 2", vmin=0, vmax=1)
 
 ###############################################################################
+# **Scaling** - Each process operates on its local portion of
+# the array and scales the corresponding elements by a given scalar.
+scale_arr = .5 * arr1
+pylops_mpi.plot_local_arrays(scale_arr, "Scaling", vmin=0, vmax=1)
+
+###############################################################################
 # **Element-wise Addition** - Each process operates on its local portion of
 # the array and adds the corresponding elements together.
 sum_arr = arr1 + arr2
 pylops_mpi.plot_local_arrays(sum_arr, "Addition", vmin=0, vmax=1)
 
 ###############################################################################
+# **Element-wise In-place Addition** - Similar to the previous one but the
+# addition is performed directly on one of the addends without creating a new
+# distributed array.
+sum_arr += arr2
+pylops_mpi.plot_local_arrays(sum_arr, "Addition", vmin=0, vmax=1)
+
+###############################################################################
 # **Element-wise Subtraction** - Each process operates on its local portion
 # of the array and subtracts the corresponding elements together.
 diff_arr = arr1 - arr2
 pylops_mpi.plot_local_arrays(diff_arr, "Subtraction", vmin=0, vmax=1)
 
 ###############################################################################
 # **Element-wise Multiplication** - Each process operates on its local portion
```

### Comparing `pylops-mpi-0.0.1/examples/plot_mpilinop.py` & `pylops-mpi-0.1.0/examples/plot_mpilinop.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/examples/plot_stacking.py` & `pylops-mpi-0.1.0/examples/plot_stacking.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/pylops_mpi/DistributedArray.py` & `pylops-mpi-0.1.0/pylops_mpi/DistributedArray.py`

 * *Files 23% similar despite different names*

```diff
@@ -337,44 +337,67 @@
                                dtype=self.dtype)
         arr[:] = -self.local_array
         return arr
 
     def __add__(self, x):
         return self.add(x)
 
+    def __iadd__(self, x):
+        return self.iadd(x)
+
     def __sub__(self, x):
         return self.__add__(-x)
 
+    def __isub__(self, x):
+        return self.__iadd__(-x)
+
     def __mul__(self, x):
         return self.multiply(x)
 
+    def __rmul__(self, x):
+        return self.multiply(x)
+
     def add(self, dist_array):
         """Distributed Addition of arrays
         """
         self._check_partition_shape(dist_array)
         SumArray = DistributedArray(global_shape=self.global_shape,
                                     base_comm=self.base_comm,
                                     dtype=self.dtype,
                                     partition=self.partition,
                                     local_shapes=self.local_shapes,
                                     axis=self.axis)
         SumArray[:] = self.local_array + dist_array.local_array
         return SumArray
 
+    def iadd(self, dist_array):
+        """Distributed In-place Addition of arrays
+        """
+        self._check_partition_shape(dist_array)
+        self[:] = self.local_array + dist_array.local_array
+        return self
+
     def multiply(self, dist_array):
         """Distributed Element-wise multiplication
         """
-        self._check_partition_shape(dist_array)
+        if isinstance(dist_array, DistributedArray):
+            self._check_partition_shape(dist_array)
+
         ProductArray = DistributedArray(global_shape=self.global_shape,
                                         base_comm=self.base_comm,
                                         dtype=self.dtype,
                                         partition=self.partition,
                                         local_shapes=self.local_shapes,
                                         axis=self.axis)
-        ProductArray[:] = self.local_array * dist_array.local_array
+        if isinstance(dist_array, DistributedArray):
+            # multiply two DistributedArray
+            ProductArray[:] = self.local_array * dist_array.local_array
+        else:
+            # multiply with scalar
+            ProductArray[:] = self.local_array * dist_array
         return ProductArray
 
     def dot(self, dist_array):
         """Distributed Dot Product
         """
         self._check_partition_shape(dist_array)
         # Convert to Partition.SCATTER if Partition.BROADCAST
@@ -553,7 +576,171 @@
         return ghosted_array
 
     def __repr__(self):
         return f"<DistributedArray with global shape={self.global_shape}, " \
                f"local shape={self.local_shape}" \
                f", dtype={self.dtype}, " \
                f"processes={[i for i in range(self.size)]})> "
+
+
+class StackedDistributedArray:
+    r"""Stacked DistributedArrays
+
+    Stack DistributedArray objects and power them with basic mathematical operations.
+    This class allows one to work with a series of distributed arrays to avoid having to create
+    a single distributed array with some special internal sorting.
+
+    Parameters
+    ----------
+    distarrays : :obj:`list`
+        List of :class:`pylops_mpi.DistributedArray` objects.
+    base_comm : :obj:`mpi4py.MPI.Comm`, optional
+        Base MPI Communicator.
+        Defaults to ``mpi4py.MPI.COMM_WORLD``.
+    """
+
+    def __init__(self, distarrays: List, base_comm: MPI.Comm = MPI.COMM_WORLD):
+        self.distarrays = distarrays
+        self.narrays = len(distarrays)
+        self.base_comm = base_comm
+        self.rank = base_comm.Get_rank()
+        self.size = base_comm.Get_size()
+
+    def __getitem__(self, index):
+        return self.distarrays[index]
+
+    def __setitem__(self, index, value):
+        self.distarrays[index][:] = value
+
+    def asarray(self):
+        """Global view of the array
+
+        Gather all the distributed arrays
+
+        Returns
+        -------
+        final_array : :obj:`numpy.ndarray`
+            Global Array gathered at all ranks
+
+        """
+        return np.hstack([distarr.asarray().ravel() for distarr in self.distarrays])
+
+    def _check_stacked_size(self, stacked_array):
+        """Check that arrays have consistent size
+
+        """
+        if self.narrays != stacked_array.narrays:
+            raise ValueError("Stacked arrays must be composed the same number of of distributed arrays")
+        for iarr in range(self.narrays):
+            if self.distarrays[iarr].global_shape != stacked_array[iarr].global_shape:
+                raise ValueError(f"Stacked arrays {iarr} have different global shape:"
+                                 f"{self.distarrays[iarr].global_shape} / "
+                                 f"{stacked_array[iarr].global_shape}")
+
+    def __neg__(self):
+        arr = self.copy()
+        for iarr in range(self.narrays):
+            arr[iarr][:] = -arr[iarr][:]
+        return arr
+
+    def __add__(self, x):
+        return self.add(x)
+
+    def __iadd__(self, x):
+        return self.iadd(x)
+
+    def __sub__(self, x):
+        return self.__add__(-x)
+
+    def __isub__(self, x):
+        return self.__iadd__(-x)
+
+    def __mul__(self, x):
+        return self.multiply(x)
+
+    def __rmul__(self, x):
+        return self.multiply(x)
+
+    def add(self, stacked_array):
+        """Stacked Distributed Addition of arrays
+
+        """
+        self._check_stacked_size(stacked_array)
+        SumArray = self.copy()
+        for iarr in range(self.narrays):
+            SumArray[iarr][:] = (self[iarr] + stacked_array[iarr])[:]
+        return SumArray
+
+    def iadd(self, stacked_array):
+        """Stacked Distributed In-Place Addition of arrays
+        """
+        self._check_stacked_size(stacked_array)
+        for iarr in range(self.narrays):
+            self[iarr][:] = (self[iarr] + stacked_array[iarr])[:]
+        return self
+
+    def multiply(self, stacked_array):
+        """Stacked Distributed Multiplication of arrays
+        """
+        if isinstance(stacked_array, StackedDistributedArray):
+            self._check_stacked_size(stacked_array)
+        ProductArray = self.copy()
+
+        if isinstance(stacked_array, StackedDistributedArray):
+            # multiply two DistributedArray
+            for iarr in range(self.narrays):
+                ProductArray[iarr][:] = (self[iarr] * stacked_array[iarr])[:]
+        else:
+            # multiply with scalar
+            for iarr in range(self.narrays):
+                ProductArray[iarr][:] = (self[iarr] * stacked_array)[:]
+        return ProductArray
+
+    def dot(self, stacked_array):
+        """Dot Product of Stacked Distributed Arrays
+        """
+        self._check_stacked_size(stacked_array)
+        dotprod = 0.
+        for iarr in range(self.narrays):
+            dotprod += self[iarr].dot(stacked_array[iarr])
+        return dotprod
+
+    def norm(self, ord: Optional[int] = None):
+        """numpy.linalg.norm method on stacked Distributed arrays
+
+        Parameters
+        ----------
+        ord : :obj:`int`, optional
+            Order of the norm.
+        """
+        norms = np.array([distarray.norm(ord) for distarray in self.distarrays])
+        ord = 2 if ord is None else ord
+        if ord in ['fro', 'nuc']:
+            raise ValueError(f"norm-{ord} not possible for vectors")
+        elif ord == 0:
+            # Count non-zero then sum reduction
+            norm = np.sum(norms)
+        elif ord == np.inf:
+            # Calculate max followed by max reduction
+            norm = np.max(norms)
+        elif ord == -np.inf:
+            # Calculate min followed by max reduction
+            norm = np.min(norms)
+        else:
+            norm = np.power(np.sum(np.power(norms, ord)), 1. / ord)
+        return norm
+
+    def conj(self):
+        """Distributed conj() method
+        """
+        ConjArray = StackedDistributedArray([distarray.conj() for distarray in self.distarrays])
+        return ConjArray
+
+    def copy(self):
+        """Creates a copy of the DistributedArray
+        """
+        arr = StackedDistributedArray([distarray.copy() for distarray in self.distarrays])
+        return arr
+
+    def __repr__(self):
+        repr_dist = "\n".join([distarray.__repr__() for distarray in self.distarrays])
+        return f"<StackedDistributedArray with {self.narrays} distributed arrays: \n" + repr_dist
```

### Comparing `pylops-mpi-0.0.1/pylops_mpi/LinearOperator.py` & `pylops-mpi-0.1.0/pylops_mpi/LinearOperator.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/pylops_mpi/__init__.py` & `pylops-mpi-0.1.0/pylops_mpi/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .DistributedArray import DistributedArray, Partition
+from .DistributedArray import DistributedArray, Partition, StackedDistributedArray
 from .LinearOperator import *
+from .StackedLinearOperator import *
 from .basicoperators import *
 from . import (
     basicoperators,
     optimization,
     plotting
 )
 from .plotting.plotting import *
```

### Comparing `pylops-mpi-0.0.1/pylops_mpi/basicoperators/BlockDiag.py` & `pylops-mpi-0.1.0/pylops_mpi/basicoperators/BlockDiag.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,97 +2,97 @@
 from scipy.sparse.linalg._interface import _get_dtype
 from mpi4py import MPI
 from typing import Optional, Sequence
 
 from pylops.utils import DTypeLike
 from pylops import LinearOperator
 
-from pylops_mpi import MPILinearOperator
-from pylops_mpi import DistributedArray
+from pylops_mpi import MPILinearOperator, MPIStackedLinearOperator
+from pylops_mpi import DistributedArray, StackedDistributedArray
 from pylops_mpi.utils.decorators import reshaped
 
 
 class MPIBlockDiag(MPILinearOperator):
     r"""MPI Block-diagonal operator.
 
-        Create a block-diagonal operator from a set of linear operators using MPI.
-        Each rank must initialize this operator by providing one or more linear operators
-        which will be computed within such rank.
-
-        Both model and data vectors must be of :class:`pylops_mpi.DistributedArray` type and partitioned between ranks
-        according to the shapes of the different linear operators.
-
-        Parameters
-        ----------
-        ops : :obj:`list`
-            One or more :class:`pylops.LinearOperator` to be stacked.
-        base_comm : :obj:`mpi4py.MPI.Comm`, optional
-            Base MPI Communicator. Defaults to ``mpi4py.MPI.COMM_WORLD``.
-        dtype : :obj:`str`, optional
-            Type of elements in input array.
-
-        Attributes
-        ----------
-        shape : :obj:`tuple`
-            Operator shape
-
-        Notes
-        -----
-        An MPI Block Diagonal operator is composed of N linear operators, represented by **L**.
-        Each rank has one or more :class:`pylops.LinearOperator`, which we represent here compactly
-        as :math:`\mathbf{L}_i` for rank :math:`i`.
-
-        Each operator performs forward mode operations using its corresponding model vector, denoted as **m**.
-        This vector is effectively a :class:`pylops_mpi.DistributedArray` partitioned at each rank in such a way that
-        its local shapes agree with those of the corresponding linear operators.
-        The forward mode of each operator is then collected from all ranks as a DistributedArray, referred to as **d**.
-
-        .. math::
-          \begin{bmatrix}
-            \mathbf{d}_1 \\
-            \mathbf{d}_2 \\
-            \vdots \\
-            \mathbf{d}_n
-          \end{bmatrix} =
-          \begin{bmatrix}
-            \mathbf{L}_1 & \mathbf{0} & \ldots & \mathbf{0} \\
-            \mathbf{0} & \mathbf{L}_2 & \ldots & \mathbf{0} \\
-            \vdots & \vdots & \ddots & \vdots \\
-            \mathbf{0} & \mathbf{0} & \ldots & \mathbf{L}_n
-          \end{bmatrix}
-          \begin{bmatrix}
-            \mathbf{m}_1 \\
-            \mathbf{m}_2 \\
-            \vdots \\
-            \mathbf{m}_n
-          \end{bmatrix}
-
-        Likewise, for the adjoint mode, each operator executes operations in the adjoint mode,
-        the adjoint mode of each operator is then collected from all ranks as a DistributedArray
-        referred as **d**.
-
-        .. math::
-          \begin{bmatrix}
-            \mathbf{d}_1 \\
-            \mathbf{d}_2 \\
-            \vdots \\
-            \mathbf{d}_n
-          \end{bmatrix} =
-          \begin{bmatrix}
-            \mathbf{L}_1^H & \mathbf{0} & \ldots & \mathbf{0} \\
-            \mathbf{0} & \mathbf{L}_2^H & \ldots & \mathbf{0} \\
-            \vdots & \vdots & \ddots & \vdots \\
-            \mathbf{0} & \mathbf{0} & \ldots & \mathbf{L}_n^H
-          \end{bmatrix}
-          \begin{bmatrix}
-            \mathbf{m}_1 \\
-            \mathbf{m}_2 \\
-            \vdots \\
-            \mathbf{m}_n
-          \end{bmatrix}
+    Create a block-diagonal operator from a set of linear operators using MPI.
+    Each rank must initialize this operator by providing one or more linear operators
+    which will be computed within such rank.
+
+    Both model and data vectors must be of :class:`pylops_mpi.DistributedArray` type and partitioned between ranks
+    according to the shapes of the different linear operators.
+
+    Parameters
+    ----------
+    ops : :obj:`list`
+        One or more :class:`pylops.LinearOperator` to be stacked.
+    base_comm : :obj:`mpi4py.MPI.Comm`, optional
+        Base MPI Communicator. Defaults to ``mpi4py.MPI.COMM_WORLD``.
+    dtype : :obj:`str`, optional
+        Type of elements in input array.
+
+    Attributes
+    ----------
+    shape : :obj:`tuple`
+        Operator shape
+
+    Notes
+    -----
+    An MPI Block Diagonal operator is composed of N linear operators, represented by **L**.
+    Each rank has one or more :class:`pylops.LinearOperator`, which we represent here compactly
+    as :math:`\mathbf{L}_i` for rank :math:`i`.
+
+    Each operator performs forward mode operations using its corresponding model vector, denoted as **m**.
+    This vector is effectively a :class:`pylops_mpi.DistributedArray` partitioned at each rank in such a way that
+    its local shapes agree with those of the corresponding linear operators.
+    The forward mode of each operator is then collected from all ranks as a DistributedArray, referred to as **d**.
+
+    .. math::
+        \begin{bmatrix}
+        \mathbf{d}_1 \\
+        \mathbf{d}_2 \\
+        \vdots \\
+        \mathbf{d}_n
+        \end{bmatrix} =
+        \begin{bmatrix}
+        \mathbf{L}_1 & \mathbf{0} & \ldots & \mathbf{0} \\
+        \mathbf{0} & \mathbf{L}_2 & \ldots & \mathbf{0} \\
+        \vdots & \vdots & \ddots & \vdots \\
+        \mathbf{0} & \mathbf{0} & \ldots & \mathbf{L}_n
+        \end{bmatrix}
+        \begin{bmatrix}
+        \mathbf{m}_1 \\
+        \mathbf{m}_2 \\
+        \vdots \\
+        \mathbf{m}_n
+        \end{bmatrix}
+
+    Likewise, for the adjoint mode, each operator executes operations in the adjoint mode,
+    the adjoint mode of each operator is then collected from all ranks as a DistributedArray
+    referred as **d**.
+
+    .. math::
+        \begin{bmatrix}
+        \mathbf{d}_1 \\
+        \mathbf{d}_2 \\
+        \vdots \\
+        \mathbf{d}_n
+        \end{bmatrix} =
+        \begin{bmatrix}
+        \mathbf{L}_1^H & \mathbf{0} & \ldots & \mathbf{0} \\
+        \mathbf{0} & \mathbf{L}_2^H & \ldots & \mathbf{0} \\
+        \vdots & \vdots & \ddots & \vdots \\
+        \mathbf{0} & \mathbf{0} & \ldots & \mathbf{L}_n^H
+        \end{bmatrix}
+        \begin{bmatrix}
+        \mathbf{m}_1 \\
+        \mathbf{m}_2 \\
+        \vdots \\
+        \mathbf{m}_n
+        \end{bmatrix}
 
     """
 
     def __init__(self, ops: Sequence[LinearOperator],
                  base_comm: MPI.Comm = MPI.COMM_WORLD,
                  dtype: Optional[DTypeLike] = None):
         self.ops = ops
@@ -126,7 +126,51 @@
         y = DistributedArray(global_shape=self.shape[1], local_shapes=self.local_shapes_m, dtype=self.dtype)
         y1 = []
         for iop, oper in enumerate(self.ops):
             y1.append(oper.rmatvec(x.local_array[self.nnops[iop]:
                                                  self.nnops[iop + 1]]))
         y[:] = np.concatenate(y1)
         return y
+
+
+class MPIStackedBlockDiag(MPIStackedLinearOperator):
+    r"""MPI Stacked BlockDiag Operator
+
+    Create a diagonal stack of :class:`pylops_mpi.MPILinearOperator` operators.
+
+    Parameters
+    ----------
+    ops : :obj:`list`
+        One or more :class:`pylops_mpi.MPILinearOperator` to be stacked.
+
+    Attributes
+    ----------
+    shape : :obj:`tuple`
+        Operator shape
+
+    Notes
+    -----
+    A MPIStackedBlockDiag is composed of N :class:pylops_mpi.MPILinearOperator instances stacked along the diagonal.
+    These MPI operators will be applied sequentially, with distributed computations
+    performed within each operator.
+
+    """
+
+    def __init__(self, ops: Sequence[MPILinearOperator], base_comm: MPI.Comm = MPI.COMM_WORLD,
+                 dtype: Optional[DTypeLike] = None):
+        self.ops = ops
+        dtype = _get_dtype(self.ops) if dtype is None else np.dtype(dtype)
+        shape = (int(np.sum(op.shape[0] for op in ops)),
+                 int(np.sum(op.shape[1] for op in ops)))
+        super().__init__(shape=shape, dtype=dtype, base_comm=base_comm)
+
+    def _matvec(self, x: StackedDistributedArray) -> StackedDistributedArray:
+        y1 = []
+        for xx, oper in zip(x, self.ops):
+            y1.append(oper.matvec(xx))
+        return StackedDistributedArray(y1)
+
+    def _rmatvec(self, x: StackedDistributedArray) -> StackedDistributedArray:
+        y1 = []
+        for xx, oper in zip(x, self.ops):
+            y1.append(oper.rmatvec(xx))
+        return StackedDistributedArray(y1)
```

### Comparing `pylops-mpi-0.0.1/pylops_mpi/basicoperators/FirstDerivative.py` & `pylops-mpi-0.1.0/pylops_mpi/basicoperators/FirstDerivative.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/pylops_mpi/basicoperators/HStack.py` & `pylops-mpi-0.1.0/pylops_mpi/basicoperators/HStack.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/pylops_mpi/basicoperators/Laplacian.py` & `pylops-mpi-0.1.0/pylops_mpi/basicoperators/Laplacian.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/pylops_mpi/basicoperators/SecondDerivative.py` & `pylops-mpi-0.1.0/pylops_mpi/basicoperators/SecondDerivative.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/pylops_mpi/basicoperators/VStack.py` & `pylops-mpi-0.1.0/pylops_mpi/basicoperators/VStack.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 from scipy.sparse.linalg._interface import _get_dtype
 from mpi4py import MPI
 from typing import Sequence, Optional
 
 from pylops import LinearOperator
 from pylops.utils import DTypeLike
 
-from pylops_mpi import MPILinearOperator, DistributedArray, Partition
+from pylops_mpi import (
+    MPILinearOperator,
+    MPIStackedLinearOperator,
+    DistributedArray,
+    Partition,
+    StackedDistributedArray
+)
 from pylops_mpi.utils.decorators import reshaped
 
 
 class MPIVStack(MPILinearOperator):
     r"""MPI VStack Operator
 
     Create a vertical stack of a set of linear operators using MPI. Each rank must
@@ -124,7 +130,59 @@
         y = DistributedArray(global_shape=self.shape[1], partition=Partition.BROADCAST, dtype=self.dtype)
         y1 = []
         for iop, oper in enumerate(self.ops):
             y1.append(oper.rmatvec(x.local_array[self.nnops[iop]: self.nnops[iop + 1]]))
         y1 = np.sum(y1, axis=0)
         y[:] = self.base_comm.allreduce(y1, op=MPI.SUM)
         return y
+
+
+class MPIStackedVStack(MPIStackedLinearOperator):
+    r"""MPI Stacked VStack Operator
+
+    Create a vertical stack of :class:`pylops_mpi.MPILinearOperator` operators.
+
+    Parameters
+    ----------
+    ops : :obj:`list`
+        One or more :class:`pylops_mpi.MPILinearOperator` to be vertically stacked.
+
+    Attributes
+    ----------
+    shape : :obj:`tuple`
+        Operator shape
+
+    Raises
+    ------
+    ValueError
+        If ``ops`` have different number of columns
+
+    Notes
+    -----
+    An MPIStackedVStack is composed of N  :class:`pylops_mpi.MPILinearOperator` stacked
+    vertically. These MPI operators will be applied sequentially, however distributed
+    computations will be performed within each operator.
+
+    """
+
+    def __init__(self, ops: Sequence[MPILinearOperator],
+                 base_comm: MPI.Comm = MPI.COMM_WORLD,
+                 dtype: Optional[DTypeLike] = None):
+        self.ops = ops
+        if len(set(op.shape[1] for op in ops)) > 1:
+            raise ValueError("Operators have different number of columns")
+        shape = (int(np.sum(op.shape[0] for op in ops)), ops[0].shape[1])
+        dtype = _get_dtype(self.ops) if dtype is None else np.dtype(dtype)
+        super().__init__(shape=shape, dtype=dtype, base_comm=base_comm)
+
+    def _matvec(self, x: DistributedArray) -> StackedDistributedArray:
+        y1 = []
+        for oper in self.ops:
+            y1.append(oper.matvec(x))
+        y = StackedDistributedArray(y1)
+        return y
+
+    def _rmatvec(self, x: StackedDistributedArray) -> DistributedArray:
+        y = self.ops[0].rmatvec(x[0])
+        for xx, oper in zip(x[1:], self.ops[1:]):
+            y = y + oper.rmatvec(xx)
+        return y
```

### Comparing `pylops-mpi-0.0.1/pylops_mpi/optimization/basic.py` & `pylops-mpi-0.1.0/pylops_mpi/optimization/basic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,41 @@
-from typing import Optional, Tuple, Callable
+from typing import Callable, Optional, Tuple, Union
 
 from pylops.utils import NDArray
-from pylops_mpi import MPILinearOperator, DistributedArray
+from pylops_mpi import (
+    MPILinearOperator,
+    DistributedArray,
+    StackedDistributedArray,
+    MPIStackedLinearOperator
+)
 from pylops_mpi.optimization.cls_basic import CG, CGLS
 
 
 def cg(
-        Op: MPILinearOperator,
-        y: DistributedArray,
-        x0: Optional[DistributedArray] = None,
+        Op: Union[MPILinearOperator, MPIStackedLinearOperator],
+        y: Union[DistributedArray, StackedDistributedArray],
+        x0: Union[DistributedArray, StackedDistributedArray],
         niter: int = 10,
         tol: float = 1e-4,
         show: bool = False,
         itershow: Tuple[int, int, int] = (10, 10, 10),
         callback: Optional[Callable] = None,
-) -> Tuple[DistributedArray, int, NDArray]:
+) -> Tuple[Union[DistributedArray, StackedDistributedArray], int, NDArray]:
     r"""Conjugate gradient
 
-    Solve a square system of equations given an MPILinearOperator ``Op`` and
+    Solve a square system of equations given either an MPILinearOperator or an MPIStackedLinearOperator ``Op`` and
     distributed data ``y`` using conjugate gradient iterations.
 
     Parameters
     ----------
-    Op : :obj:`pylops_mpi.MPILinearOperator`
+    Op : :obj:`pylops_mpi.MPILinearOperator` or :obj:`pylops_mpi.MPIStackedLinearOperator`
         Operator to invert of size :math:`[N \times N]`
-    y : :obj:`pylops_mpi.DistributedArray`
+    y : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
         DistributedArray of size (N,)
-    x0 : :obj:`pylops_mpi.DistributedArray`, optional
+    x0 : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
         Initial guess
     niter : :obj:`int`, optional
         Number of iterations
     tol : :obj:`float`, optional
         Tolerance on residual norm
     show : :obj:`bool`, optional
         Display iterations log
@@ -40,15 +45,15 @@
             three element of the list.
     callback : :obj:`callable`, optional
         Function with signature (``callback(x)``) to call after each iteration
         where ``x`` is the current model vector
 
     Returns
     -------
-    x : :obj:`pylops_mpi.DistributedArray`
+    x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
         Estimated model of size (N,)
     iit : :obj:`int`
         Number of executed iterations
     cost : :obj:`numpy.ndarray`, optional
         History of the L2 norm of the residual
 
     Notes
@@ -62,36 +67,36 @@
     x, iiter, cost = cgsolve.solve(
         y=y, x0=x0, tol=tol, niter=niter, show=show, itershow=itershow
     )
     return x, iiter, cost
 
 
 def cgls(
-        Op: MPILinearOperator,
-        y: DistributedArray,
-        x0: Optional[DistributedArray] = None,
+        Op: Union[MPILinearOperator, MPIStackedLinearOperator],
+        y: Union[DistributedArray, StackedDistributedArray],
+        x0: Union[DistributedArray, StackedDistributedArray],
         niter: int = 10,
         damp: float = 0.0,
         tol: float = 1e-4,
         show: bool = False,
         itershow: Tuple[int, int, int] = (10, 10, 10),
         callback: Optional[Callable] = None,
 ) -> Tuple[DistributedArray, int, int, float, float, NDArray]:
     r"""Conjugate gradient least squares
 
-    Solve an overdetermined system of equations given a MPILinearOperator ``Op`` and
+    Solve an overdetermined system of equations given either an MPILinearOperator or an MPIStackedLinearOperator``Op`` and
     distributed data ``y`` using conjugate gradient iterations.
 
     Parameters
     ----------
-    Op : :obj:`pylops_mpi.MPILinearOperator`
+    Op : :obj:`pylops_mpi.MPILinearOperator` or :obj:`pylops_mpi.MPIStackedLinearOperator`
         MPI Linear Operator to invert of size :math:`[N \times M]`
-    y : :obj:`pylops_mpi.DistributedArray`
+    y : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
         DistributedArray of size (N,)
-    x0 : :obj:`pylops_mpi.DistributedArray`, optional
+    x0 : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
         Initial guess
     niter : :obj:`int`, optional
         Number of iterations
     damp : :obj:`float`, optional
         Damping coefficient
     tol : :obj:`float`, optional
         Tolerance on residual norm
@@ -103,15 +108,15 @@
         three element of the list.
     callback : :obj:`callable`, optional
         Function with signature (``callback(x)``) to call after each iteration
         where ``x`` is the DistributedArray.
 
     Returns
     -------
-    x : :obj:`pylops_mpi.DistributedArray`
+    x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
         Estimated model of size (M, )
     istop : :obj:`int`
         Gives the reason for termination
 
         ``1`` means :math:`\mathbf{x}` is an approximate solution to
         :math:`\mathbf{y} = \mathbf{Op}\,\mathbf{x}`
```

### Comparing `pylops-mpi-0.0.1/pylops_mpi/optimization/cls_basic.py` & `pylops-mpi-0.1.0/pylops_mpi/optimization/cls_basic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Union
 import numpy as np
 import time
 
 from pylops.optimization.basesolver import Solver
 from pylops.utils import NDArray
 
-from pylops_mpi import DistributedArray
+from pylops_mpi import DistributedArray, StackedDistributedArray
 
 
 class CG(Solver):
     r"""Conjugate gradient
 
-    Solve a square system of equations given an MPILinearOperator ``Op`` and
+    Solve a square system of equations given either an MPILinearOperator or an MPIStackedLinearOperator ``Op`` and
     distributed data ``y`` using conjugate gradient iterations.
 
     Parameters
     ----------
-    Op : :obj:`pylops_mpi.MPILinearOperator`
+    Op : :obj:`pylops_mpi.MPILinearOperator` or :obj:`pylops_mpi.MPIStackedLinearOperator`
         Operator to invert of size :math:`[N \times N]`
 
     Notes
     -----
     Solve the :math:`\mathbf{y} = \mathbf{Op}\,\mathbf{x}` problem using conjugate gradient
     iterations.
 
@@ -37,135 +37,132 @@
         print("-" * 55 + "\n")
         if not xcomplex:
             head1 = "    Itn           x[0]              r2norm"
         else:
             head1 = "    Itn              x[0]                  r2norm"
         print(head1)
 
-    def _print_step(self, x: DistributedArray) -> None:
+    def _print_step(self, x: Union[DistributedArray, StackedDistributedArray]) -> None:
+        if isinstance(x, StackedDistributedArray):
+            x = x.distarrays[0]
         strx = f"{x[0]:1.2e}        " if np.iscomplexobj(x.local_array) else f"{x[0]:11.4e}        "
         msg = f"{self.iiter:6g}        " + strx + f"{self.cost[self.iiter]:11.4e}"
         print(msg)
 
     def setup(
             self,
-            y: DistributedArray,
-            x0: Optional[DistributedArray] = None,
+            y: Union[DistributedArray, StackedDistributedArray],
+            x0: Union[DistributedArray, StackedDistributedArray],
             niter: Optional[int] = None,
             tol: float = 1e-4,
             show: bool = False,
-    ) -> DistributedArray:
+    ) -> Union[DistributedArray, StackedDistributedArray]:
         r"""Setup solver
 
         Parameters
         ----------
-        y : :obj:`pylops_mpi.DistributedArray`
+        y : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Data of size (N,)
-        x0 : :obj:`pylops_mpi.DistributedArray`, optional
-            Initial guess of size (N,). If ``None``, initialize
-            internally as zero vector
+        x0 : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
+            Initial guess of size (N,).
         niter : :obj:`int`, optional
-            Number of iterations (default to ``None`` in case a user wants to
-            manually step over the solver)
+            Number of iterations (default to ``None`` in case a user wants to manually step over the solver)
         tol : :obj:`float`, optional
             Tolerance on residual norm
         show : :obj:`bool`, optional
             Display setup log
 
         Returns
         -------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Initial guess of size (N,).
 
         """
 
         self.y = y
         self.niter = niter
         self.tol = tol
 
-        if x0 is None:
-            self.r = self.y.copy()
-            x = DistributedArray(global_shape=self.Op.shape[1],
-                                 partition=self.r.partition,
-                                 local_shapes=self.r.local_shapes,
-                                 dtype=y.dtype)
-            x[:] = 0
-        else:
-            x = x0.copy()
-            self.r = self.y - self.Op.matvec(x)
+        x = x0.copy()
+        self.r = self.y - self.Op.matvec(x)
         self.rank = x.rank
         self.c = self.r.copy()
         self.kold = np.abs(self.r.dot(self.r.conj()))
 
         # create variables to track the residual norm and iterations
         self.cost: List = []
         self.cost.append(float(np.sqrt(self.kold)))
         self.iiter = 0
 
         if show and self.rank == 0:
-            self._print_setup(np.iscomplexobj(x.local_array))
+            if isinstance(x, StackedDistributedArray):
+                self._print_setup(np.iscomplexobj([x1.local_array for x1 in x.distarrays]))
+            else:
+                self._print_setup(np.iscomplexobj(x.local_array))
         return x
 
-    def step(self, x: DistributedArray, show: bool = False) -> DistributedArray:
+    def step(self, x: Union[DistributedArray, StackedDistributedArray],
+             show: bool = False
+             ) -> Union[DistributedArray, StackedDistributedArray]:
         r"""Run one step of solver
 
         Parameters
         ----------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Current model vector to be updated by a step of CG
         show : :obj:`bool`, optional
             Display iteration log
 
         Returns
         -------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Updated model vector
 
         """
         Opc = self.Op.matvec(self.c)
         cOpc = np.abs(self.c.dot(Opc.conj()))
         a = self.kold / cOpc
-        x[:] += a * self.c.local_array
-        self.r[:] -= a * Opc.local_array
+        x += a * self.c
+        self.r -= a * Opc
         k = np.abs(self.r.dot(self.r.conj()))
         b = k / self.kold
-        self.c[:] = self.r.local_array + b * self.c.local_array
+        self.c = self.r + b * self.c
         self.kold = k
         self.iiter += 1
         self.cost.append(float(np.sqrt(self.kold)))
         if show and self.rank == 0:
             self._print_step(x)
         return x
 
     def run(
             self,
-            x: DistributedArray,
+            x: Union[DistributedArray, StackedDistributedArray],
             niter: Optional[int] = None,
             show: bool = False,
             itershow: Tuple[int, int, int] = (10, 10, 10),
-    ) -> DistributedArray:
+    ) -> Union[DistributedArray, StackedDistributedArray]:
         r"""Run solver
 
         Parameters
         ----------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Current model vector to be updated by multiple steps of CG
         niter : :obj:`int`, optional
             Number of iterations. Can be set to ``None`` if already
             provided in the setup call
         show : :obj:`bool`, optional
             Display logs
         itershow : :obj:`tuple`, optional
             Display set log for the first N1 steps, last N2 steps,
             and every N3 steps in between where N1, N2, N3 are the
             three element of the list.
 
         Returns
         -------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Estimated model of size (M,)
 
         """
 
         niter = self.niter if niter is None else niter
         if niter is None:
             raise ValueError("niter must not be None")
@@ -198,44 +195,43 @@
         self.telapsed = self.tend - self.tstart
         self.cost = np.array(self.cost)
         if show and self.rank == 0:
             self._print_finalize(nbar=55)
 
     def solve(
             self,
-            y: DistributedArray,
-            x0: Optional[DistributedArray] = None,
+            y: Union[DistributedArray, StackedDistributedArray],
+            x0: Union[DistributedArray, StackedDistributedArray],
             niter: int = 10,
             tol: float = 1e-4,
             show: bool = False,
             itershow: Tuple[int, int, int] = (10, 10, 10),
-    ) -> Tuple[DistributedArray, int, NDArray]:
+    ) -> Tuple[Union[DistributedArray, StackedDistributedArray], int, NDArray]:
         r"""Run entire solver
 
         Parameters
         ----------
-        y : :obj:`pylops_mpi.DistributedArray`
+        y : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Data of size (N,)
-        x0 : :obj:`pylops_mpi.DistributedArray`, optional
-            Initial guess of size (N,). If ``None``, initialize
-            internally as zero vector
+        x0 : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
+            Initial guess of size (N,).
         niter : :obj:`int`, optional
             Number of iterations
         tol : :obj:`float`, optional
             Tolerance on residual norm
         show : :obj:`bool`, optional
             Display logs
         itershow : :obj:`tuple`, optional
             Display set log for the first N1 steps, last N2 steps,
             and every N3 steps in between where N1, N2, N3 are the
             three element of the list.
 
         Returns
         -------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Estimated model of size (N,)
         iit : :obj:`int`
             Number of executed iterations
         cost : :obj:`numpy.ndarray`
             History of the L2 norm of the residual
 
         """
@@ -245,20 +241,20 @@
         self.finalize(show)
         return x, self.iiter, self.cost
 
 
 class CGLS(Solver):
     r"""Conjugate gradient least squares
 
-    Solve an overdetermined system of equations given a MPILinearOperator ``Op``
+    Solve an overdetermined system of equations given either an MPILinearOperator or an MPIStackedLinearOperator ``Op``
     and distributed data ``y`` using conjugate gradient iterations.
 
     Parameters
     ----------
-    Op : :obj:`pylops_mpi.MPILinearOperator`
+    Op : :obj:`pylops_mpi.MPILinearOperator` or :obj:`pylops_mpi.MPIStackedLinearOperator`
         Operator to invert of size :math:`[N \times M]`
 
     Notes
     -----
     Minimize the following functional using conjugate gradient iterations:
 
     .. math::
@@ -282,155 +278,146 @@
         print("-" * 65 + "\n")
         if not xcomplex:
             head1 = "    Itn          x[0]              r1norm         r2norm"
         else:
             head1 = "    Itn             x[0]             r1norm         r2norm"
         print(head1)
 
-    def _print_step(self, x: DistributedArray) -> None:
+    def _print_step(self, x: Union[DistributedArray, StackedDistributedArray]) -> None:
+        if isinstance(x, StackedDistributedArray):
+            x = x.distarrays[0]
         strx = f"{x[0]:1.2e}   " if np.iscomplexobj(x.local_array) else f"{x[0]:11.4e}        "
         msg = (
             f"{self.iiter:6g}       "
             + strx
             + f"{self.cost[self.iiter]:11.4e}    {self.cost1[self.iiter]:11.4e}"
         )
         print(msg)
 
     def setup(self,
-              y: DistributedArray,
-              x0: Optional[DistributedArray] = None,
+              y: Union[DistributedArray, StackedDistributedArray],
+              x0: Union[DistributedArray, StackedDistributedArray],
               niter: Optional[int] = None,
               damp: float = 0.0,
               tol: float = 1e-4,
               show: bool = False,
-              ) -> DistributedArray:
+              ) -> Union[DistributedArray, StackedDistributedArray]:
         r"""Setup solver
 
         Parameters
         ----------
-        y : :obj:`pylops_mpi.DistributedArray`
+        y : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Data of size :math:`[N \times 1]`
-        x0 : :obj:`pylops_mpi.DistributedArray`, optional
-            Initial guess  of size (M,). If ``None``, Defaults to a
-            zero vector
+        x0 : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
+            Initial guess  of size (M,).
         niter : :obj:`int`, optional
             Number of iterations (default to ``None`` in case a user wants to
             manually step over the solver)
         damp : :obj:`float`, optional
             Damping coefficient
         tol : :obj:`float`, optional
             Tolerance on residual norm
         show : :obj:`bool`, optional
             Display setup log
 
         Returns
         -------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Initial guess of size (N,).
 
         """
         self.y = y
         self.damp = damp ** 2
         self.tol = tol
         self.niter = niter
 
-        # initialize solver
-        if x0 is None:
-            self.s = y.copy()
-            r = self.Op.rmatvec(self.s)
-            x = DistributedArray(global_shape=self.Op.shape[1], dtype=y.dtype,
-                                 local_shapes=r.local_shapes,
-                                 partition=r.partition)
-            x[:] = 0
-        else:
-            x = x0.copy()
-            self.s = self.y - self.Op.matvec(x)
-            damped_x = DistributedArray(global_shape=x.global_shape, dtype=x.dtype,
-                                        local_shapes=x.local_shapes,
-                                        partition=x.partition)
-            damped_x[:] = damp * x.local_array
-            r = self.Op.rmatvec(self.s) - damped_x
+        x = x0.copy()
+        self.s = self.y - self.Op.matvec(x)
+        damped_x = x * damp
+        r = self.Op.rmatvec(self.s) - damped_x
         self.rank = x.rank
         self.c = r.copy()
         self.q = self.Op.matvec(self.c)
         self.kold = np.abs(r.dot(r.conj()))
 
         # create variables to track the residual norm and iterations
         self.cost = []
         self.cost1 = []
         self.cost.append(float(self.s.norm()))
         self.cost1.append(np.sqrt(float(self.cost[0] ** 2 + damp * np.abs(x.dot(x.conj())))))
         self.iiter = 0
 
         # print setup
         if show and self.rank == 0:
-            self._print_setup(np.iscomplexobj(x.local_array))
+            if isinstance(x, StackedDistributedArray):
+                self._print_setup(np.iscomplexobj([x1.local_array for x1 in x.distarrays]))
+            else:
+                self._print_setup(np.iscomplexobj(x.local_array))
         return x
 
-    def step(self, x: DistributedArray, show: bool = False) -> DistributedArray:
+    def step(self, x: Union[DistributedArray, StackedDistributedArray],
+             show: bool = False
+             ) -> Union[DistributedArray, StackedDistributedArray]:
         r"""Run one step of solver
 
         Parameters
         ----------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Current model vector to be updated by a step of CG
         show : :obj:`bool`, optional
             Display iteration log
 
         Returns
         -------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Updated model vector
 
         """
 
         a = self.kold / (self.q.dot(self.q.conj()) + self.damp * self.c.dot(self.c.conj()))
-        x[:] = x.local_array + a * self.c.local_array
-        self.s[:] = self.s.local_array - a * self.q.local_array
-        damped_x = DistributedArray(global_shape=x.global_shape, dtype=x.dtype,
-                                    local_shapes=x.local_shapes,
-                                    partition=x.partition)
-        damped_x[:] = self.damp * x.local_array
+        x += a * self.c
+        self.s -= a * self.q
+        damped_x = self.damp * x
         r = self.Op.rmatvec(self.s) - damped_x
         k = np.abs(r.dot(r.conj()))
         b = k / self.kold
-        self.c[:] = r.local_array + b * self.c.local_array
+        self.c = r + b * self.c
         self.q = self.Op.matvec(self.c)
         self.kold = k
         self.iiter += 1
         self.cost.append(float(self.s.norm()))
         self.cost1.append(np.sqrt(float(self.cost[self.iiter] ** 2 + self.damp * np.abs(x.dot(x.conj())))))
         if show and self.rank == 0:
             self._print_step(x)
         return x
 
     def run(self,
-            x: DistributedArray,
+            x: Union[DistributedArray, StackedDistributedArray],
             niter: Optional[int] = None,
             show: bool = False,
-            itershow: Tuple[int, int, int] = (10, 10, 10), ) -> DistributedArray:
+            itershow: Tuple[int, int, int] = (10, 10, 10), ) -> Union[DistributedArray, StackedDistributedArray]:
         r"""Run solver
 
         Parameters
         ----------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Current model vector to be updated by multiple steps of CGLS
         niter : :obj:`int`, optional
             Number of iterations. Can be set to ``None`` if already
             provided in the setup call
         show : :obj:`bool`, optional
             Display iterations log
         itershow : :obj:`tuple`, optional
             Display set log for the first N1 steps, last N2 steps,
             and every N3 steps in between where N1, N2, N3 are the
             three element of the list.
 
         Returns
         -------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray
             Estimated model of size (M, ).
 
         """
         niter = self.niter if niter is None else niter
         if niter is None:
             raise ValueError("niter must not be None")
         while self.iiter < niter and self.kold > self.tol:
@@ -465,31 +452,30 @@
         self.r1norm = self.kold
         self.r2norm = self.cost1[self.iiter]
         if show and self.rank == 0:
             self._print_finalize(nbar=65)
         self.cost = np.array(self.cost)
 
     def solve(self,
-              y: DistributedArray,
-              x0: Optional[DistributedArray] = None,
+              y: Union[DistributedArray, StackedDistributedArray],
+              x0: Union[DistributedArray, StackedDistributedArray],
               niter: int = 10,
               damp: float = 0.0,
               tol: float = 1e-4,
               show: bool = False,
               itershow: Tuple[int, int, int] = (10, 10, 10),
               ) -> Tuple[DistributedArray, int, int, float, float, NDArray]:
         r"""Run entire solver
 
         Parameters
         ----------
-        y : :obj:`pylops_mpi.DistributedArray`
+        y : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Data of size (N, )
-        x0 : :obj:`pylops_mpi.DistributedArray`
-            Initial guess  of size (M, ). If ``None``, initialize
-            internally as zero vector
+        x0 : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
+            Initial guess  of size (M, ).
         niter : :obj:`int`, optional
             Number of iterations (default to ``None`` in case a user wants to
             manually step over the solver)
         damp : :obj:`float`, optional
             Damping coefficient
         tol : :obj:`float`, optional
             Tolerance on residual norm
@@ -498,15 +484,15 @@
         itershow : :obj:`tuple`, optional
             Display set log for the first N1 steps, last N2 steps,
             and every N3 steps in between where N1, N2, N3 are the
             three element of the list.
 
         Returns
         -------
-        x : :obj:`pylops_mpi.DistributedArray`
+        x : :obj:`pylops_mpi.DistributedArray` or :obj:`pylops_mpi.StackedDistributedArray`
             Estimated model of size (M, ).
         istop : :obj:`int`
             Gives the reason for termination
 
             ``1`` means :math:`\mathbf{x}` is an approximate solution to
             :math:`\mathbf{y} = \mathbf{Op}\,\mathbf{x}`
```

### Comparing `pylops-mpi-0.0.1/pylops_mpi/plotting/plotting.py` & `pylops-mpi-0.1.0/pylops_mpi/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/pylops_mpi/utils/decorators.py` & `pylops-mpi-0.1.0/pylops_mpi/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/pylops_mpi.egg-info/SOURCES.txt` & `pylops-mpi-0.1.0/pylops_mpi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 CHANGELOG.md
 LICENSE
 Makefile
 README.md
 environment-dev.yml
 environment.yml
 mpi_examples.sh
+pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.cfg
-setup.py
 .github/workflows/build.yml
 .github/workflows/deploy-docs.yml
 .github/workflows/deploy.yml
 .github/workflows/flake.yml
 docs/Makefile
 docs/modules.rst
 docs/pylops_mpi.rst
@@ -37,27 +37,29 @@
 docs/source/_templates/autosummary/module.rst
 docs/source/api/index.rst
 examples/README.rst
 examples/plot_cgls.py
 examples/plot_derivative.py
 examples/plot_distributed_array.py
 examples/plot_mpilinop.py
+examples/plot_stacked_array.py
 examples/plot_stacking.py
 pylops_mpi/DistributedArray.py
 pylops_mpi/LinearOperator.py
+pylops_mpi/StackedLinearOperator.py
 pylops_mpi/__init__.py
 pylops_mpi/version.py
 pylops_mpi.egg-info/PKG-INFO
 pylops_mpi.egg-info/SOURCES.txt
 pylops_mpi.egg-info/dependency_links.txt
 pylops_mpi.egg-info/requires.txt
 pylops_mpi.egg-info/top_level.txt
-pylops_mpi.egg-info/zip-safe
 pylops_mpi/basicoperators/BlockDiag.py
 pylops_mpi/basicoperators/FirstDerivative.py
+pylops_mpi/basicoperators/Gradient.py
 pylops_mpi/basicoperators/HStack.py
 pylops_mpi/basicoperators/Laplacian.py
 pylops_mpi/basicoperators/SecondDerivative.py
 pylops_mpi/basicoperators/VStack.py
 pylops_mpi/basicoperators/__init__.py
 pylops_mpi/optimization/__init__.py
 pylops_mpi/optimization/basic.py
@@ -69,10 +71,12 @@
 testdata/avo/poststack_model.npz
 tests/test_blockdiag.py
 tests/test_derivative.py
 tests/test_distributedarray.py
 tests/test_linearop.py
 tests/test_solver.py
 tests/test_stack.py
+tests/test_stackedarray.py
+tests/test_stackedlinearop.py
 tutorials/README.rst
-tutorials/plot_lsm.py
-tutorials/plot_post_stack_inversion.py
+tutorials/lsm.py
+tutorials/poststack.py
```

### Comparing `pylops-mpi-0.0.1/testdata/avo/poststack_model.npz` & `pylops-mpi-0.1.0/testdata/avo/poststack_model.npz`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/tests/test_derivative.py` & `pylops-mpi-0.1.0/tests/test_derivative.py`

 * *Files 7% similar despite different names*

```diff
@@ -392,7 +392,50 @@
                                    kind=kind, edge=par['edge'],
                                    dtype=par['dtype'])
             assert Lop_MPI.shape == Lop.shape
             y_np = Lop @ x_global
             y_adj_np = Lop.H @ x_global
             assert_allclose(y, y_np, rtol=1e-14)
             assert_allclose(y_adj, y_adj_np, rtol=1e-14)
+
+
+@pytest.mark.mpi(min_size=2)
+@pytest.mark.parametrize("par", [(par5), (par5e), (par6), (par6e)])
+def test_gradient(par):
+    """MPIGradient Operator"""
+    for kind in ["forward", "backward", "centered"]:
+        Gop_MPI = pylops_mpi.basicoperators.MPIGradient(dims=par['n'], sampling=par['sampling'],
+                                                        kind=kind, edge=par['edge'],
+                                                        dtype=par['dtype'])
+        x_fwd = pylops_mpi.DistributedArray(global_shape=np.prod(par['n']), dtype=par['dtype'])
+        x_fwd[:] = np.random.normal(rank, 10, x_fwd.local_shape)
+        x_global = x_fwd.asarray()
+        # Forward
+        y_dist = Gop_MPI @ x_fwd
+        assert isinstance(y_dist, pylops_mpi.StackedDistributedArray)
+        y = y_dist.asarray()
+
+        # Adjoint
+        x_adj_dist1 = pylops_mpi.DistributedArray(global_shape=int(np.prod(par['n'])), dtype=par['dtype'])
+        x_adj_dist1[:] = np.random.normal(rank, 10, x_adj_dist1.local_shape)
+        x_adj_dist2 = pylops_mpi.DistributedArray(global_shape=int(np.prod(par['n'])), dtype=par['dtype'])
+        x_adj_dist2[:] = np.random.normal(rank, 20, x_adj_dist2.local_shape)
+        x_adj_dist3 = pylops_mpi.DistributedArray(global_shape=int(np.prod(par['n'])), dtype=par['dtype'])
+        x_adj_dist3[:] = np.random.normal(rank, 30, x_adj_dist3.local_shape)
+
+        x_adj = pylops_mpi.StackedDistributedArray(distarrays=[x_adj_dist1, x_adj_dist2, x_adj_dist3])
+
+        x_adj_global = x_adj.asarray()
+        y_adj_dist = Gop_MPI.H @ x_adj
+        assert isinstance(y_adj_dist, pylops_mpi.DistributedArray)
+
+        y_adj = y_adj_dist.asarray()
+
+        if rank == 0:
+            Gop = pylops.Gradient(dims=par['n'], sampling=par['sampling'],
+                                  kind=kind, edge=par['edge'],
+                                  dtype=par['dtype'])
+            assert Gop_MPI.shape == Gop.shape
+            y_np = Gop @ x_global
+            y_adj_np = Gop.H @ x_adj_global
+            assert_allclose(y, y_np, rtol=1e-14)
+            assert_allclose(y_adj, y_adj_np, rtol=1e-14)
```

### Comparing `pylops-mpi-0.0.1/tests/test_distributedarray.py` & `pylops-mpi-0.1.0/tests/test_distributedarray.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/tests/test_linearop.py` & `pylops-mpi-0.1.0/tests/test_linearop.py`

 * *Files identical despite different names*

### Comparing `pylops-mpi-0.0.1/tests/test_solver.py` & `pylops-mpi-0.1.0/tests/test_solver.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 
 from pylops_mpi import (
     cg,
     cgls,
     DistributedArray,
     MPIBlockDiag,
     MPIHStack,
+    MPIStackedBlockDiag,
     MPIVStack,
-    Partition
+    Partition,
+    StackedDistributedArray
 )
 
 np.random.seed(42)
 size = MPI.COMM_WORLD.Get_size()
 rank = MPI.COMM_WORLD.Get_rank()
 
 par1 = {
@@ -100,25 +102,28 @@
     if par["x0"]:
         x0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
         x0[:] = np.random.normal(0, 10, par["nx"]) + par["imag"] * np.random.normal(
             10, 10, par["nx"]
         )
         x0_global = x0.asarray()
     else:
-        x0 = None
+        # Set TO 0s if x0 = False
+        x0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        x0[:] = 0
+        x0_global = x0.asarray()
     y = BDiag_MPI * x
     xinv = cg(BDiag_MPI, y, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
     assert isinstance(xinv, DistributedArray)
     xinv_array = xinv.asarray()
     if rank == 0:
         mats = [np.ones(shape=(par["ny"], par["nx"])) + par[
             "imag"] * np.ones(shape=(par["ny"], par["nx"])) for i in range(size)]
         ops = [MatrixMult(np.conj(mats[i].T) @ mats[i], dtype=par['dtype']) for i in range(size)]
         # To make BlockDiag a positive definite matrix
-        BDiag = BlockDiag(ops=ops)
+        BDiag = BlockDiag(ops=ops, forceflat=True)
         if par["x0"]:
             x0 = x0_global
         else:
             x0 = None
         y1 = BDiag * x_global
         xinv1 = pylops.cg(BDiag, y1, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
         assert_allclose(xinv_array, xinv1, rtol=1e-14)
@@ -143,26 +148,29 @@
     if par["x0"]:
         x0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
         x0[:] = np.random.normal(0, 10, par["nx"]) + par["imag"] * np.random.normal(
             10, 10, par["nx"]
         )
         x0_global = x0.asarray()
     else:
-        x0 = None
+        # Set TO 0s if x0 = False
+        x0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        x0[:] = 0
+        x0_global = x0.asarray()
     y = BDiag_MPI * x
     xinv = cgls(BDiag_MPI, y, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
     assert isinstance(xinv, DistributedArray)
     xinv_array = xinv.asarray()
     if rank == 0:
         mats = [np.ones(shape=(par["ny"], par["nx"])) + par[
             "imag"] * np.ones(shape=(par["ny"], par["nx"])) for i in range(size)]
         ops = [MatrixMult(np.conj(mats[i].T) @ mats[i] + 1e-5 * np.eye(par["nx"], dtype=par['dtype']),
                           dtype=par['dtype']) for i in range(size)]
         # To make BlockDiag a positive definite matrix
-        BDiag = BlockDiag(ops=ops)
+        BDiag = BlockDiag(ops=ops, forceflat=True)
         if par["x0"]:
             x0 = x0_global
         else:
             x0 = None
         y1 = BDiag * x_global
         xinv1 = pylops.cgls(BDiag, y1, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
         assert_allclose(xinv_array, xinv1, rtol=1e-14)
@@ -186,27 +194,29 @@
     if par["x0"]:
         x0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
         x0[:] = np.random.normal(0, 10, par["nx"]) + par["imag"] * np.random.normal(
             10, 10, par["nx"]
         )
         x0_global = x0.asarray()
     else:
-        x0 = None
-
+        # Set TO 0s if x0 = False
+        x0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        x0[:] = 0
+        x0_global = x0.asarray()
     y = HStack_MPI @ x
     assert y.partition is Partition.BROADCAST
 
     xinv = cgls(HStack_MPI, y, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
     assert isinstance(xinv, DistributedArray)
     xinv_array = xinv.asarray()
     if rank == 0:
         ops = [MatrixMult((i + 1) * np.ones((par["ny"], par["nx"])) + (i + 2) * par[
             "imag"
         ] * np.ones((par["ny"], par["nx"])), dtype=par['dtype']) for i in range(size)]
-        Hstack = HStack(ops=ops)
+        Hstack = HStack(ops=ops, forceflat=True)
         if par["x0"]:
             x0 = x0_global
         else:
             x0 = None
         y1 = Hstack @ x_global
         xinv1 = pylops.cgls(Hstack, y1, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
         assert_allclose(xinv_array, xinv1, rtol=1e-14)
@@ -231,29 +241,159 @@
     if par["x0"]:
         x0 = DistributedArray(global_shape=par['nx'], dtype=par['dtype'], partition=Partition.BROADCAST)
         x0[:] = np.random.normal(0, 10, par["nx"]) + par["imag"] * np.random.normal(
             10, 10, par["nx"]
         )
         x0_global = x0.asarray()
     else:
-        x0 = None
-
+        # Set TO 0s if x0 = False
+        x0 = DistributedArray(global_shape=par['nx'], dtype=par['dtype'], partition=Partition.BROADCAST)
+        x0[:] = 0
+        x0_global = x0.asarray()
     y = VStack_MPI @ x
     assert y.partition is Partition.SCATTER
 
     xinv = cgls(VStack_MPI, y, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
     assert isinstance(xinv, DistributedArray)
     xinv_array = xinv.asarray()
     if rank == 0:
         mats = [np.ones(shape=(par["ny"], par["nx"])) + par[
             "imag"] * np.ones(shape=(par["ny"], par["nx"])) for i in range(size)]
         ops = [MatrixMult(np.conj(mats[i].T) @ mats[i] + 1e-5 * np.eye(par["nx"], dtype=par['dtype']),
                           dtype=par['dtype']) for i in range(size)]
         # To make VStack a positive definite matrix
-        Vstack = VStack(ops=ops)
+        Vstack = VStack(ops=ops, forceflat=True)
         if par["x0"]:
             x0 = x0_global
         else:
             x0 = None
         y1 = Vstack @ x_global
         xinv1 = pylops.cgls(Vstack, y1, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
         assert_allclose(xinv_array, xinv1, rtol=1e-14)
+
+
+@pytest.mark.mpi(min_size=2)
+@pytest.mark.parametrize(
+    "par", [(par1), (par1j), (par2), (par2j), (par3), (par3j), (par4), (par4j)]
+)
+def test_cg_stacked(par):
+    """CG with MPIStackedBlockDiag"""
+    A = np.ones((par["ny"], par["nx"])) + par[
+        "imag"] * np.ones((par["ny"], par["nx"]))
+    Aop = MatrixMult(np.conj(A.T) @ A + 1e-5 * np.eye(par["nx"], dtype=par['dtype']),
+                     dtype=par['dtype'])
+    # To make positive definite matrix
+    BDiag_MPI = MPIBlockDiag(ops=[Aop, ])
+    StackedBDiag_MPI = MPIStackedBlockDiag(ops=[BDiag_MPI, BDiag_MPI])
+
+    dist1 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+    dist1[:] = np.random.normal(1, 10, par["nx"]) + par["imag"] * np.random.normal(10, 10, par["nx"])
+    dist2 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+    dist2[:] = np.random.normal(5, 10, par["nx"]) + par["imag"] * np.random.normal(50, 10, par["nx"])
+    x = StackedDistributedArray([dist1, dist2])
+    x_global = x.asarray()
+
+    if par["x0"]:
+        dist1_0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        dist1_0[:] = np.random.normal(0, 10, par["nx"]) + par["imag"] * np.random.normal(
+            10, 10, par["nx"]
+        )
+        dist2_0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        dist2_0[:] = np.random.normal(10, 10, par["nx"]) + par["imag"] * np.random.normal(
+            0, 10, par["nx"]
+        )
+        x0 = StackedDistributedArray([dist1_0, dist2_0])
+        x0_global = x0.asarray()
+    else:
+        # Set TO 0s if x0 = False
+        dist1_0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        dist1_0[:] = 0
+        dist2_0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        dist2_0[:] = 0
+        x0 = StackedDistributedArray([dist1_0, dist2_0])
+        x0_global = x0.asarray()
+
+    y = StackedBDiag_MPI * x
+    xinv = cg(StackedBDiag_MPI, y, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
+    assert isinstance(xinv, StackedDistributedArray)
+    xinv_array = xinv.asarray()
+
+    if rank == 0:
+        mats = [np.ones(shape=(par["ny"], par["nx"])) + par[
+            "imag"] * np.ones(shape=(par["ny"], par["nx"])) for i in range(size)]
+        ops = [MatrixMult(np.conj(mats[i].T) @ mats[i] + 1e-5 * np.eye(par["nx"], dtype=par['dtype']),
+                          dtype=par['dtype']) for i in range(size)]
+        # To make positive definite matrix
+        BDiag = BlockDiag(ops=ops, forceflat=True)
+        StackedBDiag = BlockDiag(ops=[BDiag, BDiag], forceflat=True)
+        if par["x0"]:
+            x0 = x0_global
+        else:
+            x0 = None
+        y1 = StackedBDiag * x_global
+        xinv1 = pylops.cg(StackedBDiag, y1, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
+        assert_allclose(xinv_array, xinv1, rtol=1e-14)
+
+
+@pytest.mark.mpi(min_size=2)
+@pytest.mark.parametrize(
+    "par", [(par1), (par1j), (par2), (par2j), (par3), (par3j), (par4), (par4j)]
+)
+def test_cgls_stacked(par):
+    """CGLS with MPIStackedBlockDiag"""
+    A = np.ones((par["ny"], par["nx"])) + par[
+        "imag"] * np.ones((par["ny"], par["nx"]))
+    Aop = MatrixMult(np.conj(A.T) @ A + 1e-5 * np.eye(par["nx"], dtype=par['dtype']),
+                     dtype=par['dtype'])
+    # To make positive definite matrix
+    BDiag_MPI = MPIBlockDiag(ops=[Aop, ])
+    VStack_MPI = MPIVStack(ops=[Aop, ])
+    StackedBDiag_MPI = MPIStackedBlockDiag(ops=[BDiag_MPI, VStack_MPI])
+
+    dist1 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+    dist1[:] = np.random.normal(1, 10, par["nx"]) + par["imag"] * np.random.normal(10, 10, par["nx"])
+    dist2 = DistributedArray(global_shape=par['nx'], partition=Partition.BROADCAST, dtype=par['dtype'])
+    dist2[:] = np.random.normal(5, 10, dist2.local_shape) + par["imag"] * np.random.normal(50, 10, dist2.local_shape)
+    x = StackedDistributedArray([dist1, dist2])
+    x_global = x.asarray()
+
+    if par["x0"]:
+        dist1_0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        dist1_0[:] = np.random.normal(0, 10, par["nx"]) + par["imag"] * np.random.normal(
+            10, 10, par["nx"]
+        )
+        dist2_0 = DistributedArray(global_shape=par['nx'], partition=Partition.BROADCAST, dtype=par['dtype'])
+        dist2_0[:] = np.random.normal(10, 10, dist2_0.local_shape) + par["imag"] * np.random.normal(
+            0, 10, dist2_0.local_shape
+        )
+        x0 = StackedDistributedArray([dist1_0, dist2_0])
+        x0_global = x0.asarray()
+    else:
+        # Set TO 0s if x0 = False
+        dist1_0 = DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+        dist1_0[:] = 0
+        dist2_0 = DistributedArray(global_shape=par['nx'], partition=Partition.BROADCAST, dtype=par['dtype'])
+        dist2_0[:] = 0
+        x0 = StackedDistributedArray([dist1_0, dist2_0])
+        x0_global = x0.asarray()
+
+    y = StackedBDiag_MPI * x
+    xinv = cgls(StackedBDiag_MPI, y, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
+    assert isinstance(xinv, StackedDistributedArray)
+    xinv_array = xinv.asarray()
+
+    if rank == 0:
+        mats = [np.ones(shape=(par["ny"], par["nx"])) + par[
+            "imag"] * np.ones(shape=(par["ny"], par["nx"])) for i in range(size)]
+        ops = [MatrixMult(np.conj(mats[i].T) @ mats[i] + 1e-5 * np.eye(par["nx"], dtype=par['dtype']),
+                          dtype=par['dtype']) for i in range(size)]
+        # To make positive definite matrix
+        BDiag = BlockDiag(ops=ops, forceflat=True)
+        V_Stack = VStack(ops=ops, forceflat=True)
+        StackedBDiag = BlockDiag(ops=[BDiag, V_Stack], forceflat=True)
+        if par["x0"]:
+            x0 = x0_global
+        else:
+            x0 = None
+        y1 = StackedBDiag * x_global
+        xinv1 = pylops.cgls(StackedBDiag, y1, x0=x0, niter=par["nx"], tol=1e-5, show=True)[0]
+        assert_allclose(xinv_array, xinv1, rtol=1e-14)
```

### Comparing `pylops-mpi-0.0.1/tests/test_stack.py` & `pylops-mpi-0.1.0/tests/test_blockdiag.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,92 @@
+from mpi4py import MPI
 import numpy as np
 from numpy.testing import assert_allclose
-from mpi4py import MPI
+np.random.seed(42)
+
 import pytest
 
 import pylops
 import pylops_mpi
 
-par1 = {'ny': 101, 'nx': 101, 'imag': 0, 'dtype': np.float64}
-par1j = {'ny': 101, 'nx': 101, 'imag': 1j, 'dtype': np.complex128}
-par2 = {'ny': 301, 'nx': 101, 'imag': 0, 'dtype': np.float64}
-par2j = {'ny': 301, 'nx': 101, 'imag': 1j, 'dtype': np.complex128}
+par1 = {'ny': 101, 'nx': 101, 'dtype': np.float64}
+par1j = {'ny': 101, 'nx': 101, 'dtype': np.complex128}
+par2 = {'ny': 301, 'nx': 101, 'dtype': np.float64}
+par2j = {'ny': 301, 'nx': 101, 'dtype': np.complex128}
 
 
 @pytest.mark.mpi(min_size=2)
 @pytest.mark.parametrize("par", [(par1), (par1j), (par2), (par2j)])
-def test_vstack(par):
-    """Test the MPIVStack operator"""
+def test_blockdiag(par):
     size = MPI.COMM_WORLD.Get_size()
     rank = MPI.COMM_WORLD.Get_rank()
-    A = np.ones(shape=(par['ny'], par['nx'])) + par['imag'] * np.ones(shape=(par['ny'], par['nx']))
-    Op = pylops.MatrixMult(A=((rank + 1) * A).astype(par['dtype']))
-    VStack_MPI = pylops_mpi.MPIVStack(ops=[Op, ])
-
-    # Broadcasted DistributedArray(global_shape == local_shape)
-    x = pylops_mpi.DistributedArray(global_shape=par['nx'],
-                                    partition=pylops_mpi.Partition.BROADCAST,
-                                    dtype=par['dtype'])
+    Op = pylops.MatrixMult(A=((rank + 1) * np.ones(shape=(par['ny'], par['nx']))).astype(par['dtype']))
+    BDiag_MPI = pylops_mpi.MPIBlockDiag(ops=[Op, ])
+
+    x = pylops_mpi.DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
     x[:] = np.ones(shape=par['nx'], dtype=par['dtype'])
     x_global = x.asarray()
 
-    # Scattered DistributedArray
-    y = pylops_mpi.DistributedArray(global_shape=size * par['ny'],
-                                    partition=pylops_mpi.Partition.SCATTER,
-                                    dtype=par['dtype'])
+    y = pylops_mpi.DistributedArray(global_shape=size * par['ny'], dtype=par['dtype'])
     y[:] = np.ones(shape=par['ny'], dtype=par['dtype'])
     y_global = y.asarray()
 
-    x_mat = VStack_MPI @ x
-    y_rmat = VStack_MPI.H @ y
+    x_mat = BDiag_MPI @ x
+    y_rmat = BDiag_MPI.H @ y
     assert isinstance(x_mat, pylops_mpi.DistributedArray)
     assert isinstance(y_rmat, pylops_mpi.DistributedArray)
 
     x_mat_mpi = x_mat.asarray()
     y_rmat_mpi = y_rmat.asarray()
 
     if rank == 0:
-        ops = [pylops.MatrixMult(A=((i + 1) * A).astype(par['dtype'])) for i in range(size)]
-        VStack = pylops.VStack(ops=ops)
-        x_mat_np = VStack @ x_global
-        y_rmat_np = VStack.H @ y_global
+        ops = [pylops.MatrixMult((i + 1) * np.ones(shape=(par['ny'], par['nx'])).astype(par['dtype'])) for i in range(size)]
+        BDiag = pylops.BlockDiag(ops=ops)
+
+        x_mat_np = BDiag @ x_global
+        y_rmat_np = BDiag.H @ y_global
         assert_allclose(x_mat_mpi, x_mat_np, rtol=1e-14)
         assert_allclose(y_rmat_mpi, y_rmat_np, rtol=1e-14)
 
 
 @pytest.mark.mpi(min_size=2)
 @pytest.mark.parametrize("par", [(par1), (par1j), (par2), (par2j)])
-def test_hstack(par):
-    """Test the MPIHStack operator"""
+def test_stacked_blockdiag(par):
+    """Tests for MPIStackedBlogDiag"""
     size = MPI.COMM_WORLD.Get_size()
     rank = MPI.COMM_WORLD.Get_rank()
-    A = np.ones(shape=(par['ny'], par['nx'])) + par['imag'] * np.ones(shape=(par['ny'], par['nx']))
-    Op = pylops.MatrixMult(A=((rank + 1) * A).astype(par['dtype']))
-    HStack_MPI = pylops_mpi.MPIHStack(ops=[Op, ])
-
-    # Scattered DistributedArray
-    x = pylops_mpi.DistributedArray(global_shape=size * par['nx'],
-                                    partition=pylops_mpi.Partition.SCATTER,
-                                    dtype=par['dtype'])
-    x[:] = np.ones(shape=par['nx'], dtype=par['dtype'])
+    Op = pylops.MatrixMult(A=((rank + 1) * np.ones(shape=(par['ny'], par['nx']))).astype(par['dtype']))
+    BDiag_MPI = pylops_mpi.MPIBlockDiag(ops=[Op, ])
+    FirstDeriv_MPI = pylops_mpi.MPIFirstDerivative(dims=(par['ny'], par['nx']), dtype=par['dtype'])
+    StackedBDiag_MPI = pylops_mpi.MPIStackedBlockDiag(ops=[BDiag_MPI, FirstDeriv_MPI])
+
+    dist1 = pylops_mpi.DistributedArray(global_shape=size * par['nx'], dtype=par['dtype'])
+    dist1[:] = np.ones(dist1.local_shape, dtype=par['dtype'])
+    dist2 = pylops_mpi.DistributedArray(global_shape=par['nx'] * par['ny'], dtype=par['dtype'])
+    dist2[:] = np.ones(dist2.local_shape, dtype=par['dtype'])
+    x = pylops_mpi.StackedDistributedArray(distarrays=[dist1, dist2])
     x_global = x.asarray()
 
-    # Broadcasted DistributedArray(global_shape == local_shape)
-    y = pylops_mpi.DistributedArray(global_shape=par['ny'],
-                                    partition=pylops_mpi.Partition.BROADCAST,
-                                    dtype=par['dtype'])
-    y[:] = np.ones(shape=par['ny'], dtype=par['dtype'])
+    dist1 = pylops_mpi.DistributedArray(global_shape=size * par['ny'], dtype=par['dtype'])
+    dist1[:] = np.ones(dist1.local_shape, dtype=par['dtype'])
+    dist2 = pylops_mpi.DistributedArray(global_shape=par['nx'] * par['ny'], dtype=par['dtype'])
+    dist2[:] = np.ones(dist2.local_shape, dtype=par['dtype'])
+    y = pylops_mpi.StackedDistributedArray(distarrays=[dist1, dist2])
     y_global = y.asarray()
 
-    x_mat = HStack_MPI @ x
-    y_rmat = HStack_MPI.H @ y
-    assert isinstance(x_mat, pylops_mpi.DistributedArray)
-    assert isinstance(y_rmat, pylops_mpi.DistributedArray)
+    x_mat = StackedBDiag_MPI @ x
+    y_rmat = StackedBDiag_MPI.H @ y
+    assert isinstance(x_mat, pylops_mpi.StackedDistributedArray)
+    assert isinstance(y_rmat, pylops_mpi.StackedDistributedArray)
 
     x_mat_mpi = x_mat.asarray()
     y_rmat_mpi = y_rmat.asarray()
 
     if rank == 0:
-        ops = [pylops.MatrixMult(A=((i + 1) * A).astype(par['dtype'])) for i in range(size)]
-        HStack = pylops.HStack(ops=ops)
-        x_mat_np = HStack @ x_global
-        y_rmat_np = HStack.H @ y_global
+        ops = [pylops.MatrixMult((i + 1) * np.ones(shape=(par['ny'], par['nx'])).astype(par['dtype'])) for i in range(size)]
+        BDiag = pylops.BlockDiag(ops=ops)
+        FirstDeriv = pylops.FirstDerivative(dims=(par['ny'], par['nx']), axis=0, dtype=par['dtype'])
+        BDiag_final = pylops.BlockDiag([BDiag, FirstDeriv])
+        x_mat_np = BDiag_final @ x_global
+        y_rmat_np = BDiag_final.H @ y_global
         assert_allclose(x_mat_mpi, x_mat_np, rtol=1e-14)
         assert_allclose(y_rmat_mpi, y_rmat_np, rtol=1e-14)
```

### Comparing `pylops-mpi-0.0.1/tutorials/plot_lsm.py` & `pylops-mpi-0.1.0/tutorials/lsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,18 @@
 d_adj = d_adj_dist.asarray().reshape((nstot, nr, nt))
 
 ###############################################################################
 # We calculate the inverse using the :py:func:`pylops_mpi.optimization.basic.cgls`
 # solver.
 
 # Inverse
-minv_dist = pylops_mpi.cgls(VStack, d_dist, niter=100, show=True)[0]
+# Initializing x0 to zeroes
+x0 = pylops_mpi.DistributedArray(VStack.shape[1], partition=pylops_mpi.Partition.BROADCAST)
+x0[:] = 0
+minv_dist = pylops_mpi.cgls(VStack, d_dist, x0=x0, niter=100, show=True)[0]
 minv = minv_dist.asarray().reshape((nx, nz))
 d_inv_dist = VStack @ minv_dist
 d_inv = d_inv_dist.asarray().reshape(nstot, nr, nt)
 
 ###############################################################################
 if rank == 0:
     # Visualize
```

### Comparing `pylops-mpi-0.0.1/tutorials/plot_post_stack_inversion.py` & `pylops-mpi-0.1.0/tutorials/poststack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 r"""
 Post Stack Inversion - 3D
 =========================
 This tutorial demonstrates the implementation of a distributed 3D Post-stack inversion. It consists
 of a first part showing how to model a 3D synthetic post-stack seismic data from a 3D model of the
-subsurface acoustic impedence in a distributed manner, following by a second part when inversion
+subsurface acoustic impedance in a distributed manner, following by a second part when inversion
 is carried out.
 
 This tutorial builds on the :py:func:`pylops.avo.poststack.PoststackLinearModelling`
 operator to model 1d post-stack seismic traces 1d profiles of the subsurface acoustic impedence
 by means of the following equation
 
 .. math::
@@ -132,66 +132,78 @@
 # We perform 2 different kinds of inversions:
 #
 # * Inversion calculated iteratively using the :py:class:`pylops_mpi.optimization.cls_basic.CGLS` solver.
 #
 # * Inversion with spatial regularization using normal equations along all three dimensions (x, y and z).
 #   This requires extending the operator and data in the following manner:
 #
-#  .. math::
-#    \mathbf{NormEqOp} =
-#    \begin{bmatrix}
-#         \mathbf{G}_1  & \mathbf{0}   &  \ldots &  \mathbf{0}  \\
-#         \mathbf{0}    & \mathbf{G}_2 &  \ldots &  \mathbf{0}  \\
-#         \vdots        & \vdots       &  \ddots &  \vdots         \\
-#         \mathbf{0}    & \mathbf{0}   &  \ldots &  \mathbf{G}_N
-#    \end{bmatrix}
-#    \begin{bmatrix}
+# .. math::
+#   \mathbf{N} =
+#   \begin{bmatrix}
 #         \mathbf{G}_1^H  & \mathbf{0}   &  \ldots &  \mathbf{0}  \\
 #         \mathbf{0}    & \mathbf{G}_2^H &  \ldots &  \mathbf{0}  \\
 #         \vdots        & \vdots       &  \ddots &  \vdots         \\
 #         \mathbf{0}    & \mathbf{0}   &  \ldots &  \mathbf{G}_N^H
-#    \end{bmatrix} + \epsilon \mathbf{LapOp} \\
+#   \end{bmatrix}
+#   \begin{bmatrix}
+#         \mathbf{G}_1  & \mathbf{0}   &  \ldots &  \mathbf{0}  \\
+#         \mathbf{0}    & \mathbf{G}_2 &  \ldots &  \mathbf{0}  \\
+#         \vdots        & \vdots       &  \ddots &  \vdots         \\
+#         \mathbf{0}    & \mathbf{0}   &  \ldots &  \mathbf{G}_N
+#   \end{bmatrix} + \epsilon \mathbf{L}^H \mathbf{L} \\
 #
-#  .. math::
+# .. math::
 #   \begin{bmatrix}
 #         \mathbf{d}_{1}^{Norm}  \\
 #         \mathbf{d}_{2}^{Norm}  \\
 #         \vdots     \\
 #         \mathbf{d}_{N}^{Norm}
-#    \end{bmatrix} =
-#    \begin{bmatrix}
+#   \end{bmatrix} =
+#   \begin{bmatrix}
 #         \mathbf{G}_1^H  & \mathbf{0}   &  \ldots &  \mathbf{0}  \\
 #         \mathbf{0}    & \mathbf{G}_2^H &  \ldots &  \mathbf{0}  \\
 #         \vdots        & \vdots       &  \ddots &  \vdots         \\
 #         \mathbf{0}    & \mathbf{0}   &  \ldots &  \mathbf{G}_N^H
-#    \end{bmatrix}
-#    \begin{bmatrix}
+#   \end{bmatrix}
+#   \begin{bmatrix}
 #         \mathbf{d}_{1}  \\
 #         \mathbf{d}_{2}  \\
 #         \vdots     \\
 #         \mathbf{d}_{N}
-#    \end{bmatrix}
+#   \end{bmatrix}
 #
-# where :math:`\mathbf{LapOp}` is the :py:class:`pylops_mpi.basicoperators.MPILaplacian` operator
-# which is used to apply second derivative along all three axes, :math:`\mathbf{NormEqOp}` is the regularized operator
-# which operates using normal equations and :math:`\mathbf{d}^{Norm}` is the data of the operator used for inversion.
+# where :math:`\mathbf{L}` is the :py:class:`pylops_mpi.basicoperators.MPILaplacian` operator
+# which is used to apply second derivative along all three axes, :math:`\mathbf{N}` is an operator computing the
+# normal equations, and :math:`\mathbf{d}^{Norm}` is the data of the normal equation operator used for inversion.
 
 # Inversion using CGLS solver
 minv3d_iter_dist = pylops_mpi.optimization.basic.cgls(BDiag, d_dist, x0=mback3d_dist, niter=100, show=True)[0]
 minv3d_iter = minv3d_iter_dist.asarray().reshape((ny, nx, nz))
 
 ###############################################################################
 
 # Regularized inversion with normal equations
 epsR = 1e2
 LapOp = pylops_mpi.MPILaplacian(dims=(ny, nx, nz), axes=(0, 1, 2), weights=(1, 1, 1),
                                 sampling=(1, 1, 1), dtype=BDiag.dtype)
-NormEqOp = BDiag.H @ BDiag + epsR * LapOp
+NormEqOp = BDiag.H @ BDiag + epsR * LapOp.H @ LapOp
 dnorm_dist = BDiag.H @ d_dist
-minv3d_reg_dist = pylops_mpi.optimization.basic.cg(NormEqOp, dnorm_dist, x0=mback3d_dist, niter=100, show=True)[0]
+minv3d_ne_dist = pylops_mpi.optimization.basic.cg(NormEqOp, dnorm_dist, x0=mback3d_dist, niter=100, show=True)[0]
+minv3d_ne = minv3d_ne_dist.asarray().reshape((ny, nx, nz))
+
+###############################################################################
+
+# Regularized inversion with regularized equations
+StackOp = pylops_mpi.MPIStackedVStack([BDiag, np.sqrt(epsR) * LapOp])
+d0_dist = pylops_mpi.DistributedArray(global_shape=ny * nx * nz)
+d0_dist[:] = 0.
+dstack_dist = pylops_mpi.StackedDistributedArray([d_dist, d0_dist])
+
+dnorm_dist = BDiag.H @ d_dist
+minv3d_reg_dist = pylops_mpi.optimization.basic.cgls(StackOp, dstack_dist, x0=mback3d_dist, niter=100, show=False)[0]
 minv3d_reg = minv3d_reg_dist.asarray().reshape((ny, nx, nz))
 
 ###############################################################################
 # Finally, we display the modeling and inversion results
 
 if rank == 0:
     # Check the distributed implementation gives the same result
@@ -201,15 +213,15 @@
     d0_0 = (PPop0 @ m3d.transpose(2, 0, 1)).transpose(1, 2, 0)
 
     # Check the two distributed implementations give the same modelling results
     print('Distr == Local', np.allclose(d, d0))
     print('Smooth Distr == Local', np.allclose(d_0, d0_0))
 
     # Visualize
-    fig, axs = plt.subplots(nrows=5, ncols=3, figsize=(9, 14), constrained_layout=True)
+    fig, axs = plt.subplots(nrows=6, ncols=3, figsize=(9, 14), constrained_layout=True)
     axs[0][0].imshow(m3d[5, :, :].T, cmap="gist_rainbow", vmin=m.min(), vmax=m.max())
     axs[0][0].set_title("Model x-z")
     axs[0][0].axis("tight")
     axs[0][1].imshow(m3d[:, 200, :].T, cmap="gist_rainbow", vmin=m.min(), vmax=m.max())
     axs[0][1].set_title("Model y-z")
     axs[0][1].axis("tight")
     axs[0][2].imshow(m3d[:, :, 220].T, cmap="gist_rainbow", vmin=m.min(), vmax=m.max())
@@ -242,16 +254,26 @@
     axs[3][1].imshow(minv3d_iter[:, 200, :].T, cmap='gist_rainbow', vmin=m.min(), vmax=m.max())
     axs[3][1].set_title('Inverted Model iter y-z')
     axs[3][1].axis('tight')
     axs[3][2].imshow(minv3d_iter[:, :, 220].T, cmap='gist_rainbow', vmin=m.min(), vmax=m.max())
     axs[3][2].set_title('Inverted Model iter x-y')
     axs[3][2].axis('tight')
 
-    axs[4][0].imshow(minv3d_reg[5, :, :].T, cmap="gist_rainbow", vmin=m.min(), vmax=m.max())
-    axs[4][0].set_title("Regularized Inverted Model iter x-z")
+    axs[4][0].imshow(minv3d_ne[5, :, :].T, cmap="gist_rainbow", vmin=m.min(), vmax=m.max())
+    axs[4][0].set_title("Normal Equations Inverted Model iter x-z")
     axs[4][0].axis("tight")
-    axs[4][1].imshow(minv3d_reg[:, 200, :].T, cmap='gist_rainbow', vmin=m.min(), vmax=m.max())
-    axs[4][1].set_title('Regularized Inverted Model iter y-z')
+    axs[4][1].imshow(minv3d_ne[:, 200, :].T, cmap='gist_rainbow', vmin=m.min(), vmax=m.max())
+    axs[4][1].set_title('Normal Equations Inverted Model iter y-z')
     axs[4][1].axis('tight')
-    axs[4][2].imshow(minv3d_reg[:, :, 220].T, cmap='gist_rainbow', vmin=m.min(), vmax=m.max())
-    axs[4][2].set_title('Regularized Inverted Model iter x-y')
+    axs[4][2].imshow(minv3d_ne[:, :, 220].T, cmap='gist_rainbow', vmin=m.min(), vmax=m.max())
+    axs[4][2].set_title('Normal Equations Inverted Model iter x-y')
     axs[4][2].axis('tight')
+
+    axs[5][0].imshow(minv3d_reg[5, :, :].T, cmap="gist_rainbow", vmin=m.min(), vmax=m.max())
+    axs[5][0].set_title("Regularized Inverted Model iter x-z")
+    axs[5][0].axis("tight")
+    axs[5][1].imshow(minv3d_reg[:, 200, :].T, cmap='gist_rainbow', vmin=m.min(), vmax=m.max())
+    axs[5][1].set_title('Regularized Inverted Model iter y-z')
+    axs[5][1].axis('tight')
+    axs[5][2].imshow(minv3d_reg[:, :, 220].T, cmap='gist_rainbow', vmin=m.min(), vmax=m.max())
+    axs[5][2].set_title('Regularized Inverted Model iter x-y')
+    axs[5][2].axis('tight')
```

