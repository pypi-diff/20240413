# Comparing `tmp/django-opensearch-dsl-0.6.0.tar.gz` & `tmp/django_opensearch_dsl-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-opensearch-dsl-0.6.0.tar", last modified: Fri Mar 22 10:07:30 2024, max compression
+gzip compressed data, was "django_opensearch_dsl-0.6.1.tar", last modified: Sat Apr 13 21:23:39 2024, max compression
```

## Comparing `django-opensearch-dsl-0.6.0.tar` & `django_opensearch_dsl-0.6.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 qcoumes    (501) staff       (20)        0 2024-03-22 10:07:30.788116 django-opensearch-dsl-0.6.0/
--rw-r--r--   0 qcoumes    (501) staff       (20)     3902 2024-03-22 06:46:36.000000 django-opensearch-dsl-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 qcoumes    (501) staff       (20)      579 2021-12-03 02:16:36.000000 django-opensearch-dsl-0.6.0/LICENSE
--rw-r--r--   0 qcoumes    (501) staff       (20)      173 2021-12-13 13:43:36.000000 django-opensearch-dsl-0.6.0/MANIFEST.in
--rw-r--r--   0 qcoumes    (501) staff       (20)    14420 2024-03-22 10:07:30.787675 django-opensearch-dsl-0.6.0/PKG-INFO
--rw-r--r--   0 qcoumes    (501) staff       (20)     5103 2024-03-22 06:46:36.000000 django-opensearch-dsl-0.6.0/README.md
-drwxr-xr-x   0 qcoumes    (501) staff       (20)        0 2024-03-22 10:07:30.776306 django-opensearch-dsl-0.6.0/django_opensearch_dsl/
--rw-r--r--   0 qcoumes    (501) staff       (20)      295 2024-03-22 09:15:40.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/__init__.py
--rw-r--r--   0 qcoumes    (501) staff       (20)     2630 2024-03-22 08:20:36.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/apps.py
--rw-r--r--   0 qcoumes    (501) staff       (20)     9237 2024-03-22 07:31:10.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/documents.py
--rw-r--r--   0 qcoumes    (501) staff       (20)      491 2022-06-22 00:15:17.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/exceptions.py
--rw-r--r--   0 qcoumes    (501) staff       (20)     8213 2024-03-22 06:46:36.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/fields.py
--rw-r--r--   0 qcoumes    (501) staff       (20)      783 2024-03-20 09:16:22.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/indices.py
-drwxr-xr-x   0 qcoumes    (501) staff       (20)        0 2024-03-22 10:07:30.780559 django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/
--rw-r--r--   0 qcoumes    (501) staff       (20)        0 2021-12-03 02:08:28.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/__init__.py
-drwxr-xr-x   0 qcoumes    (501) staff       (20)        0 2024-03-22 10:07:30.781955 django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/commands/
--rw-r--r--   0 qcoumes    (501) staff       (20)        0 2021-12-03 02:08:28.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/commands/__init__.py
--rw-r--r--   0 qcoumes    (501) staff       (20)    14826 2024-03-22 06:46:36.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/commands/opensearch.py
--rw-r--r--   0 qcoumes    (501) staff       (20)      674 2023-05-17 22:47:59.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/enums.py
--rw-r--r--   0 qcoumes    (501) staff       (20)     1939 2024-03-22 06:46:36.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/types.py
--rw-r--r--   0 qcoumes    (501) staff       (20)       56 2022-06-22 04:29:57.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/models.py
--rw-r--r--   0 qcoumes    (501) staff       (20)     7476 2024-03-22 06:46:36.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/registries.py
--rw-r--r--   0 qcoumes    (501) staff       (20)     1830 2024-03-22 06:46:36.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/search.py
--rw-r--r--   0 qcoumes    (501) staff       (20)     4063 2024-03-22 06:46:36.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl/signals.py
-drwxr-xr-x   0 qcoumes    (501) staff       (20)        0 2024-03-22 10:07:30.785489 django-opensearch-dsl-0.6.0/django_opensearch_dsl.egg-info/
--rw-r--r--   0 qcoumes    (501) staff       (20)    14420 2024-03-22 10:07:30.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl.egg-info/PKG-INFO
--rw-r--r--   0 qcoumes    (501) staff       (20)      878 2024-03-22 10:07:30.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl.egg-info/SOURCES.txt
--rw-r--r--   0 qcoumes    (501) staff       (20)        1 2024-03-22 10:07:30.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl.egg-info/dependency_links.txt
--rw-r--r--   0 qcoumes    (501) staff       (20)       55 2024-03-22 10:07:30.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl.egg-info/requires.txt
--rw-r--r--   0 qcoumes    (501) staff       (20)       22 2024-03-22 10:07:30.000000 django-opensearch-dsl-0.6.0/django_opensearch_dsl.egg-info/top_level.txt
-drwxr-xr-x   0 qcoumes    (501) staff       (20)        0 2024-03-22 10:07:30.782789 django-opensearch-dsl-0.6.0/docs/
--rw-r--r--   0 qcoumes    (501) staff       (20)     8111 2024-03-22 09:17:46.000000 django-opensearch-dsl-0.6.0/docs/CHANGELOG.md
--rw-r--r--   0 qcoumes    (501) staff       (20)     1689 2024-03-22 10:07:30.789641 django-opensearch-dsl-0.6.0/setup.cfg
--rwxr-xr-x   0 qcoumes    (501) staff       (20)     1701 2024-03-22 10:07:19.000000 django-opensearch-dsl-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.895295 django_opensearch_dsl-0.6.1/django_opensearch_dsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/indices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14826 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/commands/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/registries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 21:23:39.000000 django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-13 21:23:39.899296 django_opensearch_dsl-0.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1701 2024-04-13 21:23:37.000000 django_opensearch_dsl-0.6.1/setup.py
```

### Comparing `django-opensearch-dsl-0.6.0/CONTRIBUTING.md` & `django_opensearch_dsl-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/LICENSE` & `django_opensearch_dsl-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/PKG-INFO` & `django_opensearch_dsl-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-opensearch-dsl
-Version: 0.6.0
+Version: 0.6.1
 Summary: Wrapper around opensearch-py for django models
 Home-page: https://github.com/qcoumes/django-opensearch-dsl
 Author: Quentin Coumes (Codoc)
 Author-email: coumes.quentin@gmail.com
 License: Apache Software License 2.0
 Keywords: django elasticsearch elasticsearch-dsl opensearch opensearch-dsl opensearch-py
 Classifier: Development Status :: 4 - Beta
@@ -151,15 +151,23 @@
         # Paginate the django queryset used to populate the index with the specified size
         # This per-Document setting overrides settings.OPENSEARCH_DSL_QUERYSET_PAGINATION.
         queryset_pagination = 5000
 ```
 
 # Changelog
 
-### 0.6.0 (2024-03-22)
+### 0.6.1 (2024-04-13)
+
+* Multiple fixes to `CelerySignalProcessor` ([#62](https://github.com/Codoc-os/django-opensearch-dsl/pull/63)),
+  Contributed by [Jordan Hyatt](https://github.com/JordanHyatt) and [jlariza](https://github.com/jlariza).
+  * Correctly use `.delay` when calling tasks.
+  * Only initiate tasks when needed by checking beforehand if an instance is connected to a Document (directly or related)
+  * The tasks will only be created on transaction commit.
+
+## 0.6.0 (2024-03-22)
 
 * Add `mananage.py opensearch index update` subcommand to update an existing index mappings ([#52](https://github.com/Codoc-os/django-opensearch-dsl/pull/52)).
 * Add `CelerySignalProcessor` as an alternative to `RealTimeSignalProcessor` to process signals asynchronously using Celery
   ([#51](https://github.com/Codoc-os/django-opensearch-dsl/pull/51)).
 * Add `registry.get_models()` and `registry.__contains__()` methods ([#48](https://github.com/Codoc-os/django-opensearch-dsl/pull/48), Contributed by [ghkdxofla - Taelim Hwang (Limy)](https://github.com/ghkdxofla)).
 * When using the `opensearch` command, any error now displays the raw OpenSearch response ([#49](https://github.com/Codoc-os/django-opensearch-dsl/pull/49)).
 * Autosync and related model features are now [properly documented](https://django-opensearch-dsl.readthedocs.io/en/latest/document/#autosync) ([#53](https://github.com/Codoc-os/django-opensearch-dsl/pull/53)).
```

### Comparing `django-opensearch-dsl-0.6.0/README.md` & `django_opensearch_dsl-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/apps.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/apps.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/documents.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/documents.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/fields.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/fields.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/indices.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/indices.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/commands/opensearch.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/commands/opensearch.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/enums.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/enums.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/management/types.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/management/types.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/registries.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/registries.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/search.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/search.py`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl/signals.py` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl/signals.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Attach django-opensearch-dsl to Django's signals and cause things to index."""
 
 import abc
+from functools import partial
 
 from django.apps import apps
 from django.core.serializers import deserialize, serialize
-from django.db import models
+from django.db import models, transaction
 from django.dispatch import Signal
 
 from .apps import DODConfig
 from .registries import registry
 
 # Sent after document indexing is completed
 post_index = Signal()
@@ -33,14 +34,23 @@
     def handle_pre_delete(self, sender, instance, **kwargs):
         """Delete the instance from model and associated model indices."""
 
     @abc.abstractmethod
     def handle_m2m_changed(self, sender, instance, action, **kwargs):
         """Handle changes in ManyToMany relations."""
 
+    def instance_requires_update(self, instance):
+        """Check if an instance is connected to a Document (directly or related)."""
+        m1 = instance._meta.model in registry._models
+        m2 = instance.__class__.__base__ in registry._models
+        m3 = bool(list(registry._get_related_doc(instance)))
+        if m1 or m2 or m3:
+            return True
+        return False
+
     def setup(self):
         """Set up the SignalProcessor."""
         models.signals.post_save.connect(self.handle_save)
         models.signals.pre_delete.connect(self.handle_pre_delete)
         models.signals.m2m_changed.connect(self.handle_m2m_changed)
 
     def teardown(self):
@@ -80,17 +90,21 @@
 except ImportError:
     pass
 else:
 
     @shared_task()
     def handle_save_task(app_label, model, pk):
         """Handle the update on the registry as a Celery task."""
-        instance = apps.get_model(app_label, model).objects.get(pk=pk)
-        registry.update(instance)
-        registry.update_related(instance)
+        model_object = apps.get_model(app_label, model)
+        try:
+            instance = model_object.objects.get(pk=pk)
+            registry.update(instance)
+            registry.update_related(instance)
+        except model_object.DoesNotExist:
+            pass
 
     @shared_task()
     def handle_pre_delete_task(data):
         """Delete the instance from model and associated model indices."""
         instance = next(deserialize("json", data, cls=DODConfig.signal_processor_deserializer_class())).object
         registry.delete(instance, raise_on_error=False)
         registry.delete_related(instance, raise_on_error=False)
@@ -98,14 +112,29 @@
     class CelerySignalProcessor(RealTimeSignalProcessor):
         """Celery signal processor.
 
         Allows automatic updates on the index as delayed background tasks using
         Celery.
         """
 
-        def handle_save(self, sender, instance, **kwargs):
-            """Update the instance in model and associated model indices."""
-            handle_save_task(instance._meta.app_label, instance.__class__.__name__, instance.pk)
-
-        def handle_pre_delete(self, sender, instance, **kwargs):
-            """Delete the instance from model and associated model indices."""
-            handle_pre_delete_task(serialize("json", [instance], cls=DODConfig.signal_processor_serializer_class()))
+    def handle_save(self, sender, instance, **kwargs):
+        """Update the instance in model and associated model indices."""
+        if self.instance_requires_update(instance):
+            transaction.on_commit(
+                partial(
+                    handle_save_task.delay,
+                    app_label=instance._meta.app_label,
+                    model=instance.__class__.__name__,
+                    pk=instance.pk,
+                )
+            )
+
+    def handle_pre_delete(self, sender, instance, **kwargs):
+        """Delete the instance from model and associated model indices."""
+        if self.instance_requires_update(instance):
+            handle_pre_delete_task.delay(
+                serialize(
+                    "json",
+                    [instance],
+                    cls=DODConfig.signal_processor_serializer_class(),
+                )
+            )
```

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl.egg-info/PKG-INFO` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-opensearch-dsl
-Version: 0.6.0
+Version: 0.6.1
 Summary: Wrapper around opensearch-py for django models
 Home-page: https://github.com/qcoumes/django-opensearch-dsl
 Author: Quentin Coumes (Codoc)
 Author-email: coumes.quentin@gmail.com
 License: Apache Software License 2.0
 Keywords: django elasticsearch elasticsearch-dsl opensearch opensearch-dsl opensearch-py
 Classifier: Development Status :: 4 - Beta
@@ -151,15 +151,23 @@
         # Paginate the django queryset used to populate the index with the specified size
         # This per-Document setting overrides settings.OPENSEARCH_DSL_QUERYSET_PAGINATION.
         queryset_pagination = 5000
 ```
 
 # Changelog
 
-### 0.6.0 (2024-03-22)
+### 0.6.1 (2024-04-13)
+
+* Multiple fixes to `CelerySignalProcessor` ([#62](https://github.com/Codoc-os/django-opensearch-dsl/pull/63)),
+  Contributed by [Jordan Hyatt](https://github.com/JordanHyatt) and [jlariza](https://github.com/jlariza).
+  * Correctly use `.delay` when calling tasks.
+  * Only initiate tasks when needed by checking beforehand if an instance is connected to a Document (directly or related)
+  * The tasks will only be created on transaction commit.
+
+## 0.6.0 (2024-03-22)
 
 * Add `mananage.py opensearch index update` subcommand to update an existing index mappings ([#52](https://github.com/Codoc-os/django-opensearch-dsl/pull/52)).
 * Add `CelerySignalProcessor` as an alternative to `RealTimeSignalProcessor` to process signals asynchronously using Celery
   ([#51](https://github.com/Codoc-os/django-opensearch-dsl/pull/51)).
 * Add `registry.get_models()` and `registry.__contains__()` methods ([#48](https://github.com/Codoc-os/django-opensearch-dsl/pull/48), Contributed by [ghkdxofla - Taelim Hwang (Limy)](https://github.com/ghkdxofla)).
 * When using the `opensearch` command, any error now displays the raw OpenSearch response ([#49](https://github.com/Codoc-os/django-opensearch-dsl/pull/49)).
 * Autosync and related model features are now [properly documented](https://django-opensearch-dsl.readthedocs.io/en/latest/document/#autosync) ([#53](https://github.com/Codoc-os/django-opensearch-dsl/pull/53)).
```

### Comparing `django-opensearch-dsl-0.6.0/django_opensearch_dsl.egg-info/SOURCES.txt` & `django_opensearch_dsl-0.6.1/django_opensearch_dsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/docs/CHANGELOG.md` & `django_opensearch_dsl-0.6.1/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # Changelog
 
-### 0.6.0 (2024-03-22)
+### 0.6.1 (2024-04-13)
+
+* Multiple fixes to `CelerySignalProcessor` ([#62](https://github.com/Codoc-os/django-opensearch-dsl/pull/63)),
+  Contributed by [Jordan Hyatt](https://github.com/JordanHyatt) and [jlariza](https://github.com/jlariza).
+  * Correctly use `.delay` when calling tasks.
+  * Only initiate tasks when needed by checking beforehand if an instance is connected to a Document (directly or related)
+  * The tasks will only be created on transaction commit.
+
+## 0.6.0 (2024-03-22)
 
 * Add `mananage.py opensearch index update` subcommand to update an existing index mappings ([#52](https://github.com/Codoc-os/django-opensearch-dsl/pull/52)).
 * Add `CelerySignalProcessor` as an alternative to `RealTimeSignalProcessor` to process signals asynchronously using Celery
   ([#51](https://github.com/Codoc-os/django-opensearch-dsl/pull/51)).
 * Add `registry.get_models()` and `registry.__contains__()` methods ([#48](https://github.com/Codoc-os/django-opensearch-dsl/pull/48), Contributed by [ghkdxofla - Taelim Hwang (Limy)](https://github.com/ghkdxofla)).
 * When using the `opensearch` command, any error now displays the raw OpenSearch response ([#49](https://github.com/Codoc-os/django-opensearch-dsl/pull/49)).
 * Autosync and related model features are now [properly documented](https://django-opensearch-dsl.readthedocs.io/en/latest/document/#autosync) ([#53](https://github.com/Codoc-os/django-opensearch-dsl/pull/53)).
```

### Comparing `django-opensearch-dsl-0.6.0/setup.cfg` & `django_opensearch_dsl-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-opensearch-dsl-0.6.0/setup.py` & `django_opensearch_dsl-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ]
 EXTRA_REQUIREMENTS = {
     'celery': ["celery>=4.1.0"],
 }
 
 setup(
     name='django-opensearch-dsl',
-    version='0.6.0',
+    version='0.6.1',
     description="""Wrapper around opensearch-py for django models""",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     author='Quentin Coumes (Codoc)',
     author_email='coumes.quentin@gmail.com',
     url='https://github.com/qcoumes/django-opensearch-dsl',
     packages=['django_opensearch_dsl'],
```

