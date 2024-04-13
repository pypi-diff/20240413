# Comparing `tmp/laorm-2.2.0.tar.gz` & `tmp/laorm-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laorm-2.2.0.tar", max compression
+gzip compressed data, was "laorm-2.3.0.tar", max compression
```

## Comparing `laorm-2.2.0.tar` & `laorm-2.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      208 2024-04-12 16:23:38.155130 laorm-2.2.0/laorm/__init__.py
--rw-r--r--   0        0        0     1425 2024-03-10 14:20:23.040591 laorm-2.2.0/laorm/PPA.py
--rw-r--r--   0        0        0    14711 2024-04-12 16:21:34.004920 laorm-2.2.0/laorm/stream.py
--rw-r--r--   0        0        0    11558 2024-01-12 14:31:32.745557 laorm-2.2.0/LICENSE
--rw-r--r--   0        0        0     1362 2024-04-12 16:23:37.972664 laorm-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 laorm-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      208 2024-04-12 17:13:39.621043 laorm-2.3.0/laorm/__init__.py
+-rw-r--r--   0        0        0     1505 2024-04-12 16:47:47.467701 laorm-2.3.0/laorm/PPA.py
+-rw-r--r--   0        0        0    15227 2024-04-12 17:10:35.120531 laorm-2.3.0/laorm/stream.py
+-rw-r--r--   0        0        0    11558 2024-01-12 14:31:32.745557 laorm-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1362 2024-04-12 17:13:39.486455 laorm-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 laorm-2.3.0/PKG-INFO
```

### Comparing `laorm-2.2.0/laorm/PPA.py` & `laorm-2.3.0/laorm/PPA.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,19 @@
         # sql注入攻击过滤处理
         sql = sql.replace("?", "%s")
 
         if isinstance(params, (dict)):
             # 参数化查询（使用字典）,转元组
             sql = sql.format_map(dict.fromkeys(params.keys(), "%s"))
             params = tuple(params.values())
-        if PPA.showMode:
-            print(sql.replace("%s", "{}").format(*params))
+        if  PPA.showMode:
+            if params:
+                print(sql.replace("%s", "{}").format(*params))
+            else:
+                print(sql)    
         try:
             async with cls.pool.acquire() as conn:
                 async with conn.cursor(aiomysql.DictCursor) as cur:
                     await cur.execute(sql, params)
                     return await cur.fetchone() if execOne else await cur.fetchall()
         except Exception as e:
             print(e)
```

### Comparing `laorm-2.2.0/laorm/stream.py` & `laorm-2.3.0/laorm/stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,18 +285,29 @@
 
     @classmethod
     async def page(cls: type[T], page: dict) -> T:
         pageIndex = page.get("page")
         size = page.get("size")
         pageIndex = (pageIndex - 1) * size
         cls.state_machine.process_keyword("limit", f"limit {pageIndex},{size}")
-        res, _ = await cls.exec()
+        res, sql = await cls.exec()
+        pageData = {
+            "list": res,
+        }
+        # 定义正则表达式模式，匹配"SELECT *"和"FROM"之间的任何字符（包括换行符）
+        countSql = re.sub(r"(?i)SELECT .* FROM", "count(*) from", sql)
+        countSql = f"select {countSql.split("limit")[0]}"
+        total = await PPA.exec(sql=countSql, execOne=True)
         # 封装新page
-
-        return res
+        pageData["page"] = {
+            "total": total.get("count(*)"),
+            "page": page.get("page"),
+            "size": size,
+        }
+        return pageData
 
     @classmethod
     async def post(cls: type[T], data: T | list[T] = None):
         cls.state_machine.mode = "post"
         if data and not isinstance(data, (list, tuple)):
             data = [data]
```

### Comparing `laorm-2.2.0/LICENSE` & `laorm-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laorm-2.2.0/pyproject.toml` & `laorm-2.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "laorm"
-version = "2.2.0"
+version = "2.3.0"
 description = "A python async orm tool"
 authors = ["larry <176286171@qq.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/mryzhou/laorm"
 
 repository = "https://github.com/mryzhou/laorm.git"  # 可选，指定项目仓库地址
```

### Comparing `laorm-2.2.0/PKG-INFO` & `laorm-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laorm
-Version: 2.2.0
+Version: 2.3.0
 Summary: A python async orm tool
 Home-page: https://github.com/mryzhou/laorm
 License: Apache-2.0
 Author: larry
 Author-email: 176286171@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

