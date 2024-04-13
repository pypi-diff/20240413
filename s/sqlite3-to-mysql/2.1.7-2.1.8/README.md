# Comparing `tmp/sqlite3_to_mysql-2.1.7.tar.gz` & `tmp/sqlite3_to_mysql-2.1.8.tar.gz`

## Comparing `sqlite3_to_mysql-2.1.7.tar` & `sqlite3_to_mysql-2.1.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/requirements_dev.txt
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/__init__.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/cli.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/click_utils.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/debug_info.py
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/mysql_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/py.typed
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/sqlite_utils.py
--rw-r--r--   0        0        0    32012 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/transporter.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/__init__.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/conftest.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/database.py
--rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/factories.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/faker_providers.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/func/__init__.py
--rw-r--r--   0        0        0    24175 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/func/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/func/test_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/unit/__init__.py
--rw-r--r--   0        0        0    18702 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/tests/unit/sqlite3_to_mysql_test.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/LICENSE
--rw-r--r--   0        0        0     6969 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/README.md
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/pyproject.toml
--rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/requirements_dev.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/__init__.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/cli.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/click_utils.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/debug_info.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/mysql_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/py.typed
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/sqlite_utils.py
+-rw-r--r--   0        0        0    32465 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/transporter.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/__init__.py
+-rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/conftest.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/database.py
+-rw-r--r--   0        0        0     4736 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/factories.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/faker_providers.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/func/__init__.py
+-rw-r--r--   0        0        0    24161 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/func/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0    18726 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/unit/__init__.py
+-rw-r--r--   0        0        0    18702 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/tests/unit/sqlite3_to_mysql_test.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/LICENSE
+-rw-r--r--   0        0        0     6969 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/README.md
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 sqlite3_to_mysql-2.1.8/PKG-INFO
```

### Comparing `sqlite3_to_mysql-2.1.7/CHANGELOG.md` & `sqlite3_to_mysql-2.1.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# 2.1.8
+
+* [CHORE] migrate package from flat layout to src layout
+
+# 2.1.7
+
+* [FEAT] add copyright header
+
 # 2.1.6
 
 * [FEAT] build both linux/amd64 and linux/arm64 Docker images
 
 # 2.1.5
 
 * [FEAT] add support for UNSIGNED numeric data type conversion
```

### Comparing `sqlite3_to_mysql-2.1.7/CODE-OF-CONDUCT.md` & `sqlite3_to_mysql-2.1.8/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/cli.py` & `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The command line interface of SQLite3toMySQL."""
+
 import os
 import sys
 import typing as t
 from datetime import datetime
 
 import click
 from mysql.connector import CharacterSet
```

### Comparing `sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/click_utils.py` & `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/click_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/debug_info.py` & `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/debug_info.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/mysql_utils.py` & `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/mysql_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MySQL helpers."""
+
 import re
 import typing as t
 
 from mysql.connector import CharacterSet
 from mysql.connector.charsets import MYSQL_CHARACTER_SETS
 from packaging import version
 from packaging.version import Version
```

### Comparing `sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/sqlite_utils.py` & `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/transporter.py` & `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/transporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,14 @@
                 return self._mysql_string_type
             match = self._valid_column_type(self._mysql_string_type)
             if match:
                 return match.group(0).upper() + length
         if data_type == "UNSIGNED BIG INT":
             return f"BIGINT{self._column_type_length(column_type)} UNSIGNED"
         if data_type.startswith(("TINYINT", "INT1")):
-            print("length", self._column_type_length(column_type))
             return f"TINYINT{self._column_type_length(column_type)}{' UNSIGNED' if unsigned else ''}"
         if data_type.startswith(("SMALLINT", "INT2")):
             return f"SMALLINT{self._column_type_length(column_type)}{' UNSIGNED' if unsigned else ''}"
         if data_type.startswith(("MEDIUMINT", "INT3")):
             return f"MEDIUMINT{self._column_type_length(column_type)}{' UNSIGNED' if unsigned else ''}"
         if data_type.startswith("INT4"):
             return f"INT{self._column_type_length(column_type)}{' UNSIGNED' if unsigned else ''}"
@@ -345,17 +344,21 @@
             )
 
             sql += " `{name}` {type} {notnull} {default} {auto_increment}, ".format(
                 name=mysql_safe_name,
                 type=column_type,
                 notnull="NOT NULL" if column["notnull"] or column["pk"] else "NULL",
                 auto_increment="AUTO_INCREMENT" if auto_increment else "",
-                default="DEFAULT " + column["dflt_value"]
-                if column["dflt_value"] and column_type not in MYSQL_COLUMN_TYPES_WITHOUT_DEFAULT and not auto_increment
-                else "",
+                default=(
+                    "DEFAULT " + column["dflt_value"]
+                    if column["dflt_value"]
+                    and column_type not in MYSQL_COLUMN_TYPES_WITHOUT_DEFAULT
+                    and not auto_increment
+                    else ""
+                ),
             )
 
             if column["pk"] > 0:
                 primary_key: t.Dict[str, str] = {
                     "column": mysql_safe_name,
                     "length": "",
                 }
@@ -434,17 +437,19 @@
                         f'`{safe_identifier_length(index_info["name"])}`' for index_info in index_infos
                     )
                 else:
                     # Limit the max TEXT field index length to 255
                     index_columns = ", ".join(
                         "`{column}`{length}".format(
                             column=safe_identifier_length(index_info["name"]),
-                            length="(255)"
-                            if table_columns[index_info["name"]].upper() in MYSQL_TEXT_COLUMN_TYPES_WITH_JSON
-                            else "",
+                            length=(
+                                "(255)"
+                                if table_columns[index_info["name"]].upper() in MYSQL_TEXT_COLUMN_TYPES_WITH_JSON
+                                else ""
+                            ),
                         )
                         for index_info in index_infos
                     )
             else:
                 column_list: t.List[str] = []
                 for index_info in index_infos:
                     index_length: str = ""
@@ -474,17 +479,19 @@
                     self._add_index(
                         table_name=table_name,
                         index_type="UNIQUE" if int(index["unique"]) == 1 else "INDEX",
                         index=index,
                         index_columns=", ".join(
                             "`{column}`{length}".format(
                                 column=safe_identifier_length(index_info["name"]),
-                                length="(255)"
-                                if table_columns[index_info["name"]].upper() in MYSQL_TEXT_COLUMN_TYPES_WITH_JSON
-                                else "",
+                                length=(
+                                    "(255)"
+                                    if table_columns[index_info["name"]].upper() in MYSQL_TEXT_COLUMN_TYPES_WITH_JSON
+                                    else ""
+                                ),
                             )
                             for index_info in index_infos
                         ),
                         index_infos=index_infos,
                     )
                 else:
                     raise
@@ -494,24 +501,28 @@
         table_name: str,
         index_type: str,
         index: t.Dict[str, t.Any],
         index_columns: str,
         index_infos: t.Tuple[t.Dict[str, t.Any], ...],
         index_iteration: int = 0,
     ) -> None:
-        sql: str = """
+        sql: str = (
+            """
             ALTER TABLE `{table}`
             ADD {index_type} `{name}`({columns})
         """.format(
-            table=safe_identifier_length(table_name),
-            index_type=index_type,
-            name=safe_identifier_length(index["name"])
-            if index_iteration == 0
-            else f'{safe_identifier_length(index["name"], max_length=60)}_{index_iteration}',
-            columns=index_columns,
+                table=safe_identifier_length(table_name),
+                index_type=index_type,
+                name=(
+                    safe_identifier_length(index["name"])
+                    if index_iteration == 0
+                    else f'{safe_identifier_length(index["name"], max_length=60)}_{index_iteration}'
+                ),
+                columns=index_columns,
+            )
         )
 
         try:
             self._logger.info(
                 """Adding %s to column "%s" in table %s""",
                 "unique index" if int(index["unique"]) == 1 else "index",
                 ", ".join(safe_identifier_length(index_info["name"]) for index_info in index_infos),
@@ -576,20 +587,24 @@
             """.format(
                 id=foreign_key["id"],
                 seq=foreign_key["seq"],
                 table=safe_identifier_length(table_name),
                 column=safe_identifier_length(foreign_key["from"]),
                 ref_table=safe_identifier_length(foreign_key["table"]),
                 ref_column=safe_identifier_length(foreign_key["to"]),
-                on_delete=foreign_key["on_delete"].upper()
-                if foreign_key["on_delete"].upper() != "SET DEFAULT"
-                else "NO ACTION",
-                on_update=foreign_key["on_update"].upper()
-                if foreign_key["on_update"].upper() != "SET DEFAULT"
-                else "NO ACTION",
+                on_delete=(
+                    foreign_key["on_delete"].upper()
+                    if foreign_key["on_delete"].upper() != "SET DEFAULT"
+                    else "NO ACTION"
+                ),
+                on_update=(
+                    foreign_key["on_update"].upper()
+                    if foreign_key["on_update"].upper() != "SET DEFAULT"
+                    else "NO ACTION"
+                ),
             )
 
             try:
                 self._logger.info(
                     "Adding foreign key to %s.%s referencing %s.%s",
                     safe_identifier_length(table_name),
                     safe_identifier_length(foreign_key["from"]),
@@ -682,26 +697,28 @@
                             table_name=table["name"],
                         )
                     )
                     columns: t.List[str] = [
                         safe_identifier_length(column[0]) for column in self._sqlite_cur.description
                     ]
                     if self._mysql_insert_method.upper() == "UPDATE":
-                        sql: str = """
+                        sql: str = (
+                            """
                             INSERT
                             INTO `{table}` ({fields})
                             VALUES ({placeholders}) AS `__new__`
                             ON DUPLICATE KEY UPDATE {field_updates}
                         """.format(
-                            table=safe_identifier_length(table["name"]),
-                            fields=("`{}`, " * len(columns)).rstrip(" ,").format(*columns),
-                            placeholders=("%s, " * len(columns)).rstrip(" ,"),
-                            field_updates=("`{}`=`__new__`.`{}`, " * len(columns))
-                            .rstrip(" ,")
-                            .format(*list(chain.from_iterable((column, column) for column in columns))),
+                                table=safe_identifier_length(table["name"]),
+                                fields=("`{}`, " * len(columns)).rstrip(" ,").format(*columns),
+                                placeholders=("%s, " * len(columns)).rstrip(" ,"),
+                                field_updates=("`{}`=`__new__`.`{}`, " * len(columns))
+                                .rstrip(" ,")
+                                .format(*list(chain.from_iterable((column, column) for column in columns))),
+                            )
                         )
                     else:
                         sql = """
                             INSERT {ignore}
                             INTO `{table}` ({fields})
                             VALUES ({placeholders})
                         """.format(
```

### Comparing `sqlite3_to_mysql-2.1.7/sqlite3_to_mysql/types.py` & `sqlite3_to_mysql-2.1.8/src/sqlite3_to_mysql/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Types for sqlite3-to-mysql."""
+
 import os
 import typing as t
 from logging import Logger
 from sqlite3 import Connection, Cursor
 
 import typing_extensions as tx
 from mysql.connector import MySQLConnection
```

### Comparing `sqlite3_to_mysql-2.1.7/tests/conftest.py` & `sqlite3_to_mysql-2.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/tests/database.py` & `sqlite3_to_mysql-2.1.8/tests/database.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/tests/factories.py` & `sqlite3_to_mysql-2.1.8/tests/factories.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/tests/faker_providers.py` & `sqlite3_to_mysql-2.1.8/tests/faker_providers.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/tests/models.py` & `sqlite3_to_mysql-2.1.8/tests/models.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/tests/func/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.1.8/tests/func/sqlite3_to_mysql_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,22 +309,22 @@
             json_serializer=json.dumps,
             json_deserializer=json.loads,
         )
         mysql_cnx: Connection = mysql_engine.connect()
         mysql_inspect: Inspector = inspect(mysql_engine)
         mysql_tables: t.List[str] = mysql_inspect.get_table_names()
 
-        mysql_connector_connection: t.Union[
-            PooledMySQLConnection, MySQLConnection, CMySQLConnection
-        ] = mysql.connector.connect(
-            user=mysql_credentials.user,
-            password=mysql_credentials.password,
-            host=mysql_credentials.host,
-            port=mysql_credentials.port,
-            database=mysql_credentials.database,
+        mysql_connector_connection: t.Union[PooledMySQLConnection, MySQLConnection, CMySQLConnection] = (
+            mysql.connector.connect(
+                user=mysql_credentials.user,
+                password=mysql_credentials.password,
+                host=mysql_credentials.host,
+                port=mysql_credentials.port,
+                database=mysql_credentials.database,
+            )
         )
         server_version: t.Tuple[int, ...] = mysql_connector_connection.get_server_version()
 
         """ Test if both databases have the same table names """
         assert sqlite_tables == mysql_tables
 
         """ Test if all the tables have the same column names """
@@ -366,17 +366,15 @@
                 FROM information_schema.TABLE_CONSTRAINTS AS i
                 {JOIN} information_schema.KEY_COLUMN_USAGE AS k ON i.CONSTRAINT_NAME = k.CONSTRAINT_NAME
                 WHERE i.TABLE_SCHEMA = :table_schema
                 AND i.TABLE_NAME = :table_name
                 AND i.CONSTRAINT_TYPE = :constraint_type
             """.format(
                     # MySQL 8.0.19 still works with "LEFT JOIN" everything above requires "JOIN"
-                    JOIN="JOIN"
-                    if (server_version[0] == 8 and server_version[2] > 19)
-                    else "LEFT JOIN"
+                    JOIN="JOIN" if (server_version[0] == 8 and server_version[2] > 19) else "LEFT JOIN"
                 )
             ).bindparams(
                 table_schema=mysql_credentials.database,
                 table_name=table_name,
                 constraint_type="FOREIGN KEY",
             )
             mysql_fk_result: CursorResult = mysql_cnx.execute(mysql_fk_stmt)
```

### Comparing `sqlite3_to_mysql-2.1.7/tests/func/test_cli.py` & `sqlite3_to_mysql-2.1.8/tests/func/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,13 +536,12 @@
             arguments.append(str(chunk))
         if with_rowid:
             arguments.append("--with-rowid")
         result = cli_runner.invoke(
             sqlite3mysql,
             arguments,
         )
-        print(result.output)
         assert result.exit_code == 0
         assert (
             f"{sqlite3mysql.name} version {package_version} Copyright (c) 2018-{datetime.now().year} Klemen Tusar"
             in result.output
         )
```

### Comparing `sqlite3_to_mysql-2.1.7/tests/unit/sqlite3_to_mysql_test.py` & `sqlite3_to_mysql-2.1.8/tests/unit/sqlite3_to_mysql_test.py`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/.gitignore` & `sqlite3_to_mysql-2.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/LICENSE` & `sqlite3_to_mysql-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/README.md` & `sqlite3_to_mysql-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sqlite3_to_mysql-2.1.7/pyproject.toml` & `sqlite3_to_mysql-2.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,19 @@
 [project.urls]
 Source = "https://github.com/techouse/sqlite3-to-mysql"
 Changelog = "https://github.com/techouse/sqlite3-to-mysql/blob/master/CHANGELOG.md"
 Sponsor = "https://github.com/sponsors/techouse"
 PayPal = "https://paypal.me/ktusar"
 
 [tool.hatch.version]
-path = "sqlite3_to_mysql/__init__.py"
+path = "src/sqlite3_to_mysql/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "sqlite3_to_mysql",
+    "src",
     "tests",
     "README.md",
     "CHANGELOG.md",
     "CODE-OF-CONDUCT.md",
     "LICENSE",
     "requirements_dev.txt",
 ]
@@ -99,26 +99,28 @@
 line_length = 120
 profile = "black"
 lines_after_imports = 2
 known_first_party = "sqlite3_to_mysql"
 skip_gitignore = true
 
 [tool.pytest.ini_options]
+pythonpath = ["src"]
 testpaths = ["tests"]
 norecursedirs = [".*", "venv", "env", "*.egg", "dist", "build"]
 minversion = "7.3.1"
 addopts = "-rsxX -l --tb=short --strict-markers"
 timeout = 300
 markers = [
     "init: Run the initialisation test functions",
     "transfer: Run the main transfer test functions",
     "cli: Run the cli test functions",
 ]
 
 [tool.mypy]
+mypy_path = "src"
 python_version = "3.8"
 exclude = [
     "tests",
     "build",
     "dist",
     "venv",
     "env",
```

### Comparing `sqlite3_to_mysql-2.1.7/PKG-INFO` & `sqlite3_to_mysql-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sqlite3-to-mysql
-Version: 2.1.7
+Version: 2.1.8
 Summary: A simple Python tool to transfer data from SQLite 3 to MySQL
 Project-URL: Source, https://github.com/techouse/sqlite3-to-mysql
 Project-URL: Changelog, https://github.com/techouse/sqlite3-to-mysql/blob/master/CHANGELOG.md
 Project-URL: Sponsor, https://github.com/sponsors/techouse
 Project-URL: PayPal, https://paypal.me/ktusar
 Author-email: Klemen Tusar <techouse@gmail.com>
 License: MIT
```

