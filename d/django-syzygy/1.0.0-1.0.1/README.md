# Comparing `tmp/django-syzygy-1.0.0.tar.gz` & `tmp/django-syzygy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-syzygy-1.0.0.tar", last modified: Wed Oct 11 02:21:46 2023, max compression
+gzip compressed data, was "django-syzygy-1.0.1.tar", last modified: Sat Apr 13 05:16:11 2024, max compression
```

## Comparing `django-syzygy-1.0.0.tar` & `django-syzygy-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/django_syzygy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/django_syzygy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/django_syzygy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/django_syzygy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/django_syzygy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/django_syzygy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1298 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/syzygy/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/autodetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/syzygy/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/syzygy/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/management/commands/makemigrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/management/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9308 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/syzygy/quorum/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/quorum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/syzygy/quorum/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/quorum/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/quorum/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/quorum/backends/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/syzygy/quorum/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 02:21:46.000000 django-syzygy-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/tests/test_autodetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10688 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2023-10-11 02:21:31.000000 django-syzygy-1.0.0/tests/test_quorum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/django_syzygy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12949 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 05:16:11.000000 django-syzygy-1.0.1/django_syzygy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1261 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.318294 django-syzygy-1.0.1/syzygy/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/autodetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/syzygy/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/syzygy/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/management/commands/makemigrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/management/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12804 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/syzygy/quorum/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/syzygy/quorum/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/backends/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/syzygy/quorum/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:16:11.322294 django-syzygy-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20857 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_autodetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14689 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10688 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-13 05:16:01.000000 django-syzygy-1.0.1/tests/test_quorum.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-syzygy-1.0.0/LICENSE` & `django-syzygy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.0/django_syzygy.egg-info/SOURCES.txt` & `django-syzygy-1.0.1/django_syzygy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 django_syzygy.egg-info/dependency_links.txt
 django_syzygy.egg-info/requires.txt
 django_syzygy.egg-info/top_level.txt
 syzygy/__init__.py
 syzygy/apps.py
 syzygy/autodetector.py
 syzygy/checks.py
+syzygy/compat.py
 syzygy/conf.py
 syzygy/constants.py
 syzygy/exceptions.py
 syzygy/operations.py
 syzygy/plan.py
 syzygy/management/__init__.py
 syzygy/management/commands/__init__.py
```

### Comparing `django-syzygy-1.0.0/setup.py` & `django-syzygy-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,35 @@
 from setuptools import find_packages, setup
 
 with open("README.rst") as file_:
     long_description = file_.read()
 
 setup(
     name="django-syzygy",
-    version="1.0.0",
+    version="1.0.1",
     description="",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/charettes/django-syzygy",
     author="Simon Charette",
     author_email="charette.s@gmail.com",
     install_requires=["Django>=3.2"],
     packages=find_packages(exclude=["tests", "tests.*"]),
     license="MIT License",
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
-        "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
+        "Framework :: Django :: 5.0",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `django-syzygy-1.0.0/syzygy/autodetector.py` & `django-syzygy-1.0.1/syzygy/autodetector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 import itertools
 import sys
+from typing import NamedTuple
 
 from django.db.migrations import operations
 from django.db.migrations.autodetector import (
     MigrationAutodetector as _MigrationAutodetector,
 )
 from django.db.migrations.operations.base import Operation
 from django.db.migrations.questioner import InteractiveMigrationQuestioner
 from django.db.models.fields import NOT_PROVIDED
 from django.utils.functional import cached_property
 
+from .compat import OperationDependency
 from .constants import Stage
 from .exceptions import AmbiguousStage
 from .operations import (
-    AddField,
     AlterField,
-    PostAddField,
-    PreRemoveField,
     RenameField,
     RenameModel,
+    get_post_add_field_operation,
+    get_pre_add_field_operation,
+    get_pre_remove_field_operation,
 )
 from .plan import partition_operations
 
+STAGE_SPLIT = "__stage__"
+
 
 class OperationStage(Operation):
     """
     Fake operation that serves as a placeholder to break operations into
     multiple migrations.
     """
 
 
+class StageDependency(NamedTuple):
+    app_label: str
+    operation: OperationStage
+
+
+class StagedOperationDependency(NamedTuple):
+    app_label: str
+    model_name: str
+    operation: Operation
+
+
 class MigrationAutodetector(_MigrationAutodetector):
     """
     Migration auto-detector that splits migrations containing sequence of
     operations incompatible with staged deployments.
 
     It works by inserting fake `Stage` operations into a fake __stage__
     application since `_build_migration_list` will only split operations of a
@@ -50,16 +65,14 @@
         __stage__.Migration1(operations=[OperationStage])
         app.Migration2(operations=[FirstOperation])
 
     And automatically remove the __stage__ migrations since it's a not
     an existing application.
     """
 
-    STAGE_SPLIT = "__stage__"
-
     def __init__(self, *args, **kwargs):
         self.style = kwargs.pop("style", None)
         super().__init__(*args, **kwargs)
 
     @cached_property
     def has_interactive_questionner(self) -> bool:
         return not self.questioner.dry_run and isinstance(
@@ -159,38 +172,59 @@
                 app_label, operation.model_name_lower
             ].fields[operation.name]
             if from_field.null:
                 operation = AlterField.for_stage(operation, Stage.POST_DEPLOY)
         super().add_operation(app_label, operation, dependencies, beginning)
 
     def _generate_added_field(self, app_label, model_name, field_name):
+        # Delegate most of the logic to super() ...
         super()._generate_added_field(app_label, model_name, field_name)
-        add_field = self.generated_operations[app_label][-1]
-        add_field.__class__ = AddField
+        old_add_field = self.generated_operations[app_label][-1]
+        field = old_add_field.field
+        if (
+            field.many_to_many
+            or (field.null and not field.has_default())
+            or getattr(field, "db_default", NOT_PROVIDED) is not NOT_PROVIDED
+        ):
+            return
+        # ... otherwise swap the added operation by an adjusted one.
+        add_field = get_pre_add_field_operation(
+            old_add_field.model_name,
+            old_add_field.name,
+            old_add_field.field,
+            preserve_default=old_add_field.preserve_default,
+        )
+        add_field._auto_deps = old_add_field._auto_deps
+        self.generated_operations[app_label][-1] = add_field
         stage = OperationStage()
         self.add_operation(
-            self.STAGE_SPLIT,
+            STAGE_SPLIT,
             stage,
-            dependencies=[(app_label, self.STAGE_SPLIT, add_field)],
+            dependencies=[StagedOperationDependency(app_label, STAGE_SPLIT, add_field)],
         )
-        post_add_field = PostAddField(
-            model_name=model_name, name=field_name, field=add_field.field
+        post_add_field = get_post_add_field_operation(
+            model_name=model_name,
+            name=field_name,
+            field=field,
+            preserve_default=add_field.preserve_default,
         )
         super().add_operation(
             app_label,
             post_add_field,
             dependencies=[
-                (self.STAGE_SPLIT, stage),
+                StageDependency(STAGE_SPLIT, stage),
             ],
         )
 
     def _generate_removed_field(self, app_label, model_name, field_name):
         field = self.from_state.models[app_label, model_name].fields[field_name]
         remove_default = field.default
-        if remove_default is NOT_PROVIDED and field.null:
+        if (remove_default is NOT_PROVIDED and field.null) or getattr(
+            field, "db_default", NOT_PROVIDED
+        ) is not NOT_PROVIDED:
             return super()._generate_removed_field(app_label, model_name, field_name)
 
         if remove_default is NOT_PROVIDED:
             if self.has_interactive_questionner:
                 choice = self.questioner._choice_input(
                     "You are trying to remove a non-nullable field '%s' from %s without a default; "
                     "we can't do that (the database needs a default for inserts before the removal).\n"
@@ -205,58 +239,69 @@
                             "field removal might fail)"
                         ),
                     ],
                 )
                 if choice == 1:
                     remove_default = self.questioner._ask_default()
                 elif choice == 2:
-                    pass
+                    remove_default = None
                 else:
                     sys.exit(3)
             else:
                 remove_default = self.questioner.defaults.get("ask_remove_default")
             if remove_default is not NOT_PROVIDED:
                 field = field.clone()
-                field.default = remove_default
-        pre_remove_field = PreRemoveField(
+                if remove_default is None:
+                    field.null = True
+                else:
+                    field.default = remove_default
+        pre_remove_field = get_pre_remove_field_operation(
             model_name=model_name, name=field_name, field=field
         )
         self.add_operation(app_label, pre_remove_field)
         stage = OperationStage()
         self.add_operation(
-            self.STAGE_SPLIT,
+            STAGE_SPLIT,
             stage,
             dependencies=[
-                (app_label, self.STAGE_SPLIT, self.generated_operations[app_label][-1])
+                StagedOperationDependency(
+                    app_label, STAGE_SPLIT, self.generated_operations[app_label][-1]
+                ),
             ],
         )
         self.add_operation(
             app_label,
             operations.RemoveField(model_name=model_name, name=field_name),
             dependencies=[
-                (app_label, model_name, field_name, "order_wrt_unset"),
-                (app_label, model_name, field_name, "foo_together_change"),
-                (self.STAGE_SPLIT, stage),
+                OperationDependency(
+                    app_label,
+                    model_name,
+                    field_name,
+                    OperationDependency.Type.REMOVE_ORDER_WRT,
+                ),
+                OperationDependency(
+                    app_label,
+                    model_name,
+                    field_name,
+                    OperationDependency.Type.ALTER_FOO_TOGETHER,
+                ),
+                StageDependency(STAGE_SPLIT, stage),
             ],
         )
 
     def check_dependency(self, operation, dependency):
-        # Stage dependency on a previous operation.
-        if dependency[1] == self.STAGE_SPLIT:
-            return dependency[2] is operation
-        # Dependency on a stage.
-        if dependency[0] == self.STAGE_SPLIT:
-            return dependency[1] is operation
+        if isinstance(dependency, (StageDependency, StagedOperationDependency)):
+            return dependency.operation is operation
         return super().check_dependency(operation, dependency)
 
     def _build_migration_list(self, *args, **kwargs):
         # Ensure generated operations sequence for each apps are partitioned
         # by stage.
         for app_label, app_operations in list(self.generated_operations.items()):
-            if app_label == self.STAGE_SPLIT:
+            if app_label == STAGE_SPLIT:
                 continue
             try:
                 pre_operations, post_operations = partition_operations(
                     app_operations, app_label
                 )
             except AmbiguousStage:
                 operations_description = "".join(
@@ -265,45 +310,56 @@
                 print(
                     f'The auto-detected operations for the "{app_label}" '
                     "app cannot be partitioned into deployment stages:\n"
                     f"{operations_description}",
                     file=sys.stderr,
                 )
                 if self.has_interactive_questionner:
-                    choice = self.questioner._boolean_input(
-                        "Please select a fix:",
-                        [
-                            (
-                                "Let `makemigrations` complete. You'll have to "
-                                "manually break you operations in migrations "
-                                "with non-ambiguous stages."
-                            ),
-                            (
-                                "Abort `makemigrations` and and let me reduce "
-                                "my number of model changes before running "
-                                "`makemigrations` again."
-                            ),
-                        ],
+                    abort = (
+                        self.questioner._choice_input(
+                            "",
+                            [
+                                (
+                                    "Let `makemigrations` complete. You'll have to "
+                                    "manually break you operations in migrations "
+                                    "with non-ambiguous stages."
+                                ),
+                                (
+                                    "Abort `makemigrations`. You'll have to reduce "
+                                    "the number of model changes before running "
+                                    "`makemigrations` again."
+                                ),
+                            ],
+                        )
+                        == 2
                     )
-                    if not choice:
-                        sys.exit(3)
+                else:
+                    abort = self.questioner.defaults.get("ask_ambiguous_abort", False)
+                if abort:
+                    sys.exit(3)
                 continue
             if pre_operations and post_operations:
                 stage = OperationStage()
                 self.add_operation(
-                    self.STAGE_SPLIT,
+                    STAGE_SPLIT,
                     stage,
-                    dependencies=[(app_label, self.STAGE_SPLIT, pre_operations[-1])],
+                    dependencies=[
+                        StagedOperationDependency(
+                            app_label, STAGE_SPLIT, pre_operations[-1]
+                        )
+                    ],
+                )
+                post_operations[0]._auto_deps.append(
+                    StageDependency(STAGE_SPLIT, stage)
                 )
-                post_operations[0]._auto_deps.append((self.STAGE_SPLIT, stage))
                 # Assign updated operations as they might have be re-ordered by
                 # `partition_operations`.
                 self.generated_operations[app_label] = pre_operations + post_operations
         super()._build_migration_list(*args, **kwargs)
         # Remove all dangling references to stage migrations.
-        if self.migrations.pop(self.STAGE_SPLIT, None):
+        if self.migrations.pop(STAGE_SPLIT, None):
             for migration in itertools.chain.from_iterable(self.migrations.values()):
                 migration.dependencies = [
                     dependency
                     for dependency in migration.dependencies
-                    if dependency[0] != self.STAGE_SPLIT
+                    if dependency[0] != STAGE_SPLIT
                 ]
```

### Comparing `django-syzygy-1.0.0/syzygy/checks.py` & `django-syzygy-1.0.1/syzygy/checks.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.0/syzygy/conf.py` & `django-syzygy-1.0.1/syzygy/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 MigrationStagesSetting = Dict[str, Stage]
 
 MIGRATION_STAGES_OVERRIDE: MigrationStagesSetting
 MIGRATION_STAGES_FALLBACK: MigrationStagesSetting
 
 
-def _configure():
+def _configure() -> None:
     global MIGRATION_STAGES_OVERRIDE
     global MIGRATION_STAGES_FALLBACK
     MIGRATION_STAGES_OVERRIDE = getattr(settings, "MIGRATION_STAGES_OVERRIDE", {})
     MIGRATION_STAGES_FALLBACK = getattr(settings, "MIGRATION_STAGES_FALLBACK", {})
     third_party_stages_fallback: Optional[Stage] = getattr(
         settings, "MIGRATION_THIRD_PARTY_STAGES_FALLBACK", Stage.PRE_DEPLOY
     )
```

### Comparing `django-syzygy-1.0.0/syzygy/management/commands/makemigrations.py` & `django-syzygy-1.0.1/syzygy/management/commands/makemigrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.core.management.commands import makemigrations  # type: ignore
+from django.core.management.commands import makemigrations
 
 from syzygy.autodetector import MigrationAutodetector
 
 
 class Command(makemigrations.Command):
     def add_arguments(self, parser):
         super().add_arguments(parser)
```

### Comparing `django-syzygy-1.0.0/syzygy/management/commands/migrate.py` & `django-syzygy-1.0.1/syzygy/management/commands/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 from contextlib import contextmanager
 from datetime import timedelta
 from typing import Iterator
 
 from django.apps import apps
 from django.core.management import CommandError
-from django.core.management.commands import migrate  # type: ignore
+from django.core.management.commands import migrate
 from django.db import connections
 from django.db.migrations.exceptions import AmbiguityError
 from django.db.migrations.executor import MigrationExecutor
 
 from syzygy.constants import Stage
 from syzygy.plan import Plan, get_pre_deploy_plan, hash_plan
 from syzygy.quorum import (
```

### Comparing `django-syzygy-1.0.0/syzygy/operations.py` & `django-syzygy-1.0.1/syzygy/operations.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from contextlib import contextmanager
 
 from django.db.migrations import operations
 from django.db.models.fields import NOT_PROVIDED
+from django.utils.functional import cached_property
 
+from .compat import field_db_default_supported
 from .constants import Stage
 
 
 def _alter_field_db_default_sql_params(schema_editor, model, name, drop=False):
     field = model._meta.get_field(name)
     changes_sql, params = schema_editor._alter_column_default_sql(
         model, None, field, drop=drop
@@ -118,14 +120,47 @@
             return "Set database DEFAULT of field %s on %s" % (
                 self.name,
                 self.model_name,
             )
         return "Set field %s of %s NULLable" % (self.name, self.model_name)
 
 
+if field_db_default_supported:
+    # XXX: This allows for a more descriptive migration_name_fragment
+    # to be associated with instances of AlterField.
+    operations.AlterField.migration_name_fragment = cached_property(  # type: ignore[assignment,method-assign]
+        operations.AlterField.migration_name_fragment.fget  # type: ignore[attr-defined]
+    )
+    operations.AlterField.migration_name_fragment.name = "migration_name_fragment"  # type: ignore[attr-defined]
+
+    def get_pre_remove_field_operation(model_name, name, field, **kwargs):
+        if field.db_default is not NOT_PROVIDED:
+            raise ValueError(
+                "Fields with a db_default don't require a pre-deployment operation."
+            )
+        field = field.clone()
+        if field.has_default():
+            field.db_default = field.get_default()
+            fragment = f"set_db_default_{model_name.lower()}_{name}"
+            description = f"Set database DEFAULT of field {name} on {model_name}"
+        else:
+            field.null = True
+            fragment = f"set_nullable_{model_name.lower()}_{name}"
+            description = f"Set field {name} of {model_name} NULLable"
+        operation = operations.AlterField(model_name, name, field, **kwargs)
+        operation.migration_name_fragment = fragment
+        operation.describe = lambda: description
+        return operation
+
+    # XXX: Shim kept for historical migrations generated before Django 5.
+    PreRemoveField = get_pre_remove_field_operation  # type: ignore[assignment,misc] # noqa: F811
+else:
+    get_pre_remove_field_operation = PreRemoveField  # type: ignore[assignment]
+
+
 class AddField(operations.AddField):
     """
     Subclass of `AddField` that preserves the database default on database
     application.
     """
 
     @contextmanager
@@ -163,14 +198,32 @@
         # Defer the removal of DEFAUT to `PostAddField`
         with self._preserve_column_default(schema_editor, model):
             return super().database_forwards(
                 app_label, schema_editor, from_state, to_state
             )
 
 
+if field_db_default_supported:
+
+    def get_pre_add_field_operation(model_name, name, field, preserve_default=True):
+        if field.db_default is not NOT_PROVIDED:
+            raise ValueError(
+                "Fields with a db_default don't require a pre-deployment operation."
+            )
+        field = field.clone()
+        field.db_default = field.get_default()
+        operation = operations.AddField(model_name, name, field, preserve_default)
+        return operation
+
+    # XXX: Shim kept for historical migrations generated before Django 5.
+    AddField = get_pre_add_field_operation  # type: ignore[assignment,misc] # noqa: F811
+else:
+    get_pre_add_field_operation = AddField
+
+
 class PostAddField(operations.AlterField):
     """
     Elidable operation that drops a previously preserved database default.
     """
 
     stage = Stage.POST_DEPLOY
 
@@ -214,14 +267,45 @@
     def describe(self):
         return "Drop database DEFAULT of field %s on %s" % (
             self.name,
             self.model_name,
         )
 
 
+if field_db_default_supported:
+
+    def get_post_add_field_operation(model_name, name, field, preserve_default=True):
+        if field.db_default is not NOT_PROVIDED:
+            raise ValueError(
+                "Fields with a db_default don't require a post-deployment operation."
+            )
+        field = field.clone()
+        field.db_default = NOT_PROVIDED
+        if not preserve_default:
+            field.default = NOT_PROVIDED
+        operation = AlterField(
+            model_name,
+            name,
+            field,
+            stage=Stage.POST_DEPLOY,
+        )
+        operation.migration_name_fragment = (
+            f"drop_db_default_{model_name.lower()}_{name}"
+        )
+        operation.describe = (
+            lambda: f"Drop database DEFAULT of field {name} on {model_name}"
+        )
+        return operation
+
+    # XXX: Shim kept for historical migrations generated before Django 5.
+    PostAddField = get_post_add_field_operation  # type: ignore[assignment,misc] # noqa: F811
+else:
+    get_post_add_field_operation = PostAddField
+
+
 class StagedOperation(operations.base.Operation):
     stage: Stage
 
     def __init__(self, *args, **kwargs):
         self.stage = kwargs.pop("stage")
         super().__init__(*args, **kwargs)
```

### Comparing `django-syzygy-1.0.0/syzygy/plan.py` & `django-syzygy-1.0.1/syzygy/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     post_deploy_operations = stage_operations[Stage.POST_DEPLOY]
     for operation in operations:
         operation_stage = get_operation_stage(operation)
         if operation_stage is Stage.PRE_DEPLOY and post_deploy_operations:
             # If a pre-deploy operation is encountered after a post-deployment
             # one attempt to re-order operation is allowed.
             if all(
-                op.reduce(operation, app_label) is True for op in post_deploy_operations  # type: ignore
+                op.reduce(operation, app_label) is True for op in post_deploy_operations
             ):
                 stage_operations[Stage.PRE_DEPLOY].append(operation)
                 continue
             raise AmbiguousStage(
                 "Post-deployment operations cannot be followed by "
                 "pre-deployments operations"
             )
@@ -158,22 +158,24 @@
     """
     pre_deploy_plan: Plan = []
     post_deploy_plan = {}
     for migration, backward in plan:
         if must_post_deploy_migration(migration, backward):
             post_deploy_plan[migration.app_label, migration.name] = migration
         else:
-            post_deploy_dep = post_deploy_plan and next(
-                (
-                    post_deploy_plan[dependency]
-                    for dependency in migration.dependencies
-                    if dependency in post_deploy_plan
-                ),
-                None,
-            )
+            post_deploy_dep = None
+            if post_deploy_plan:
+                post_deploy_dep = next(
+                    (
+                        post_deploy_plan[dependency]
+                        for dependency in migration.dependencies
+                        if dependency in post_deploy_plan
+                    ),
+                    None,
+                )
             if post_deploy_dep:
                 inferred = []
                 stage_defined = _get_defined_stage(migration) is not None
                 post_stage_defined = _get_defined_stage(post_deploy_dep) is not None
                 if stage_defined:
                     stage_origin = "defined"
                 else:
```

### Comparing `django-syzygy-1.0.0/syzygy/quorum/__init__.py` & `django-syzygy-1.0.1/syzygy/quorum/__init__.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.0/syzygy/quorum/backends/base.py` & `django-syzygy-1.0.1/syzygy/quorum/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.0/syzygy/quorum/backends/cache.py` & `django-syzygy-1.0.1/syzygy/quorum/backends/cache.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.0/tests/test_autodetector.py` & `django-syzygy-1.0.1/tests/test_autodetector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from typing import List, Optional
-from unittest import mock
+from unittest import mock, skipUnless
 
 from django.core.management.color import color_style
 from django.db import migrations, models
 from django.db.migrations.questioner import (
     InteractiveMigrationQuestioner,
     MigrationQuestioner,
 )
 from django.db.migrations.state import ModelState, ProjectState
 from django.test import TestCase
 from django.test.utils import captured_stderr, captured_stdin, captured_stdout
 
-from syzygy.autodetector import MigrationAutodetector
+from syzygy.autodetector import STAGE_SPLIT, MigrationAutodetector
+from syzygy.compat import field_db_default_supported
 from syzygy.constants import Stage
 from syzygy.exceptions import AmbiguousStage
 from syzygy.operations import (
     AddField,
+    AlterField,
     PostAddField,
     PreRemoveField,
     RenameField,
     RenameModel,
 )
 from syzygy.plan import get_migration_stage
 
@@ -42,44 +44,110 @@
     ) -> List[migrations.Migration]:
         changes = MigrationAutodetector(
             self.make_project_state(before_states),
             self.make_project_state(after_states),
             questioner=questioner,
             style=self.style,
         )._detect_changes()
-        self.assertNotIn(MigrationAutodetector.STAGE_SPLIT, changes)
+        self.assertNotIn(STAGE_SPLIT, changes)
         return changes
 
 
 class AutodetectorTests(AutodetectorTestCase):
-    def test_field_addition(self):
+    def _test_field_addition(self, field):
         from_model = ModelState("tests", "Model", [])
-        to_model = ModelState(
-            "tests", "Model", [("field", models.IntegerField(default=42))]
-        )
+        to_model = ModelState("tests", "Model", [("field", field)])
         changes = self.get_changes([from_model], [to_model])["tests"]
         self.assertEqual(len(changes), 2)
         self.assertEqual(get_migration_stage(changes[0]), Stage.PRE_DEPLOY)
         self.assertEqual(changes[0].dependencies, [])
         self.assertEqual(len(changes[0].operations), 1)
-        self.assertIsInstance(changes[0].operations[0], AddField)
+        pre_operation = changes[0].operations[0]
+        if field_db_default_supported:
+            self.assertIsInstance(pre_operation, migrations.AddField)
+            self.assertEqual(pre_operation.field.db_default, field.default)
+        else:
+            self.assertIsInstance(pre_operation, AddField)
         self.assertEqual(get_migration_stage(changes[1]), Stage.POST_DEPLOY)
         self.assertEqual(changes[1].dependencies, [("tests", "auto_1")])
         self.assertEqual(len(changes[1].operations), 1)
-        self.assertIsInstance(changes[1].operations[0], PostAddField)
+        post_operation = changes[1].operations[0]
+        if field_db_default_supported:
+            self.assertIsInstance(post_operation, AlterField)
+            self.assertIs(post_operation.field.db_default, models.NOT_PROVIDED)
+        else:
+            self.assertIsInstance(post_operation, PostAddField)
+
+    def test_field_addition(self):
+        fields = [
+            models.IntegerField(default=42),
+            models.IntegerField(null=True, default=42),
+        ]
+        for field in fields:
+            with self.subTest(field=field):
+                self._test_field_addition(field)
+
+    def test_many_to_many_addition(self):
+        from_model = ModelState("tests", "Model", [])
+        to_model = ModelState(
+            "tests", "Model", [("field", models.ManyToManyField("self"))]
+        )
+        changes = self.get_changes([from_model], [to_model])["tests"]
+        self.assertEqual(len(changes), 1)
+        self.assertEqual(get_migration_stage(changes[0]), Stage.PRE_DEPLOY)
+        self.assertEqual(changes[0].dependencies, [])
+        self.assertEqual(len(changes[0].operations), 1)
+        operation = changes[0].operations[0]
+        self.assertIsInstance(operation, migrations.AddField)
+
+    def test_nullable_field_addition(self):
+        """
+        No action required if the field is already NULL'able and doesn't have
+        a `default`.
+        """
+        from_model = ModelState("tests", "Model", [])
+        to_model = ModelState(
+            "tests", "Model", [("field", models.IntegerField(null=True))]
+        )
+        changes = self.get_changes([from_model], [to_model])["tests"]
+        self.assertEqual(len(changes), 1)
+        self.assertEqual(get_migration_stage(changes[0]), Stage.PRE_DEPLOY)
+
+    @skipUnless(field_db_default_supported, "Field.db_default is not supported")
+    def test_db_default_field_addition(self):
+        """
+        No action required if the field already has a `db_default`
+        """
+        from_model = ModelState("tests", "Model", [])
+        to_model = ModelState(
+            "tests", "Model", [("field", models.IntegerField(db_default=42))]
+        )
+        changes = self.get_changes([from_model], [to_model])["tests"]
+        self.assertEqual(len(changes), 1)
+        self.assertEqual(get_migration_stage(changes[0]), Stage.PRE_DEPLOY)
 
     def _test_field_removal(self, field):
         from_model = ModelState("tests", "Model", [("field", field)])
         to_model = ModelState("tests", "Model", [])
         changes = self.get_changes([from_model], [to_model])["tests"]
         self.assertEqual(len(changes), 2)
         self.assertEqual(get_migration_stage(changes[0]), Stage.PRE_DEPLOY)
         self.assertEqual(changes[0].dependencies, [])
         self.assertEqual(len(changes[0].operations), 1)
-        self.assertIsInstance(changes[0].operations[0], PreRemoveField)
+        pre_operation = changes[0].operations[0]
+        if field_db_default_supported:
+            self.assertIsInstance(pre_operation, migrations.AlterField)
+            if field.has_default():
+                self.assertEqual(pre_operation.field.db_default, 42)
+            else:
+                self.assertIs(pre_operation.field.null, True)
+        else:
+            self.assertIsInstance(pre_operation, PreRemoveField)
+        if not field.has_default():
+            self.assertIs(pre_operation.field.null, True)
         self.assertEqual(get_migration_stage(changes[1]), Stage.POST_DEPLOY)
         self.assertEqual(changes[1].dependencies, [("tests", "auto_1")])
         self.assertEqual(len(changes[1].operations), 1)
         self.assertIsInstance(changes[1].operations[0], migrations.RemoveField)
 
     def test_field_removal(self):
         fields = [
@@ -100,14 +168,27 @@
             "tests", "Model", [("field", models.IntegerField(null=True))]
         )
         to_model = ModelState("tests", "Model", [])
         changes = self.get_changes([from_model], [to_model])["tests"]
         self.assertEqual(len(changes), 1)
         self.assertEqual(get_migration_stage(changes[0]), Stage.POST_DEPLOY)
 
+    @skipUnless(field_db_default_supported, "Field.db_default is not supported")
+    def test_db_default_field_removal(self):
+        """
+        No action required if the field already has a `db_default`
+        """
+        from_model = ModelState(
+            "tests", "Model", [("field", models.IntegerField(db_default=42))]
+        )
+        to_model = ModelState("tests", "Model", [])
+        changes = self.get_changes([from_model], [to_model])["tests"]
+        self.assertEqual(len(changes), 1)
+        self.assertEqual(get_migration_stage(changes[0]), Stage.POST_DEPLOY)
+
     def test_non_nullable_field_removal_default(self):
         from_model = ModelState("tests", "Model", [("field", models.IntegerField())])
         to_model = ModelState("tests", "Model", [])
         changes = self.get_changes(
             [from_model], [to_model], MigrationQuestioner({"ask_remove_default": 42})
         )["tests"]
         self.assertEqual(len(changes), 2)
@@ -263,15 +344,18 @@
         self.assertEqual(get_migration_stage(changes[0]), Stage.PRE_DEPLOY)
         self.assertEqual(changes[0].dependencies, [])
         self.assertEqual(len(changes[0].operations), 1)
         self.assertIsInstance(changes[0].operations[0], migrations.AddField)
         self.assertEqual(get_migration_stage(changes[1]), Stage.POST_DEPLOY)
         self.assertEqual(changes[1].dependencies, [("tests", "auto_1")])
         self.assertEqual(len(changes[1].operations), 2)
-        self.assertIsInstance(changes[1].operations[0], PostAddField)
+        if field_db_default_supported:
+            self.assertIsInstance(changes[1].operations[0], AlterField)
+        else:
+            self.assertIsInstance(changes[1].operations[0], PostAddField)
         self.assertIsInstance(changes[1].operations[1], migrations.DeleteModel)
 
     def test_mixed_stage_failure(self):
         from_models = [
             ModelState("tests", "Foo", [("id", models.IntegerField(primary_key=True))]),
             ModelState(
                 "tests",
@@ -300,14 +384,19 @@
             'The auto-detected operations for the "tests" app cannot be partitioned into deployment stages:',
             stderr.getvalue(),
         )
         self.assertIn(
             "- Remove field foo from bar",
             stderr.getvalue(),
         )
+        questioner = MigrationQuestioner({"ask_ambiguous_abort": True})
+        with self.assertRaisesMessage(SystemExit, "3"), mock.patch(
+            "syzygy.autodetector.partition_operations", side_effect=AmbiguousStage
+        ), captured_stderr() as stderr:
+            self.get_changes(from_models, to_models, questioner)["tests"]
 
 
 class InteractiveAutodetectorTests(AutodetectorTestCase):
     def test_field_rename(self):
         from_models = [
             ModelState(
                 "tests",
@@ -387,7 +476,43 @@
         )
         self.assertIn(
             self.style.MIGRATE_LABEL(
                 "This might cause downtime if your assumption is wrong"
             ),
             stdout.getvalue(),
         )
+
+    def test_mixed_stage_failure(self):
+        from_models = [
+            ModelState("tests", "Foo", [("id", models.IntegerField(primary_key=True))]),
+            ModelState(
+                "tests",
+                "Bar",
+                [
+                    ("id", models.IntegerField(primary_key=True)),
+                    ("foo", models.ForeignKey("Foo", models.CASCADE)),
+                ],
+            ),
+        ]
+        to_models = [
+            ModelState(
+                "tests",
+                "Foo",
+                [
+                    ("id", models.IntegerField(primary_key=True)),
+                    ("bar", models.BooleanField(default=False)),
+                ],
+            ),
+        ]
+        with mock.patch(
+            "syzygy.autodetector.partition_operations", side_effect=AmbiguousStage
+        ), captured_stdin() as stdin, captured_stdout() as stdout, captured_stderr():
+            questioner = InteractiveMigrationQuestioner()
+            stdin.write("1\n")
+            stdin.seek(0)
+            self.get_changes(from_models, to_models, questioner)["tests"]
+        self.assertEqual(
+            stdout.getvalue(),
+            "\n 1) Let `makemigrations` complete. You'll have to manually break you operations in migrations "
+            "with non-ambiguous stages.\n 2) Abort `makemigrations`. You'll have to reduce the number of model "
+            "changes before running `makemigrations` again.\nSelect an option: ",
+        )
```

### Comparing `django-syzygy-1.0.0/tests/test_checks.py` & `django-syzygy-1.0.1/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.0/tests/test_commands.py` & `django-syzygy-1.0.1/tests/test_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from io import StringIO
 from multiprocessing.pool import ThreadPool
 from unittest import mock
 
-import django
 from django.core.cache import cache
 from django.core.management import CommandError, call_command
 from django.db import connection, connections
 from django.db.migrations.recorder import MigrationRecorder
 from django.test import TestCase, TransactionTestCase, override_settings
 
 from syzygy.constants import Stage
@@ -200,21 +199,18 @@
     )
     def test_null_field_removal(self):
         stdout = StringIO()
         call_command(
             "makemigrations", "tests", no_color=True, dry_run=True, stdout=stdout
         )
         output = stdout.getvalue()
-        if django.VERSION >= (3, 2):
-            self.assertIn("null_field_removal/0002_set_db_default_foo_bar.py", output)
-        else:
-            self.assertIn("null_field_removal/0002_auto", output)
-        self.assertIn("- Set database DEFAULT of field bar on foo", output)
+        self.assertIn("null_field_removal/0002_set_nullable_foo_bar.py", output)
+        self.assertIn("Set field bar of foo NULLable", output)
         self.assertIn("null_field_removal/0003_remove_foo_bar.py", output)
-        self.assertIn("- Remove field bar from foo", output)
+        self.assertIn("Remove field bar from foo", output)
 
     @override_settings(
         MIGRATION_MODULES={"tests": "tests.test_migrations.merge_conflict"}
     )
     def test_merge_conflict(self):
         stdout = StringIO()
         call_command(
```

### Comparing `django-syzygy-1.0.0/tests/test_operations.py` & `django-syzygy-1.0.1/tests/test_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from typing import List, Optional, Tuple
+from unittest import mock, skipUnless
 
 from django.db import connection, migrations, models
 from django.db.migrations.operations.base import Operation
 from django.db.migrations.optimizer import MigrationOptimizer
 from django.db.migrations.serializer import OperationSerializer
 from django.db.migrations.state import ProjectState
 from django.db.models.fields import NOT_PROVIDED
 from django.test import TestCase
 
 from syzygy.autodetector import MigrationAutodetector
+from syzygy.compat import field_db_default_supported
 from syzygy.constants import Stage
-from syzygy.operations import AddField, PostAddField, PreRemoveField
+from syzygy.operations import (
+    get_post_add_field_operation,
+    get_pre_add_field_operation,
+    get_pre_remove_field_operation,
+)
 from syzygy.plan import get_operation_stage
 
 
 class OperationTestCase(TestCase):
     @classmethod
     def setUpClass(cls):
         connection.disable_constraint_checking()
@@ -53,70 +59,95 @@
         optimized = MigrationOptimizer().optimize(operations, "tests")
         deep_deconstruct = MigrationAutodetector(
             ProjectState(), ProjectState()
         ).deep_deconstruct
         self.assertEqual(deep_deconstruct(optimized), deep_deconstruct(expected))
 
 
-class AddFieldTests(OperationTestCase):
+class PreAddFieldTests(OperationTestCase):
     def test_database_forwards(self, preserve_default=True):
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
         state = self.apply_operation(
             migrations.CreateModel(model_name, [("id", models.AutoField())]),
         )
         pre_model = state.apps.get_model("tests", model_name)
         state = self.apply_operation(
-            AddField(model_name, field_name, field, preserve_default=preserve_default),
+            get_pre_add_field_operation(
+                model_name, field_name, field, preserve_default=preserve_default
+            ),
             state,
         )
         post_model = state.apps.get_model("tests", model_name)
         pre_model.objects.create()
         self.assertEqual(post_model.objects.get().foo, 42)
 
     def test_database_forwards_discard_default(self):
         self.test_database_forwards(preserve_default=False)
 
     def test_deconstruct(self):
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
-        operation = AddField(model_name, field_name, field)
-        self.assertEqual(
-            operation.deconstruct(),
-            (
-                "AddField",
-                [],
-                {"model_name": model_name, "name": field_name, "field": field},
-            ),
-        )
-        serializer = OperationSerializer(operation)
-        serialized, imports = serializer.serialize()
-        self.assertTrue(serialized.startswith("syzygy.operations.AddField"))
-        self.assertIn("import syzygy.operations", imports)
+        operation = get_pre_add_field_operation(model_name, field_name, field)
+        deconstructed = operation.deconstruct()
+        if field_db_default_supported:
+            self.assertEqual(
+                operation.deconstruct(),
+                (
+                    "AddField",
+                    [],
+                    {"model_name": model_name, "name": field_name, "field": mock.ANY},
+                ),
+            )
+            self.assertEqual(
+                deconstructed[2]["field"].deconstruct(),
+                (
+                    None,
+                    "django.db.models.IntegerField",
+                    [],
+                    {"default": 42, "db_default": 42},
+                ),
+            )
+        else:
+            self.assertEqual(
+                deconstructed,
+                (
+                    "AddField",
+                    [],
+                    {"model_name": model_name, "name": field_name, "field": field},
+                ),
+            )
+            serializer = OperationSerializer(operation)
+            serialized, imports = serializer.serialize()
+            self.assertTrue(serialized.startswith("syzygy.operations.AddField"))
+            self.assertIn("import syzygy.operations", imports)
 
 
 class PostAddFieldTests(OperationTestCase):
     def test_database_forwards(
         self, preserve_default=True
     ) -> Tuple[ProjectState, ProjectState]:
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
         from_state = self.apply_operations(
             [
                 migrations.CreateModel(model_name, [("id", models.AutoField())]),
-                AddField(
+                get_pre_add_field_operation(
                     model_name, field_name, field, preserve_default=preserve_default
                 ),
             ]
         )
         to_state = self.apply_operation(
-            PostAddField(model_name, field_name, field), from_state.clone()
+            get_post_add_field_operation(
+                model_name, field_name, field, preserve_default=preserve_default
+            ),
+            from_state.clone(),
         )
         if not preserve_default:
             self.assertIs(
                 NOT_PROVIDED,
                 to_state.models["tests", model_name.lower()].fields[field_name].default,
             )
         with connection.cursor() as cursor:
@@ -131,83 +162,115 @@
 
     def test_database_backwards(self, preserve_default=True):
         from_state, to_state = self.test_database_forwards(preserve_default)
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
         with connection.schema_editor() as schema_editor:
-            PostAddField(model_name, field_name, field).database_backwards(
-                "tests", schema_editor, to_state, from_state
-            )
+            get_post_add_field_operation(
+                model_name, field_name, field
+            ).database_backwards("tests", schema_editor, to_state, from_state)
         if not preserve_default:
             self.assertIs(
                 NOT_PROVIDED,
                 from_state.models["tests", model_name.lower()]
                 .fields[field_name]
                 .default,
             )
         with connection.cursor() as cursor:
             fields = connection.introspection.get_table_description(
                 cursor, "tests_testmodel"
             )
-        self.assertEqual(int(fields[-1].default), 42)
+        for field in fields:
+            if field.name == "foo":
+                break
+        else:
+            self.fail('Could not find field "foo"')
+        self.assertEqual(int(field.default), 42)
 
     def test_database_backwards_discard_default(self):
         self.test_database_backwards(preserve_default=False)
 
     def test_stage(self):
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
         self.assertEqual(
-            get_operation_stage(PostAddField(model_name, field_name, field)),
+            get_operation_stage(
+                get_post_add_field_operation(model_name, field_name, field)
+            ),
             Stage.POST_DEPLOY,
         )
 
     def test_migration_name_fragment(self):
         self.assertEqual(
-            PostAddField(
+            get_post_add_field_operation(
                 "TestModel", "foo", models.IntegerField(default=42)
             ).migration_name_fragment,
             "drop_db_default_testmodel_foo",
         )
 
     def test_describe(self):
         self.assertEqual(
-            PostAddField(
+            get_post_add_field_operation(
                 "TestModel", "foo", models.IntegerField(default=42)
             ).describe(),
             "Drop database DEFAULT of field foo on TestModel",
         )
 
     def test_deconstruct(self):
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
-        operation = PostAddField(model_name, field_name, field)
-        self.assertEqual(
-            operation.deconstruct(),
-            (
-                "PostAddField",
-                [],
-                {"model_name": model_name, "name": field_name, "field": field},
-            ),
-        )
-        serializer = OperationSerializer(operation)
-        serialized, imports = serializer.serialize()
-        self.assertTrue(serialized.startswith("syzygy.operations.PostAddField"))
-        self.assertIn("import syzygy.operations", imports)
+        operation = get_post_add_field_operation(model_name, field_name, field)
+        deconstructed = operation.deconstruct()
+        if field_db_default_supported:
+            self.assertEqual(
+                deconstructed,
+                (
+                    "AlterField",
+                    [],
+                    {
+                        "model_name": model_name,
+                        "name": field_name,
+                        "field": mock.ANY,
+                        "stage": Stage.POST_DEPLOY,
+                    },
+                ),
+            )
+            self.assertEqual(
+                deconstructed[2]["field"].deconstruct(),
+                (
+                    None,
+                    "django.db.models.IntegerField",
+                    [],
+                    {"default": 42},
+                ),
+            )
+        else:
+            self.assertEqual(
+                deconstructed,
+                (
+                    "PostAddField",
+                    [],
+                    {"model_name": model_name, "name": field_name, "field": field},
+                ),
+            )
+            serializer = OperationSerializer(operation)
+            serialized, imports = serializer.serialize()
+            self.assertTrue(serialized.startswith("syzygy.operations.PostAddField"))
+            self.assertIn("import syzygy.operations", imports)
 
     def test_reduce(self):
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
         operations = [
-            AddField(model_name, field_name, field),
-            PostAddField(model_name, field_name, field),
+            get_pre_add_field_operation(model_name, field_name, field),
+            get_post_add_field_operation(model_name, field_name, field),
         ]
         self.assert_optimizes_to(
             operations,
             [
                 migrations.AddField(model_name, field_name, field),
             ],
         )
@@ -215,15 +278,15 @@
 
 class PreRemoveFieldTests(OperationTestCase):
     def test_database_forwards_null(self):
         model_name = "TestModel"
         field = models.IntegerField()
         operations = [
             migrations.CreateModel(model_name, [("foo", field)]),
-            PreRemoveField(
+            get_pre_remove_field_operation(
                 model_name,
                 "foo",
                 field,
             ),
         ]
         state = self.apply_operations(operations)
         pre_model = state.apps.get_model("tests", model_name)
@@ -234,15 +297,15 @@
         self.assertIsNone(pre_model.objects.get().foo)
 
     def test_database_forwards_default(self):
         model_name = "TestModel"
         field = models.IntegerField(default=42)
         operations = [
             migrations.CreateModel(model_name, [("foo", field)]),
-            PreRemoveField(
+            get_pre_remove_field_operation(
                 model_name,
                 "foo",
                 field,
             ),
         ]
         state = self.apply_operations(operations)
         pre_model = state.apps.get_model("tests", model_name)
@@ -250,66 +313,98 @@
         remove_field.state_forwards("tests", state)
         post_model = state.apps.get_model("tests", model_name)
         post_model.objects.create()
         self.assertEqual(pre_model.objects.get().foo, 42)
 
     def test_migration_name_fragment(self):
         self.assertEqual(
-            PreRemoveField(
+            get_pre_remove_field_operation(
                 "TestModel", "foo", models.IntegerField(default=42)
             ).migration_name_fragment,
             "set_db_default_testmodel_foo",
         )
         self.assertEqual(
-            PreRemoveField(
+            get_pre_remove_field_operation(
                 "TestModel", "foo", models.IntegerField()
             ).migration_name_fragment,
             "set_nullable_testmodel_foo",
         )
 
     def test_describe(self):
         self.assertEqual(
-            PreRemoveField(
+            get_pre_remove_field_operation(
                 "TestModel", "foo", models.IntegerField(default=42)
             ).describe(),
             "Set database DEFAULT of field foo on TestModel",
         )
         self.assertEqual(
-            PreRemoveField("TestModel", "foo", models.IntegerField()).describe(),
+            get_pre_remove_field_operation(
+                "TestModel", "foo", models.IntegerField()
+            ).describe(),
             "Set field foo of TestModel NULLable",
         )
 
     def test_deconstruct(self):
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
-        operation = PreRemoveField(
+        operation = get_pre_remove_field_operation(
             model_name,
             field_name,
             field,
         )
-        self.assertEqual(
-            operation.deconstruct(),
-            (
-                "PreRemoveField",
-                [],
-                {"model_name": model_name, "name": field_name, "field": field},
-            ),
-        )
-        serializer = OperationSerializer(operation)
-        serialized, imports = serializer.serialize()
-        self.assertTrue(serialized.startswith("syzygy.operations.PreRemoveField"))
-        self.assertIn("import syzygy.operations", imports)
+        deconstructed = operation.deconstruct()
+        if field_db_default_supported:
+            self.assertEqual(
+                deconstructed,
+                (
+                    "AlterField",
+                    [],
+                    {"model_name": model_name, "name": field_name, "field": mock.ANY},
+                ),
+            )
+            self.assertEqual(
+                deconstructed[2]["field"].deconstruct(),
+                (
+                    None,
+                    "django.db.models.IntegerField",
+                    [],
+                    {"default": 42, "db_default": 42},
+                ),
+            )
+        else:
+            self.assertEqual(
+                deconstructed,
+                (
+                    "PreRemoveField",
+                    [],
+                    {"model_name": model_name, "name": field_name, "field": field},
+                ),
+            )
+            serializer = OperationSerializer(operation)
+            serialized, imports = serializer.serialize()
+            self.assertTrue(serialized.startswith("syzygy.operations.PreRemoveField"))
+            self.assertIn("import syzygy.operations", imports)
 
     def test_elidable(self):
         model_name = "TestModel"
         field_name = "foo"
         field = models.IntegerField(default=42)
         operations = [
-            PreRemoveField(
+            get_pre_remove_field_operation(
                 model_name,
                 field_name,
                 field,
             ),
             migrations.RemoveField(model_name, field_name, field),
         ]
         self.assert_optimizes_to(operations, [operations[-1]])
+
+    @skipUnless(field_db_default_supported, "Field.db_default not supported")
+    def test_defined_db_default(self):
+        with self.assertRaisesMessage(
+            ValueError,
+            "Fields with a db_default don't require a pre-deployment operation.",
+        ):
+            get_pre_remove_field_operation(
+                "model", "field", models.IntegerField(db_default=42)
+            )
```

### Comparing `django-syzygy-1.0.0/tests/test_plan.py` & `django-syzygy-1.0.1/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-1.0.0/tests/test_quorum.py` & `django-syzygy-1.0.1/tests/test_quorum.py`

 * *Files identical despite different names*

