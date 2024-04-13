# Comparing `tmp/djangocms-frontend-1.3.0.tar.gz` & `tmp/djangocms_frontend-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-frontend-1.3.0.tar", last modified: Thu Mar 21 15:40:49 2024, max compression
+gzip compressed data, was "djangocms_frontend-1.3.1.tar", last modified: Sat Apr 13 13:34:20 2024, max compression
```

## Comparing `djangocms-frontend-1.3.0.tar` & `djangocms_frontend-1.3.1.tar`

### file list

```diff
@@ -1,682 +1,690 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.604814 djangocms-frontend-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-03-21 15:40:49.604814 djangocms-frontend-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.512813 djangocms-frontend-1.3.0/djangocms_frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/background.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/common/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/bootstrap5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/bootstrap5/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/bootstrap5/responsive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/bootstrap5/sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/responsive.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/sizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/spacing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/common/title.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.488813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.488813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.488813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.488813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.516813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.488813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.520814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.524814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.528814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.528814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.528814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.528814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.528814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.528814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.528814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.528814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.532814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.492813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.532814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.532814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.532814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.532814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.532814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.548814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    59572 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   277297 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    63664 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   123564 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   516494 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)   123376 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   123452 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    89988 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    76736 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   101648 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    78268 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)   150535 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)    56976 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    32020 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)    28196 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
--rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
--rw-r--r--   0 runner    (1001) docker     (127)    54789 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28028 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    14984 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   729984 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
--rw-r--r--   0 runner    (1001) docker     (127)  2883039 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)   729800 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   386256 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)   282928 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    99774 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   184969 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99564 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44720 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.556814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
--rw-r--r--   0 runner    (1001) docker     (127)    48146 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)    30533 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    48978 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
--rw-r--r--   0 runner    (1001) docker     (127)    35481 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    18498 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    30092 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
--rw-r--r--   0 runner    (1001) docker     (127)    23027 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    24992 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
--rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
--rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)    21372 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
--rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.556814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.556814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    21397 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.556814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.560814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    15830 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   137737 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)   115209 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    20997 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    77647 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    65062 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    32569 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (127)    26765 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.560814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/icon/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/icon/ckeditor.icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.560814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.560814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.560814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.560814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.560814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.560814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/image_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.496813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.564814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.568814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.572814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.572814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.500813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.572814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.572814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.572814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.572814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.572814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.572814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.576814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.576814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.576814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.576814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.576814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.576814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.576814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.576814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.508813 djangocms-frontend-1.3.0/djangocms_frontend/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    37745 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    44784 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    34087 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.504813 djangocms-frontend-1.3.0/djangocms_frontend/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    27932 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    45014 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.508813 djangocms-frontend-1.3.0/djangocms_frontend/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.580814 djangocms-frontend-1.3.0/djangocms_frontend/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    29475 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    46279 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.508813 djangocms-frontend-1.3.0/djangocms_frontend/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.584814 djangocms-frontend-1.3.0/djangocms_frontend/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    38302 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.508813 djangocms-frontend-1.3.0/djangocms_frontend/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.584814 djangocms-frontend-1.3.0/djangocms_frontend/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    43934 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.584814 djangocms-frontend-1.3.0/djangocms_frontend/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17985 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/bootstrap4_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.584814 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.584814 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/stale_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/sync_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/icon_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/management/styled_link_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.584814 djangocms-frontend-1.3.0/djangocms_frontend/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.508813 djangocms-frontend-1.3.0/djangocms_frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.508813 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/
--rw-r--r--   0 runner    (1001) docker     (127)    79431 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/base.css
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/button_group.css
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/div_select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
--rw-r--r--   0 runner    (1001) docker     (127)    95562 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/templates/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/bootstrap5/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/bootstrap5/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/bootstrap5/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/deprecated.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/html_container.html
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.588814 djangocms-frontend-1.3.0/djangocms_frontend/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/djangocms_frontend/templatetags/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.600814 djangocms-frontend-1.3.0/djangocms_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-03-21 15:40:49.000000 djangocms-frontend-1.3.0/djangocms_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31296 2024-03-21 15:40:49.000000 djangocms-frontend-1.3.0/djangocms_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 15:40:49.000000 djangocms-frontend-1.3.0/djangocms_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 15:40:49.000000 djangocms-frontend-1.3.0/djangocms_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-21 15:40:49.000000 djangocms-frontend-1.3.0/djangocms_frontend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-21 15:40:49.000000 djangocms-frontend-1.3.0/djangocms_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-21 15:40:49.604814 djangocms-frontend-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.592814 djangocms-frontend-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.592814 djangocms-frontend-1.3.0/tests/accordion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/accordion/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/accordion/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.592814 djangocms-frontend-1.3.0/tests/alert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/alert/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/alert/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.592814 djangocms-frontend-1.3.0/tests/badge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/badge/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/badge/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.592814 djangocms-frontend-1.3.0/tests/card/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/card/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/card/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.596814 djangocms-frontend-1.3.0/tests/carousel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/carousel/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/carousel/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.596814 djangocms-frontend-1.3.0/tests/collapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/collapse/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/collapse/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.596814 djangocms-frontend-1.3.0/tests/content/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/content/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/content/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.596814 djangocms-frontend-1.3.0/tests/grid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/grid/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/grid/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.596814 djangocms-frontend-1.3.0/tests/icon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/icon/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/icon/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.596814 djangocms-frontend-1.3.0/tests/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/image/test_drag_n_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/image/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/image/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.596814 djangocms-frontend-1.3.0/tests/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/jumbotron/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/jumbotron/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.600814 djangocms-frontend-1.3.0/tests/link/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/link/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/link/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/link/test_urlconf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.600814 djangocms-frontend-1.3.0/tests/listgroup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/listgroup/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/listgroup/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.600814 djangocms-frontend-1.3.0/tests/media/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/media/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/media/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.600814 djangocms-frontend-1.3.0/tests/navigation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/navigation/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/navigation/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.600814 djangocms-frontend-1.3.0/tests/tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/tabs/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/tabs/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:49.600814 djangocms-frontend-1.3.0/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/utilities/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-21 15:40:45.000000 djangocms-frontend-1.3.0/tests/utilities/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.456842 djangocms_frontend-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-13 13:34:20.456842 djangocms_frontend-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.360842 djangocms_frontend-1.3.1/djangocms_frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.360842 djangocms_frontend-1.3.1/djangocms_frontend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/background.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/common/title.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.364842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.332842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.368842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.372842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.336842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.376842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.380842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.384842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.384842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.400842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    59572 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   277297 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    63664 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   123564 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   516494 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   123376 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   123452 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    89988 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76736 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   101648 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    78268 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   150535 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    56976 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    32020 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    28196 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
+-rw-r--r--   0 runner    (1001) docker     (127)    54789 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28028 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    14984 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   729984 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (127)  2883039 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   729800 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   386256 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   282928 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    99774 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   184969 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99564 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    56468 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44720 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.408841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)    48146 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30533 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10004 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    48978 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35481 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6934 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18498 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30092 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23027 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24992 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24997 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35227 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21372 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.408841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.412842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    21397 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.412842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    28165 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15830 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   137737 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)   115209 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20997 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18213 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    77647 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    65062 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    32569 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (127)    26765 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_text_ckeditor/ckeditor/icon/ckeditor.icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.340842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9287 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/image_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.416842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14745 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.344842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.420842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.424842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.428841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.348842 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    37745 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.432841 djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    28135 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    44784 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    34087 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    27932 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    45014 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    29475 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    46279 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19546 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    41787 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    34140 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    14324 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    38302 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    24556 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    43934 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17985 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/bootstrap4_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.436842 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/stale_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/sync_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/icon_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/management/styled_link_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.352842 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    79431 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/div_select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95562 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.440842 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/deprecated.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/html_container.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/djangocms_frontend/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/djangocms_frontend/templatetags/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-13 13:34:20.000000 djangocms_frontend-1.3.1/djangocms_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-13 13:34:20.456842 djangocms_frontend-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/tests/accordion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/accordion/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/accordion/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.444841 djangocms_frontend-1.3.1/tests/alert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/alert/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/alert/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/badge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/badge/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/badge/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/card/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/card/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/card/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/carousel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/carousel/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/carousel/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/collapse/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/collapse/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/content/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/content/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/content/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/grid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/grid/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/grid/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/icon/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/icon/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/image/test_drag_n_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/image/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/image/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.448841 djangocms_frontend-1.3.1/tests/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/jumbotron/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/jumbotron/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/link/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/link/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6382 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/link/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/link/test_urlconf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/listgroup/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/listgroup/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/media/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/media/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/media/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/navigation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/navigation/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/navigation/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/tabs/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/tabs/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:20.452841 djangocms_frontend-1.3.1/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/utilities/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-13 13:34:14.000000 djangocms_frontend-1.3.1/tests/utilities/test_plugins.py
```

### Comparing `djangocms-frontend-1.3.0/LICENSE` & `djangocms_frontend-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/PKG-INFO` & `djangocms_frontend-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.3.0
+Version: 1.3.1
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -44,27 +44,28 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django>=2.2
 Requires-Dist: django-cms>=3.7
 Requires-Dist: django-filer>=1.7
 Requires-Dist: easy-thumbnails
 Requires-Dist: djangocms-attributes-field>=1
-Requires-Dist: djangocms-text-ckeditor>=3.1.0
 Requires-Dist: django-entangled>=0.5.4
 Provides-Extra: djangocms-icon
 Requires-Dist: djangocms-icon>=1.4.0; extra == "djangocms-icon"
 Provides-Extra: static-ace
 Requires-Dist: djangocms-static-ace; extra == "static-ace"
 Provides-Extra: cms-4
 Requires-Dist: django-cms>=4.1.0; extra == "cms-4"
 Requires-Dist: django-parler; extra == "cms-4"
 Requires-Dist: djangocms-versioning>=2.0.0; extra == "cms-4"
 Requires-Dist: djangocms-alias>=2.0.0; extra == "cms-4"
+Requires-Dist: djangocms-text; extra == "cms-4"
 Provides-Extra: cms-3
 Requires-Dist: django-cms<4; extra == "cms-3"
+Requires-Dist: djangocms-text-ckeditor>=3.1.0; extra == "cms-3"
 Requires-Dist: django-parler; extra == "cms-3"
 
 #####################
  django CMS Frontend
 #####################
 
 |pypi| |docs| |coverage| |python| |django| |djangocms| |djangocms4|
```

### Comparing `djangocms-frontend-1.3.0/README.rst` & `djangocms_frontend-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/__init__.py` & `djangocms_frontend-1.3.1/djangocms_frontend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
  9. git push
 10. Assure that all tests pass on https://github.com/django-cms/djangocms-frontend/actions
 11. Create a new release on https://github.com/django-cms/djangocms-frontend/releases/new
 12. Publish the release when ready
 13. Github actions will publish the new package to pypi
 """
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
```

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/common/attributes.py` & `djangocms_frontend-1.3.1/djangocms_frontend/common/attributes.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/common/bootstrap5/background.py` & `djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/background.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/common/bootstrap5/responsive.py` & `djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/responsive.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/common/bootstrap5/sizing.py` & `djangocms_frontend-1.3.1/djangocms_frontend/common/bootstrap5/sizing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/common/spacing.py` & `djangocms_frontend-1.3.1/djangocms_frontend/common/spacing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/common/title.py` & `djangocms_frontend-1.3.1/djangocms_frontend/common/title.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/badge/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/badge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/constants.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/frameworks/foundation6.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/constants.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/collapse/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/collapse/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/constants.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/frameworks/foundation6.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/conf.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/conf.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/fields.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/icon/templatetags/icon_tags.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/icon/templatetags/icon_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/image_save.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/image_save.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/constants.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/helpers.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/link/views.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/link/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/listgroup/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/listgroup/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy as _
 
 from ...models import FrontendUIItem
 
 
 class ListGroup(FrontendUIItem):
     """
     Components > "List Group" Plugin
```

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/media/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/media/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy as _
 
 from djangocms_frontend.models import FrontendUIItem
 
 
 class Media(FrontendUIItem):
     """
     Layout > "Media" Plugin
```

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/constants.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy as _
 
 from ...models import FrontendUIItem
 
 
 class Tab(FrontendUIItem):
     class Meta:
         proxy = True
```

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/cms_plugins.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/forms.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.utils.translation import gettext as _
+from django.utils.translation import gettext_lazy as _
 
 from ...models import FrontendUIItem
 
 
 class Spacing(FrontendUIItem):
     """
     Utilities > "Spacing" Plugin
```

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html` & `djangocms_frontend-1.3.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/fields.py` & `djangocms_frontend-1.3.1/djangocms_frontend/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/frameworks/bootstrap5.py` & `djangocms_frontend-1.3.1/djangocms_frontend/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/helpers.py` & `djangocms_frontend-1.3.1/djangocms_frontend/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/ar/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/de/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/de/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/en/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/es/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/es/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/fr/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/nl/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/locale/sq/LC_MESSAGES/django.po` & `djangocms_frontend-1.3.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/bootstrap4_migration.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/bootstrap4_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/commands/frontend.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/base.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/frequency_analysis.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/migrate.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/migrate.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/stale_references.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/stale_references.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/commands/subcommands/sync_permissions.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/commands/subcommands/sync_permissions.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/icon_migration.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/icon_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/management/styled_link_migration.py` & `djangocms_frontend-1.3.1/djangocms_frontend/management/styled_link_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/migrations/0001_initial.py` & `djangocms_frontend-1.3.1/djangocms_frontend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/models.py` & `djangocms_frontend-1.3.1/djangocms_frontend/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from cms.models import CMSPlugin
 from cms.utils.compat import DJANGO_3_0
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
 from django.utils.html import conditional_escape, mark_safe
 from django.utils.translation import gettext
+from django.utils.translation import gettext_lazy as _
 
 from djangocms_frontend.fields import TagTypeField
 from djangocms_frontend.settings import FRAMEWORK_PLUGIN_INFO
 
 if DJANGO_3_0:
     from django_jsonfield_backport.models import JSONField
 else:
@@ -39,15 +40,15 @@
         - framework_info: Returns the framework information for the UI item.
 
     Note: This is an abstract base class and should not be used directly.
     """
 
     class Meta:
         abstract = True
-        verbose_name = gettext("UI item")
+        verbose_name = _("UI item")
 
     ui_item = models.CharField(max_length=30)
     tag_type = TagTypeField(blank=True)
     config = JSONField(default=dict, encoder=DjangoJSONEncoder)
 
     def __init__(self, *args, **kwargs):
         self._additional_classes = []
@@ -137,8 +138,8 @@
     - verbose_name (str): The verbose name of the UI item.
 
     Methods:
     None
 
     """
     class Meta:
-        verbose_name = gettext("UI item")
+        verbose_name = _("UI item")
```

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/settings.py` & `djangocms_frontend-1.3.1/djangocms_frontend/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/base.css` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/base.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/base.css.map` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/base.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/button_group.css` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/auto_input.js` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/auto_input.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/static/djangocms_frontend/js/django_select2.js` & `djangocms_frontend-1.3.1/djangocms_frontend/static/djangocms_frontend/js/django_select2.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/bootstrap5/base.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/bootstrap5/menu.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/bootstrap5/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/deprecated.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/deprecated.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templates/djangocms_frontend.html` & `djangocms_frontend-1.3.1/djangocms_frontend/templates/djangocms_frontend.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 <!DOCTYPE html>{% load cms_tags menu_tags sekizai_tags static i18n %}{% spaceless %}
-    <html lang="{{ LANGUAGE_CODE }}">
+    {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
+    <html lang="{{ LANGUAGE_CODE|default:"en-us" }}" dir="{{ LANGUAGE_BIDI|yesno:'rtl,ltr,auto' }}">
         <head>
             <meta charset="utf-8"/>
             <meta http-equiv="X-UA-Compatible" content="IE=edge"/>
             <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no"/>
             {% block meta %}
                 <meta name="description" content="{% page_attribute meta_description %}"/>
                 <meta property="og:type" content="website"/>
@@ -11,15 +12,15 @@
                 <meta property="og:description" content="{% page_attribute meta_description %}"/>
             {% endblock meta %}
             {% block canonical_url %}
                 <link rel="canonical" href="{{ request.build_absolute_uri|urlencode:"&?" }}"/>
                 <meta property="og:url" content="{{ request.build_absolute_uri|urlencode:"&?" }}"/>
             {% endblock canonical_url %}
             {% block fb_meta %}{% endblock fb_meta %}
-            <title>{% block title %}{% page_attribute "page_title" %}{% endblock %}</title>
+            <title>{% block title %}{{ request.current_page.get_page_title|striptags }}{% endblock %}</title>
             {% block base_css %}{% endblock %}
 {% endspaceless %}{% render_block 'css' %}{% spaceless %}
     {% block page_head %}{% endblock %}
     </head>
     <body {% block body_attrs %}{% endblock %}>
 {% endspaceless %}{% cms_toolbar %}{% block navbar %}{% endblock %}
     {% block content %}
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
-{% load cms_tags menu_tags sekizai_tags static i18n %}{% spaceless %}
+{% load cms_tags menu_tags sekizai_tags static i18n %}{% spaceless %} {%
+get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as
+LANGUAGE_BIDI %}
+}" dir="{{ LANGUAGE_BIDI|yesno:'rtl,ltr,auto' }}">
 {% block meta %}
 }"/>
 {% endblock meta %} {% block canonical_url %}
 ?" }}"/>
 ?" }}"/> {% endblock canonical_url %} {% block fb_meta %}{% endblock fb_meta %}
 {% block base_css %}{% endblock %} {% endspaceless %}{% render_block 'css' %}{%
 spaceless %} {% block page_head %}{% endblock %}
```

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend/templatetags/frontend.py` & `djangocms_frontend-1.3.1/djangocms_frontend/templatetags/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend.egg-info/PKG-INFO` & `djangocms_frontend-1.3.1/djangocms_frontend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.3.0
+Version: 1.3.1
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -44,27 +44,28 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Django>=2.2
 Requires-Dist: django-cms>=3.7
 Requires-Dist: django-filer>=1.7
 Requires-Dist: easy-thumbnails
 Requires-Dist: djangocms-attributes-field>=1
-Requires-Dist: djangocms-text-ckeditor>=3.1.0
 Requires-Dist: django-entangled>=0.5.4
 Provides-Extra: djangocms-icon
 Requires-Dist: djangocms-icon>=1.4.0; extra == "djangocms-icon"
 Provides-Extra: static-ace
 Requires-Dist: djangocms-static-ace; extra == "static-ace"
 Provides-Extra: cms-4
 Requires-Dist: django-cms>=4.1.0; extra == "cms-4"
 Requires-Dist: django-parler; extra == "cms-4"
 Requires-Dist: djangocms-versioning>=2.0.0; extra == "cms-4"
 Requires-Dist: djangocms-alias>=2.0.0; extra == "cms-4"
+Requires-Dist: djangocms-text; extra == "cms-4"
 Provides-Extra: cms-3
 Requires-Dist: django-cms<4; extra == "cms-3"
+Requires-Dist: djangocms-text-ckeditor>=3.1.0; extra == "cms-3"
 Requires-Dist: django-parler; extra == "cms-3"
 
 #####################
  django CMS Frontend
 #####################
 
 |pypi| |docs| |coverage| |python| |django| |djangocms| |djangocms4|
```

### Comparing `djangocms-frontend-1.3.0/djangocms_frontend.egg-info/SOURCES.txt` & `djangocms_frontend-1.3.1/djangocms_frontend.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -360,14 +360,18 @@
 djangocms_frontend/locale/de/LC_MESSAGES/django.po
 djangocms_frontend/locale/en/LC_MESSAGES/django.mo
 djangocms_frontend/locale/en/LC_MESSAGES/django.po
 djangocms_frontend/locale/es/LC_MESSAGES/django.mo
 djangocms_frontend/locale/es/LC_MESSAGES/django.po
 djangocms_frontend/locale/fr/LC_MESSAGES/django.mo
 djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+djangocms_frontend/locale/hr/LC_MESSAGES/django.mo
+djangocms_frontend/locale/hr/LC_MESSAGES/django.po
+djangocms_frontend/locale/it/LC_MESSAGES/django.mo
+djangocms_frontend/locale/it/LC_MESSAGES/django.po
 djangocms_frontend/locale/nl/LC_MESSAGES/django.mo
 djangocms_frontend/locale/nl/LC_MESSAGES/django.po
 djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
 djangocms_frontend/locale/sq/LC_MESSAGES/django.po
 djangocms_frontend/management/__init__.py
 djangocms_frontend/management/bootstrap4_migration.py
 djangocms_frontend/management/icon_migration.py
```

### Comparing `djangocms-frontend-1.3.0/pyproject.toml` & `djangocms_frontend-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/setup.py` & `djangocms_frontend-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 REQUIREMENTS = [
     "Django>=2.2",
     "django-cms>=3.7",
     "django-filer>=1.7",
     "easy-thumbnails",
     "djangocms-attributes-field>=1",
-    "djangocms-text-ckeditor>=3.1.0",
     "django-entangled>=0.5.4",
 ]
 
 EXTRA_REQUIREMENTS = {
     "djangocms-icon": [
         "djangocms-icon>=1.4.0",
     ],
@@ -21,17 +20,19 @@
         "djangocms-static-ace",
     ],
     "cms-4": [
         "django-cms>=4.1.0",
         "django-parler",
         "djangocms-versioning>=2.0.0",
         "djangocms-alias>=2.0.0",
+        "djangocms-text",
     ],
     "cms-3": [
         "django-cms<4",
+        "djangocms-text-ckeditor>=3.1.0",
         "django-parler",
     ],
 }
 
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
```

### Comparing `djangocms-frontend-1.3.0/tests/accordion/test_models.py` & `djangocms_frontend-1.3.1/tests/accordion/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/accordion/test_plugins.py` & `djangocms_frontend-1.3.1/tests/accordion/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/alert/test_plugins.py` & `djangocms_frontend-1.3.1/tests/alert/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/badge/test_plugins.py` & `djangocms_frontend-1.3.1/tests/badge/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/card/test_models.py` & `djangocms_frontend-1.3.1/tests/card/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/card/test_plugins.py` & `djangocms_frontend-1.3.1/tests/card/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/carousel/test_models.py` & `djangocms_frontend-1.3.1/tests/carousel/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/carousel/test_plugins.py` & `djangocms_frontend-1.3.1/tests/carousel/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/collapse/test_models.py` & `djangocms_frontend-1.3.1/tests/collapse/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/collapse/test_plugins.py` & `djangocms_frontend-1.3.1/tests/collapse/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/content/test_models.py` & `djangocms_frontend-1.3.1/tests/content/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/content/test_plugins.py` & `djangocms_frontend-1.3.1/tests/content/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/fixtures.py` & `djangocms_frontend-1.3.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/grid/test_models.py` & `djangocms_frontend-1.3.1/tests/grid/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/grid/test_plugins.py` & `djangocms_frontend-1.3.1/tests/grid/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/helpers.py` & `djangocms_frontend-1.3.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/icon/test_models.py` & `djangocms_frontend-1.3.1/tests/icon/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/icon/test_plugins.py` & `djangocms_frontend-1.3.1/tests/icon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/image/test_drag_n_drop.py` & `djangocms_frontend-1.3.1/tests/image/test_drag_n_drop.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/image/test_plugins.py` & `djangocms_frontend-1.3.1/tests/image/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/jumbotron/test_plugins.py` & `djangocms_frontend-1.3.1/tests/jumbotron/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/link/test_plugins.py` & `djangocms_frontend-1.3.1/tests/link/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/link/test_urlconf.py` & `djangocms_frontend-1.3.1/tests/link/test_urlconf.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/listgroup/test_models.py` & `djangocms_frontend-1.3.1/tests/listgroup/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/listgroup/test_plugins.py` & `djangocms_frontend-1.3.1/tests/listgroup/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/media/test_models.py` & `djangocms_frontend-1.3.1/tests/media/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/media/test_plugins.py` & `djangocms_frontend-1.3.1/tests/media/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/navigation/test_models.py` & `djangocms_frontend-1.3.1/tests/navigation/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/navigation/test_plugins.py` & `djangocms_frontend-1.3.1/tests/navigation/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/tabs/test_models.py` & `djangocms_frontend-1.3.1/tests/tabs/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/tabs/test_plugins.py` & `djangocms_frontend-1.3.1/tests/tabs/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/test_constants.py` & `djangocms_frontend-1.3.1/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/test_fields.py` & `djangocms_frontend-1.3.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/test_helpers.py` & `djangocms_frontend-1.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/test_migrations.py` & `djangocms_frontend-1.3.1/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/test_settings.py` & `djangocms_frontend-1.3.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/utilities/test_models.py` & `djangocms_frontend-1.3.1/tests/utilities/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.3.0/tests/utilities/test_plugins.py` & `djangocms_frontend-1.3.1/tests/utilities/test_plugins.py`

 * *Files identical despite different names*

