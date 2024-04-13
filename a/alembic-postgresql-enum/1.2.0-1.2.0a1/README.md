# Comparing `tmp/alembic_postgresql_enum-1.2.0.tar.gz` & `tmp/alembic_postgresql_enum-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic_postgresql_enum-1.2.0.tar", max compression
+gzip compressed data, was "alembic_postgresql_enum-1.2.0a1.tar", max compression
```

## Comparing `alembic_postgresql_enum-1.2.0.tar` & `alembic_postgresql_enum-1.2.0a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1082 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/LICENSE
--rw-r--r--   0        0        0     7936 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/README.md
--rw-r--r--   0        0        0       98 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/__init__.py
--rw-r--r--   0        0        0     2783 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/add_create_type_false.py
--rw-r--r--   0        0        0     2073 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/add_postgres_using_to_text.py
--rw-r--r--   0        0        0     2672 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/compare_dispatch.py
--rw-r--r--   0        0        0      461 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/connection.py
--rw-r--r--   0        0        0      137 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/detection_of_changes/__init__.py
--rw-r--r--   0        0        0     1402 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/detection_of_changes/enum_alteration.py
--rw-r--r--   0        0        0      738 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/detection_of_changes/enum_creation.py
--rw-r--r--   0        0        0      763 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/detection_of_changes/enum_deletion.py
--rw-r--r--   0        0        0      230 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/get_enum_data/__init__.py
--rw-r--r--   0        0        0     4214 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/get_enum_data/declared_enums.py
--rw-r--r--   0        0        0     1018 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/get_enum_data/defined_enums.py
--rw-r--r--   0        0        0     1885 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/get_enum_data/types.py
--rw-r--r--   0        0        0      119 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/__init__.py
--rw-r--r--   0        0        0      954 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/create_enum.py
--rw-r--r--   0        0        0      946 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/drop_enum.py
--rw-r--r--   0        0        0      582 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/enum_lifecycle_base.py
--rw-r--r--   0        0        0     8175 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/sync_enum_values.py
--rw-r--r--   0        0        0        0 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/py.typed
--rw-r--r--   0        0        0     1996 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/sql_commands/column_default.py
--rw-r--r--   0        0        0     3016 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/sql_commands/comparison_operators.py
--rw-r--r--   0        0        0     3385 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/sql_commands/enum_type.py
--rw-r--r--   0        0        0      979 2024-04-13 06:22:18.276207 alembic_postgresql_enum-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8824 1970-01-01 00:00:00.000000 alembic_postgresql_enum-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-03-31 17:56:03.738151 alembic_postgresql_enum-1.2.0a1/LICENSE
+-rw-r--r--   0        0        0     7936 2024-03-31 17:56:03.738151 alembic_postgresql_enum-1.2.0a1/README.md
+-rw-r--r--   0        0        0       98 2024-03-31 17:56:03.738151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/__init__.py
+-rw-r--r--   0        0        0     2783 2024-03-31 17:56:03.738151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/add_create_type_false.py
+-rw-r--r--   0        0        0     2073 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/add_postgres_using_to_text.py
+-rw-r--r--   0        0        0     2672 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/compare_dispatch.py
+-rw-r--r--   0        0        0      461 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/connection.py
+-rw-r--r--   0        0        0      137 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/detection_of_changes/__init__.py
+-rw-r--r--   0        0        0     1402 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/detection_of_changes/enum_alteration.py
+-rw-r--r--   0        0        0      738 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/detection_of_changes/enum_creation.py
+-rw-r--r--   0        0        0      763 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/detection_of_changes/enum_deletion.py
+-rw-r--r--   0        0        0      230 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/get_enum_data/__init__.py
+-rw-r--r--   0        0        0     4214 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/get_enum_data/declared_enums.py
+-rw-r--r--   0        0        0     1018 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/get_enum_data/defined_enums.py
+-rw-r--r--   0        0        0     1883 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/get_enum_data/types.py
+-rw-r--r--   0        0        0      119 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/__init__.py
+-rw-r--r--   0        0        0      954 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/create_enum.py
+-rw-r--r--   0        0        0      946 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/drop_enum.py
+-rw-r--r--   0        0        0      582 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/enum_lifecycle_base.py
+-rw-r--r--   0        0        0     8175 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/sync_enum_values.py
+-rw-r--r--   0        0        0        0 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/py.typed
+-rw-r--r--   0        0        0     1996 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/sql_commands/column_default.py
+-rw-r--r--   0        0        0     3016 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/sql_commands/comparison_operators.py
+-rw-r--r--   0        0        0     3385 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/sql_commands/enum_type.py
+-rw-r--r--   0        0        0      981 2024-03-31 17:56:03.742151 alembic_postgresql_enum-1.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     8826 1970-01-01 00:00:00.000000 alembic_postgresql_enum-1.2.0a1/PKG-INFO
```

### Comparing `alembic_postgresql_enum-1.2.0/LICENSE` & `alembic_postgresql_enum-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/README.md` & `alembic_postgresql_enum-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/add_create_type_false.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/add_create_type_false.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/add_postgres_using_to_text.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/add_postgres_using_to_text.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/compare_dispatch.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/compare_dispatch.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/detection_of_changes/enum_alteration.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/detection_of_changes/enum_alteration.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/detection_of_changes/enum_creation.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/detection_of_changes/enum_creation.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/detection_of_changes/enum_deletion.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/detection_of_changes/enum_deletion.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/get_enum_data/declared_enums.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/get_enum_data/declared_enums.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/get_enum_data/defined_enums.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/get_enum_data/defined_enums.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/get_enum_data/types.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/get_enum_data/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     @property
     def table_name_with_schema(self):
         if self.table_schema:
             prefix = f"{self.table_schema}."
         else:
             prefix = ""
-        return f'{prefix}"{self.table_name}"'
+        return f"{prefix}{self.table_name}"
 
 
 EnumNamesToValues = Dict[str, Tuple[str, ...]]
 EnumNamesToTableReferences = Dict[str, FrozenSet[TableReference]]
 
 
 @dataclass
```

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/create_enum.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/create_enum.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/drop_enum.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/drop_enum.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/enum_lifecycle_base.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/enum_lifecycle_base.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/operations/sync_enum_values.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/operations/sync_enum_values.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/sql_commands/column_default.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/sql_commands/column_default.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/sql_commands/comparison_operators.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/sql_commands/comparison_operators.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/alembic_postgresql_enum/sql_commands/enum_type.py` & `alembic_postgresql_enum-1.2.0a1/alembic_postgresql_enum/sql_commands/enum_type.py`

 * *Files identical despite different names*

### Comparing `alembic_postgresql_enum-1.2.0/pyproject.toml` & `alembic_postgresql_enum-1.2.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alembic-postgresql-enum"
-version = "1.2.0"
+version = "1.2.0a1"
 description = "Alembic autogenerate support for creation, alteration and deletion of enums"
 authors = ["RustyGuard"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "alembic_postgresql_enum" }]
 classifiers = [
     'Development Status :: 4 - Beta',
```

### Comparing `alembic_postgresql_enum-1.2.0/PKG-INFO` & `alembic_postgresql_enum-1.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alembic-postgresql-enum
-Version: 1.2.0
+Version: 1.2.0a1
 Summary: Alembic autogenerate support for creation, alteration and deletion of enums
 License: MIT
 Author: RustyGuard
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

