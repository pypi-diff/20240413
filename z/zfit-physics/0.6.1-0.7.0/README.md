# Comparing `tmp/zfit_physics-0.6.1.tar.gz` & `tmp/zfit_physics-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfit_physics-0.6.1.tar", last modified: Mon Oct  9 09:08:07 2023, max compression
+gzip compressed data, was "zfit_physics-0.7.0.tar", last modified: Sat Apr 13 18:58:55 2024, max compression
```

## Comparing `zfit_physics-0.6.1.tar` & `zfit_physics-0.7.0.tar`

### file list

```diff
@@ -1,78 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.654097 zfit_physics-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.all-contributorsrc
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.646097 zfit_physics-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.646097 zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/behaviorunderdiscussion.md
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/physics-specific-question.md
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/zfit-usage-question.md
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.646097 zfit_physics-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/.scrutinizer.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2023-10-09 09:08:07.654097 zfit_physics-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.646097 zfit_physics-0.6.1/docs/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/docs/api/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/api/tools/change_headline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9505 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127528 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/images/scikit-hep-logo_168x168.png
--rw-r--r--   0 runner    (1001) docker     (127)   274482 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/images/zfit-fin_400x168.png
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/images/zfit-fin_57x24.png
--rw-r--r--   0 runner    (1001) docker     (127)    42170 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/images/zfit_workflow_v1.png
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      632 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/docs/make_docs.sh
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-10-09 09:08:07.654097 zfit_physics-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/tests/test_pdf_argus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/tests/test_pdf_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/tests/test_pdf_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/tests/test_pdf_kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/tests/test_pdf_relbw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.646097 zfit_physics-0.6.1/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/utils/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/utils/ci/test_examples.sh
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/utils/ci/testbuild_docs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/zfit_physics/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/zfit_physics/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7580 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/models/pdf_argus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/models/pdf_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/models/pdf_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/models/pdf_kde.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/models/pdf_relbw.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/zfit_physics/unstable/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/unstable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-09 09:07:57.000000 zfit_physics-0.6.1/zfit_physics/unstable/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 09:08:07.650097 zfit_physics-0.6.1/zfit_physics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2023-10-09 09:08:07.000000 zfit_physics-0.6.1/zfit_physics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-10-09 09:08:07.000000 zfit_physics-0.6.1/zfit_physics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 09:08:07.000000 zfit_physics-0.6.1/zfit_physics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 09:08:07.000000 zfit_physics-0.6.1/zfit_physics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-09 09:08:07.000000 zfit_physics-0.6.1/zfit_physics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-09 09:08:07.000000 zfit_physics-0.6.1/zfit_physics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.917617 zfit_physics-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.all-contributorsrc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.905617 zfit_physics-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.905617 zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/behaviorunderdiscussion.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/physics-specific-question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/zfit-usage-question.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.905617 zfit_physics-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-13 18:58:55.917617 zfit_physics-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.905617 zfit_physics-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.901617 zfit_physics-0.7.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.905617 zfit_physics-0.7.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.901617 zfit_physics-0.7.0/docs/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.909617 zfit_physics-0.7.0/docs/api/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/api/static/zfit_physics.pdf.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.909617 zfit_physics-0.7.0/docs/api/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/api/tools/change_headline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.909617 zfit_physics-0.7.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/scikit-hep-logo_168x168.png
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22421 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-fin_400x168.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-fin_57x24.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13744 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-logo-light_400x168.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-logo_400x168.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-logo_57x24.png
+-rw-r--r--   0 runner    (1001) docker     (127)    39722 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-logo_hires.png
+-rw-r--r--   0 runner    (1001) docker     (127)   256823 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-logo_veryhires.png
+-rw-r--r--   0 runner    (1001) docker     (127)   117114 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit-vector.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10957 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit_workflow_v1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   156414 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/images/zfit_workflow_v2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      632 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/docs/make_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-13 18:58:55.917617 zfit_physics-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.913617 zfit_physics-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_argus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_cmsshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_cruijff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_erfexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_novosibirsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_relbw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/tests/test_pdf_tsallis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.901617 zfit_physics-0.7.0/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.913617 zfit_physics-0.7.0/utils/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/utils/ci/test_examples.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/utils/ci/testbuild_docs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.913617 zfit_physics-0.7.0/zfit_physics/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.913617 zfit_physics-0.7.0/zfit_physics/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_argus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_cmsshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_cruijff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_erfexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_kde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6875 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_novosibirsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_relbw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/models/pdf_tsallis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.913617 zfit_physics-0.7.0/zfit_physics/unstable/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/unstable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-13 18:58:51.000000 zfit_physics-0.7.0/zfit_physics/unstable/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:58:55.913617 zfit_physics-0.7.0/zfit_physics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-13 18:58:55.000000 zfit_physics-0.7.0/zfit_physics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-13 18:58:55.000000 zfit_physics-0.7.0/zfit_physics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 18:58:55.000000 zfit_physics-0.7.0/zfit_physics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 18:58:55.000000 zfit_physics-0.7.0/zfit_physics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-13 18:58:55.000000 zfit_physics-0.7.0/zfit_physics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-13 18:58:55.000000 zfit_physics-0.7.0/zfit_physics.egg-info/top_level.txt
```

### Comparing `zfit_physics-0.6.1/.all-contributorsrc` & `zfit_physics-0.7.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/behaviorunderdiscussion.md` & `zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/behaviorunderdiscussion.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md` & `zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/feature-request.md` & `zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/.github/ISSUE_TEMPLATE/zfit-usage-question.md` & `zfit_physics-0.7.0/.github/ISSUE_TEMPLATE/zfit-usage-question.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/.github/ISSUE_TEMPLATE.md` & `zfit_physics-0.7.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/.github/workflows/cd.yml` & `zfit_physics-0.7.0/.github/workflows/cd.yml`

 * *Files 3% similar despite different names*

```diff
@@ -18,33 +18,33 @@
 jobs:
   dist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4.7.0
+      - uses: actions/setup-python@v5.1.0
 
       - name: Build SDist and wheel
         run: pipx run --spec build pyproject-build
 
       - name: Check metadata
         run: pipx run twine check dist/*
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
           path: dist/*
 
   publish:
     needs: [ dist ]
     environment: pypi
     permissions:
       id-token: write
     runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `zfit_physics-0.6.1/.gitignore` & `zfit_physics-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/.pre-commit-config.yaml` & `zfit_physics-0.7.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ci:
     autoupdate_schedule: quarterly
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: check-toml
@@ -31,34 +31,34 @@
     hooks:
       - id: python-use-type-annotations
       - id: python-check-mock-methods
       - id: python-no-eval
       - id: rst-directive-colons
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.14.0
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [ --py38-plus ]
 
   - repo: https://github.com/asottile/setup-cfg-fmt
     rev: v2.5.0
     hooks:
       - id: setup-cfg-fmt
-        args: [ --max-py-version=3.10, --include-version-classifiers ]
+        args: [ --max-py-version=3.12, --include-version-classifiers ]
 
 
   # Notebook formatting
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.7.0
+    rev: 1.8.5
     hooks:
       - id: nbqa-isort
         additional_dependencies: [ isort ]
 
       - id: nbqa-pyupgrade
         additional_dependencies: [ pyupgrade ]
         args: [ --py38-plus ]
@@ -70,11 +70,21 @@
         stages: [ manual ]
   - repo: https://github.com/sondrelg/pep585-upgrade
     rev: 'v1.0'
     hooks:
     - id: upgrade-type-hints
       args: [ '--futures=true' ]
 
-  - repo: https://github.com/psf/black
-    rev: 23.9.1
+  - repo: https://github.com/MarcoGorelli/auto-walrus
+    rev: v0.2.2
     hooks:
-      - id: black
+     - id: auto-walrus
+
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.3.5"
+    hooks:
+      - id: ruff
+        types_or: [ python, pyi, jupyter ]
+        args: [ --fix, --unsafe-fixes, --show-fixes , --line-length=120]
+      # Run the formatter.
+      - id: ruff-format
+        types_or: [ python, pyi, jupyter ]
```

### Comparing `zfit_physics-0.6.1/LICENSE` & `zfit_physics-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/README.rst` & `zfit_physics-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/docs/Makefile` & `zfit_physics-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/docs/conf.py` & `zfit_physics-0.7.0/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,55 +13,72 @@
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
-import os
-import sys
+from __future__ import annotations
 
-import sphinx_bootstrap_theme
+import sys
+from pathlib import Path
 
-sys.path.insert(0, os.path.abspath(".."))
+sys.path.insert(0, str(Path("..").resolve()))
 
 import zfit_physics
 
 project = "zfit-physics"
 
 copyright = zfit_physics.__copyright__
 author = zfit_physics.__author__
 
 # The short X.Y version
-version = zfit_physics.__version__
+version = zfit_physics.__version__.split("+")[0]
 # The full version, including alpha/beta/rc tags
 release = zfit_physics.__version__
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
+#
+needs_sphinx = "3.0.0"
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     "sphinx.ext.autodoc",
-    "sphinx.ext.doctest",
+    "sphinx.ext.napoleon",
+    "sphinx_autodoc_typehints",
+    # sphinx_autodoc_typehints must be imported after napoleon to properly work.
+    # See https://github.com/agronholm/sphinx-autodoc-typehints/issues/15
+    "jupyter_sphinx",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.viewcode",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.todo",
+    "sphinxcontrib.images",
     "sphinx.ext.coverage",
     "sphinx.ext.mathjax",
-    "sphinx.ext.ifconfig",
-    "sphinx.ext.viewcode",
     "sphinx.ext.githubpages",
-    "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+    "sphinx_copybutton",
+    "sphinxcontrib.youtube",
+    "sphinx_panels",
+    "seed_intersphinx_mapping",
+    "myst_nb",
+    "sphinx_togglebutton",
 ]
 
+panels_add_bootstrap_css = False  # for sphinx_panel, use custom css from theme, not bootstrap
+
 using_numpy_style = False  # False -> google style
 
 # Napoleon settings (convert numpy/google docstrings to proper ReST
 napoleon_google_docstring = not using_numpy_style
 napoleon_numpy_docstring = using_numpy_style
 napoleon_include_init_with_doc = False
 napoleon_include_private_with_doc = False
@@ -69,25 +86,56 @@
 napoleon_use_admonition_for_examples = False
 napoleon_use_admonition_for_notes = False
 napoleon_use_admonition_for_references = False
 napoleon_use_ivar = False
 napoleon_use_param = True
 napoleon_use_rtype = True
 
+# -- sphinx_autodoc_typehints settings ---------------------------------------------
+
+# if True, set typing.TYPE_CHECKING to True to enable “expensive” typing imports
+set_type_checking_flag = True
+# if True, class names are always fully qualified (e.g. module.for.Class). If False, just the class
+# name displays (e.g. Class)
+typehints_fully_qualified = False
+# (default: False): If False, do not add ktype info for undocumented parameters. If True, add stub documentation for
+# undocumented parameters to be able to add type info.
+always_document_param_types = False
+# (default: True): If False, never add an :rtype: directive. If True, add the :rtype: directive if no existing :rtype:
+# is found.
+typehints_document_rtype = True
+
+# -- autodoc settings ---------------------------------------------
+
+# also doc __init__ docstrings
+autoclass_content = "both"
+autodoc_member_order = "bysource"
+autodoc_default_options = {
+    "show-inheritance": True,
+    "inherited-members": True,
+}
+autodoc_inherit_docstrings = False
+
+# -- autosummary settings ---------------------------------------------
+
+autosummary_generate = True
+autosummary_generate_overwrite = True
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # also doc __init__ docstrings
 autoclass_content = "both"
 #
 # source_suffix = ['.rst', '.md']
 source_suffix = ".rst"
 
+
 # The master toctree document.
 master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
@@ -104,88 +152,55 @@
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 
-html_theme = "bootstrap"
-html_theme_path = sphinx_bootstrap_theme.get_html_theme_path()
+# -- Options for HTML output -------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+
+html_theme = "pydata_sphinx_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
+html_css_files = [
+    "css/custom.css",
+]
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.
+
 html_theme_options = {
-    # Navigation bar title. (Default: ``project`` value)
-    "navbar_title": "zfit",
-    # Tab name for entire site. (Default: "Site")
-    # 'navbar_site_name': "Docs",
-    # 'navbar_site_name': "Overview",
-    # A list of tuples containing pages or urls to link to.
-    # Valid tuples should be in the following forms:
-    #    (name, page)                 # a link to a page
-    #    (name, "/aa/bb", 1)          # a link to an arbitrary relative url
-    #    (name, "http://example.com", True) # arbitrary absolute url
-    # Note the "1" or "True" value above as the third argument to indicate
-    # an arbitrary url.
-    "navbar_links": [
-        ("Getting started", "getting_started"),
-        ("Amplitude", "amplitude"),
-        # ("Parameter", "parameter"),
-        # ("Model", "model"),
-        # ("Data", "data"),
-        # ("Loss", "loss"),
-        # ("Minimize", "minimize"),
-        ("API", "API"),
-        # ("Link", "http://example.com", True),
-    ],
-    # Render the next and previous page links in navbar. (Default: true)
-    "navbar_sidebarrel": False,
-    # Render the current pages TOC in the navbar. (Default: true)
-    "navbar_pagenav": False,
-    # Tab name for the current pages TOC. (Default: "Page")
-    # 'navbar_pagenav_name': "Page",
-    # Global TOC depth for "site" navbar tab. (Default: 1)
-    # Switching to -1 shows all levels.
-    "globaltoc_depth": 1,
-    # Include hidden TOCs in Site navbar?
-    #
-    # Note: If this is "false", you cannot have mixed ``:hidden:`` and
-    # non-hidden ``toctree`` directives in the same page, or else the build
-    # will break.
-    #
-    # Values: "true" (default) or "false"
-    "globaltoc_includehidden": "true",
-    # HTML navbar class (Default: "navbar") to attach to <div> element.
-    # For black navbar, do "navbar navbar-inverse"
-    # 'navbar_class': "navbar navbar-inverse",
-    "navbar_class": "navbar",
-    # Fix navigation bar to top of page?
-    # Values: "true" (default) or "false"
-    "navbar_fixed_top": "true",
-    # Location of link to source.
-    # Options are "nav" (default), "footer" or anything else to exclude.
-    # 'source_link_position': "nav",
-    "source_link_position": False,
-    # Bootswatch (http://bootswatch.com/) theme.
-    #
-    # Options are nothing (default) or the name of a valid theme
-    # such as "cosmo" or "sandstone".
-    #
-    # The set of valid themes depend on the version of Bootstrap
-    # that's used (the next config option).
-    #
-    # Currently, the supported themes are:
-    # - Bootstrap 2: https://bootswatch.com/2
-    # - Bootstrap 3: https://bootswatch.com/3
-    "bootswatch_theme": "flatly",
-    # Choose Bootstrap version.
-    # Values: "3" (default) or "2" (in quotes)
-    "bootstrap_version": "4",
+    "logo": {
+        "image_light": "images/zfit-logo_400x168.png",
+        "image_dark": "images/zfit-logo-light_400x168.png",
+    },
+    "github_url": "https://github.com/zfit/zfit",
+    "use_edit_page_button": True,
+    "navigation_depth": 3,
+    "search_bar_text": "Search zfit...",
+    "navigation_with_keys": True,
+    "search_bar_position": "sidebar",
+    "icon_links": [{}],  # temporary fix for https://github.com/pydata/pydata-sphinx-theme/issues/1220
+    # "repository_url": "https://github.com/zfit/zfit",  # adding jupyter book somehow?
+    # "repository_branch": "develop",
+    # "path_to_docs": "docs",
+}
+
+html_context = {
+    "github_user": "zfit",
+    "github_repo": "zfit",
+    "github_version": "develop",
+    "doc_path": "docs",
 }
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
@@ -270,13 +285,36 @@
 epub_exclude_files = ["search.html"]
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {"https://docs.python.org/": None}
+# cross reference
+default_role = "py:obj"
+primary_domain = "py"
+# nitpicky = True  # warn if cross-references are missing
+# nitpick_ignore = [
+#     ("py:class", "tensorflow.keras.losses.Loss"),
+# ]
+# Example configuration for intersphinx: refer to the Python standard library.
+intersphinx_mapping = {
+    # 'numdifftools': ('https://numdifftools.readthedocs.io/en/latest/index.html', None),
+    "tensorflow": (
+        "https://www.tensorflow.org/api_docs/python",
+        "https://raw.githubusercontent.com/GPflow/tensorflow-intersphinx/master/tf2_py_objects.inv",
+    ),
+    "tensorflow_probability": (
+        "https://www.tensorflow.org/probability/api_docs/python",
+        " https://raw.githubusercontent.com/GPflow/tensorflow-intersphinx/master/tfp_py_objects.inv",
+    ),
+    "uproot": ("https://uproot.readthedocs.io/en/latest/", None),
+    "python": ("https://docs.python.org/3", None),
+    "matplotlib": ("https://matplotlib.org/stable/", None),
+    "pandas": ("https://pandas.pydata.org/docs/", None),
+    "numpy": ("https://numpy.org/doc/stable/", None),
+}
 
 # -- Options for todo extension ----------------------------------------------
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zfit_physics-0.6.1/docs/make_docs.sh` & `zfit_physics-0.7.0/docs/make_docs.sh`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/setup.cfg` & `zfit_physics-0.7.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: MacOS
 	Operating System :: Unix
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Physics
 keywords = TensorFlow, model, fitting, scalable, HEP, physics
 
 [options]
-python_requires = >=3.8
+python_requires = >=3.9
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
 exclude = 
 	docs,
```

### Comparing `zfit_physics-0.6.1/tests/conftest.py` & `zfit_physics-0.7.0/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from __future__ import annotations
+
 import sys
 
 import pytest
 
 init_modules = sys.modules.keys()
 
 
 @pytest.fixture(autouse=True)
-def setup_teardown():
+def _setup_teardown():
     import zfit
 
     old_chunksize = zfit.run.chunking.max_n_points
     old_active = zfit.run.chunking.active
     old_graph_mode = zfit.run.get_graph_mode()
     old_autograd_mode = zfit.run.get_autograd_mode()
 
-    for m in sys.modules.keys():
+    for m in sys.modules:
         if m not in init_modules:
             del sys.modules[m]
 
     yield
     from zfit.core.parameter import ZfitParameterMixin
 
     ZfitParameterMixin._existing_params.clear()
@@ -28,13 +30,13 @@
     clear_graph_cache()
     import zfit
 
     zfit.run.chunking.active = old_active
     zfit.run.chunking.max_n_points = old_chunksize
     zfit.run.set_graph_mode(old_graph_mode)
     zfit.run.set_autograd_mode(old_autograd_mode)
-    for m in sys.modules.keys():
+    for m in sys.modules:
         if m not in init_modules:
             del sys.modules[m]
     import gc
 
     gc.collect()
```

### Comparing `zfit_physics-0.6.1/tests/test_pdf_argus.py` & `zfit_physics-0.7.0/tests/test_pdf_argus.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/tests/test_pdf_conv.py` & `zfit_physics-0.7.0/tests/test_pdf_conv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Example test for a pdf or function."""
+
 import numpy as np
 import pytest
 import tensorflow as tf
 import zfit
 
 import zfit_physics as zphys
```

### Comparing `zfit_physics-0.6.1/tests/test_pdf_example.py` & `zfit_physics-0.7.0/tests/test_pdf_example.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.6.1/tests/test_pdf_kde.py` & `zfit_physics-0.7.0/tests/test_pdf_kde.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Example test for a pdf or function."""
+
 import numpy as np
 import pytest
 import tensorflow as tf
 import zfit
 from zfit.core.testing import tester
 
 import zfit_physics as zphys
```

### Comparing `zfit_physics-0.6.1/tests/test_pdf_relbw.py` & `zfit_physics-0.7.0/tests/test_pdf_relbw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for relativistic Breit-Wigner PDF."""
+
 import pytest
 import tensorflow as tf
 import zfit
 
 # Important, do the imports below
 from zfit.core.testing import tester
```

### Comparing `zfit_physics-0.6.1/zfit_physics/__init__.py` & `zfit_physics-0.7.0/zfit_physics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Top-level package for zfit."""
+
 from pkg_resources import get_distribution
 
 __version__ = get_distribution(__name__).version
 
 __license__ = "BSD 3-Clause"
 __copyright__ = "Copyright 2019, zfit"
 __status__ = "Pre-alpha"
```

### Comparing `zfit_physics-0.6.1/zfit_physics/models/pdf_argus.py` & `zfit_physics-0.7.0/zfit_physics/models/pdf_argus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ARGUS PDF (https://en.wikipedia.org/wiki/ARGUS_distribution)"""
-from typing import Optional
+
+from __future__ import annotations
 
 import numpy as np
 import tensorflow as tf
 import tensorflow_probability as tfp
 import zfit
 from zfit import z
 from zfit.util import ztyping
@@ -37,27 +38,29 @@
     Returns:
         `tf.Tensor`: the values matching the (broadcasted) shapes of the input
     """
     m = tfp.math.clip_by_value_preserve_gradient(m, 0.0, m0)
     m_frac = m / m0
 
     m_factor = 1 - z.square(m_frac)
-    argus = m * z.pow(m_factor, p) * (z.exp(c * m_factor))
-    return argus
+    return m * z.pow(m_factor, p) * (z.exp(c * m_factor))
 
 
 class Argus(zfit.pdf.BasePDF):
     def __init__(
         self,
-        obs: ztyping.ObsTypeInput,
+        *,
         m0,
         c,
         p,
+        obs: ztyping.ObsTypeInput,
+        extended: ztyping.ParamTypeInput | None = None,
+        norm: ztyping.NormTypeInput = None,
         name: str = "ArgusPDF",
-        extended: Optional[ztyping.ParamTypeInput] = None,
+        label: str | None = None,
     ):
         r"""`ARGUS shape <https://en.wikipedia.org/wiki/ARGUS_distribution>`_ describing the invariant mass of a particle
         in a continuous background.
 
         The ARGUS shaped function describes the reconstructed invariant mass of a decayed particle, especially at the
         kinematic boundaries of the maximum beam energy. It is defined as
 
@@ -67,55 +70,74 @@
             \cdot \exp\left[ c \cdot \left(1 - \left(\frac{m}{m_0}\right)^2 \right) \right]
 
         and normalized to one over the `norm_range` (which defaults to `obs`).
 
         The implementation follows the `RooFit version <https://root.cern.ch/doc/master/classRooArgusBG.html>`_
 
         Args:
-            obs: Observable the PDF is defined on
+            obs: |@doc:pdf.init.obs| Observables of the
+               model. This will be used as the default space of the PDF and,
+               if not given explicitly, as the normalization range.
+
+               The default space is used for example in the sample method: if no
+               sampling limits are given, the default space is used.
+
+               The observables are not equal to the domain as it does not restrict or
+               truncate the model outside this range. |@docend:pdf.init.obs|
             m0: Maximal energetically allowed mass, cutoff
             c: Shape parameter; "peakiness" of the distribution
             p: Generalization of the ARGUS shape, for p = 0.5, the normal ARGUS shape is recovered
+            extended: |@doc:pdf.init.extended| The overall yield of the PDF.
+               If this is parameter-like, it will be used as the yield,
+               the expected number of events, and the PDF will be extended.
+               An extended PDF has additional functionality, such as the
+               ``ext_*`` methods and the ``counts`` (for binned PDFs). |@docend:pdf.init.extended|
+            norm: |@doc:pdf.init.norm| Normalization of the PDF.
+               By default, this is the same as the default space of the PDF. |@docend:pdf.init.norm|
+            name: |@doc:pdf.init.name| Human-readable name
+               or label of
+               the PDF for better identification. |@docend:pdf.init.name|
+           label: |@doc:pdf.init.label| Label of the PDF, if None is given, it will be the name. |@docend:pdf.init.label|
 
         Returns:
             `tf.Tensor`: the values matching the (broadcasted) shapes of the input
         """
         params = {"m0": m0, "c": c, "p": p}
-        super().__init__(obs=obs, name=name, params=params, extended=extended)
+        super().__init__(obs=obs, name=name, params=params, extended=extended, norm=norm, label=label)
 
     _N_OBS = 1
 
-    def _unnormalized_pdf(self, x):
+    @zfit.supports()
+    def _unnormalized_pdf(self, x, params):
         """
         Calculation of ARGUS PDF value
         (Docs: https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.argus.html)
         """
-        m = zfit.z.unstack_x(x)
+        m = x[0]
 
-        m0 = self.params["m0"]
-        c = self.params["c"]
-        p = self.params["p"]
+        m0 = params["m0"]
+        c = params["c"]
+        p = params["p"]
         return argus_func(m, m0, c, p)
 
 
 # Keep? move to math?
 # @z.function_tf
 def uppergamma(s, x):
     return tf.math.igammac(s, x=x) * z.exp(tf.math.lgamma(x))
 
 
 @z.function(wraps="tensor")
 def argus_cdf_p_half_nonpositive(lim, c, m0):
     lim = tf.clip_by_value(lim, 0.0, m0)
-    cdf = tf.cond(
+    return tf.cond(
         tf.math.less(c, 0.0),
         lambda: argus_cdf_p_half_c_neg(lim=lim, c=c, m0=m0),
         lambda: argus_cdf_p_half_c_zero(lim=lim, c=c, m0=m0),
     )
-    return cdf
 
 
 # Does not work, why?
 # # @z.function_tf
 # def argus_cdf_p_half_sympy(lim, c, m0):
 #     # lim = tf.where(tf.less_equal(lim, m0), lim, m0)  # take the smaller one, only integrate up to m0
 #     # lim = tf.where(tf.greater(lim, 0.), lim, z.constant(0.))  # start from 0 as minimum
@@ -135,16 +157,15 @@
     return cdf
 
 
 @z.function(wraps="tensor")
 def argus_cdf_p_half_c_zero(lim, c, m0):
     del c
     f1 = 1 - z.square(lim / m0)
-    cdf = -z.square(m0) / 3.0 * f1 * z.sqrt(f1)
-    return cdf
+    return -z.square(m0) / 3.0 * f1 * z.sqrt(f1)
 
 
 # TODO: add Faddeev function approximation
 # def argus_cdf_p_half_c_pos(lim, c, m0):
 #     f1 = 1 - z.square(lim)
 #     cdf = 0.5 * z.square(m0) * z.exp(c * f1) / (c * z.sqrt(c))
 #     # cdf *= (0.5 * z.sqrt(z.pi) * (RooMath::faddeeva(sqrt(c * f1))).imag() - z.sqrt(c * f1))
@@ -153,27 +174,27 @@
 
 @z.function(wraps="tensor")
 def argus_integral_p_half_func(lower, upper, c, m0):
     return argus_cdf_p_half_nonpositive(upper, c=c, m0=m0) - argus_cdf_p_half_nonpositive(lower, c=c, m0=m0)
 
 
 def argus_integral_p_half(limits, params, model):
+    del model
     p = params["p"]
     if not isinstance(p, zfit.param.ConstantParameter) or not np.isclose(p.static_value, 0.5):
         raise zfit.exception.AnalyticIntegralNotImplementedError()
     c = params["c"]
     if not isinstance(c, zfit.param.ConstantParameter) or c.static_value > 0:
         raise zfit.exception.AnalyticIntegralNotImplementedError()
 
     m0 = params["m0"]
     lower, upper = limits.limit1d
     lower = z.convert_to_tensor(lower)
     upper = z.convert_to_tensor(upper)
-    integral = argus_integral_p_half_func(lower=lower, upper=upper, c=c, m0=m0)
-    return integral
+    return argus_integral_p_half_func(lower=lower, upper=upper, c=c, m0=m0)
 
 
 argus_integral_limits = zfit.Space(axes=(0,), limits=(zfit.Space.ANY_LOWER, zfit.Space.ANY_UPPER))
 Argus.register_analytic_integral(func=argus_integral_p_half, limits=argus_integral_limits)
 
 if __name__ == "__main__":
     # create the integral
@@ -207,14 +228,12 @@
     # global_assumptions.add(sp.Q.integer(p))
     global_assumptions.add(sp.Q.finite(c))
     global_assumptions.add(sp.Q.positive(c))
     m_factor = 1 - (m / m0) ** 2
     integral_expression = m * m_factor**p * (sp.exp(c * m_factor))
     # integral_expression = (N * m * (1 - (m / m0) ** 2) ** p * sp.exp(c * (1 - (m / m0) ** 2)))
     integral = sp.integrate(integral_expression, m)
-    print(integral)
     func1 = sp.lambdify(integral.free_symbols, integral, "tensorflow")
     import inspect
 
     source = inspect.getsource(func1)
-    print(source)
     # sp.lambdify()
```

### Comparing `zfit_physics-0.6.1/zfit_physics/models/pdf_conv.py` & `zfit_physics-0.7.0/zfit_physics/models/pdf_conv.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from __future__ import annotations
 
 import tensorflow as tf
 import tensorflow_probability as tfp
 import zfit
 import zfit.models.functor
 from zfit import z
 from zfit.exception import FunctionNotImplementedError
@@ -15,37 +15,57 @@
         self,
         func: zfit.pdf.BasePDF,
         kernel: zfit.pdf.BasePDF,
         limits: ztyping.ObsTypeInput,
         obs: ztyping.ObsTypeInput,
         ndraws: int = 20000,
         *,
-        extended: Optional[ztyping.ParamTypeInput] = None,
+        extended: ztyping.ParamTypeInput | None = None,
+        norm: ztyping.NormTypeInput = None,
         name: str = "Convolution",
+        label: str | None = None,
         experimental_pdf_normalized=False,
     ):
         """Numerical Convolution pdf of *func* convoluted with *kernel*.
 
         Args:
             func (:py:class:`zfit.pdf.BasePDF`): PDF  with `pdf` method that takes x and returns the function value.
                 Here x is a `Data` with the obs and limits of *limits*.
             kernel (:py:class:`zfit.pdf.BasePDF`): PDF with `pdf` method that takes x acting as the kernel.
                 Here x is a `Data` with the obs and limits of *limits*.
             limits (:py:class:`zfit.Space`): Limits for the numerical integration.
-            obs (:py:class:`zfit.Space`): Observables of the class
-            extended: If the PDF should be extended, i.e. a yield.
-            ndraws (int): Number of draws for the mc integration
-            name (str): Human readable name of the pdf
+            obs: |@doc:pdf.init.obs| Observables of the
+               model. This will be used as the default space of the PDF and,
+               if not given explicitly, as the normalization range.
+
+               The default space is used for example in the sample method: if no
+               sampling limits are given, the default space is used.
+
+               The observables are not equal to the domain as it does not restrict or
+               truncate the model outside this range. |@docend:pdf.init.obs|
+            extended: |@doc:pdf.init.extended| The overall yield of the PDF.
+               If this is parameter-like, it will be used as the yield,
+               the expected number of events, and the PDF will be extended.
+               An extended PDF has additional functionality, such as the
+               ``ext_*`` methods and the ``counts`` (for binned PDFs). |@docend:pdf.init.extended|
+            norm: |@doc:pdf.init.norm| Normalization of the PDF.
+               By default, this is the same as the default space of the PDF. |@docend:pdf.init.norm|
+            name: |@doc:pdf.init.name| Human-readable name
+               or label of
+               the PDF for better identification. |@docend:pdf.init.name|
+           label: |@doc:pdf.init.label| Label of the PDF, if None is given, it will be the name. |@docend:pdf.init.label|
         """
-        super().__init__(obs=obs, pdfs=[func, kernel], params={}, name=name, extended=extended)
+        super().__init__(obs=obs, pdfs=[func, kernel], params={}, name=name, extended=extended, norm=norm, label=label)
         limits = self._check_input_limits(limits=limits)
         if limits.n_limits == 0:
-            raise exception.LimitsNotSpecifiedError("obs have to have limits to define where to integrate over.")
+            msg = "obs have to have limits to define where to integrate over."
+            raise exception.LimitsNotSpecifiedError(msg)
         if limits.n_limits > 1:
-            raise WorkInProgressError("Multiple Limits not implemented")
+            msg = "Multiple Limits not implemented"
+            raise WorkInProgressError(msg)
 
         #        if not isinstance(func, zfit.pdf.BasePDF):
         #            raise TypeError(f"func has to be a PDF, not {type(func)}")
         #        if isinstance(kernel, zfit.pdf.BasePDF):
         #            raise TypeError(f"kernel has to be a PDF, not {type(kernel)}")
 
         # func = lambda x: func.unnormalized_pdf(x=x)
@@ -78,15 +98,16 @@
         return tf.map_fn(
             lambda xi: area * tf.reduce_mean(func_values * self.pdfs[1].pdf(xi - samples.value(), norm=False)),
             x.value(),
         )
 
     @zfit.supports(norm=True)
     @z.function
-    def _pdf(self, x, norm_range):
+    def _pdf(self, x, norm):
+        del norm
         if not self._experimental_pdf_normalized:
             raise FunctionNotImplementedError
 
         limits = self.conv_limits
         # area = limits.area()  # new spaces
         area = limits.rect_area()[0]  # new spaces
```

### Comparing `zfit_physics-0.6.1/zfit_physics/models/pdf_kde.py` & `zfit_physics-0.7.0/zfit_physics/models/pdf_kde.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 from collections import OrderedDict
-from typing import Optional
 
 import tensorflow as tf
 import tensorflow_probability.python.distributions as tfd
 import zfit
 from zfit import z
 from zfit.models.dist_tfp import WrapDistribution
 from zfit.util import ztyping
@@ -13,75 +14,96 @@
 
 class GaussianKDE(WrapDistribution):  # multidimensional kde with gaussian kernel
     def __init__(
         self,
         data: tf.Tensor,
         bandwidth: ztyping.ParamTypeInput,
         obs: ztyping.ObsTypeInput,
-        name: str = "GaussianKDE",
         *,
-        extended: Optional[ztyping.ParamTypeInput] = None,
+        extended: ztyping.ParamTypeInput | None = None,
+        norm: ztyping.NormTypeInput = None,
+        name: str = "GaussianKDE",
+        label: str | None = None,
     ):
         """Gaussian Kernel Density Estimation using Silverman's rule of thumb.
 
         Args:
             data: Data points to build a kernel around
             bandwidth: sigmas for the covariance matrix of the multivariate gaussian
-            obs:
-            name: Name of the PDF
+            obs: |@doc:pdf.init.obs| Observables of the
+               model. This will be used as the default space of the PDF and,
+               if not given explicitly, as the normalization range.
+
+               The default space is used for example in the sample method: if no
+               sampling limits are given, the default space is used.
+
+               The observables are not equal to the domain as it does not restrict or
+               truncate the model outside this range. |@docend:pdf.init.obs|
+            extended: |@doc:pdf.init.extended| The overall yield of the PDF.
+               If this is parameter-like, it will be used as the yield,
+               the expected number of events, and the PDF will be extended.
+               An extended PDF has additional functionality, such as the
+               ``ext_*`` methods and the ``counts`` (for binned PDFs). |@docend:pdf.init.extended|
+            norm: |@doc:pdf.init.norm| Normalization of the PDF.
+               By default, this is the same as the default space of the PDF. |@docend:pdf.init.norm|
+            name: |@doc:pdf.init.name| Human-readable name
+               or label of
+               the PDF for better identification. |@docend:pdf.init.name|
+           label: |@doc:pdf.init.label| Label of the PDF, if None is given, it will be the name. |@docend:pdf.init.label|
         """
         dtype = zfit.settings.ztypes.float
         if isinstance(data, zfit.core.interfaces.ZfitData):
-            raise WorkInProgressError("Currently, no dataset supported yet")
+            msg = "Currently, no dataset supported yet"
+            raise WorkInProgressError(msg)
             # size = data.nevents
             # dims = data.n_obs
             # with data.
             # data = data.value()
             # if data.weights is not None:
 
-        else:
-            if not isinstance(data, tf.Tensor):
-                data = z.convert_to_tensor(value=data)
-            data = z.to_real(data)
-
-            shape_data = tf.shape(data)
-            size = tf.cast(shape_data[0], dtype=dtype)
-            dims = tf.cast(shape_data[-1], dtype=dtype)
+        if not isinstance(data, tf.Tensor):
+            data = z.convert_to_tensor(value=data)
+        data = z.to_real(data)
+
+        shape_data = tf.shape(data)
+        size = tf.cast(shape_data[0], dtype=dtype)
+        dims = tf.cast(shape_data[-1], dtype=dtype)
         bandwidth = convert_to_container(bandwidth)
 
         # Bandwidth definition, use silverman's rule of thumb for nd
         def reshaped_kerner_factory():
             cov_diag = [
                 tf.square((4.0 / (dims + 2.0)) ** (1 / (dims + 4)) * size ** (-1 / (dims + 4)) * s) for s in bandwidth
             ]
             # cov = tf.linalg.diag(cov_diag)
             # kernel prob output shape: (n,)
             # kernel = tfd.MultivariateNormalFullCovariance(loc=data, covariance_matrix=cov)
-            kernel = tfd.MultivariateNormalDiag(loc=data, scale_diag=cov_diag)
+            return tfd.MultivariateNormalDiag(loc=data, scale_diag=cov_diag)
 
-            return kernel
             # return tfd.Independent(kernel)
 
         # reshaped_kernel = kernel
 
         probs = tf.broadcast_to(1 / size, shape=(tf.cast(size, tf.int32),))
         categorical = tfd.Categorical(probs=probs)  # no grad -> no need to recreate
-        dist_kwargs = lambda: dict(
-            mixture_distribution=categorical,
-            components_distribution=reshaped_kerner_factory(),
-        )
+
+        def dist_kwargs():
+            return {"mixture_distribution": categorical, "components_distribution": reshaped_kerner_factory()}
+
         distribution = tfd.MixtureSameFamily
         # TODO lambda for params
         params = OrderedDict((f"bandwidth_{i}", h) for i, h in enumerate(bandwidth))
         super().__init__(
             distribution=distribution,
             dist_params={},
             dist_kwargs=dist_kwargs,
             params=params,
             obs=obs,
             name=name,
             extended=extended,
+            norm=norm,
+            label=label,
         )
 
     # @zfit.supports()
     # def _analytic_integrate(self, limits, norm_range):
     #     raise AnalyticIntegralNotImplementedError
```

### Comparing `zfit_physics-0.6.1/zfit_physics.egg-info/SOURCES.txt` & `zfit_physics-0.7.0/zfit_physics.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .all-contributorsrc
-.codeclimate.yml
 .git_archival.txt
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
-.scrutinizer.yml
+.readthedocs.yaml
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements.txt
 requirements_dev.txt
@@ -25,38 +24,57 @@
 .github/ISSUE_TEMPLATE/zfit-usage-question.md
 .github/workflows/cd.yml
 .github/workflows/ci.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make_docs.sh
+docs/_static/css/custom.css
+docs/api/static/zfit_physics.pdf.rst
 docs/api/tools/change_headline.py
 docs/images/scikit-hep-logo_168x168.png
+docs/images/zfit-favicon.png
 docs/images/zfit-fin_400x168.png
 docs/images/zfit-fin_57x24.png
+docs/images/zfit-logo-light_400x168.png
+docs/images/zfit-logo_400x168.png
+docs/images/zfit-logo_57x24.png
+docs/images/zfit-logo_hires.png
+docs/images/zfit-logo_veryhires.png
+docs/images/zfit-vector.svg
 docs/images/zfit_workflow_v1.png
+docs/images/zfit_workflow_v2.png
 tests/__init__.py
 tests/conftest.py
 tests/test_pdf_argus.py
+tests/test_pdf_cmsshape.py
 tests/test_pdf_conv.py
+tests/test_pdf_cruijff.py
+tests/test_pdf_erfexp.py
 tests/test_pdf_example.py
 tests/test_pdf_kde.py
+tests/test_pdf_novosibirsk.py
 tests/test_pdf_relbw.py
+tests/test_pdf_tsallis.py
 utils/ci/test_examples.sh
 utils/ci/testbuild_docs.sh
 zfit_physics/__init__.py
 zfit_physics/pdf.py
-zfit_physics/plot.py
 zfit_physics.egg-info/PKG-INFO
 zfit_physics.egg-info/SOURCES.txt
 zfit_physics.egg-info/dependency_links.txt
 zfit_physics.egg-info/not-zip-safe
 zfit_physics.egg-info/requires.txt
 zfit_physics.egg-info/top_level.txt
 zfit_physics/models/__init__.py
 zfit_physics/models/pdf_argus.py
+zfit_physics/models/pdf_cmsshape.py
 zfit_physics/models/pdf_conv.py
+zfit_physics/models/pdf_cruijff.py
+zfit_physics/models/pdf_erfexp.py
 zfit_physics/models/pdf_example.py
 zfit_physics/models/pdf_kde.py
+zfit_physics/models/pdf_novosibirsk.py
 zfit_physics/models/pdf_relbw.py
+zfit_physics/models/pdf_tsallis.py
 zfit_physics/unstable/__init__.py
 zfit_physics/unstable/pdf.py
```

